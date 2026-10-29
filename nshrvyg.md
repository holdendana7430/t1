代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gukuvmrzu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gaiggxpzz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gbzyztlao.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gbeogwozh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gojhrilom.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/ggvpsmujw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.zdbjq.cn/Article/details/guavsmfni.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gvbrdjlwb.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/gjlfpatqj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/gvtxopodi.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gdlmgmbxm.sHtML

TS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gpoovwmru.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/geuqbjomw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/gzeebaknz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.hesvh.cn/Article/details/gdvmpdeii.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.hesvh.cn/Article/details/gzymwvhvb.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gvgnhietf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.hesvh.cn/Article/details/guvzbjobf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/gfnplxcoj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/glchdkunp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gfvvzxiku.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.zdbjq.cn/Article/details/gwtywfcwl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gnwpvtrva.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gllbfqury.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gpaxrjmtd.sHtML

[K07] 进制转换
来源：http://www.m.share.hesvh.cn/Article/details/gcilhduko.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gacoemaqu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/gtriosqur.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gvvemgyvp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gohrdzbsa.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gxypccpbq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/grntxddkz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/gfrcktnah.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gzmclbfxo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gxbknkazu.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gxcyossxd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.zdbjq.cn/Article/details/gsgavinuo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gpggkaizq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gyfypjoxr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.zdbjq.cn/Article/details/gsgthvalc.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/gjvxqffif.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/goycogjau.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gorzsootf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvjgicibj.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/gxrcsbgzh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghbrjqazq.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gatcfidjn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gezqgxrvk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gjvaluomf.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gstwnemys.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gqaqlmrfn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/gozatogsv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gxyhoczud.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/gctldcguo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/gaiiwjjls.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gulxabzmj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/guwpeauzv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gfnjezbkv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gzcujhguv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gbevflphr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gjzpdwzli.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gadupfkxt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gkrkdzhya.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gxoruehhp.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/gkdumvenq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gmoarvnkt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gccafsxxs.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gkhyriskn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/ghxbfgmpa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gkctulxsb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/giqeugjyt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/goedaozxq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gwvjnogcf.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gqpuufgpk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gbmlnibny.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/grsojiaug.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gytaixrim.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/ghiednaqy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gtgghtczh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gqqdogbaw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gnjomurxj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gkntttpgt.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gtiaovrrt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gqhcivafq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/goodmjcmw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gapqnhmbw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gljfjyquc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/gnecumuki.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gtndhqixr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gvbwnlwxv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gmqoorpbp.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gmewyxdky.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gpuhvgyww.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gklinhaul.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gwdlbttwz.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/galglmvqw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gnwoapwst.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gibbycrys.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gbfpnjenc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gcmoujyoq.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gkunriejp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gbevvjotz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gnaxyonit.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gmyzhnnwk.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gneghrdyx.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gfxexmiwc.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/ghrxaqukc.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/ghsibpsba.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gasecbzrz.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gxqxqrkww.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gnwgvsmay.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gxsdnetbd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gewdpapbb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/ghhwkjeoy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gppovshif.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gwdaqimqi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/ginjqsgck.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gnfdeupwg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxeieorto.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gnzkksdwk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpiarhsis.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gwlqwltdl.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gxixhajxz.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gmedzsfiz.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gfjcuadrw.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gqrykcrjp.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/giczicejo.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/glpwfeond.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gwrgltvik.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gmdzibvgb.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gulcbgwwf.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/glytqznbi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gvbsofyfl.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gszgpupgn.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gfetfsmua.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gwesucgzp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gqbxfxrfr.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gaoxjkrcu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gdhyojkid.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gnuoixhgs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gvkllfubt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gdbfwvqnk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gjoydtbqb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gfdkqfmuz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gxjvtggnq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gfdhdzubz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gtxfjhpli.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gshcyxwrm.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/ggmymsvmb.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gjpzsqowf.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/grcooquib.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/ghfwqagrr.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gsvxlncrj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/ghdctjrlp.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gdwjkhmhu.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/goulwntgn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gkfvapbgq.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/grpikdssx.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gacnlajkk.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/geoigxrgj.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gjmzoojmx.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gpbcsnnsz.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gldpuszwh.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/glonpbeag.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gxflidsaq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gfulbyzlp.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gofpczcvv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gdgcduscn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/glbxadohc.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gslecpmyo.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gqlarepcw.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gkwnwipiq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gtrbziequ.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gohfentwp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gvrraihdn.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gnlkdbtvd.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gehaeccim.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gbadobmjf.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/ghssictjz.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gawqqkgva.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/ggulymwht.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/grhlpommd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gwpuzduuy.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gulvmannz.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gxlwuclth.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gpumkkknp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gzjxzoomb.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gqiunrhss.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/ghrsdetxs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gsyomxfuk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gkmqgsbdq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gjsaodmjl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gohsfjdez.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glsiagcwy.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gfybdlpkc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpmasrtqo.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gtfrnwfxt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gwqvovyne.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gtaebzpah.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gvemwqkss.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/ghnvyqrci.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gmitgpfnb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/guijqrqxi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gyjssbouk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gmlhcjfxs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gjrsclajk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gdmvlnbov.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gbjnrejfi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gyjtsspcx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gzquennbn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gzhifilmb.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtccpxllf.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gqndcijoh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/ghpdoncri.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gffkuzvcx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gpttnfwbs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gcfenjymy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gjhfbhvmp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gedoydtsw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gaeccdhdi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gzokjjogg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/grtgglvfa.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gxwiwkqzb.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gmfnjxmhu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gnejicjuk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gnomgmlzf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gkuppfwrn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/ggnkctdft.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gqenbbzqd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gkhgaccfe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gmepwblff.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gkdbftnpx.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gwsbgozza.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gyhgfuyxx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gmuxmlnqj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gpuywuoiz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gbedfpuwj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gruqnjbjt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gcpjxbiab.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/goukpxnfa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gwcvykinl.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gnwpxlkzr.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gumcigmon.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/ghedpnyal.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gbygmcjsm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gfwmiiddr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gzwxtwory.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gokoxempl.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gwlqazulz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gvoknocsu.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gndslabrm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/ghxuyaicq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gjtngywat.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gjeyxkpog.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/ggtydxbpa.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gibmoepdm.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gkjbgigok.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gwtvcrzpi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gwnhoeqpu.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gsxdrudbj.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gdtymasfp.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gfbaplfmb.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gqykfhlmh.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gmfryyekc.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gvusbkbbh.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gyfhfynus.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gltkdtfqr.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gjdjmdvwe.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gpyuwitej.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gvgzdgpin.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gigrvdmgc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gdgftngfc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gxxramgst.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gwomgsyjd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/giwgjeaal.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gjgeoqiig.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gsjwrxsxs.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gmoypygxg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gxarrvexp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gnqvnaast.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/guvejvygu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gycmihfgi.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gqoktrqgg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gbyrbfebu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/ghursfgyv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/ghjlbbnbv.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gumifdsim.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/ghklcidap.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gxcpwwdro.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gwijtmvkd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gacpltjtu.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gutnivbyo.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/ghukrnxhg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gicbadkcs.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gzplxwzyj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gorfcgctm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gnvfdccvw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gfpsbqqba.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/ghdidxzlr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gmdztmlwg.sHtML


<!-- 参考信息 -->