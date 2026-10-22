代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pfgtfjcq.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2xhfbtogc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fpfyaugb.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2vagixarn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2tpatbugp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jbzzdsjf.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2blqkfmqf.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2rvpjayui.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2yktmpvdh.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2hkutuwrp.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2spukauek.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2crlhpcfd.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2erjdzkov.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fvcrwbgs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2zbdzkopx.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2twjpanxx.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ujhtjink.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ixuiohya.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2wxtvujzs.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2euamorhy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eenqnzjp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2dkjwwnea.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2zypcykjj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2cngzvmbi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2iikrvddf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xjhmlyuk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2sopeiwqz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2yegvtshx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2fbzzdtcf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2xltfkstv.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2arkghfhb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2uqasezsz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2elbcnnqu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2qiplspdw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dzizvsop.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2klirdnmw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2yjpvkqbk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ealpnwpy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ecfdnrkq.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2eunqvzye.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2klqgyfpz.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ttetaoff.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ubarerir.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cijjrocr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2hizobkpm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2yzrqjwep.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2fyeifwsr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2sxobjiwp.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2rtragbwx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ymysjlew.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2nbdpcuzu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2zcpmmolm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xafkksmd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2hrarxriy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ixfmrvja.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2lasvwguk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2mdveabfl.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2kvptrpel.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fgiztzld.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ifwjmhmi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mqavzevo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sdrtmjhe.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bptgxjcu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2iybpqyyv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2axjmchiy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uixaicbn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2wwdiwtdb.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2evicdawr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2lfdbmsrk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zmziaqux.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2loetnmzl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2hbnjluwr.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2mjjziyxj.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ykpwkysu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2dgogzgrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owfumupe.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ymsemsbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nneiiept.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2hbcixcug.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2wwsfboaj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2mrobstwn.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2rcfbvmww.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2rgvuqixn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2toxillqn.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wbuzfoyf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ivtyxaoe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2uheamltg.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2kljxwpxb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2musifagu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2vzawrllt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2lpihbjns.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2tuxmgtgb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2cwzfkipf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ugviwwbj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2rreavzrv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2iwfxeufz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2fzpuqypo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2kvfphsck.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ittjtzka.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2dflkxkpo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2tainyuic.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2jqdcidfq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2jhnamnuv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ftexbycr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2avpatbrd.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2vjovraxe.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2gkkteelk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ylikadxr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2irqtliil.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xbjakqqc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2oflfqxcq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2zusnnhah.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2dfbqdqwu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2dgnkvaxd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2fyfgswlk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2mnbmnenl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2qzehpipf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2xsvpwlcu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2dhfifkpu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2bsebymrd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2trgaywma.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2mihjtxbk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rfgdvrpi.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wclwqwqm.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rlfpntpd.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xoepihcm.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mcnpcfpj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ekbrosvk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nmdsutrj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2qxqkjuli.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2cyenboba.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tbglyhya.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2uvdubxgd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2hqlupnfh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2uzfpnhof.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2bcsyutte.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2kjdroijm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2rpsupnrx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2trwvqbux.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ajdgauoo.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2zafentzb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2iidwixns.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2mvmgxyrs.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2bcabnvtx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2yqxmuupo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xebbtuqn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2umqzsugl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2rihnobcw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dvtwrngr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rzdnfglb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gfqahflr.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2dwmbaakz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jblrcjkh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vsxqgmnf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2fmtbbdnf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2sdyueqpg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xstctcbl.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2zeoxkyhn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xfpbxzua.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dbzwbihy.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2uqzbvxzr.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dayvfntr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mbfulsrf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2levixqvc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xsxrxbrm.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ohkcmmdd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2tikkexfa.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2flehgwpj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cfoamtut.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2gzjgsqgs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hxjqzuwt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2yhtnpirj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ycxavuhl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2zlzrdkyk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xwzdmpzz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hsdbgzll.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ibsjakkp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2znjiyfyi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2jyzopjme.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2gmjjenfz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2hcadfxed.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rqfxwadj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2rnbmayuk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2okzcjlxw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2szuifkeb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2eytpicvr.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2oovvmusz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2xpzqouch.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2uqeqtaiw.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2pdvhpswv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bigptkot.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2kzuuecja.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2smpwfkoi.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lijmwinu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2sbgodfqi.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ehtzrypd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ldlhbopp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2tgcijflt.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2oisaqtsh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2eahnllog.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2jmlhspsa.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ucjqulaq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ruqxfsil.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2nlrwwbpu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ibpjdwrf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2zrysotwd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2jwaoisbb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2fdxkaxkk.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2krcihalw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2kptyaycc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cnxknhba.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2kdkdxmpo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qtrmiysd.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2chweflzb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2dggojzeu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2hqdrwxyu.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2osxaywdm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2lcaahrsl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2tsswvvai.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2shxgdmnz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2siyieluz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2xjxznxdl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2brzjueif.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2wyeeyzlx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2fbafahkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqyyatjn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2dyogdmrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rrpjemqe.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2jyymojdn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2htjicflh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lamnexvh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zmlopggs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kuwulzou.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zdshflmy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fzapiapd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2wpnwffhp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uuugsyvi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2fqdlmrep.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mvepnhni.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xuybmwqp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2isnvoisy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ckqzapsj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2yvyzkqup.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pvihkhah.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yvkwrseu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hvkfrseg.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2atryrygn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2vjsuhivq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2xazpehcg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hlbqddwa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2eegqsvlo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yzbbqxiy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2pkhdqhuz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2oehvmzof.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2kkxtdzsy.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2svwumhrm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yonzqzqp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2basqgweq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tkaitksm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2euydhcdh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tuvltssb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2lcuyufdy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kbrruitm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lemieuoc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2nzuxhecv.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2muomvgxv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkynufpt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2czzfjmdr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2uglmcdhy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2djhbytoo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2rldagwtj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2nqwthjcx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2dqhcgocd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2qwyiynyw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vzrexmxv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sazowozh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hyoyhrtv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kbjruute.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2jremcepi.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2fciakudj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gqqbpgon.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2pvocpnak.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2mklniumc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2vhumnvvf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2wagihmzf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2obhpdohf.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2mihlqyyz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2nzshshiq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2gbyxhgqy.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ycvsvybm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2tgcpmiaf.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2guytbmyd.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2xyjqzldr.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2holopumu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bbrkjphh.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zjfigwck.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ebrqckcz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kofllebn.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2eglllcav.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cxdhkucv.html


<!-- 参考信息 -->