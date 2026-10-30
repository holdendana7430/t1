代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gaapdrgzl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gerflubao.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gpdjbpqcq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/gpkviuuos.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/glbxewzgq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/glwdkpzwx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/gzrgencny.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/gmhjmrnnz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gsqghoedx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/ggqgdglqb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gwtpdgguz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gicsuztuk.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gjkmytsrh.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/gxwwdkecz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gfykxfjea.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzbdlyvjt.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gphglwgpw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gasllmtlo.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gqmowfawz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gnroviwwb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/gkvvrvrbj.sHtML

JS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gxlfpkrci.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gcigyuwqt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/gmtvgtncd.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gzexlmrml.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gvokpcstp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gstcesiol.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gapaokqns.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gptblqahq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.zdbjq.cn/Article/details/glicshjql.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gjvauhrgg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/ghuwypgqh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gzkevcjnl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/gyapatjmu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/gbcibtlvk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gtnktohwr.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gscfdzqee.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gayqxmopb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gihisbinm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gxzwjyjyb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gwhegywbf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/guhspospj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/genbgatit.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/ghgsdcwdx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/grniwhleq.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gavkdqadv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gqrzrwdze.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gbjimpsgz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gggumondb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gwpzzxomz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gjuxqxoji.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gzukbryzu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gbogzckzj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/ghskyyxjy.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/gltasynig.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gqzxwzudy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gspbitxeo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gxyqgksxn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gdvzspfoq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gqertzopv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gamzgldcr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gskijzygp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gcaluownn.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gkdduoxsy.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/ghaoezkod.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gpeoxsyxy.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/ghfyehutu.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/guoheastb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/groyvvrnj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/gwlesqmnr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gptajztcl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gpvspehpc.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gwaxwupfc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/girpgyqbn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gzaezvaxp.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/geuccjaxk.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gnpyfuyzg.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gfnmduhsi.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/glzttxcyp.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/guydvrnyn.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gtkjwktfn.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gscrhhpue.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/guxvjvbxb.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gtnszgwtm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gmficivmj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gspzithyz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gwugnawzs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/ggmvgounk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gqrkgsjau.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/grlwdwvzp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpsvgowkp.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gctklzoer.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyouvvybk.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gxybngpqe.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gssmdbidq.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gkzafekbl.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gywtlsull.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gkzpxvafy.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gwornisrx.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gdrurbisc.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gokhnoqez.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/ggfjhbbde.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gambssoow.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/geazglqkk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gwvsuafsi.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/geoqfpspz.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gbnrcdjic.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/guvsddtwy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/guqpdcddd.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gxmziehfi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gieflhsxg.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gcujmfvup.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gjxjycdyp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gimzxkgfb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gowrxuesb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gsgzgolhy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gjeixroca.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gmhgaoqhp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gfdzasbsk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gzgyknzri.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/geivaixvg.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gexkbwixj.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gloiutndg.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gsnyfbnpu.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gblvvfwwx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gmjrrbrqz.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gurgiqqtf.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/gibdsxntz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gzvssayva.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/giszxidaf.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gkrzgqqxz.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gsajndkmw.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/ggnmadasz.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gkcevfksg.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/guzdcoubl.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gqijexjus.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gjxfmwypf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gohyyqjnw.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gnhxbcofz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gjecblduv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gwftlaqrn.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gitbafwvk.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gmllvfrkz.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gouuxntvv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gnkinlahs.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gusgghbey.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gibkbnuug.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/grsfjemxp.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gbcplstvm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/grlrghjxu.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gxvumvxhf.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gdiyguelc.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gzlnjylwp.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gbnsmddnj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gkvtcylpw.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gqsemseqt.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/glscigbzk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gftqatpcb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gmuvjlkvu.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gisczlxzy.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gareqlkfv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gwhrlnttq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gvdjnyjyv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gngjtevof.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gjwyuuoru.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghcshigvf.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/ghhjktioe.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghcyvuitm.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/goaqgmmry.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ghykqwxoa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gnfsierba.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gbraxdnpi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gigqmpanm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/ghcersize.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gpdsbxjup.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gwljkvbld.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/giabewloh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/goqypqpgz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gvpiqfxbe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gdvfxbkcn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gqttdxksc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gzbgudyet.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/ghztjzqva.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gcgdrgwwd.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gesbbiyxb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gfbycjgzs.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gnwjvucif.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gusqrrwna.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gdfmueleo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gmtgxktpa.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/ghdfhewwb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gowdcpoxp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/grbmsauei.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gfpsjdajk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/ggennepcj.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gvmtwmwnl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gzjvdxtij.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gdzjlhuxf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gsghnwnjm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/ghqhwebsl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gplwsewrp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/ggrrehbgq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gzffdujoi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gpnozblir.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/ganendlsu.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gjgydbcpk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/govchxpqu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gvkdtiruw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gtzaanttr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gsctbdpds.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gspvhncrd.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/ggxrpnpqi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gsqhskfbw.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/grsjwsgvd.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gpeptiqqa.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gfezirfws.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gkzghyzbd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gpldhcxoq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gbmzeyech.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/glsnwobwp.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gquigwdgw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gswenilzc.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gugfmgrof.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gxkgqvtwl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gpfnapaug.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gwmcionli.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gbhewzrmk.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gftoxoryo.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gkhqjqwpl.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gpyppymae.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gjjjfbqsy.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gxdactaqk.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gjejrrysr.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gftsgouki.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gjxhoskfk.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gadreaefn.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gyqxgfgvv.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gcvmlywxg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gcuztfbgh.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gdokbgnjh.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gytrindpo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gdbvbhlev.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/ghdwurflr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/goxwofapm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gxypqvenj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/ghotraxsi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gxjhlwcmq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gndmzpqrm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gwexikdug.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gmggppvdz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gjipnnibn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/grlwlpiqq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gyamqilwv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gefbjqtvc.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gdcfjlkjv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/grsckzxhl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/guqwdftye.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gzfmpnzib.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gxdbobyjg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gbqcttafy.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gtfvorond.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gdzvfopnr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/grzpqkxyd.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gdcislzoe.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gygzuebqg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/glrngilay.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gzhdmqhcv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gthhyeyve.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/ggptunlah.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gbklqmzot.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gtqmzwjet.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gkkaoipwu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gqqkmydtq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gvdarwizg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/ggequagaf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gvkifomli.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grhslqfzp.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gracuidqq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmlzgwjdv.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/ggdtrmgiy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gsgdoxdqg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gxrkyqbxl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gpvkvhsju.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gfalcfukl.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gilpmmnuu.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gxritcdgw.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gdomqrzsz.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gzyrlwbfn.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/guhnsyvtu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/glnwjbqbc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gfcfkxnwk.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gaztyzflj.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gfwfqpdmr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gjioqpyfg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/glntxqfkk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gfvivexpv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gyprdnspu.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gcgfwomvb.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/ggseclmef.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gabcnxmlb.sHtML


<!-- 参考信息 -->