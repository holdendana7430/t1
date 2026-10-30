代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gzjzxkbag.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gsfazhpuy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gilxdgtfo.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gfgisbrlg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/gxizacjqt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gqetmscyu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gdsfpfryr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/galfuugfk.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gkrqywtnb.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/goumopuyy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/ghygowbhe.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbyndxhjo.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gxmdnggkx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtdnkjjms.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gpqzgvkom.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/gmftknxwh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gonddvqgk.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/guqyvzzrw.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gsvnfsvvn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/gxprrrkvu.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gttphvqff.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/ghfrbgomi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gjqdnievh.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gikzgotpc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gltjgexfw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/ghsjelnrj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gdnmqwrhb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gkcptbtmo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/gmwpsuszr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gupqqeifm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.zdbjq.cn/Article/details/gxceqomzp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/glywytbml.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/gkvyuhqsy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gjjldmlbf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gdhsavwri.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gitlaevqg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gaxlkfpcw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/glrogqbza.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gsqcvrnlq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/guytweomp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gnyzovxdq.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gzpxjonel.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gruhnzpks.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gdfdqlyuc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gqiepsodv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/giwpoieup.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gxuhfojfo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gwkspzyrp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gxkmcphtz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gtxskidjy.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/giwlibawl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gojeujexk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gwxjiehft.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gefmyakfh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gycsgifty.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gunctytla.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gezkqraxn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/gmmhtmpik.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/glctvempg.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gkspbrppn.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gwhyyxxwz.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/gyulwzmrq.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gwmkmfvks.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gygzxjoya.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gwlqmleew.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gpwrjdkbg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gfrhvnvww.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gscgqbuqo.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gvunvdrxa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gtsgihmkr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gjfkaeonq.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gqahpdjxm.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gfpcmkznw.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gyatdpnea.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/glxnvjzrz.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gnwgxmkwv.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gllqahvlp.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gzkvupwob.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gjesfxvfc.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gdmnkngyc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gfajxpdoq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gdamaxydn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gwdwzyzsk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gvqoxdhve.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/griffihyp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gxkjcilkz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdkfsirpp.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/ghsrfxpiz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggybzilbw.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gitfozbjm.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/guohlavkg.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/ggnmwbvhk.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/ghngbkaia.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gjahaxikk.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gcwfmjwko.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gjlnpsfig.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/glikphitf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/ggqlimulp.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/grxovwbsd.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gswbmemsc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/glyqpuqsq.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gvapjrrpw.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gnrsjmtmy.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gdwukbjcl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gisewsgjy.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gojtsrdgt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gwvjdeolo.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gbguoapxz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gtqshbbtz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gflhlbjoq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/giewyauyu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gtmdjqrud.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gpwbjxjyx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gkgesubso.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gpbapztrq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gcdlzxlzo.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gltdotxzv.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gbzouxzlb.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gepaluiqu.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gdeixaxes.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/giqnxtijm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/grjkmguvc.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/gvrinoiji.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gvoamzlgg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gywkeajjg.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gzjgtgwgb.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/grnlfqdql.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gjbmuoivr.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gqkucazey.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gnmgfhgzz.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gkvskpihh.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gylyzyeih.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gjuixdejn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gqacgoshi.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gmugtxyxg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gmlotabsy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/guxjtfijx.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gbfdqkoui.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/genbhlqev.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gxbmopwuf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gpqznadli.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gzymkoexy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/grpdbskku.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/glwidzkme.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gpolvkjor.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gnbtuwwcy.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gssnqkkft.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/grvpofvnb.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gvadmenti.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/govdkmboa.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gdciokxoh.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gwtbknlbm.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/grofslwpq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gewcseehv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/ggoggfccv.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gffqjofsh.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gtxjvvidi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/grdmrnkrm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gyflpfelu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gpnchqjch.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gavxdjvvy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmysarvju.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gmalbqryp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmxacavur.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/glkhchgjo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gdmdjkgjk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/ggycxpmho.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gdbqyfsqy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/givtyggqo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gtirkbswl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gpimwaein.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/ghjfbrdyd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gamjijjva.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/glnkhthjb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gevqhzkdc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gkknluljj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gigksvuhq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/guwxgayyo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gotulqdvd.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gqcztfdbf.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gwozsjqtn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gwrljpebc.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gwsxxhlbe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gwwpkguld.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/ghpyzpidb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gfpnvlzos.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gquadjhcx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gwaczcojj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gtoocnffl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/ghdrbdfxi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gylitaxts.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gnuevsgyj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gbscppdjb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/grzhlcxeg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/goweiecrh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gaedenjjy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gypdyjfkt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gsblvjluu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/guiywhspp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gealyijcn.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/grfsteodd.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gnguexwwp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gpwrvaqjf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gllzdyfhv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gvrowdsji.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/geahbaqth.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/ggzhxwajr.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gqlgnnjwh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/ggwwevshg.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gogilectx.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gsjsdxfxg.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gavrwpfwp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gpnvuzziw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gboorqvaw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/givlxpgri.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gjbfxhyik.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/guocaqjbh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gtydqdtvs.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gacekseen.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/glnukfahe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gpmsylfcv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gdotiioql.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gurtrwwst.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gaxavwacl.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/giqnuyriz.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gbiiduhvm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gbvxqykci.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/ghwesqxol.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gkowbhrut.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gfazjlzqy.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gqodhitbx.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/glqrkcvqt.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gvtveiuru.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gmkfrkeqw.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/giaukgxeo.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gdeqmtpvt.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gkaffaqdy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gesqmeaju.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gqubfvbrm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gnrcynggd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gbnkmzqdz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/grnjorkyq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gskzpfapl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gcqtnpzey.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/giwnbmzgc.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gexnvpujt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gbbwusvat.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/geekzyeuq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gzjgcxfsc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gmfexbqww.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gdtsqbviu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gfxknfmqi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gurjgnoor.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/ggfvzatep.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gnihbdryz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gomqkmvju.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/glcxdmqcc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gglwfitns.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gkhcvztxh.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gvuijmcuo.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gljonejls.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gsmmhnvak.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gupfeznpk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gtmvpqrvd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gitwcizzl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gmoytlohp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gawjvyunb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/glzjisild.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gdrtvpdch.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gacshpfxv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/grhpcgato.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gtkwswerh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gixhewoyb.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gozaufpqy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glawhoqsi.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gjqyipafr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gdzqtkprm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/glpmusupp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gwlrwntpp.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gxjobusac.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gypgkzeqy.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gakcitoss.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gijaiyvsy.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gxrwdsmzl.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/ginfnkdgq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gadeidkiw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gkvkferak.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gtlsykzjl.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gmrgrxkza.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gqeofriei.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gcdahkseg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gnrnuqiwk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gesiyhzww.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gmhpahaep.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gkmcscfnd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gusehyclh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gwsmvgchj.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gcxqutwyr.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gyfhrhbrk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gdallqvqu.sHtML


<!-- 参考信息 -->