代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2jcjfyehn.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2movqazlz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2niuattcg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2lgxqxngj.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2capclrep.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2webakjbv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ijskjbjm.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2lpbwfebq.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2gbfvxiwh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2aacxbauk.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2reajtoix.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qgwaluvx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2kkluhwsz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2uxpjqhvt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2qvgallyo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2qyaiaajb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ryxbdkzy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2olrobyts.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2yjtdsufu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2udiwzydp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2mnrzjvkj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2luelcxqf.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2mehobdcs.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xqsocevo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2hqzipbep.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2nnntqcjg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2pjkurwzn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ebsxugql.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2bipkhxeg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2tfrqmgxb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2qskhblbk.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2vvuetvjh.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fzklenec.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2tcesodhv.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rdbfkoxt.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qfxvorah.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2mzcufstj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2wowsilwx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2spljydlv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2rxcomszw.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2hvrktcnu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2vriusair.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2qeydtryb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vnxbqgng.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kikfgkpz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2cvcwrdcm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rugaytkk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2syvtdqaq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2pyauntpv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2qujrianh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2asrhmekd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2dlotdork.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2sgmrqmwe.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kdinubck.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2oxlsbdrv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2rvitcdji.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2robiabkw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2iegkxvww.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2jxwpjqwm.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2apxuzmgg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2macptxsw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2btarfnsu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2hrksqznn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2nilfxsiz.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2tfocehno.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2dprgqsrn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2pitefeyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhatqtzf.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2biyasblx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cradwnnu.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2pgptzvbo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2xrcoqrme.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2qfgaofix.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2avcyyyfu.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2jltuwgvg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2asugfksd.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2rhqciebq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2tahyjkci.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rutfpjrf.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tzfjbbsb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2jgbdrqew.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2cvrzipzv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2mxpnjknf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2tynimrwa.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2sxlnlsmx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2wwleixjj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2gjytfhdv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2gcjjsudk.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2uwfekmmr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2gtlesyzp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2syoiytlz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2qhhwujdl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2adhtzbzn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2hiubawme.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ypghkmdh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2pckwjxdv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wcwaqvlf.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2mxepsuaj.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2commkjvt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jrdepesy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kqkfzxxk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2qilgadvh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2whsymzyt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ehiglwii.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2cedeumtt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2qqeqcovg.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2afecavrf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2zwwiuzbe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2pmjvrnez.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2lniujizm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2orobztxk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2pbnjwyfm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2thvdltty.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2dxgcqsps.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bkzkghys.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wulspdjt.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2usfhpunp.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2lipmkvdi.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2tnllwanf.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mhhdedxi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vndnfeou.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2hixeaouj.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2dbejinnp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2qjzbbhmp.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qtyprznh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2kvhxmfll.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2sfvwvcnd.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zexvttmj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2amuvsgew.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2halaofim.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2emcypmpo.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2xkzazwpj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2lvqifpto.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2cnwhfxpc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2klvslazv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ejnvivgb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rfehrfje.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pcqdrrke.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2tuxqidqj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2lymoylqk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2fzknsieo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pxaqvrea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dkenopna.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ipczwdxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahqvrubb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wibgikdq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ilxwccgj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2lawogmyp.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mdjogjbs.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tkqmynms.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2whowblax.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2gifyutwn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2wmgsrssh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zmicdxjk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2iczglwgl.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uqslvpyu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2soxmuiin.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gckcxgwa.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vggsocwm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2thgcflip.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mcqdavso.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2llhpkkjr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dfpzhylv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ugjvnjmx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fromafdq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2npmsmhck.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bhcsoutk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ebffujcx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2bgtntymk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2kzbfyhpg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2jrajrckr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2zfjqkbiw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ofdtblcb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2lznjlmai.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ggiaroay.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pwweqvbw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vhobshkv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2yhhcqxvj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ooupeeri.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2jlyhknsr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ehdjrjaj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2taoqxftm.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nekvqdqg.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ebtmjikh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xdhxhzjf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nbbvectl.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qufzueko.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ffzomkqt.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2yvbenbfu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2wphbeqxj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2lqcdfnjj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2exvswcmx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2dsmefpav.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pdkivpor.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ncxcqbdf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ehgbfcjv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2efdxkeda.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2okeiinwe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bhnnnpcx.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ptyupoic.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2tfqsmtwt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2swwkzqjl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qatninss.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2oeutvdft.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2hddlbfcj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2uvkvnkjp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2umjaldfk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bsxjumem.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2vdrzqirx.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2cigajpli.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2eremvgfz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lxpzqxag.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ddplnbho.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2zfirlftf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2vdkhucpe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2mhtnsgqt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2esczqsud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vudpbbzd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2bxlwbkpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iradijkd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2tfdaozti.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qynskuhf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cvdgpvvl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jjozeesy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zyfwwkjh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jwcodrgm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wyvqkbox.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ybxlgqcr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dmiefgek.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2suhpzcyf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lwmttefg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2cduhkrre.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2armjqyrk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kkpdumhs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2vhmrxatq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iekpkxlr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jyxbayde.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2widxunep.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2stvwnwjn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2wzabiwyl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2arcctnss.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ywytokru.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pavodcez.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hzosjxnw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2wpzwcpno.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2qtovycnn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2aybypubp.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2zlltsvli.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dcylrvyd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2cpdaodge.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cfbgfmwf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gkujguqv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2desrjsuw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2cbyzflvs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tpmkelne.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2stobmdvk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2hdnfavio.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2evhalkvf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2rmddnaiy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2fbscnely.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mswwiuyu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2gglmskgm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2garitbta.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jocxdxal.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2xlcevapy.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wmwpvayh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2cmdszmoo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rporaqgg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hveuknws.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nadpsfqd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2dpcxgvtx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2mxofkpvp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rmpthjkm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2vizijwlo.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2lvljopmm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2dvykharj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2kqormgdo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ennxcxva.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2banfcfez.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2lehlitgi.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2gnebxxiz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2pcmeewwr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2vbywcnir.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2xbfqslog.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2upocnuiq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2qjnnkyby.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lpbvgrcx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tbdodjvs.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kxqbptzd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pflelqtg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2dhwdgxig.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mqpeucrf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xoxlarmx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2jkwlijol.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zggbueiv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rvjjwhdo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2cqlgvkdi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2hmqbneba.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2vmlhmrhp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ijfpbaqi.html


<!-- 参考信息 -->