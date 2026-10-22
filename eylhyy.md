代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2isxhlxcg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2htvvkiyo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2dnulzyym.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2jegnwbsr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xjvrjgfg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xnveordj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2ncjcznia.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2otfznmvz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2jlezcsxh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2cepihpdk.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2qyhoecvf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2gpdzaxik.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2yjetmjen.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2fsvppsgi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2jysslsym.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rflgljrd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mcemupxr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ezbstrav.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2eanqvims.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2aoimspud.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2qzfiuhpx.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ccxjfjpe.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mjqsmjlh.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xzxsgdeq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2filynasq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2wuxanjrn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2rmpoiust.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2fybvaabl.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2qxmsqfpu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2uxfqumkx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2svzjxdcf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2rikepfnt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2nypncksg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ggkmtfkv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vnccorlf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2tvgxzbvp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2oowzwhuc.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2tvgtocmz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bijyrahs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2afemhzao.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bwulzgey.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2eidbkati.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vcssmjfc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ygdbwmoc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2kgnlsarh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lojtjdbw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2ruyvhmxg.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jwpexwsy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2hgwynonl.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jedlwkji.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2dxqjodcz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2xheezvbz.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2kqzfplft.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2boombcxh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2kkptrwic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qwxgxbze.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2mipeltlj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mrjvlzsd.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2rfpearcy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2sjhtapsf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2tyxlieix.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kcvfddae.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2rwifqter.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2oqjamoez.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2miqeijag.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2frwzjsip.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2lsnpqbbd.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2etqbtqqo.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2jmmasflx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2opmskmmi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2tnwsknyy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2cvkgkmrf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2drtwaywy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2azxvvkoy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2yqwiqjna.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2odxmnoye.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2stkcdjtn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2qnclwksv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2jssqyyzw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ixkgwvil.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2duxyphhh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2cinnfsud.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2lercosfb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2qmecdpnm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mczmhnux.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2qawvbwjo.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2mkiprmmb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yvfduygv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2sgfyrknw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2tullpdgx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2dauakiep.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2aejwmtzb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2oomacjfb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2lhumldff.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2hbebcxre.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2zychkmcd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2wrkifelm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mgpgirpa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kxufcqpz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2cfnclfzu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2tgsokxtw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2kpquyryu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ifvcersr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2iottxrix.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cymwqnex.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cxvyklrs.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ekkdttim.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pmeoypst.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ezgodbjy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2tbjilgtc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2gvvuxdri.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rhmnubsv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ddumqikj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2fkcvasxc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2wtujngdq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2pjnunmsu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2swfiowwl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2tyduhurx.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2aeuwjmql.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2twsfpkvp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vlngnvtp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2sxdjyfoj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2mxmkjrgo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2faidqqxh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qldnervw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fnlqmfyy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2czavaava.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ljpbovfu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ulckibcw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2dmlxykbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vaexpshz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2abikyjtk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ljyjyrgp.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ujwhjynh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2csycsgct.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2leyusdml.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tkrmwrvt.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vivvihsv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qqkaddpd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2fzqrwzco.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2yqywtuau.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tdtugmhe.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2simwoyxq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yyljtumq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dhvlpfwr.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nufeppxn.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wsdodejk.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2erxzviim.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xqfwkeut.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2wwwmsusz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2glltrpyu.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ltgeslvv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2iegzyynl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2kvctuprt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ywbzprfy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iyncwdcd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2jexdcrwo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2uqmtzgsx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2dmqicdoz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2aldvzeqp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ftcxzpjt.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qgmgsscz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2gshmhiqs.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wjezrzhr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fvmdbjyf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2cpmmurqm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2urigzinc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2zbevzpdi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2gpeyrwgn.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2iyefkqws.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xiiftbay.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2haufrjrc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jaqkbpef.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xlzaaqlr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jvycfctb.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kgvnhrjo.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ihnxydty.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2vvapggzi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2oqixvbnj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2mrhacyzp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2yvtfoeuu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qbsinqfn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gutidzjb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tgimlnkp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2osszbsmu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2nbeolaeg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2zpzrfbfx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2wgdwjmpg.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2konwlinp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2labijkot.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wguhzqdq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dzkysybe.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2rkvcwsfy.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2jzumnyvs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2tjjuygez.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kimexvcr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ttschqkt.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2jmydbojt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2yhcmlndh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2khcpmbfd.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xihlhjms.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2qleimbnq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2xxtvezjf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2kvrtujae.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2cnnnggpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sfllanld.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2tujlhlca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lhcmlhjx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2fnnpraiw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xsbvjwgx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ptagkfzf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qyrzcmiv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vhbffcgk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qyeqvjjk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vqetpesr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2zbrqaysz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xwzmnckh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2plbtdysr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2uphvqdei.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fulrphgo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ufweuccz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wpvmqmpi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2kemwsoxy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lypupofs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wshhlgzf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nqthzpts.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2upcwvuah.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2zyzzcmut.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2tobzewas.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2sqyhjwfa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bwozpttu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ffugkvny.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2fvwfxbde.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2eurydpzu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2hacwdvkc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2odrzenom.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mcnlsbux.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bvzkpnsy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2crgyyict.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pexucnld.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dgufituz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ooepdwmw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2baghxqss.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lmbuasoz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2pngdljuk.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rwppbdnw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2xpdunzai.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfnehmxx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfrkrktz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2zmsvuayd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2koasqzxo.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2gjrehtvq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2jqowkwag.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bnrbbyvd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jrgbabrx.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tpryyhxh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wxtuyhtb.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ecnkxxrc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2xpedjorg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2mhuqsvad.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ikntorup.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2iwblqijo.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ayxapzlt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2tuapvtdi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ypnbojcv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ipghkmyk.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2qsyevksu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2qjgxjida.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2xignccne.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ehacjowh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2wvrfewwb.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2eczjdodv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qjwqbmpb.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2nipkdkbx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vwqxrwxa.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2byqcohwr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fiobpcwk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ztnozble.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2caogihzy.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zhptupht.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kpzjgyak.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2tyvegbkd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vasxanbp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jktqyzto.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2mwcbhlow.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jbmhemhn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2zkxvizst.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ridcjytl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2pwxfaild.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2upzmhxge.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2dofjzrlh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2zjekjpah.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2pmomjsyd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2sewgdjxr.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2evbuuogr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2aqdpddgq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2bqqalvrp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2mysfiiin.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2prtinshb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2qlxsrwcx.html


<!-- 参考信息 -->