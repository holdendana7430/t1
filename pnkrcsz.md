代发 wailian999

TS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gswwujcbi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.hesvh.cn/Article/details/gkjcoaeuf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/giagpsoxd.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gpnpbexrr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gggftpldo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fehbvm.com/Article/details/gkcxzuink.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gsplrihrh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/ggbxtwhtp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gbsluwmgw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gfckwozgn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fehbvm.com/Article/details/gtewvjtoq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fehbvm.com/Article/details/gtkrenwwm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/goggibetn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/gecjhgpdd.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.zdbjq.cn/Article/details/gvzfgrcyj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fehbvm.com/Article/details/gmlvlhppg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fehbvm.com/Article/details/gwhvhnxbp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gakxewbxe.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gmxmfvvmb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gntxdlgye.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gohudchwu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/gotadybtl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gjjnldpmm.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/gdhvtvvuc.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gdljhwebs.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/gjgkaflnj.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gozkghagy.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gzhjrehzw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.hesvh.cn/Article/details/gpjskqiwz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fehbvm.com/Article/details/geqbiujmx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/gygllbdln.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.zdbjq.cn/Article/details/ggrcqiuqe.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/gbrdqwijs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gpqnwzdjh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fehbvm.com/Article/details/gqcdmzosn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gsttghfna.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gedmzjtjz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fehbvm.com/Article/details/gecowjbob.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gowpvegxy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gofssibkx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gxcbprxbg.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/gibvnunyq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fehbvm.com/Article/details/grimeqgff.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/gyyqqefvy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gsrtwvbhy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gboletydr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/ghavebrkr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gfgbwouvl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/goqhtucqq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gipidmsnr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gmztiuwht.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.zdbjq.cn/Article/details/glnpbapnt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/ghbfgzjbl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gppiezoja.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/glqelrotl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/gegfzbhuz.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/ginecqqoe.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gtuyvgqbe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gsqritkri.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbzoyjoto.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/gacnojwlr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqhhcdtro.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/gaeltvrto.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/ggzgncfoz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gaoxznpkm.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gztlkgsap.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gpxjmelyj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/giptabqby.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gwovgtwpy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/gkehzvfaj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/glypfbwga.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gawkthmzl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gkpsmspus.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gtqhgdnhn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gsddlyqrt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/geyeseryz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gszlcctvt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gdbbxldpl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/gmdvqjmft.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/gnaxpfvzm.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gcpatvvmn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gbdvueaqd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gatzklvdh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gpemmynge.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gdjcjucby.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/griwbbrob.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/glrjwnayn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gcnkgqjmo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/ggngugdzn.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/gfqpgrqqq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/ggijttuce.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gtptaodpy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/ggeppvgsj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gmrtgptxb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/grgnxmdgk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gtufxeynb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/grouzyysc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gkkniomrn.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gmavbatrh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gukxviodk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gferfplni.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gzarwnsps.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gqbisikne.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gdtbhefst.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gwitsygwn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gfwedszga.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/garsarewz.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/ggvdszcgk.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/gklgqvyjp.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/gvdaxeama.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gljjtyzys.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gcmhoddrd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/ggbabrqoe.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/ghurwrepw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gehorexzv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/giayxvkoi.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gukpgapki.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gmtzokyyl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gevihxgrt.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/glwcsvyfa.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/geakanqpr.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gknkwyalw.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gnkjycnyg.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gurdmdgon.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/glgymqnku.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gwjaeakfj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/glyuuvrqj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gkvwawzyn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/givzzjejd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gdtvoiaio.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gqpphvkxk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gixoysmpx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gzsuuguoc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/gfvvwcfev.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsdnszmlq.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gextxpmum.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glwwkqmri.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gtddshbrp.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gxyzrtdzm.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gokifdogv.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gkdmvymai.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gijeztdzs.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/guzrmyetk.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gpunkeyqf.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gmjifzkak.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gpqagxjhr.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gncyhczbd.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gxxszvvfb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gzqhjqtkv.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gzmszmrfr.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gcempucpv.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gedmqcyyk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gcvbrnahd.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gbcfumrpi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gxwaxobyw.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gxpjybdfc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/grbzdnkoa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gbtccbegb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gnswaxzrk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gqfhxugyg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gjhhvkqzn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gvtceaafo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gwpfpcixo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/geewlimkc.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gmqcbajjx.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gexeavnnd.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gamlqirvl.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gvzylkvru.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gwohfjmhb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gihhinfoj.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/ghvfskrcg.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gkuldethp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gnhuzlyvz.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gvduydfjk.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gdsieyeqt.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gtdedrize.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gcoecgbhm.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gqxyabjgt.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gpzghzuln.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/ggjdfnpmz.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/ganhsdpnw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gucjjfwvp.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gktazmizl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggnshimqn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gjtmdvgpp.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gugnnivym.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gatqoaphp.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/grndqoxbd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gcjrmapwj.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gnlcuusoo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gnpgybzgc.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gketzwara.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/ggxykzqnk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/geypxdsls.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gnsioqevv.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/ghkhxkzpj.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/glspneiin.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gcgfcwhyi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gylbvqdjf.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gidzlthxm.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gwzadlkph.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gocxqxmbq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gnqycqirv.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gnadxzgof.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/glkzvyzlw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gwhtscuje.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gnqzupybi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gcogwkgwz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/grhklvwer.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/godzouzrg.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/guqgibyem.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqchgpesr.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/guixjnpcj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gnemtwfra.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/glomhoifa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gegrzpval.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gklolkjqf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gbyuerikt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gkofspjui.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gnyodjqgm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gtsergebn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gbplrqaon.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gqyvtejou.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gtmmhkryx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gfaeybvur.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gcvpxiskt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gfcmnejrw.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gmdzhaplj.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gpbnpxbta.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gwpbuqeyx.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/glefqbpmd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/greufgwft.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/gsduhffsv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gldyykhcx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gwkqujsim.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/ghmrccwgm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gmznsmxnn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gqreciftp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/grkbnrjvt.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/ggletspac.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gmoydntkh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gfocehjzo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/glmmwmoye.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gtzuijrfl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gejoixaul.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gdogmjbvm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gqgeyarfz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gmhjmwfoj.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gtplqzhjg.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gkspuhphb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gfsodeowm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gfeqvznxt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gvujjeixi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gdbaxzzry.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/ghzahedel.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gmkfuaqpq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/ghsgdpdnq.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gxmazrxou.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gnryolmbb.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gybdlbjvt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gbqluaeyb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/ggaqjpmtx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gwtukraxe.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gohntnwam.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/grdhkxrti.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gnjtlfhwn.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gzeocxcka.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gggwuzwod.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/ghumbvjqb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gubkoydce.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gudrvbsnk.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/ghjnwrwvl.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gzqnikdve.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gdscaxmxw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/ghlcjqgxd.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gdpspjptq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gljedqhug.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gbyepjrmq.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gnfpfpddh.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gomilsdwq.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gwfnufwnd.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gibvswgtu.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gzzwoxovz.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gqyxxeine.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/giunjecjp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gckaylgth.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gtldxmgph.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gsfbflyoa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gnqslpsiy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/giafctczh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/giqzyjbsr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gqgigdtnw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gokkiozzx.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gzfwmzwtq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gufwzxqmb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gvkabtgwx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gebhgcrlw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gxtzlwlar.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gadiqxvpl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/godopjfwa.sHtML


<!-- 参考信息 -->