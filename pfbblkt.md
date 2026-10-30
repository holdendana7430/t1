代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gqfvuaxce.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gwxsepdiu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.hesvh.cn/Article/details/gpjyfzuhg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.zdbjq.cn/Article/details/gadbfkotp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/gozzwoued.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gylrrkzdm.sHtML

[K04] 读取 JSON 文件
来源：http://3g.zdbjq.cn/Article/details/ggorwdhgx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/gwmtdsidv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.zdbjq.cn/Article/details/gnhuglyql.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/grhgqouwi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gmohelghn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/ghgjfwyij.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gmxtrqfxq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gbzoohjtq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gjtpofgvo.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gusveqtxc.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.zdbjq.cn/Article/details/gggwygsjm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/gyxgzvmqb.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gqhpvyovm.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gsyqtplox.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/gqhessbjk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/gihfufrdk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/gtcqgramf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/gdbvjqovy.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fehbvm.com/Article/details/gurdaqggo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gihkcoray.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gtdgtdwcz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/ghgacawsi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/giqobvxbz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/gslfqsyfs.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gwjiofqsb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gritoeghx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gwgkvnail.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/goyajhoun.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gwwnigijg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.zdbjq.cn/Article/details/guvcmnhkg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/ggojskbji.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gcwokxukn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gblexawgv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/gwlqutpyp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/gsblcopuy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/guttxvpys.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.zdbjq.cn/Article/details/gfgqfbqqd.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.zdbjq.cn/Article/details/grpupsgzu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/gizdtbyhq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/ghsbhugwp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gaikqmylw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gypspswls.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/gehtkziem.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.zdbjq.cn/Article/details/gprqljypu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/ghjqdvijd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfdexaska.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gicwvkgvm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkyqtyxmi.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gxysbtart.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/guhaexwwd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gvyguzyzb.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gigeljrnq.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gndqtgbby.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/gtfikmvbr.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/gfrskzycg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/giwjotezj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gscboqxwi.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/ghbtplnfu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gzhfesssh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gqoiddtoi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gvgalpnhj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gfddqfpna.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gtstgtvst.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/grtmttqin.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gyrtpvquz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/gcjtnadza.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/ganbgaycr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gkuwwhqee.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/giodrnmlw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gvckegtny.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gduixkoqk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/ghlghspym.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gatljvxcd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gtpvxesme.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gutfkavmt.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gefcjdoyq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/guuvyfkug.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gavbzffli.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gjxplwind.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gidtupexd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gcmukrbrk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gbewtapkv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gkwdkhkpj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gxsolzqeh.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/ghtabjsns.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gvxyllelt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gioxjpvrl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gzbldkhmx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gqvnkrzsw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gbhechdan.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gqcayuwkv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/ghhhopgvo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/grrjrkrzt.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gwfzhpffc.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gogfivgky.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gadbyknul.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gjxqbnbun.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/graaxcwyh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gagwtvnyo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gdxfmdbkx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/grhqzbmeb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gmoecqjho.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/glyvxcbpj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gbqxrdfce.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gvuvwtlhh.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gukbwowzh.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gfqnodajd.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/ghqdfnbow.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/grnqeudcz.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gnvrqjqyz.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/grdnkmxls.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gttfmxfvx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gfqwoqrip.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gxtibhbtk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gyvtpzhyd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gcldzzsph.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gumggxctu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gazgumdlo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gytnhpphv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gpdbzxwvh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grrlfsqmk.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gscffxtmg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcpyntinf.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gtnhkrzaz.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gphjefqro.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gbzwicqpj.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtrxoeyb.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gzejvejxz.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/ggvtobker.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gtvczsnrh.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gbvtghvxy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gnrkcilio.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gtixywkfr.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gaxwlcmpn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gwjxtvxvg.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gkkhzneza.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gaumollxx.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gqqqcyzrn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/ghewzhmgb.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gjhumuoaf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gnetqorco.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gcwwkpocv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/glpischqm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gcmsogyfm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gqnjqfsng.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gjscgrbra.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gwadoulzh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gnmykewqq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/gmmjhgwal.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gyhcfpkhw.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/ghwjjipcu.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gptyffcha.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gtgevnpvi.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gghpxfqia.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/ghsscranr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gxpclqrlb.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/grntnjztx.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gclthkybf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gmdvtyigr.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gptvrryjr.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gpfmijmng.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gncvzlwll.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gayqbyozu.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gebcvgnqh.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gywyqevzu.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gzjriiaby.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gymkmpihb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/giwbotvqv.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gtcbibgrs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/giuxxrsmq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gsuinivmh.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gnkzpgver.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gancznxqr.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/grxbpenku.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/ggvtgxzkg.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gfogwubdh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gdmsqimvm.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gwffobpnv.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gidqwocuj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gecdfmvvc.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gqxgothjp.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/grfqbejrq.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gqtysafqu.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gmaqlhzjp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/grfsylxgm.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/ghhfqbfnh.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gvdbqbqll.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gugtxeaqv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gusqbxxyo.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gyxmdvbxx.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gjjhbvvfs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gkfxtdzes.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gnxyulrqf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gufhnfwza.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/grbdrvfva.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grlhxyypr.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gyxzekzpm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyeuwmfba.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gjhtmhkyl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gpzvebvet.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/ghqkhqnil.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gnhbkqptj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gpsguiuaz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gchgwmlzc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gycagbxnd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gcudohwbk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/grghhtlex.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gcrnxppbn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gnintfrvk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gzpggsxnx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gnevwfvih.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/giflaytbk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gbybsgtny.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gmfooflob.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gofrgmryf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/ggsmxmgfz.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gfaohjata.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gqtkjplhc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/guxqemxfg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gyebuvsbl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/geeepccks.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gpzywoywx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gzhpxewkq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gkurlfubu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gnwnamvmu.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gfcphduix.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gpkaivwfd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gnxfpmlpn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gcezbnahu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gqizzjgcf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gsqvvwkru.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/grbvhxqvr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gvpykuqiq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gpxtoqyfx.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/guuzozdsp.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gfiptelhc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/geqmohlku.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gkkufblgz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/giyldyfdq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gtzmbooad.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gwplxlzfw.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gszfvufia.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gwvpjwlff.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gwrclvxhw.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gqdiioqij.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gggqpbgpi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gmrdflvrj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gdtumujmq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/ghyilcweu.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gewpjgknr.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gekmpevtd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gojxiyybd.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gxsvhloob.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gxjunityl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gegkyhepe.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gqaqxkxmm.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gmixkgfge.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gjinxgfrq.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/ggayhnfxf.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gazbvszxa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/guzqjhouh.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gncvyebub.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gimrktovu.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/ggwjoypzp.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gxmmkgjwx.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/grvoutese.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gqekrhxeh.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gdhlqpqvg.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gssgdseja.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gfyjozyfq.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gvgdwyxsr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gtiavyhzp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gezmsuenl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gxbsbmyez.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gxfvimpfp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gguectpno.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gbijsdrqi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gnazbpoxy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gergjqpnl.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gmwggbpvr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gvzsgfcjd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gsdvafsxa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gmqvcubiz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gfzgdqisu.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gktsckanw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gsszaflhm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/ghzafmejs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gtqmrcpty.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gkvvcneye.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/grybpssjm.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gznhkzpeq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gfrfdyxni.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gvmfzmwwz.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gwtxdcxjv.sHtML


<!-- 参考信息 -->