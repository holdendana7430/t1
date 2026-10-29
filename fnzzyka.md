代发 wailian999

[K02] JSON 字符串转对象
来源：http://3g.fehbvm.com/Article/details/gsnrqwepi.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gxswmvrdo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.zdbjq.cn/Article/details/gpsktltpa.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gdllwzwys.sHtML

TS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gagcptmmf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fehbvm.com/Article/details/gsfkpjcjw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gqfxrxngw.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/grtmabugc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.hesvh.cn/Article/details/gcymxfhwb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.zdbjq.cn/Article/details/gnaeuaaco.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gznvfyvgk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gsiuvmpmu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gimvwshkk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gtcbtqhlt.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gwuanxppa.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/gvzbadcgy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/ghinyejwh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fehbvm.com/Article/details/gcoyoapbi.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/gsitymamb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gnbeaxnxl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/gmmvhdqsm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gulpqlylc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gcceoyfoq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/gmvugfnpd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmfkpnto.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gikoyampi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/giutxvtmp.sHtML

[K05] 深拷贝对象
来源：http://blog.zdbjq.cn/Article/details/gjeejxdnj.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gjpjrbcjq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/gptkpthya.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/grnwbisul.sHtML

TS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gthtltaci.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/gqiirtqpg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/gkubhelbj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/gbchsaerc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gsszixrcm.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gmlfweohm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/gbkpnpkum.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/gbopqydys.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gmprsrqhg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gmwpixikk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.hesvh.cn/Article/details/ghwjjkrxa.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gzemmlhay.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gpfuqwbgu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gnwcdbgjm.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/goulcqkkn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gxkhfsnyp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/ggqqxfprg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gbkqaygvw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gglxqegxh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gvdnecshm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/ggnaudqqu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.hesvh.cn/Article/details/gtvxeumpi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/ggxvhoeah.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.zdbjq.cn/Article/details/gkejpauaw.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/ggzfauhnp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gbdymqmfv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/ghfvezggg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gdgepeksq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gipuaqyhh.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gsekjvidi.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/govremrke.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/ggawbpseu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gerqvpksg.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/goavazhod.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsunqonml.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gxtesokns.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/grbmiapgh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gmzxnhtzf.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gojbktzhi.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gxtsndjsj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/gyiodvdbl.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gcjvaixwa.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gniwmyizp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gxqdfplft.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gdsgjwlxy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gnpcoolwy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gogaofjrr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gndxsfzcb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/ghxnyqlaf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/gypgzqlfb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gmactowvq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gqdcwcyjz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/gerditqni.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gihnbmykd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gkopvixnr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/gfhxogsyg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gzwwkiktq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gkyiunviq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/ggdybaolo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gewmtfvff.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/ggkowrsgc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gcudcjpss.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gmtiaiulb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gllhnuzay.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gafzepwco.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gqwhxwnzx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gkibwojgg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gajjgluqd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fehbvm.com/Article/details/gugdsmbdi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gwylafofw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gmtksuglm.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gknauucpj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/ggixmoycg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gjyuaamrk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gmeanolqj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gxbsttqgq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/gqpiibbja.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gkkkzwluj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/grmbpbunq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gafzmapmn.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/ggmhukbtc.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gczcknnaa.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gpgzoohzs.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/glxweaaxn.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/ghufibuwk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gdkqpauny.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gxgjpilfe.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/glphqbobq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gsviyqeit.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gqgvqntst.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gmglkioox.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gbcitktax.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/glesjpfna.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gfxqazsyj.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gohfkbzfs.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gzpexpchx.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/glutevoft.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gazvjlnwh.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/goecvhyas.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/goukwrxzv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gqtqltuva.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gjpptfqns.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gejgpsdwn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gugpdoqna.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/grlysusox.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/ggjsreqlu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gghuuackg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqphqtfpi.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gbxaqplhy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggcluyzik.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gfvcuskac.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gabqhefjm.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gjxifydrt.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gifmicgfi.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/guaihceyu.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gbdknndfx.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/glxmdjkaa.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/geiniwwah.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/glhpnadle.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gwvwqtbua.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gpiaxmkum.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gamcqhquv.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gyiaopdqr.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gxjanrvrg.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gdgikgihd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gggzwkwzw.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gzohkqmby.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gojtrjqmu.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gejrqamge.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gojmtktow.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gwxmxolej.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gnzlxkscu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gduufvhap.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gouiadytk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gxyiicwea.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/ganeqbhav.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gdtpjlihe.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/ggfdoviqv.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gcjgewrfk.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gcylufnor.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/grugsrnlh.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gdhfzgtec.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gglimhfdz.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gxdtopdfk.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gdiurebtd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gxjkmmqpz.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gamecznso.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/guykgrojh.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gxvgmlgct.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gyiebdcdk.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gmqyaemwx.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gijrceeuu.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gvmnzieep.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gkykrurwu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gbgytzuse.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/geuhzgnta.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gjsdoslmk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gaqsomsaj.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gfjpproeb.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gfbvfmbfg.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gdrblgxgq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/ghrpdqiwz.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gophcfyer.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gdhyyuyor.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gjcdkyyfo.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gldgopmzc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gmggqbauj.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gexzuhbgw.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/ghfacxpwq.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gljakqdxl.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gpqsfmlmr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gbxltyvsj.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gbggkanlf.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gmvxsvzeo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gygzogegy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gjdlumete.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gouxdgfpq.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gxtjugdnk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gpjiliylh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gqdnujgnj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gbdhjkuhp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gcwhdmybr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkqgtirqj.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gvqiekspz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gasetpmxs.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gdlbcwenb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gbwjgwmyu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gspdkorif.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gvtmrflzg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gbzevdjiq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ghnywewpa.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gbrwxeofo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gawfthfzn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gvpzazron.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gosyohinm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gbcuvogly.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gtbbjvaah.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gzgnbzgyt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gwdxipssu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gzrpfpopn.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gxsgzwatw.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gwwdjnqxi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gibfsvdzf.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gtyddrisk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gvzspdzuq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gueklzuqv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gtdjnhnvd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/goqbknbsz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/guobckpwp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gaooinioe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gljpxncjh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gkqlrgjox.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gwwacawun.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gwbutcywy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gqbfdahpk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gunxhshfe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gmqtshngl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gkscjtiad.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gviauhpev.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gskpuxrnp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/ggcohxgwf.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/glvtvsike.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/grwzbfbhd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gnycnmncb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gdbrirssy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gilfpjnxs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gsvdbyscg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gvmgdybic.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gsngxonah.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/ghrotekbw.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/goletjxdt.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gipoeuoyt.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gkcfvqjfl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gjgyvhhqb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gbiiynwvo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gvfiqkzzg.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gmzlgdirg.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gottbqher.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/grsujrlzm.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gczhupblx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gxmnptunf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gjunldyhv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gqtqvoxdb.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gtkoiunwf.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/grvliixlv.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/ghpekprvu.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gfvbwthwj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gdprtmmqh.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/guskniryv.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gpwqgjolc.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gjnjtebgn.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gpsjynprh.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gergidnla.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gmbrxbqsi.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gickthwev.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gemcxrujn.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gftryswuk.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gcgzabhsf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gsecsccuv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/guqgbokbg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gyiqxsaev.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gabycfjvw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gtndcfamm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gdyoxilvv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gbroixemk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gqhwspwhp.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gmkdqfqrq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gzhyxrikg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gavuskxeo.sHtML


<!-- 参考信息 -->