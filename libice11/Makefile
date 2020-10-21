#BUILDMAKE edit-mode: -*- Makefile -*-
####################64Bit Mode####################
ifeq ($(shell uname -m), x86_64)
CC=gcc
CXX=g++
CPPFLAGS=-D_GNU_SOURCE \
  -D__STDC_LIMIT_MACROS \
  -DVERSION=\"1.9.8.7\"
CFLAGS=-g \
  -pipe \
  -W \
  -Wall \
  -fPIC
CXXFLAGS=-g \
  -pipe \
  -W \
  -Wall \
  -fPIC \
  -std=gnu++11
FLAGSEXTRA=
INCPATH=-I. \
  -I./include \
  -I./output \
  -I./output/include \
  -I./deps/libev/include \
  -I./src
DEP_INCPATH=


#BUILDMAKE UUID
BUILDMAKE_MD5=843996a5be94415bdb8d7d1ebe3f5c55  BUILDMAKE


.PHONY:all
all:buildmake_makefile_check libice.a 
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40mall[0m']"
	@echo "make all done"

PHONY:buildmake_makefile_check
buildmake_makefile_check:
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40mbuildmake_makefile_check[0m']"
	#in case of error, update "Makefile" by "buildmake"
	@echo "$(BUILDMAKE_MD5)" > buildmake.md5
	@md5sum -c --status buildmake.md5
	@rm -f buildmake.md5

.PHONY:clean
clean:
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40mclean[0m']"
	rm -rf libice.a
	rm -rf ./output
	rm -rf src/p2p/ice_basic_packet_socket_factory.o
	rm -rf src/p2p/ice_basic_port_allocator.o
	rm -rf src/p2p/ice_candidate.o
	rm -rf src/p2p/ice_ice_agent.o
	rm -rf src/p2p/ice_ice_common.o
	rm -rf src/p2p/ice_ice_transport_channel.o
	rm -rf src/p2p/ice_p2p_transport_channel.o
	rm -rf src/p2p/ice_port.o
	rm -rf src/p2p/ice_port_allocator.o
	rm -rf src/p2p/ice_stun.o
	rm -rf src/p2p/ice_stun_port.o
	rm -rf src/p2p/ice_stun_request.o
	rm -rf src/rtcbase/ice_async_packet_socket.o
	rm -rf src/rtcbase/ice_async_socket.o
	rm -rf src/rtcbase/ice_async_udp_socket.o
	rm -rf src/rtcbase/ice_base64.o
	rm -rf src/rtcbase/ice_buffer_queue.o
	rm -rf src/rtcbase/ice_byte_buffer.o
	rm -rf src/rtcbase/ice_crc32.o
	rm -rf src/rtcbase/ice_critical_section.o
	rm -rf src/rtcbase/ice_event.o
	rm -rf src/rtcbase/ice_event_loop.o
	rm -rf src/rtcbase/ice_ifaddrs_converter.o
	rm -rf src/rtcbase/ice_ipaddress.o
	rm -rf src/rtcbase/ice_location.o
	rm -rf src/rtcbase/ice_logging.o
	rm -rf src/rtcbase/ice_md5.o
	rm -rf src/rtcbase/ice_md5_digest.o
	rm -rf src/rtcbase/ice_message_digest.o
	rm -rf src/rtcbase/ice_net_helpers.o
	rm -rf src/rtcbase/ice_network.o
	rm -rf src/rtcbase/ice_openssl_adapter.o
	rm -rf src/rtcbase/ice_openssl_digest.o
	rm -rf src/rtcbase/ice_openssl_identity.o
	rm -rf src/rtcbase/ice_openssl_stream_adapter.o
	rm -rf src/rtcbase/ice_physical_socket_server.o
	rm -rf src/rtcbase/ice_platform_thread.o
	rm -rf src/rtcbase/ice_random.o
	rm -rf src/rtcbase/ice_rate_statistics.o
	rm -rf src/rtcbase/ice_rtccertificate.o
	rm -rf src/rtcbase/ice_rtccertificate_generator.o
	rm -rf src/rtcbase/ice_sha1.o
	rm -rf src/rtcbase/ice_sha1_digest.o
	rm -rf src/rtcbase/ice_sigslot.o
	rm -rf src/rtcbase/ice_socket_address.o
	rm -rf src/rtcbase/ice_ssl_adapter.o
	rm -rf src/rtcbase/ice_ssl_fingerprint.o
	rm -rf src/rtcbase/ice_ssl_identity.o
	rm -rf src/rtcbase/ice_ssl_stream_adapter.o
	rm -rf src/rtcbase/ice_stream.o
	rm -rf src/rtcbase/ice_string_encode.o
	rm -rf src/rtcbase/ice_string_to_number.o
	rm -rf src/rtcbase/ice_string_utils.o
	rm -rf src/rtcbase/ice_time_utils.o
	rm -rf src/rtcbase/ice_zmalloc.o

.PHONY:dist
dist:
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40mdist[0m']"
	tar czvf output.tar.gz output
	@echo "make dist done"

.PHONY:distclean
distclean:clean
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40mdistclean[0m']"
	rm -f output.tar.gz
	@echo "make distclean done"

.PHONY:love
love:
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40mlove[0m']"
	@echo "make love done"

libice.a:src/p2p/ice_basic_packet_socket_factory.o \
  src/p2p/ice_basic_port_allocator.o \
  src/p2p/ice_candidate.o \
  src/p2p/ice_ice_agent.o \
  src/p2p/ice_ice_common.o \
  src/p2p/ice_ice_transport_channel.o \
  src/p2p/ice_p2p_transport_channel.o \
  src/p2p/ice_port.o \
  src/p2p/ice_port_allocator.o \
  src/p2p/ice_stun.o \
  src/p2p/ice_stun_port.o \
  src/p2p/ice_stun_request.o \
  src/rtcbase/ice_async_packet_socket.o \
  src/rtcbase/ice_async_socket.o \
  src/rtcbase/ice_async_udp_socket.o \
  src/rtcbase/ice_base64.o \
  src/rtcbase/ice_buffer_queue.o \
  src/rtcbase/ice_byte_buffer.o \
  src/rtcbase/ice_crc32.o \
  src/rtcbase/ice_critical_section.o \
  src/rtcbase/ice_event.o \
  src/rtcbase/ice_event_loop.o \
  src/rtcbase/ice_ifaddrs_converter.o \
  src/rtcbase/ice_ipaddress.o \
  src/rtcbase/ice_location.o \
  src/rtcbase/ice_logging.o \
  src/rtcbase/ice_md5.o \
  src/rtcbase/ice_md5_digest.o \
  src/rtcbase/ice_message_digest.o \
  src/rtcbase/ice_net_helpers.o \
  src/rtcbase/ice_network.o \
  src/rtcbase/ice_openssl_adapter.o \
  src/rtcbase/ice_openssl_digest.o \
  src/rtcbase/ice_openssl_identity.o \
  src/rtcbase/ice_openssl_stream_adapter.o \
  src/rtcbase/ice_physical_socket_server.o \
  src/rtcbase/ice_platform_thread.o \
  src/rtcbase/ice_random.o \
  src/rtcbase/ice_rate_statistics.o \
  src/rtcbase/ice_rtccertificate.o \
  src/rtcbase/ice_rtccertificate_generator.o \
  src/rtcbase/ice_sha1.o \
  src/rtcbase/ice_sha1_digest.o \
  src/rtcbase/ice_sigslot.o \
  src/rtcbase/ice_socket_address.o \
  src/rtcbase/ice_ssl_adapter.o \
  src/rtcbase/ice_ssl_fingerprint.o \
  src/rtcbase/ice_ssl_identity.o \
  src/rtcbase/ice_ssl_stream_adapter.o \
  src/rtcbase/ice_stream.o \
  src/rtcbase/ice_string_encode.o \
  src/rtcbase/ice_string_to_number.o \
  src/rtcbase/ice_string_utils.o \
  src/rtcbase/ice_time_utils.o \
  src/rtcbase/ice_zmalloc.o \
  src/p2p/basic_packet_socket_factory.h \
  src/p2p/basic_port_allocator.h \
  src/p2p/candidate.h \
  src/p2p/candidate_pair_interface.h \
  src/p2p/ice_agent.h \
  src/p2p/ice_common.h \
  src/p2p/ice_transport_channel.h \
  src/p2p/p2p_transport_channel.h \
  src/p2p/packet_socket_factory.h \
  src/p2p/packet_transport_channel.h \
  src/p2p/port.h \
  src/p2p/port_allocator.h \
  src/p2p/port_interface.h \
  src/p2p/stun.h \
  src/p2p/stun_port.h \
  src/p2p/stun_request.h \
  src/rtcbase/async_packet_socket.cpp \
  src/rtcbase/async_socket.cpp \
  src/rtcbase/async_udp_socket.cpp \
  src/rtcbase/base64.cpp \
  src/rtcbase/buffer_queue.cpp \
  src/rtcbase/byte_buffer.cpp \
  src/rtcbase/crc32.cpp \
  src/rtcbase/critical_section.cpp \
  src/rtcbase/event.cpp \
  src/rtcbase/event_loop.cpp \
  src/rtcbase/ifaddrs_converter.cpp \
  src/rtcbase/ipaddress.cpp \
  src/rtcbase/location.cpp \
  src/rtcbase/logging.cpp \
  src/rtcbase/md5.cpp \
  src/rtcbase/md5_digest.cpp \
  src/rtcbase/message_digest.cpp \
  src/rtcbase/net_helpers.cpp \
  src/rtcbase/network.cpp \
  src/rtcbase/openssl_adapter.cpp \
  src/rtcbase/openssl_digest.cpp \
  src/rtcbase/openssl_identity.cpp \
  src/rtcbase/openssl_stream_adapter.cpp \
  src/rtcbase/physical_socket_server.cpp \
  src/rtcbase/platform_thread.cpp \
  src/rtcbase/random.cpp \
  src/rtcbase/rate_statistics.cpp \
  src/rtcbase/rtccertificate.cpp \
  src/rtcbase/rtccertificate_generator.cpp \
  src/rtcbase/sha1.cpp \
  src/rtcbase/sha1_digest.cpp \
  src/rtcbase/sigslot.cpp \
  src/rtcbase/socket_address.cpp \
  src/rtcbase/ssl_adapter.cpp \
  src/rtcbase/ssl_fingerprint.cpp \
  src/rtcbase/ssl_identity.cpp \
  src/rtcbase/ssl_stream_adapter.cpp \
  src/rtcbase/stream.cpp \
  src/rtcbase/string_encode.cpp \
  src/rtcbase/string_to_number.cpp \
  src/rtcbase/string_utils.cpp \
  src/rtcbase/time_utils.cpp \
  src/rtcbase/zmalloc.cpp
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40mlibice.a[0m']"
	ar crs libice.a src/p2p/ice_basic_packet_socket_factory.o \
  src/p2p/ice_basic_port_allocator.o \
  src/p2p/ice_candidate.o \
  src/p2p/ice_ice_agent.o \
  src/p2p/ice_ice_common.o \
  src/p2p/ice_ice_transport_channel.o \
  src/p2p/ice_p2p_transport_channel.o \
  src/p2p/ice_port.o \
  src/p2p/ice_port_allocator.o \
  src/p2p/ice_stun.o \
  src/p2p/ice_stun_port.o \
  src/p2p/ice_stun_request.o \
  src/rtcbase/ice_async_packet_socket.o \
  src/rtcbase/ice_async_socket.o \
  src/rtcbase/ice_async_udp_socket.o \
  src/rtcbase/ice_base64.o \
  src/rtcbase/ice_buffer_queue.o \
  src/rtcbase/ice_byte_buffer.o \
  src/rtcbase/ice_crc32.o \
  src/rtcbase/ice_critical_section.o \
  src/rtcbase/ice_event.o \
  src/rtcbase/ice_event_loop.o \
  src/rtcbase/ice_ifaddrs_converter.o \
  src/rtcbase/ice_ipaddress.o \
  src/rtcbase/ice_location.o \
  src/rtcbase/ice_logging.o \
  src/rtcbase/ice_md5.o \
  src/rtcbase/ice_md5_digest.o \
  src/rtcbase/ice_message_digest.o \
  src/rtcbase/ice_net_helpers.o \
  src/rtcbase/ice_network.o \
  src/rtcbase/ice_openssl_adapter.o \
  src/rtcbase/ice_openssl_digest.o \
  src/rtcbase/ice_openssl_identity.o \
  src/rtcbase/ice_openssl_stream_adapter.o \
  src/rtcbase/ice_physical_socket_server.o \
  src/rtcbase/ice_platform_thread.o \
  src/rtcbase/ice_random.o \
  src/rtcbase/ice_rate_statistics.o \
  src/rtcbase/ice_rtccertificate.o \
  src/rtcbase/ice_rtccertificate_generator.o \
  src/rtcbase/ice_sha1.o \
  src/rtcbase/ice_sha1_digest.o \
  src/rtcbase/ice_sigslot.o \
  src/rtcbase/ice_socket_address.o \
  src/rtcbase/ice_ssl_adapter.o \
  src/rtcbase/ice_ssl_fingerprint.o \
  src/rtcbase/ice_ssl_identity.o \
  src/rtcbase/ice_ssl_stream_adapter.o \
  src/rtcbase/ice_stream.o \
  src/rtcbase/ice_string_encode.o \
  src/rtcbase/ice_string_to_number.o \
  src/rtcbase/ice_string_utils.o \
  src/rtcbase/ice_time_utils.o \
  src/rtcbase/ice_zmalloc.o
	mkdir -p ./output/lib
	cp -f --link libice.a ./output/lib
	mkdir -p ./output/include/ice/p2p
	cp -f --link src/p2p/*.h ./output/include/ice/p2p
	mkdir -p ./output/include/ice/rtcbase
	cp -f --link src/rtcbase/*.h ./output/include/ice/rtcbase

src/p2p/ice_basic_packet_socket_factory.o:src/p2p/basic_packet_socket_factory.cpp \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/physical_socket_server.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/logging.h \
  src/rtcbase/socket_factory.h \
  src/rtcbase/socket.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/socket_address.h \
  src/rtcbase/ipaddress.h \
  src/rtcbase/byte_order.h \
  src/rtcbase/async_socket.h \
  src/rtcbase/sigslot.h \
  src/rtcbase/async_udp_socket.h \
  src/rtcbase/async_packet_socket.h \
  src/rtcbase/dscp.h \
  src/rtcbase/time_utils.h \
  src/rtcbase/event_loop.h \
  src/p2p/ice_common.h \
  src/p2p/basic_packet_socket_factory.h \
  src/rtcbase/event_loop.h \
  src/rtcbase/memcheck.h \
  src/p2p/packet_socket_factory.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/socket_address.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/p2p/ice_basic_packet_socket_factory.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/p2p/ice_basic_packet_socket_factory.o src/p2p/basic_packet_socket_factory.cpp

src/p2p/ice_basic_port_allocator.o:src/p2p/basic_port_allocator.cpp \
  src/rtcbase/random.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/logging.h \
  src/p2p/basic_packet_socket_factory.h \
  src/rtcbase/event_loop.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/logging.h \
  src/p2p/packet_socket_factory.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/socket_address.h \
  src/rtcbase/ipaddress.h \
  src/rtcbase/byte_order.h \
  src/p2p/ice_common.h \
  src/p2p/port.h \
  src/rtcbase/log_trace_id.h \
  src/rtcbase/network.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/network_constants.h \
  src/rtcbase/sigslot.h \
  src/rtcbase/sigslot.h \
  src/rtcbase/async_packet_socket.h \
  src/rtcbase/dscp.h \
  src/rtcbase/socket.h \
  src/rtcbase/socket_address.h \
  src/rtcbase/time_utils.h \
  src/p2p/candidate.h \
  src/rtcbase/basic_types.h \
  src/p2p/candidate_pair_interface.h \
  src/p2p/port_interface.h \
  src/p2p/stun.h \
  src/rtcbase/byte_buffer.h \
  src/rtcbase/buffer.h \
  src/rtcbase/array_view.h \
  src/rtcbase/type_traits.h \
  src/p2p/stun_request.h \
  src/p2p/stun_port.h \
  src/p2p/basic_port_allocator.h \
  src/p2p/port_allocator.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/p2p/ice_basic_port_allocator.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/p2p/ice_basic_port_allocator.o src/p2p/basic_port_allocator.cpp

src/p2p/ice_candidate.o:src/p2p/candidate.cpp \
  src/p2p/candidate.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/random.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/network.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/logging.h \
  src/rtcbase/ipaddress.h \
  src/rtcbase/byte_order.h \
  src/rtcbase/network_constants.h \
  src/rtcbase/sigslot.h \
  src/rtcbase/socket_address.h \
  src/p2p/ice_common.h \
  src/rtcbase/logging.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/p2p/ice_candidate.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/p2p/ice_candidate.o src/p2p/candidate.cpp

src/p2p/ice_ice_agent.o:src/p2p/ice_agent.cpp \
  src/p2p/port.h \
  src/rtcbase/log_trace_id.h \
  src/rtcbase/network.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/ipaddress.h \
  src/rtcbase/byte_order.h \
  src/rtcbase/network_constants.h \
  src/rtcbase/sigslot.h \
  src/rtcbase/sigslot.h \
  src/rtcbase/socket_address.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/async_packet_socket.h \
  src/rtcbase/dscp.h \
  src/rtcbase/socket.h \
  src/rtcbase/socket_address.h \
  src/rtcbase/time_utils.h \
  src/rtcbase/memcheck.h \
  src/p2p/candidate.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/random.h \
  src/p2p/ice_common.h \
  src/rtcbase/logging.h \
  src/p2p/candidate_pair_interface.h \
  src/p2p/packet_socket_factory.h \
  src/rtcbase/event_loop.h \
  src/rtcbase/constructor_magic.h \
  src/p2p/port_interface.h \
  src/p2p/stun.h \
  src/rtcbase/byte_buffer.h \
  src/rtcbase/buffer.h \
  src/rtcbase/array_view.h \
  src/rtcbase/type_traits.h \
  src/p2p/stun_request.h \
  src/p2p/p2p_transport_channel.h \
  src/rtcbase/optional.h \
  src/rtcbase/sanitizer.h \
  src/p2p/port_allocator.h \
  src/p2p/ice_transport_channel.h \
  src/p2p/packet_transport_channel.h \
  src/p2p/ice_agent.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/p2p/ice_ice_agent.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/p2p/ice_ice_agent.o src/p2p/ice_agent.cpp

src/p2p/ice_ice_common.o:src/p2p/ice_common.cpp \
  src/p2p/ice_common.h \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/p2p/ice_ice_common.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/p2p/ice_ice_common.o src/p2p/ice_common.cpp

src/p2p/ice_ice_transport_channel.o:src/p2p/ice_transport_channel.cpp \
  src/p2p/ice_transport_channel.h \
  src/rtcbase/optional.h \
  src/rtcbase/array_view.h \
  src/rtcbase/type_traits.h \
  src/rtcbase/sanitizer.h \
  src/rtcbase/log_trace_id.h \
  src/p2p/ice_common.h \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/p2p/candidate.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/random.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/network.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/logging.h \
  src/rtcbase/ipaddress.h \
  src/rtcbase/byte_order.h \
  src/rtcbase/network_constants.h \
  src/rtcbase/sigslot.h \
  src/rtcbase/socket_address.h \
  src/p2p/candidate_pair_interface.h \
  src/p2p/packet_transport_channel.h \
  src/rtcbase/async_packet_socket.h \
  src/rtcbase/dscp.h \
  src/rtcbase/socket.h \
  src/rtcbase/socket_address.h \
  src/rtcbase/time_utils.h \
  src/rtcbase/sigslot.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/p2p/ice_ice_transport_channel.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/p2p/ice_ice_transport_channel.o src/p2p/ice_transport_channel.cpp

src/p2p/ice_p2p_transport_channel.o:src/p2p/p2p_transport_channel.cpp \
  src/rtcbase/crc32.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/string_encode.h \
  src/p2p/ice_common.h \
  src/p2p/p2p_transport_channel.h \
  src/rtcbase/event_loop.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/sigslot.h \
  src/rtcbase/optional.h \
  src/rtcbase/array_view.h \
  src/rtcbase/type_traits.h \
  src/rtcbase/sanitizer.h \
  src/rtcbase/log_trace_id.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/logging.h \
  src/p2p/port_allocator.h \
  src/p2p/port.h \
  src/rtcbase/network.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/ipaddress.h \
  src/rtcbase/byte_order.h \
  src/rtcbase/network_constants.h \
  src/rtcbase/sigslot.h \
  src/rtcbase/socket_address.h \
  src/rtcbase/async_packet_socket.h \
  src/rtcbase/dscp.h \
  src/rtcbase/socket.h \
  src/rtcbase/socket_address.h \
  src/rtcbase/time_utils.h \
  src/p2p/candidate.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/random.h \
  src/p2p/candidate_pair_interface.h \
  src/p2p/packet_socket_factory.h \
  src/p2p/port_interface.h \
  src/p2p/stun.h \
  src/rtcbase/byte_buffer.h \
  src/rtcbase/buffer.h \
  src/p2p/stun_request.h \
  src/p2p/ice_transport_channel.h \
  src/p2p/packet_transport_channel.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/p2p/ice_p2p_transport_channel.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/p2p/ice_p2p_transport_channel.o src/p2p/p2p_transport_channel.cpp

src/p2p/ice_port.o:src/p2p/port.cpp \
  src/rtcbase/ptr_utils.h \
  src/rtcbase/crc32.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/random.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/logging.h \
  src/rtcbase/network.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/logging.h \
  src/rtcbase/ipaddress.h \
  src/rtcbase/byte_order.h \
  src/rtcbase/network_constants.h \
  src/rtcbase/sigslot.h \
  src/rtcbase/string_encode.h \
  src/p2p/ice_common.h \
  src/p2p/port_allocator.h \
  src/rtcbase/log_trace_id.h \
  src/rtcbase/sigslot.h \
  src/p2p/port.h \
  src/rtcbase/socket_address.h \
  src/rtcbase/async_packet_socket.h \
  src/rtcbase/dscp.h \
  src/rtcbase/socket.h \
  src/rtcbase/socket_address.h \
  src/rtcbase/time_utils.h \
  src/rtcbase/memcheck.h \
  src/p2p/candidate.h \
  src/rtcbase/basic_types.h \
  src/p2p/candidate_pair_interface.h \
  src/p2p/packet_socket_factory.h \
  src/rtcbase/event_loop.h \
  src/rtcbase/constructor_magic.h \
  src/p2p/port_interface.h \
  src/p2p/stun.h \
  src/rtcbase/byte_buffer.h \
  src/rtcbase/buffer.h \
  src/rtcbase/array_view.h \
  src/rtcbase/type_traits.h \
  src/p2p/stun_request.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/p2p/ice_port.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/p2p/ice_port.o src/p2p/port.cpp

src/p2p/ice_port_allocator.o:src/p2p/port_allocator.cpp \
  src/p2p/port_allocator.h \
  src/rtcbase/log_trace_id.h \
  src/rtcbase/sigslot.h \
  src/p2p/port.h \
  src/rtcbase/network.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/ipaddress.h \
  src/rtcbase/byte_order.h \
  src/rtcbase/network_constants.h \
  src/rtcbase/sigslot.h \
  src/rtcbase/socket_address.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/async_packet_socket.h \
  src/rtcbase/dscp.h \
  src/rtcbase/socket.h \
  src/rtcbase/socket_address.h \
  src/rtcbase/time_utils.h \
  src/rtcbase/memcheck.h \
  src/p2p/candidate.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/random.h \
  src/p2p/ice_common.h \
  src/rtcbase/logging.h \
  src/p2p/candidate_pair_interface.h \
  src/p2p/packet_socket_factory.h \
  src/rtcbase/event_loop.h \
  src/rtcbase/constructor_magic.h \
  src/p2p/port_interface.h \
  src/p2p/stun.h \
  src/rtcbase/byte_buffer.h \
  src/rtcbase/buffer.h \
  src/rtcbase/array_view.h \
  src/rtcbase/type_traits.h \
  src/p2p/stun_request.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/p2p/ice_port_allocator.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/p2p/ice_port_allocator.o src/p2p/port_allocator.cpp

src/p2p/ice_stun.o:src/p2p/stun.cpp \
  src/rtcbase/ptr_utils.h \
  src/rtcbase/byte_order.h \
  src/rtcbase/crc32.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/message_digest.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/logging.h \
  src/rtcbase/string_encode.h \
  src/p2p/stun.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/byte_buffer.h \
  src/rtcbase/buffer.h \
  src/rtcbase/array_view.h \
  src/rtcbase/type_traits.h \
  src/rtcbase/socket_address.h \
  src/rtcbase/ipaddress.h \
  src/rtcbase/byte_order.h \
  src/rtcbase/memcheck.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/p2p/ice_stun.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/p2p/ice_stun.o src/p2p/stun.cpp

src/p2p/ice_stun_port.o:src/p2p/stun_port.cpp \
  src/rtcbase/random.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/ipaddress.h \
  src/rtcbase/byte_order.h \
  src/rtcbase/logging.h \
  src/rtcbase/net_helpers.h \
  src/p2p/ice_common.h \
  src/p2p/port_allocator.h \
  src/rtcbase/log_trace_id.h \
  src/rtcbase/sigslot.h \
  src/p2p/port.h \
  src/rtcbase/network.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/logging.h \
  src/rtcbase/ipaddress.h \
  src/rtcbase/network_constants.h \
  src/rtcbase/sigslot.h \
  src/rtcbase/socket_address.h \
  src/rtcbase/async_packet_socket.h \
  src/rtcbase/dscp.h \
  src/rtcbase/socket.h \
  src/rtcbase/socket_address.h \
  src/rtcbase/time_utils.h \
  src/rtcbase/memcheck.h \
  src/p2p/candidate.h \
  src/rtcbase/basic_types.h \
  src/p2p/candidate_pair_interface.h \
  src/p2p/packet_socket_factory.h \
  src/rtcbase/event_loop.h \
  src/rtcbase/constructor_magic.h \
  src/p2p/port_interface.h \
  src/p2p/stun.h \
  src/rtcbase/byte_buffer.h \
  src/rtcbase/buffer.h \
  src/rtcbase/array_view.h \
  src/rtcbase/type_traits.h \
  src/p2p/stun_request.h \
  src/p2p/stun_port.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/p2p/ice_stun_port.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/p2p/ice_stun_port.o src/p2p/stun_port.cpp

src/p2p/ice_stun_request.o:src/p2p/stun_request.cpp \
  src/rtcbase/ptr_utils.h \
  src/rtcbase/random.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/logging.h \
  src/rtcbase/string_encode.h \
  src/rtcbase/time_utils.h \
  src/p2p/stun_request.h \
  src/rtcbase/sigslot.h \
  src/rtcbase/event_loop.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/logging.h \
  src/p2p/stun.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/byte_buffer.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/buffer.h \
  src/rtcbase/array_view.h \
  src/rtcbase/type_traits.h \
  src/rtcbase/socket_address.h \
  src/rtcbase/ipaddress.h \
  src/rtcbase/byte_order.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/p2p/ice_stun_request.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/p2p/ice_stun_request.o src/p2p/stun_request.cpp

src/rtcbase/ice_async_packet_socket.o:src/rtcbase/async_packet_socket.cpp \
  src/rtcbase/async_packet_socket.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/dscp.h \
  src/rtcbase/sigslot.h \
  src/rtcbase/socket.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/socket_address.h \
  src/rtcbase/ipaddress.h \
  src/rtcbase/byte_order.h \
  src/rtcbase/time_utils.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_async_packet_socket.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_async_packet_socket.o src/rtcbase/async_packet_socket.cpp

src/rtcbase/ice_async_socket.o:src/rtcbase/async_socket.cpp \
  src/rtcbase/async_socket.h \
  src/rtcbase/sigslot.h \
  src/rtcbase/socket.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/socket_address.h \
  src/rtcbase/ipaddress.h \
  src/rtcbase/byte_order.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_async_socket.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_async_socket.o src/rtcbase/async_socket.cpp

src/rtcbase/ice_async_udp_socket.o:src/rtcbase/async_udp_socket.cpp \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/event_loop.h \
  src/rtcbase/async_udp_socket.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/async_packet_socket.h \
  src/rtcbase/dscp.h \
  src/rtcbase/sigslot.h \
  src/rtcbase/socket.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/socket_address.h \
  src/rtcbase/ipaddress.h \
  src/rtcbase/byte_order.h \
  src/rtcbase/time_utils.h \
  src/rtcbase/socket_factory.h \
  src/rtcbase/async_socket.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_async_udp_socket.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_async_udp_socket.o src/rtcbase/async_udp_socket.cpp

src/rtcbase/ice_base64.o:src/rtcbase/base64.cpp \
  src/rtcbase/base64.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_base64.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_base64.o src/rtcbase/base64.cpp

src/rtcbase/ice_buffer_queue.o:src/rtcbase/buffer_queue.cpp \
  src/rtcbase/buffer_queue.h \
  src/rtcbase/buffer.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/array_view.h \
  src/rtcbase/type_traits.h \
  src/rtcbase/critical_section.h \
  src/rtcbase/atomicops.h \
  src/rtcbase/thread_annotations.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_buffer_queue.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_buffer_queue.o src/rtcbase/buffer_queue.cpp

src/rtcbase/ice_byte_buffer.o:src/rtcbase/byte_buffer.cpp \
  src/rtcbase/basic_types.h \
  src/rtcbase/byte_order.h \
  src/rtcbase/byte_buffer.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/buffer.h \
  src/rtcbase/array_view.h \
  src/rtcbase/type_traits.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_byte_buffer.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_byte_buffer.o src/rtcbase/byte_buffer.cpp

src/rtcbase/ice_crc32.o:src/rtcbase/crc32.cpp \
  src/rtcbase/array_size.h \
  src/rtcbase/crc32.h \
  src/rtcbase/basic_types.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_crc32.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_crc32.o src/rtcbase/crc32.cpp

src/rtcbase/ice_critical_section.o:src/rtcbase/critical_section.cpp \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/critical_section.h \
  src/rtcbase/atomicops.h \
  src/rtcbase/thread_annotations.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_critical_section.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_critical_section.o src/rtcbase/critical_section.cpp

src/rtcbase/ice_event.o:src/rtcbase/event.cpp \
  src/rtcbase/event.h \
  src/rtcbase/constructor_magic.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_event.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_event.o src/rtcbase/event.cpp

src/rtcbase/ice_event_loop.o:src/rtcbase/event_loop.cpp \
  deps/libev/include/ev.h \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/time_utils.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/event_loop.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_event_loop.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_event_loop.o src/rtcbase/event_loop.cpp

src/rtcbase/ice_ifaddrs_converter.o:src/rtcbase/ifaddrs_converter.cpp \
  src/rtcbase/ifaddrs_converter.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/ipaddress.h \
  src/rtcbase/byte_order.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_ifaddrs_converter.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_ifaddrs_converter.o src/rtcbase/ifaddrs_converter.cpp

src/rtcbase/ice_ipaddress.o:src/rtcbase/ipaddress.cpp \
  src/rtcbase/net_helpers.h \
  src/rtcbase/ipaddress.h \
  src/rtcbase/byte_order.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_ipaddress.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_ipaddress.o src/rtcbase/ipaddress.cpp

src/rtcbase/ice_location.o:src/rtcbase/location.cpp \
  src/rtcbase/location.h \
  src/rtcbase/stringize_macros.h \
  src/rtcbase/string_utils.h \
  src/rtcbase/basic_types.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_location.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_location.o src/rtcbase/location.cpp

src/rtcbase/ice_logging.o:src/rtcbase/logging.cpp \
  src/rtcbase/critical_section.h \
  src/rtcbase/atomicops.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/thread_annotations.h \
  src/rtcbase/time_utils.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/string_encode.h \
  src/rtcbase/logging.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_logging.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_logging.o src/rtcbase/logging.cpp

src/rtcbase/ice_md5.o:src/rtcbase/md5.cpp \
  src/rtcbase/byte_order.h \
  src/rtcbase/md5.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_md5.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_md5.o src/rtcbase/md5.cpp

src/rtcbase/ice_md5_digest.o:src/rtcbase/md5_digest.cpp \
  src/rtcbase/md5_digest.h \
  src/rtcbase/md5.h \
  src/rtcbase/message_digest.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_md5_digest.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_md5_digest.o src/rtcbase/md5_digest.cpp

src/rtcbase/ice_message_digest.o:src/rtcbase/message_digest.cpp \
  src/rtcbase/basic_types.h \
  src/rtcbase/md5_digest.h \
  src/rtcbase/md5.h \
  src/rtcbase/message_digest.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/sha1_digest.h \
  src/rtcbase/sha1.h \
  src/rtcbase/string_encode.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_message_digest.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_message_digest.o src/rtcbase/message_digest.cpp

src/rtcbase/ice_net_helpers.o:src/rtcbase/net_helpers.cpp \
  src/rtcbase/byte_order.h \
  src/rtcbase/net_helpers.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_net_helpers.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_net_helpers.o src/rtcbase/net_helpers.cpp

src/rtcbase/ice_network.o:src/rtcbase/network.cpp \
  src/rtcbase/ifaddrs_converter.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/ipaddress.h \
  src/rtcbase/byte_order.h \
  src/rtcbase/network.h \
  src/rtcbase/network_constants.h \
  src/rtcbase/sigslot.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_network.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_network.o src/rtcbase/network.cpp

src/rtcbase/ice_openssl_adapter.o:src/rtcbase/openssl_adapter.cpp \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/openssl.h \
  src/rtcbase/openssl_adapter.h \
  src/rtcbase/ssl_adapter.h \
  src/rtcbase/ssl_stream_adapter.h \
  src/rtcbase/event_loop.h \
  src/rtcbase/stream.h \
  src/rtcbase/sigslot.h \
  src/rtcbase/ssl_identity.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_openssl_adapter.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_openssl_adapter.o src/rtcbase/openssl_adapter.cpp

src/rtcbase/ice_openssl_digest.o:src/rtcbase/openssl_digest.cpp \
  src/rtcbase/openssl_digest.h \
  src/rtcbase/message_digest.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_openssl_digest.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_openssl_digest.o src/rtcbase/openssl_digest.cpp

src/rtcbase/ice_openssl_identity.o:src/rtcbase/openssl_identity.cpp \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/random.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/openssl.h \
  src/rtcbase/openssl_digest.h \
  src/rtcbase/message_digest.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/openssl_identity.h \
  src/rtcbase/ssl_identity.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_openssl_identity.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_openssl_identity.o src/rtcbase/openssl_identity.cpp

src/rtcbase/ice_openssl_stream_adapter.o:src/rtcbase/openssl_stream_adapter.cpp \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/openssl.h \
  src/rtcbase/openssl_stream_adapter.h \
  src/rtcbase/event_loop.h \
  src/rtcbase/buffer.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/array_view.h \
  src/rtcbase/type_traits.h \
  src/rtcbase/ssl_stream_adapter.h \
  src/rtcbase/stream.h \
  src/rtcbase/sigslot.h \
  src/rtcbase/ssl_identity.h \
  src/rtcbase/openssl_identity.h \
  src/rtcbase/openssl_digest.h \
  src/rtcbase/message_digest.h \
  src/rtcbase/openssl_adapter.h \
  src/rtcbase/ssl_adapter.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_openssl_stream_adapter.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_openssl_stream_adapter.o src/rtcbase/openssl_stream_adapter.cpp

src/rtcbase/ice_physical_socket_server.o:src/rtcbase/physical_socket_server.cpp \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/time_utils.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/physical_socket_server.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/socket_factory.h \
  src/rtcbase/socket.h \
  src/rtcbase/socket_address.h \
  src/rtcbase/ipaddress.h \
  src/rtcbase/byte_order.h \
  src/rtcbase/async_socket.h \
  src/rtcbase/sigslot.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_physical_socket_server.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_physical_socket_server.o src/rtcbase/physical_socket_server.cpp

src/rtcbase/ice_platform_thread.o:src/rtcbase/platform_thread.cpp \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/atomicops.h \
  src/rtcbase/platform_thread.h \
  src/rtcbase/platform_thread_types.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_platform_thread.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_platform_thread.o src/rtcbase/platform_thread.cpp

src/rtcbase/ice_random.o:src/rtcbase/random.cpp \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/random.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_random.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_random.o src/rtcbase/random.cpp

src/rtcbase/ice_rate_statistics.o:src/rtcbase/rate_statistics.cpp \
  src/rtcbase/rate_statistics.h \
  src/rtcbase/optional.h \
  src/rtcbase/array_view.h \
  src/rtcbase/type_traits.h \
  src/rtcbase/sanitizer.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_rate_statistics.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_rate_statistics.o src/rtcbase/rate_statistics.cpp

src/rtcbase/ice_rtccertificate.o:src/rtcbase/rtccertificate.cpp \
  src/rtcbase/time_utils.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/rtccertificate.h \
  src/rtcbase/ssl_identity.h \
  src/rtcbase/constructor_magic.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_rtccertificate.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_rtccertificate.o src/rtcbase/rtccertificate.cpp

src/rtcbase/ice_rtccertificate_generator.o:src/rtcbase/rtccertificate_generator.cpp \
  src/rtcbase/rtccertificate_generator.h \
  src/rtcbase/rtccertificate.h \
  src/rtcbase/ssl_identity.h \
  src/rtcbase/constructor_magic.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_rtccertificate_generator.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_rtccertificate_generator.o src/rtcbase/rtccertificate_generator.cpp

src/rtcbase/ice_sha1.o:src/rtcbase/sha1.cpp \
  src/rtcbase/sha1.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_sha1.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_sha1.o src/rtcbase/sha1.cpp

src/rtcbase/ice_sha1_digest.o:src/rtcbase/sha1_digest.cpp \
  src/rtcbase/sha1_digest.h \
  src/rtcbase/message_digest.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/sha1.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_sha1_digest.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_sha1_digest.o src/rtcbase/sha1_digest.cpp

src/rtcbase/ice_sigslot.o:src/rtcbase/sigslot.cpp \
  src/rtcbase/sigslot.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_sigslot.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_sigslot.o src/rtcbase/sigslot.cpp

src/rtcbase/ice_socket_address.o:src/rtcbase/socket_address.cpp \
  src/rtcbase/byte_order.h \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/net_helpers.h \
  src/rtcbase/socket_address.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/ipaddress.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_socket_address.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_socket_address.o src/rtcbase/socket_address.cpp

src/rtcbase/ice_ssl_adapter.o:src/rtcbase/ssl_adapter.cpp \
  src/rtcbase/ssl_adapter.h \
  src/rtcbase/ssl_stream_adapter.h \
  src/rtcbase/event_loop.h \
  src/rtcbase/stream.h \
  src/rtcbase/sigslot.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/ssl_identity.h \
  src/rtcbase/openssl_adapter.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_ssl_adapter.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_ssl_adapter.o src/rtcbase/ssl_adapter.cpp

src/rtcbase/ice_ssl_fingerprint.o:src/rtcbase/ssl_fingerprint.cpp \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/message_digest.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/string_encode.h \
  src/rtcbase/ssl_fingerprint.h \
  src/rtcbase/ssl_identity.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_ssl_fingerprint.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_ssl_fingerprint.o src/rtcbase/ssl_fingerprint.cpp

src/rtcbase/ice_ssl_identity.o:src/rtcbase/ssl_identity.cpp \
  src/rtcbase/time_utils.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/openssl_identity.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/ssl_identity.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_ssl_identity.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_ssl_identity.o src/rtcbase/ssl_identity.cpp

src/rtcbase/ice_ssl_stream_adapter.o:src/rtcbase/ssl_stream_adapter.cpp \
  src/rtcbase/openssl_stream_adapter.h \
  src/rtcbase/event_loop.h \
  src/rtcbase/buffer.h \
  src/rtcbase/memcheck.h \
  src/rtcbase/logging.h \
  src/rtcbase/constructor_magic.h \
  src/rtcbase/array_view.h \
  src/rtcbase/type_traits.h \
  src/rtcbase/ssl_stream_adapter.h \
  src/rtcbase/stream.h \
  src/rtcbase/sigslot.h \
  src/rtcbase/ssl_identity.h \
  src/rtcbase/openssl_identity.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_ssl_stream_adapter.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_ssl_stream_adapter.o src/rtcbase/ssl_stream_adapter.cpp

src/rtcbase/ice_stream.o:src/rtcbase/stream.cpp \
  src/rtcbase/stream.h \
  src/rtcbase/sigslot.h \
  src/rtcbase/constructor_magic.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_stream.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_stream.o src/rtcbase/stream.cpp

src/rtcbase/ice_string_encode.o:src/rtcbase/string_encode.cpp \
  src/rtcbase/string_utils.h \
  src/rtcbase/basic_types.h \
  src/rtcbase/string_encode.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_string_encode.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_string_encode.o src/rtcbase/string_encode.cpp

src/rtcbase/ice_string_to_number.o:src/rtcbase/string_to_number.cpp \
  src/rtcbase/string_to_number.h \
  src/rtcbase/optional.h \
  src/rtcbase/array_view.h \
  src/rtcbase/type_traits.h \
  src/rtcbase/sanitizer.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_string_to_number.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_string_to_number.o src/rtcbase/string_to_number.cpp

src/rtcbase/ice_string_utils.o:src/rtcbase/string_utils.cpp \
  src/rtcbase/string_utils.h \
  src/rtcbase/basic_types.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_string_utils.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_string_utils.o src/rtcbase/string_utils.cpp

src/rtcbase/ice_time_utils.o:src/rtcbase/time_utils.cpp \
  src/rtcbase/time_utils.h \
  src/rtcbase/basic_types.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_time_utils.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_time_utils.o src/rtcbase/time_utils.cpp

src/rtcbase/ice_zmalloc.o:src/rtcbase/zmalloc.cpp \
  src/rtcbase/zmalloc_define.h \
  src/rtcbase/zmalloc.h
	@echo "[[1;32;40mBUILDMAKE:BUILD[0m][Target:'[1;32;40msrc/rtcbase/ice_zmalloc.o[0m']"
	$(CXX) -c $(INCPATH) $(DEP_INCPATH) $(CPPFLAGS) $(CXXFLAGS)  -o src/rtcbase/ice_zmalloc.o src/rtcbase/zmalloc.cpp

endif #ifeq ($(shell uname -m), x86_64)


