##解答  
hello_trema.rbに以下のメソッドを追加した．  

###1. switch_disconnected(datapath_id)  
def switch_disconnected(datapath_id)  
	logger.info "Bye #{datapath_id.to_hex}"  
end
	
trema stop (ID)が入力されるとTremaが停止されるため，コントローラとスイッチ間のコネクションが切断される．  
このイベントがswitch_disconnectedにより捕捉され，中の関数が実行されてByeが出力されるようになる．  