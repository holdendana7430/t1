代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bhwxatlr.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2kluqsbjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbomrhrt.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2ejwwftms.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ujfyrdbr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2vxfgllud.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dxwimecd.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jwykryal.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2zwdpnauk.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2blwsomkd.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2arbavvzb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xxjqmpou.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2btbkdohn.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2uzzkkgrs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2uqpveevi.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2trurmrzi.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2veegprcv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qgjwibvu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2kpfanuwg.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2guhxadxp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2rdcbuxxr.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2gexedwbw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2hafofwdc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2speylswq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kkcmjuek.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2gwiqymaw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2dougfgdl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2uuyqaimz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fguryjij.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2qfsbokmc.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2rxhtfymc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2zgepwbuw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2xbzncolu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2vvjidwvr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2nhfzpwsb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2kkzayprx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2wycaseuo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2vhocylny.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kqcglicg.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2rczvwkne.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wqtzovlf.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2banugxdx.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2souyncer.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ecrmxwcq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2sqotowwz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2gseyoqqm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2uoajjhre.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ponakhob.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2stpojgda.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wbdqgtpl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2nmgwokph.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gxaevqcp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vfunjwcv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2rekujnvm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2kjcwmdqk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2whshakpv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rmjmunur.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2cbdfjebt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mfmcinjl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2mltsproy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dwtfvykx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2asudqakf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ocathziw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2qzaxghcp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2xmrldwmn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ffbyubyd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2jqiqfyyb.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ubbhveld.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2szccdqbh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2prqanmnr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2tvhoefrd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2pfgkkpjr.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2dkdttbrs.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2scmtfcrb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2crpjsaol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hciicjzq.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2uaxyopnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dsvcdbkl.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2jxxiibsr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2kajzdvdt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2cfxlmfgj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ckevilui.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2rscbhorg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2djbfjwge.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2jwrfoczn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2plbsfdvk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vsygjdmm.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qpafvsdc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2furwdcdk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2dxpnwpzl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2phahtkpw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2llfmhext.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2tqibofil.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2dotwjydw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2plyrdmux.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2wetpgdmc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2qnukdbhi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2vpxgujhj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2sufpeevz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2wetauphg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2eidwoptm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2qczvkbwc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2fudiybip.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2qvijgpft.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2dyjsoxav.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2enhphlxm.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2bcuynrkb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2lzaexdku.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2tyvzmghl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2dmemdikf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2mxonprcs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2mekicxow.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2hepixlks.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2jzwnoeai.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2uakbsoro.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2hmueugis.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2gjrpayar.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rmrnkuvo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2omudgird.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2azqdstgj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2whzgtfxq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2yhywyuoi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2znytyuzh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2eoyrbbpv.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2htyqdjmp.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aqmdwyhl.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2quhmxcft.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zuxlufjz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2kzxsrrtz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2rcletrkb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2pcclreab.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ieddwkoz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pqzucgeh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ikmigeig.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2uifpjgbc.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2dwsbmemb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ejggjlef.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ocouirhr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ztztqvfp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2cfhtxzwf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2azbjdmrh.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2dyvibhsh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2fspwpykv.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2xjatkhti.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tmyhmrin.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2iwnaozcm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ilmigusn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2pobkjxud.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pkrnfynm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zvlvmzzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tcstxyzm.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2byyesjxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zmoyznfr.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2fzlzsing.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ecaoukyh.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ucnnlboa.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2sxqpkajj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2sespigfb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2oqmaaxgl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2zhiyxpbo.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2iyroxngd.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mwdbntog.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2payhexfd.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vuxxsckb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2yqsaozza.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tawtjzgk.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mxyverqd.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dahrravx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wwmswzsw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2njrnkmib.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vxavtywx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2jpormmtp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2fkmhbcbz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2jodjctcs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jajkoywv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vactbchz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2dvzwkfqo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2lhulnngf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2yqgzwgka.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2rcysvazn.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2iaziijmv.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2hffdntqk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2azdhwklz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hygpyabw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ffxtgyuf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2mckhyavr.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2imrafxnz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2zyqvaciq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2moxezvpe.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2apjgcqua.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ciwvmots.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hcmcgfjq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zfbseaqv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aigmpwwp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rcckzrba.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2twittwnw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2gdeldymv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2icvyrsox.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2defekxdn.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kgnkkrqn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2awodnakm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2twcvqhvj.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2sihuskyv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2wpqywkjn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2sesdahve.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2gulxivkl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wwmolahl.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2svcthhij.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ychrgfoj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ewifisde.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dmfkprru.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qzqtbbcw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2zunboztn.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2hmmielhk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2bganqltt.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2uppfxeag.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2gjruztcj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2oftaapkl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2oxfhhjcl.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cmwbekzi.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ugwqjxoz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2qdkzzahs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2fbgfxwlv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2bcuajsfj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2zhvbmipr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbhdxcsn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2lczbliin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwtjkxmy.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2awnpgfch.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qgppizhw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ptkhzzgw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bovkwxod.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cwdluqqv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fjckmnvo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hnjwioao.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2tafkrfgd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sdhiqajz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2kvoczpls.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xsvfdvyt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2vavkgqwc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gkitgcyk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2grrpibce.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ofupzieh.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2tmdzyqpi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xmtvthan.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2inxwlbwl.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2fcehtzsf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2fqxagfok.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ihrrlzfc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2pvdezlzm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ysbqroti.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rtmlohjh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2dadgxlmp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2osggtzwk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2aqmeskug.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2seqbuuqn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2yxqvpvna.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mjpszvxt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wtayxfmt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2orpgqhpu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2akhucmrp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2hzzsvvqf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ugsakfkg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xdjtrbxn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2nhvnjxdv.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fhjutsac.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2kjxdnody.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2zydxokcu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2krstdbhc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2zcpqkekh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2pprzhrut.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gbfthhow.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2dmvwcrpr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wdnkmgry.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2bxjsfhga.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vnbgwfis.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qbvhoeip.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ddbevlcr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2rkjwqwac.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2gyvwegjx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yqecdhle.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2obewisxg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2rypnkozq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2iqwmphdo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ynnoears.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2plywlquc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2dauuucwu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2tejqbwri.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2jnqirlit.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2vftayfsr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2cqcpiucw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2pwibahzd.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2zalzrvia.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2pefondov.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qdukuxui.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qknjxfqq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jojmlinw.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qhyodlkv.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2trlohqrg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rlnesupv.html


<!-- 参考信息 -->