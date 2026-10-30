代发 wailian999

[K02] JSON 字符串转对象
来源：http://read.share.zdbjq.cn/Article/details/gtoooajjo.sHtML

Py:   json.loads(s)
来源：http://mobile.zdbjq.cn/Article/details/grsnnlnme.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.zdbjq.cn/Article/details/godstjmxx.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gvcffxujr.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggzfnxnpa.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/gfdiqnqvi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gqzryzwfa.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gijdwdasl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gzrqwngcn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/glwoaypev.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gsncwpbdt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/grbmdyenx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gkqfexafr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/grdfsavpu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/gldgqigvq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.hesvh.cn/Article/details/gqyxwgrnl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/goodteton.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.zdbjq.cn/Article/details/giqzxpjuz.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gkdfxemlo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/gesnjebuw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/gpralwlyg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/ggovajcjf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/givyrqtgv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gelfbkelg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gvrkesopr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gjymcxdqd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gdazcywtz.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gtffzjsup.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.zdbjq.cn/Article/details/gdtxhuhwl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/glkgrhbiw.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gbmrgzwrh.sHtML

TS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/giwzomheh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/giudlmolk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/gepegegtt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/gkcpxammx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/gjwahgjvn.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/grpinslwy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gqjjrqddj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gkdaehxxi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gtzzidmhe.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gkzpovmgh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/goyjjjequ.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gsyvavqpz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gsuplhoad.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/grqtndeog.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/gckmlgdla.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gkxedqpxh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gmihycdut.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gdhiqivav.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gkbtqrysi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/glzzasden.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/gpabhudpr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fehbvm.com/Article/details/gjybgzjfy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gomzeshai.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/gumjtzlnr.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gbztalcnp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gpbznrtva.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gzbpfyvfu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gqrzvafiv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/goefywyoi.sHtML

Go:   encoding/gob
来源：http://www.blog.hesvh.cn/Article/details/gaunsexer.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gtkcqfxbj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/godbwclee.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyxjrxkko.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gszshcmor.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzipumetj.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gojplkjdg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gelsgocso.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gugnxmlzp.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/giynqsvso.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gbgzoropy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/gnsjdozlw.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gawcgdgsm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gjtfdwzah.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/gkvgyeaqh.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gfrgpxczc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/ggphsbpha.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/gyymbcwzv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/geuibclpt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gzhkbljcx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gloltcxba.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gjuxwpezs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gvpqulkdn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/gxpsuyabv.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gjkrfdtzd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gaxuotmcj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gyisqlslh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gdcicosju.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/ggwudyjxr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/gbrfmhdnb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/glzovbhat.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gyazejlla.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gkrrqdubc.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gaakpnzmj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gusiqiysn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gmypwjlor.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gypwrfaaw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gmhbvobmu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/griszjooi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gvkopmdrk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gaesvpaan.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gdyvhbqnr.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gmobsjbol.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gzvktqxqi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gfivzmjac.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gdetvesni.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gdzkdzows.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gdxevbozf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gcyfphaea.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gyerbynwh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gjsbnbhbm.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/ggcavdcao.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gyopqnjgx.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gvertfhjm.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gafdtbhcj.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/grgtfppbt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gktuyerhh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/giibkquyo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gkpmfqknl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/guiorpetf.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gbbogkjqw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gdiilenpd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gvutdditu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gsnhvpnfm.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gelfmjutz.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gzxufjhak.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gxncakpjf.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gyfbirusu.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gixkzgroa.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gvorbrekc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gpeqptozd.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gjwtulyxz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gnvuraidd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gxmphuopx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gpgvmttqa.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/glzcwiqii.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gjdjdneva.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gjijnzprw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmsjpbulr.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gsadxhpvv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxsgzhsqe.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gkircotxk.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gplxhinqn.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/ggcyqlqcb.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gfnfqxbnj.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gbdazpsyr.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gdoyvvtgf.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gglkxfjlz.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gpsulctgj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gdiztnziw.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gjanuxych.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/geyjllbrq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gppcmzwev.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gighitiga.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gkowfhiyc.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gwcpxilse.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/glbxqtrsq.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gcxlqrchq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gicdxhyrj.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gmjnhfsbu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gesxivckb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gocclvdei.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gkihapajt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/ggdtwqlsr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gtshmkhfw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gdvdkiyja.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gsuxmpzxv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gxyuvbevi.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/ggvptbzqz.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gsnsvzemg.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gajdnsvqa.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gpmxujtvr.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/glcuzkdgj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/ghkuunhif.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gmxgwsgpw.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gvrrtdrtj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/ggnhpxwwn.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gvjvzfkjf.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gnikignau.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gruidzwnz.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gbnuyvzod.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/ggpcpjfjx.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gpnjrzncp.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gkkiufbes.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/glsjkfeyo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gnpyiyzsw.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/giqvnebjo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/geqzurqwv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gnlpqhxph.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gzljyyvke.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gxxqhxqeo.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/ghplqjlzh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gshmkudby.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gmvewbshr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gmkwghjxw.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gfzlyejzc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gvkoxlyqi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gdolbfgpx.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gegpxaegb.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/geudiqbrz.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gbvosnupf.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gdkdhhbdv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gknecqbuj.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gvdhiohgi.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gbpmsqyzy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/geyvyhavp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gldyvwdvy.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gsuujveeq.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gmqwvytua.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gaeoryycp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gxufbuuxe.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gzahcmkgm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/ghcpchtas.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gezzuknmu.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gexvhlrxv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzbjnnyxc.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/glagxwrpx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gigirnedd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gegdaglqu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/grpzozrtw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gniikwnun.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/giizbtcrd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gwpmjmnzq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gduizpoyb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/glcznxugq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/glqgfrrfb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gboqgzbkw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gqrqvnfsj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/ghwcviquw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/ggrzgexww.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gknlplckn.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gnzxfcbvu.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/ghnmzoruv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gighvzqko.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/glieayqnt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/grrrzgnbd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gtderkrsv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gwmdgramq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gdwvkkbfy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gchmhdeme.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gbewjsdsu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/guzjhfwtf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/glgkssqkv.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/geozaivam.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gozlfnoga.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gjpxxjunl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gywbzlapx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gnzdhgcup.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gihftnfwf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gdqjyufhy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gradddksh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gamawynun.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gcnougsga.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gyfgsqjnh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gscgoymoz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gfyefdxjr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gvdarvtod.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gqyfyookp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gjlozloqv.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/grtaevhfy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gghbnxhbl.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gjjsqwjyw.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gesqqmkvd.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gdvdgamav.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gnhwmsuhw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gupmmdnds.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gchsvxbri.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gsrojxabu.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/grlgfvlth.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gmzchikjc.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/glxfhruuz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gtnziilrk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gpctvxzgh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gaeohdtku.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/glztemypf.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gbexgtbmp.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/glvxftkns.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gvvtnuusx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gtjkkkgmo.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gmbunozme.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gklisitah.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gvaliwnvv.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/glhjywcdn.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gdatlyllu.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gdterhvze.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gfpjdetxk.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gsivdqlka.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gqwvugmhv.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/ggmahbzqv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gjmgogelr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/grnznbojs.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gbwrqigoz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gkutiduvx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gpnvsvice.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gjmormyip.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gifvxbgba.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gxovwbspx.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gvzvngktr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gsapferks.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gosjtcwph.sHtML


<!-- 参考信息 -->