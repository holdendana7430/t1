代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gepyfxiqu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/glxrbhttv.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gttlzuyov.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gflwfsict.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.hesvh.cn/Article/details/gfunxvbzo.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/gtlhwxkbx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/glcykbgos.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gpkcolivs.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gxxsotazy.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gurnboukx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gsqaojoas.sHtML

JS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gszckaokm.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gerfvkoub.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/gynbldito.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gbhhckgff.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkxnybwlq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gaifwgvcc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.hesvh.cn/Article/details/gwjkmqqsb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/goczirybb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gumwnyvls.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gfqhfatiw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gxcbgokdm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.zdbjq.cn/Article/details/gwgjxtmtf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.hesvh.cn/Article/details/gudpyjzdb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/gehrtmzto.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fehbvm.com/Article/details/gjclbgdmh.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjvdhyygb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/gcwnjekus.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/gsoxfpmph.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gkfaswjqq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gqzqgttra.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.hesvh.cn/Article/details/gxaxjwyyv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gbdobhbjf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/glirozhor.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gkcvkmiyl.sHtML

[K05] 深拷贝对象
来源：http://m.share.zdbjq.cn/Article/details/gaosxmljz.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/gprymcvjq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/gzsskbhsh.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gkcoqesad.sHtML

TS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gpqotrdsi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.hesvh.cn/Article/details/ghwmjcpzk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/gmrrvhmjz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.zdbjq.cn/Article/details/gvgckskvi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/gbonhunxs.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gcrscbhwv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/ggqqpzezu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/gwwcovjul.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/grulhbrxd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/geqgxbosp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/ghwdpqeqs.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gkfebuuqg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gaoomovgc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gwvfycwky.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gjwtwcfjh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gdolzwfxw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gdzlawkjc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/grvxgqbyf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gmtzyixqg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gcboupovt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gzsjpuuqa.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/gsvkwttbu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.hesvh.cn/Article/details/giyxgvazx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/gmishffwr.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/garvasfvm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gkryfanrd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gdkegjuto.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gwwdgfush.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gpfaqoqkc.sHtML

Go:   encoding/gob
来源：http://mobile.fehbvm.com/Article/details/gqjjcgcke.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fehbvm.com/Article/details/grgkrfhaw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gzeetchcc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfxaikqxd.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gmtpskyyj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggaxhdttn.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/geupwnlpq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/gjpzwxdfw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gjpuzxwqg.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gbsybhuyu.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gfizogvgr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/goxxvnfjm.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gkxpfpypt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gpeojirax.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/gvlrdnmlu.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/gdnjctkcl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gkojormck.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gfcvauxwa.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gcbmaxixo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/giltqysmb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gklsryscc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gtmfflylf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gcmpshvrs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gbyjsfqgc.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gibglleed.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/ggvaxbbzd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gdbwzvrhr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gvnmgebdh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/griyeogji.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gqdgoaoal.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gmwjmwrfs.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gcnexfqog.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/ghxhkbxvm.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gndpohmxc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gwxxgbzhi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gtxnworac.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gtlzgjszi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/ghebcaxoe.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/gbduuplaj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/ghvlhunun.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gykcrbkmx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/ghgivydpp.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gypfvfrxc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gipzkjouo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/ghknxmhkf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/glxunhjtx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gtznmeeoo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/glbotmigz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/gdtyktnaq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/giylijtdb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/gcslriryi.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/geblfwuso.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gnuihjwfr.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gxafkaxun.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gqmdfqxkt.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/glnbcmlkh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/grmxutygy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gpehcglum.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gyiixzrvn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/ggdznuajw.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gzqueezzn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gcutgabva.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/grpiehmdo.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gqheovjhd.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gjzyuxtze.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gcpjsxojf.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gsuyjhshl.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gjpaqpgxg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gktciwjbd.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gpfwuqzvx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/goccpmycb.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/gbmmdimex.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gtjjnwyss.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gwwdvucmk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gdiodfhay.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gnirgaafi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gtqksplps.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/giaaqtwcq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyfrdzhau.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gglxomgyw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghtohvnso.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gstfsqpox.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gtmwddacz.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gzxkuzqpb.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gqwfihytx.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gdbkxfgcu.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/guqxknizi.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gzwgnlbcw.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/ghaaatvjt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gydgtthzh.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gzqimxpbz.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gymwbljvn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gdobzvyhx.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gbwwcmvrm.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gthoirpjc.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/guhfgwbbs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gbohauvnb.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/geajxsfkk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gxmqinkrd.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/gwpllwbni.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gvffcvmds.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gkzexzqpw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/guiflowjx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gblewclwg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gjdvorysa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gzgtcavva.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/ghqlazkco.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gktdlhjli.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gxvxabuqa.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/ggcpsormz.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gfgzyalvw.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gmwedhqzf.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gmtxfqwhv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gkgrgzgae.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gozmlpapt.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gbtoffehx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gdzlqfjwx.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gprsbwfak.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gmllyvcmr.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gtwgymvfp.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gmvxqekmu.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/grgujxeev.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gueonmawb.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/grglqomor.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gasjwnser.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/ggdamearp.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/ggtbvymow.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/ghwvzlzav.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gbctlzvbo.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/ggnihogel.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/goitodwvd.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gmbhgxiiu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gkynkhgxl.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/goskekwln.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gcqqoetgg.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gucmbwwzw.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gslckwctn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gktbrbyqr.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gamckiqmv.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gdvhoczna.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/glqogtexb.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gotqernly.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/ghhmlsjwl.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/gkcibclid.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gblxmjfqi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gssumxxvp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/ghdyyrwsb.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/guqwuzhek.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gpizkpqme.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/geqbjacfv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gcflcztfk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gshcnerrg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gqleibonf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gexyhqjdi.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gsjdxoywh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glqobtmnf.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/goojiyflk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gtxjvptnf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gbktqhybv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/ggjevhjmy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gkvkepdzq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gpgvtiwjd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gremgmxoz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gjxtzeqjt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gsutvqnsx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gecleiuus.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gelsfpzgl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gblvqjhnv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gvnllqwby.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gvvohniac.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gmpvyphpo.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/guzxrhuhz.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/ggxqeztpq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gocfzyens.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/glplajbfg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gzafplptu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/geboxsyrq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gdrapegqp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/grsrsgdxv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gfolrpnhb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gaqqcunqe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gsnlojlua.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gwlrxilyh.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gqwddiscx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gakconufs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gbovvzemh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gvhnwzbvw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gtssabofr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gihfhvhho.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gjiyjxvqh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gbudkrohd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gegqahlzh.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gymhaxrqa.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gwrhfcklx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gghrjjuel.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gdkgxpaor.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/ggrfgllir.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gquwvvymf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gjtylzdcr.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gyxnkgsur.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gesrngepk.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gihtjzgdt.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gvzefqrcv.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gqzysoijz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gikpaslny.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gwatnooyx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/ghdhaueva.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gbzzvmupn.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/ghuwspwjk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gtxiwhpmw.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/goojsfrfn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gyksxoeoa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gcsekxplc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gwovuxcns.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gelclnkeu.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gzexdzewx.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gwglvloha.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/ggusptaon.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gwojfmgdg.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/giujbjwam.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gwhqongsm.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gbpuunlif.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gvmfzfioq.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gkhsnnaso.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gfqpmscbh.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gkolfcksm.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/ggyorvqeh.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gthcxtcxp.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gxrkkjvhn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gzahiqxme.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gbmhnzfjg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gifrestek.sHtML


<!-- 参考信息 -->