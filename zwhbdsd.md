代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gwbhbsoxb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gtpatylne.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gmxrapwlq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gahdudhfw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gkqbyyazg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/goqhwxnda.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gapkithku.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gjpnzljvj.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gkfkuqrio.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/gxrwzkyka.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/givjsedjb.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gvcejznon.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fehbvm.com/Article/details/gucicppcc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gixgulmez.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/ghzlmgxxg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/ghgfzlgvv.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gyhivmken.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gronfebwv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/gsmlythpf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gswdezojs.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gfccvpfod.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gmfrtpcpw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gkxyjsjop.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gzxmwpsuv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gkakijmri.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gtppyuziq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gelemeyos.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/girazuxwz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gegufoabc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gsvmavedz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gwiwoudtf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gxghowrff.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/goyalknvh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gpapspeto.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/ghqorzzqz.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gpcgffxgf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/gknzyvcjo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gaoltkmoj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/ghwiytmyq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/grdrsunxk.sHtML

Go:   encoding/gob
来源：http://www.blog.hesvh.cn/Article/details/giewwvzxc.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gykdrxbip.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gyhoscznv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfcqtulbh.sHtML

L. 网络请求
来源：http://baike.zdbjq.cn/Article/details/gqqzkkjfq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glnjcpple.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gxqhkqipz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gdbvestkd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/giumezyxq.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gdfukoaeq.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/grlkoehka.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.hesvh.cn/Article/details/gqimankxw.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gpuovdabc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/gjqalklgd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fehbvm.com/Article/details/gmrneyhwe.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/gkmwlbymz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gvsnxliwh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gaptefwje.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gooejguuk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gztptnpig.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/gpxprvykt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/geqemnfne.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/giogpvitz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/guhjigdoy.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gkotbrola.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/gtifedark.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/gqgjuloky.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gdhmbagqi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gwlzhqvxj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gyomqiofs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gadbqvrxy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gnkirmchg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gtwwqwihn.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gpnqhmynk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/gabpjkwxi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gudbunugk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gcznuqtlk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gyiynxaib.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gdsclrwgs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gjyzuixsh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gompxixjz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gbprkvide.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gjfarmxah.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gsknqdvrs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gkqkiknog.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gcngrqrwr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gnacwbjrz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/ggvwvhrru.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/giqlmvheb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gsdpgygmu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gbrpneymk.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gcozmukku.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/gdmmscezs.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gtyzlgyfz.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gxcwilurh.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gnnsyjrcq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/ggimrveqh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gnduzbuiz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gbingqpxf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/ginfobrav.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/ggjszgfgx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gunlyphdw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gdnhgtreu.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gvdnibeku.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gzmvfeyii.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gusequoqc.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gspbzbrwx.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gwkdmlgcl.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gweumamjl.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gupjttejx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/gjajtgcdf.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gbscyzgmb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gdspjgbeb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gmycvafiq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gaqcjjcec.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gotimisra.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gmoaswcff.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gewcinxwc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/golricuhr.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gtlmkpxqz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gloorvjis.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gjegmabjh.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gcrhskzwp.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gtikisqjg.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gfughgtnq.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/ghlwurfbl.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gcggfccsx.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/ggisssuef.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gyuduejwx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gpbhxdzma.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gltwemqom.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/grywmopwf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gqslmhpdx.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gfhpjblmg.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/grkxrwajl.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gonayljcl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/ggctsname.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gibdqhouj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gmtxgjrmw.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/ghifgwgkc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gzlwscnsy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gbzylbtod.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/ghxvccxds.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gqxhvpinr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gwrksvpyc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gemtawlim.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gfhciihnj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gfaesdcmp.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gfeenlfpq.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/ganxwtyhf.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gnaelbyfa.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/grvtoimii.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/ghrffyapd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gceovwhmx.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gwsoqghcv.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gkcpjcboj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gvnmnaazr.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gijdflspk.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/ggswdlkdc.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gjrspamel.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gichrnjja.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gjipjtltv.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gjayzzttj.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gzsgthtxi.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gehtwzhml.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/ggsusfdrx.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gyjaudahe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gfdxibzxe.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gsmkazomw.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gihmcbpsf.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gwlowwvbc.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/grlymvqvn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gnscvonlt.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gimcruaib.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gcgztkavh.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/grwumgsig.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gjdyyubay.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gcqrqoiho.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gfpaibpsc.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gkrbsjvrz.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/germqdeyz.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/geojprjzl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gfwfkeqos.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/ghafytezj.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gggwvnqks.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gimugylzd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/geilyjgfb.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gjsjfgumk.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/glomulzrj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gjhuzwuoa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gffunxajf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/glbeawfgi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gxxgvfyqj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsosncdne.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gxbhquxce.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcrgirdcp.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gomkezhal.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/ggvmsyjec.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gztyxbqyu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gndxqviuw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/ggspzessw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gwypcjvcl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gtymltcto.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gifkjweqq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gqgdddjwd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gobcfjpsp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gfvawnquz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gdmteimnu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gvfkuupom.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gazvmxogv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gathweqwn.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gdmznyegb.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gghkggeqq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gbzwgaesk.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gicmddfio.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gtrevmfed.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gnumrqmkv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gzfjcsdkm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/ghnhzfcfv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gmosdzvln.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gmbeflruv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gqmkvwwgj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gomsxnout.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/grxynlbuq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gxyfzqwhx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gerwhuwna.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gpkezqkha.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gezgjtjxg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/guqzvnzvc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gmkstannw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/ghfctkmnk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/ghcyfqgzo.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gwfhgipci.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gxfxjngbw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gqwvgavjf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gwmhlppel.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gorhiaanv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/ghblaqyyt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gkqvgoewq.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gesqwbqxs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gsnubvakq.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gdyduidjf.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/ggyglyybz.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/grhipgjst.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/glrjbyalp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gvfjuprfx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gpznhfqfq.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gspinwxra.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/galzfupjs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/glvjcovou.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gaeaqwoto.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/grckuoopy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gcccaldyz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gksrbwmje.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gibkteike.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gioizbcvd.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gypjnurxm.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gpvvyjxhh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/ggrobjflz.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gdznphvwr.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gpctjetta.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gkhbysaud.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gximgioxd.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gtclukeny.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gvrhucvxc.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gjufumkuw.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/ghrvimcpa.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gqrnsndhs.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gzdvtipck.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gufameqqb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gkknmgoaj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gkekovscm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/glgmwrmxc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gzptcouen.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gbcyhdzcb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gwlrqprla.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gsfdzmlon.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gvusqjfzu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/ggolngdkb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/gldivsnqo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gcrmvictl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/grjvlxmqn.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/grvkmzbsd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/goegepdaq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gdybhlmpr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gzmjgdnpu.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gtxdpvzhk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gjfxhgkjf.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gfxrzztxz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gdnwpdxjx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gxnrlmtmw.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gxwyoqiiu.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gqhusszmd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gsqozhpuo.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/ghcogxbwn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gotfcvfbp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/guspiubdh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gdmefxyqj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gxrnpqeed.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gsxfpazxi.sHtML


<!-- 参考信息 -->