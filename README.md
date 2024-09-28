# Axone ..

    curl https://i.jpillora.com/axone-protocol/axoned! | bash

    axoned --home mynode init NODEID --chain-id axone-dentrite-1

    axoned --home mynode keys add NAME

    wget https://raw.githubusercontent.com/axone-protocol/networks/main/chains/dentrite-1/genesis.json

    mv /root/genesis.json /root/.axoned/config/

    screen -S axone
    axoned start

CTRL A+D

    axoned --home mynode genesis add-genesis-account NAME 1000000000000uaxone
    
     axoned --home mynode genesis gentx NAME 1000000000000uaxone \
     --node-id $(axoned --home mynode comet show-node-id) \
     --chain-id axone-dentrite-1 \
     --commission-rate 0.05 \
     --commission-max-rate 0.2 \
     --commission-max-change-rate 0.01 \
     --min-self-delegation 1 \
     --website "https://foo.network" \
     --details "My validator" \
     --identity "6C36E7C076BFDCE4" \
     --security-contact "validator@foo.network"

Gentx dosyanızı görmek için kodun sonuna no nuzu eklleyin

    nano ~/mynode/config/gentx/gentx-NUMBER.json

Repoya pr atın ve https://github.com/axone-protocol/networks/issues gentx ekleyin

Tebrikler! #
