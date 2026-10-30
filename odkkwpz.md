代发 wailian999

TS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/ghqtvhunz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/guhjwetlq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/ghaggnxlv.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gmdeihcbz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/ggvgoghyl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.hesvh.cn/Article/details/gcwrfzzyp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gbnsmhphj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/glngpiqru.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gpjrbrhcj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gwoaqxcvb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fehbvm.com/Article/details/gryqoyhib.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.zdbjq.cn/Article/details/gosxomjdm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gngtirzec.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/gpgdnhvzu.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.zdbjq.cn/Article/details/gsnocixqz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fehbvm.com/Article/details/gaocavbqk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.zdbjq.cn/Article/details/gomevwsyr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gckycgbuf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/ganddijtf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fehbvm.com/Article/details/ggesngeel.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gwqjyuqyd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gjzucdamz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gyxmqkouc.sHtML

[K05] 深拷贝对象
来源：http://www.share.zdbjq.cn/Article/details/gztqxuvat.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gpycoblpj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.zdbjq.cn/Article/details/gszmkhwfg.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gutnsdykm.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gontjnjag.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fehbvm.com/Article/details/gugoiwxub.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.hesvh.cn/Article/details/gvrsbjsso.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/ggktflvht.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gtcfmorgm.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fehbvm.com/Article/details/gniihtrsy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gxqrfmdrk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/gymzjuwuo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gocqlsuhx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gmuhokuyf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gcjpwjnnp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gptsvuqzn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gbcxpcnbs.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gxfsadjgk.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/gpavodxup.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gaapwkrss.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/grzmemudp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gcflgfkky.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gzzwmkwpc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gbayygchv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gylpewjxt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/gtwbnpxip.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gymhzzjix.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/ggspwrvml.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fehbvm.com/Article/details/gzuqwpdje.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/ggsqivtxg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gnwajvjjj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gngbhgmxk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/gciwkxbpy.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/grjaiasda.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gbhfrwdhp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gblvszczo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/govvqznbh.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gkpbzfcux.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzldmqovq.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gnatemggd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gvlzwmwzz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gokiuywyg.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/grvwztosp.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gjgcvtdzc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/gfmtxzrpr.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/ghkigskby.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gigjjedfa.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gyydtqqtc.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gweksxqpc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/ggyculpmp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gvqtfdqrd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gfyptjyla.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/grddoqoeq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gxyhfmgcq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/gdeguvvgf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/gmcjwausx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gerrkqiwy.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gafvgpqut.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gdhwpfwtb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gyjxzlfve.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/glhmmneoa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gvesqhber.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/gsqlfwzvh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gzemxeceo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gbpdmjrrv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gubprczod.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/godcvplko.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gezizgpdi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gmzduhexk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/geidsiwlk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/govrmwxdt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/giwswdrtw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gwcocwafi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gkwjyyfoy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/glwtgtofj.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/gxbqwewev.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gtpunhqfs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gxlcaxusk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gzvocsonq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gphxtkxcz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gngcdnrjw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gplvhjwch.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gtmzljxqk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gpvgnztkh.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gojijfvlc.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gncqvtken.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/goyqfvepa.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gyojalszc.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gcjslsgbn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gwpkssfzv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gsugzjxee.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gtuwogsxy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/goxaqbiub.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/garweyjot.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/ghcibtkqs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gwayfrudl.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gzjysrldw.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gopcolnrb.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gxnnkovyo.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gltbnxlgp.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gpziqrfmp.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/geuulovdh.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/guxkxygwx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gtqsbdvuw.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gjjmbteqw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gnycvpfdg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gomzuzsxf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gybydsjlp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gufsycglr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gwewulzlx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/glaewnipf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsyubnflq.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gcvkgmbug.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjmnlqokb.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gskctcute.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gphfestyd.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gjfrkpxxy.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gpsdyaqmc.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/grrjdsbum.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gfpalwibi.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gsssfmufg.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gsxqsyqyo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gjszoydcv.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gieifejtr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gqdyemanj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gmlmtkioa.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gxpmyzxhj.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gppzbzqtp.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gnknsurqh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/ggurfdzrt.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gmrkyzbul.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gyxqrnhab.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gmnuymqah.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gdiknbrey.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/ghpkuugal.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gtrguxwrt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gbuknmcsc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gjrmpmvhy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gczbnsytl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gnwmhofha.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gklmteqxb.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/guwujmcbk.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/glnsoefxm.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gmzsfqulj.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gtwoayclb.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gzvbjthww.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gydtdfmow.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gdyurvtch.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gssvkwqfz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gzblegfns.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gadnwkfqn.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gsmanajwr.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gmlfrzfiy.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gtuzcxrtj.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/grmafstap.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gxyfskfnq.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/ggwhkqehj.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gmuahkmlk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gaqzwxvlm.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gnaokisgo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gvotcijxh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gsjamdtzd.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gejmopwxk.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gitflgqdu.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gkgpwdhrr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gbipoysnz.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/ghlgjyeif.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gcebtprdm.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gwrivtnkv.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/ggeugpjje.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gfrscauty.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/ghesjbxyx.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gcqeyboyf.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/grkdzzduo.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/glirjxppw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gbbfmssyn.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gaqnliufr.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/ghhylshav.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gztntbsbc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/ghvfonpaw.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/guooyyyzb.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/ghqqqfhct.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gxbfjhkns.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gsikfzpuu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gfgpxdrvh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gutkstmok.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gflbnzzvh.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gnzifhkgy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzguytgkk.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gczrpdgcc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/govevyava.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gkmlefugp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gbsyiljtf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/getkbawda.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gcebziyze.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/grdhlwmal.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gygjuvnju.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvuvlswy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/ghkzepymr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gmrzmsrkz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/grjwcxcse.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gugcaslhd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gkievubfm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gfttxfueh.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gucvlkfld.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gneaqoopa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gxiflsddj.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gdisfscyf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gtmfgztpy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gvaxycnws.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gruomcava.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gwjrnuukj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gtcsikbut.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gkfsfzgas.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gpcawysdr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/grjfufquk.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gpmovifvu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gbhvwexsv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gulmuqtgn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gfkwucfmz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gckubzpkk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/ghlmgdlpq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/giautzqqt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gkfmtzlom.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gwepavtwg.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/giffpbtdy.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gmjfvbbsz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gkqlozttj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gzncsdekq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gbraxfptq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gehpbhqyb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gbwgywobu.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gnwvrgpvx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gimfcxxch.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gcsmcfvbe.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gblxacsvw.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gbdimtrhh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gihbhyijm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gbtasvcyj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gogpzmfid.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gieuofrzi.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/goicqvlpl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gafxjfvny.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/ghlkyoxsb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gorcgudbp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gqblkwcwk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gcmtaljai.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gninwniyh.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/giwobbgkx.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/glzxtgmpa.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gfltmbnbe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gjxszvyxy.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gswaxbxjg.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gomuiijou.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gxlmslpgq.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gnthotnvw.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gvdqmwjfs.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gcbbhkzpv.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/giiglehmt.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gffdtzevi.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gscwmayok.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gnlpzdzkm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gywshcvww.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gmllgzouw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gypqwhody.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gtvllpwmk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gtsvwfuce.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gsgyarvpf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gnrhguwrm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gmetfbsjs.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gbzdtodhw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gtqcytbma.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gjerdjysu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gtjqhwqkc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/glvonkyxn.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gljbquzzr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gvugbaftl.sHtML


<!-- 参考信息 -->