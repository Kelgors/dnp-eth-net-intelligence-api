\[DNP\] Ethereum Network Intelligence API
============

The purpose of this repo is to package [eth-net-intelligence-api](https://github.com/cubedro/eth-net-intelligence-api) as a DAppNode Package.

This is the backend service which runs along with ethereum and tracks the network status, fetches information through JSON-RPC and connects through WebSockets to [eth-netstats](https://github.com/cubedro/eth-netstats) to feed information. For full install instructions please read the [wiki](https://github.com/ethereum/wiki/wiki/Network-Status).

## Environment variables

#### INSTANCE_NAME

The name of your instance to recognize it in the server's list

#### CONTACT_DETAILS

Your email/skype if you wish to be contacted (optional)

#### WS_SERVER

URI to the websocket of the ethstats instance you want to send your data

#### WS_SECRET

Secret token given by the ethstats instance owner

#### RPC_HOST

Ethereum remote console (RPC) json formatted host (for DNP_ETHCHAIN, it is 172.33.1.6)

#### RPC_HOST

Ethereum remote console (RPC) json formatted port (for DNP_ETHCHAIN, it is 8545)

#### LISTENING_PORT

Your Ethereum node listening port (only used for display)

#### VERBOSITY

Set the logs verbosity (0 = silent, 1 = error, warn, 2 = error, warn, info, success, 3 = all logs)
