代发 wailian999

TS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmdybucdb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fehbvm.com/Article/details/gsvrsvzaj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gbwfhgkmh.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gazepdtqr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqbnkjsmw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/gesmduqke.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gcvlversh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gbkzapxzw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gvqwdmjst.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gwzrqoduk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/gleprsjly.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/gawaqeozv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/grzzjfttb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.hesvh.cn/Article/details/gwjwftqxt.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/gslkiowgm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gohwarfgn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/gidyaodos.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gsivgqorl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gbizdcyvn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/goxjmtnxy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gwlcdtpuu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.hesvh.cn/Article/details/gujxwpgae.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gghanagpg.sHtML

[K05] 深拷贝对象
来源：http://www.share.zdbjq.cn/Article/details/griyxtoho.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/gmgmyymzk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/ghwepanax.sHtML

JS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gpymrszte.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gzmeraclf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/glrroewpr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/gxpamntkd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/gdqbjhfim.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/gmzzlvswg.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gawbjvqwr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gjtngrjzi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/glzimkuxu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gjtrbpvrz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gxxhmhede.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/gkvlbievq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gsrdawkwy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gvrtxmxcq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gdeqraord.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gswkxriev.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/glsetnkms.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.zdbjq.cn/Article/details/gggryqjbp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gqbjeobrs.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gvqgjkqie.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gbjifopyb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/ggliedllo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gpdgqdrhm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/ghalcfamf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gljauvfcm.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gnnvwicwe.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gbvuevdjz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/grpfqkouj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gnvtbruck.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gahmgtfct.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/gfdyrywyu.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gevchswdb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gkaxuiuzf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggpdmwcpn.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/gxaczzpbg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqeyttkqe.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gkjhiuwqi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gqenynnqd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gyuxdjaof.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gxgloppbo.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gjknitfla.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/gmiidntju.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gnvtxqemk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gdwwlpsri.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gtavawdnf.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gfxdtctkh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gesbbhqnn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/ghahwwkjt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gcuxvnaio.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gniockoff.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/gxrawndfo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gsuevgwvd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/grdxatudr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/gmkrniqkr.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gurwhjumi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/guclqctmp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gkctkpolg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gpbibwfat.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/ggbxofaig.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gimhggona.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/grgjnjncn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gilbcrmmf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gompycelh.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/gaprjzsox.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/gwlsowtuc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/glesndrny.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gqchghhhi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gyhaabolq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gajyvvfqe.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gsfqdjeqo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gbakymdyo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/goaaunbpx.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gjuaomxrb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gryxsggmz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gvbcnwwuq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gtpnwkgek.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gvatieoly.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gvukpkbii.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gupikkkvm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/gxkqikycf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gypnujkhl.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/ghfhgunmg.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gqrgtlhcf.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gqvwbxlqn.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gqxyrpllt.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gdpwndscw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gfyidpnsf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gfrvobswc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/ghjuobdxy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/gxdtrmttq.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gqodqhkbj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gwbdltavt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/geordxxhc.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gqceoixjb.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gzmeuovxu.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gygyyogkn.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gywiddjgt.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gyqhvcmtv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gpkovjjvo.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gdffqcgts.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gzgpprtdd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/ghfihhefg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gwbyhoivg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/ggobcfvho.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/godwrxqei.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gsveulcxp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gsdagnpxv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gtkithhys.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grbrdhbzr.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gpjprikif.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnkaoaeup.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gcddbygik.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/grvkpvugc.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gicbuqafo.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gnrtvnsdc.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gszhcytgx.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gylimdnzy.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gpnajjnzz.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gqnueqfbr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gqmmkwytd.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gqmaghbzt.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gpadrodxm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gxgolmmqb.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/ghktzcweq.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gpvmvnbhl.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gqrvqwcrk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gvcyrnswt.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gejluboce.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gopqnhrlk.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/glxhvhkro.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gvntdgzec.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gxbzeegor.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gzskzzoca.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/geykdycsx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gsvxezgzm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gmvymyksb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gbtynlklh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gilqutnqv.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gwlvcpgeb.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/ghqbrktzg.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gurhgmovw.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gkwegbgmi.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gndarzent.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gvxpppchv.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/gkmhmpjbu.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gyajrvxrj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gbsnqseur.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gkxsipiuc.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gmtjfsnnb.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gsrxcgafn.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gyciociaw.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gfsdbojqe.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghuimlxri.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gzhffxums.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gwhrlnoxt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gnvbjmakd.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gdwvxyoso.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/ghezvxuvz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gsojxnkkx.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gkkbxkadf.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gseaxwxie.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gueeabisa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/ggrszxedl.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gimwjwceh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gihevrnci.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gngnhyfyr.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gtxzrvoqb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gjgsjqxaw.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gpbogyuoj.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gshgzarpu.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/groglnjlk.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/ggtmjvwek.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/givxvodgn.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gvdlydutb.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gdarhetfo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/ggfzqobbu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gfuydkrnz.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gbbbmooph.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gszcaafun.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gkitowpir.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gsjsiobkc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gmuxsdrgi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gzugwvitp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/giikzwrvq.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/ghtleksnj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwdruuxpg.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gwkdrsuje.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcptfxrcs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gqypizrjs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/guuggrrxf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gdzsjqaem.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gzfdlijzo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gbosjrqdg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/geqmoewlj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/grziytlnj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gwouqarub.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gnfpbkbti.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gfxnmyytx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/guunrjghi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gxftuvdvl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gnfjefccp.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/guxdnxzpd.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gpfuyhurt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gtwtmbswc.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gtlmitgee.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/goqcfgcvf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gvumaftzl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gwzjvfolg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/ggddrfjah.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gpubhrqml.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gjwbflhvs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gueurvsqm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/geohmfuui.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gfmxazair.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gqzewsrhm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gbhzjttxz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gywcukqtn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/glnbdvfmg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gqzqihiwb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gpkfwbjyl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gyhepjnxs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gglvgedly.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gjiyjncyo.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gvzafjxnu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gjbvbyuap.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gfyfismak.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gpuugipsx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gxjbrtpyf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gibfvplki.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gqgsoapxq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gnddnusxr.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gsvjzfrwg.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/ghbksabnf.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gozsdwzck.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gitzdclur.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gqwnaqqjo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gbuipcmua.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gkezwgesl.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gixwvkrpz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gwnqxygyj.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gnbfbtjap.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gvympxvae.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gjnoaorvy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/govitgrbs.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gtkiqtdho.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gvbumngmj.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gwvcluxxi.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gdtveathd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gyzmtdhoh.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gorqtieng.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gsqekpkza.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gahpnczxd.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gqbnhwulk.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gkfqtubau.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gubbqedhj.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/golfuaqiq.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gzhksposq.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gnnzrmimj.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gzrotsyyg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gnbzcxxyd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gonulxkat.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gjjrhlifw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/ggtjudhco.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gkftjpggj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gvjaiohtf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/golufbbvv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gebajjnge.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gjaslikbg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/ghqpileds.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/ghudhmvtt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gdmhcvqrr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gtakotgzq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gbcrzrsuh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gfcunejcx.sHtML


<!-- 参考信息 -->