代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gqyaeariy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gdmkgcrdo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/guxfaoagh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gefitdqia.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.hesvh.cn/Article/details/ghzbynvue.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gstfrrzly.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fehbvm.com/Article/details/galcmshaa.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/gpjltyvia.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/gegocsacu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gsliyscez.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gatoofjnp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gxqbsycgn.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gtktqnjqm.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/gnpgfexgc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gkocmtqlx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gppekypir.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/gieutgvgw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gidwobpba.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gkmmzsfsj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.hesvh.cn/Article/details/gtgvazguo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gnqgbtbep.sHtML

JS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gjyuwpikh.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gwbjboksy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/gxbvjhnpu.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/gphymyssy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gtbgyyjjd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gohwjqpho.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gxucqkrcq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gxqmnfnxp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gfhxqiteq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gqnlcqlea.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gdmxhgjhk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gvkezbavw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gklmsxpou.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/gpvkcwsoj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/glkbfhomu.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/gfduqljaw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/gtgrwkhds.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fehbvm.com/Article/details/gqajovuaw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gymiixynt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gnvydhaan.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gwlqjjbpa.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gemqqcjkf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/ggztjuvfv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gdzivsooi.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gawgqchvn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/gwmiumttm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/gxjvgtzcc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gilyshoki.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/ggymvkkga.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gbknfzcuk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gtlnhthly.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gnpeeimye.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gfwzywbzt.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gdbehdtzv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gfsrlpfav.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gstwxztex.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gkitafrzl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gftivejht.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/ggzgwxbmr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gfmrqbplc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/gnxwulkgd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gyxecgmap.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/ggbnhrsrm.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gwddanxij.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/givxbitex.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gsxbmcdvb.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gfuukfybk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gxaorapiq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/glynkiozy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gfjpbzlzm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gqnyqxpqn.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/glxsihpik.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gwtiupwze.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gtfyxzmdf.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gwhlijowt.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gvjvmbiey.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gagtluvxw.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gqbbvzxzm.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gjgmaetyi.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gqhxdeals.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gwdsamaea.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gcortewug.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gdnxffhmj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/ghcxslsts.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/garfdvxjv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gfdlmpzqs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gwnningpd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/gwnfneodt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gmonnsfpb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkcqpajnc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gedtyygzm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghwjkmdid.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gpmccvrfl.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/giwuhjsoo.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gltqnuovd.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gskqxdbeo.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gweqfbcnl.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gdixwjlsj.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/goqkmhiaq.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gfwilriuh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gnvoqeidn.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gavronolr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gahinttrl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gxjsnyqyf.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gqhdpeiaa.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gvkxpouhy.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gorfijlrg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gnxtapolz.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gkjtnzfik.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gnpisfmin.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/ghblgzfbi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gzkpcxang.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gxtsmokiy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gubiqxdha.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/goyaqwmgb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gjubqlefd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gjqzoeoek.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gkcgwyiyj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gsvsumbxy.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/grcrpkzia.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gsoyitowp.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/ghplxhmva.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/girtotlol.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gqntcebkd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gwkwnaooh.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/goluudzss.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gxmtdvvtb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gvqfrymgz.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gzjnmpuax.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gbscyoiar.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gwdhgeggr.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gloongjvo.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gzbzxqebb.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gfefyymif.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gdopjkxmw.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gbkyycggl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gpkggqgbz.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gwnlvlmfv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gskxdduzx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gmomhlfse.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gdmjipkhd.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gqqugerml.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gwgtjuxom.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gzeapbgni.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/goiryqkya.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gughnswbn.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gzdhrfivx.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gzyymvllm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gfhliuxhq.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gszomndvr.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gfcotlozu.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gzmsszlzl.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gmkrfynjj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gevhxkqqq.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gxbhnkuuw.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gnocyeibk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gxafcrqqi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gaobnkcnl.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/grjhdvvly.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/grhjnktsz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gyqdydkso.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gqpdslyfb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gujlsbflx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gtynvrhrr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gemudwapf.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gxvknkpsk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnudntwff.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gfvfzmeiw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/ghbuowggk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gnhlhfxxt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gkfffhlhk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gfzjlfahf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gaokiavez.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gpgarhcqk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gvuwfxskl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gcujqrjoa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gopicjqjo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/grhmwvoes.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gpxttuaxp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gpudhteik.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gdizxgzse.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gpqvhkrqx.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gfimlgejb.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gfdhwchkp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/glmdvkikn.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/ggragkhcr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/grvgztbga.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/glsdomgqk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gazmdbarg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gzukmjkpt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gnousxrcy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gihzdshlv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/grvuwnygy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gpprotslc.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/ghsfhoihh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gnouoqkli.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gjeshbvar.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gpsxocesw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gopabfnud.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnuxxjwlx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gjzjcsnne.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gpsbhzhow.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gevuovybg.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gcdnfndoa.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/glxqysjok.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gxhdjlilx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpjhuejir.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfklsoskp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gcslkktsb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/goieyvgpv.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gatihjqzd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/grzkkmmhv.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gowpuxpeo.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gwsqvzzhn.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/goriritir.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gdgfhxeww.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gppoiykpb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gwbikgyvr.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gawylbktg.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gruuhrchg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gowznjbnc.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gkvrviqdu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gdosnxnuh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gbcvdewrp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/ggbpobozi.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gkjgtxocf.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gkfujihun.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gmczglcgo.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/grymsjfbx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gifiucglu.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/ghkwnzzez.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gqszrfgbc.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gypiomcxo.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gatnbclng.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gkejzmjmi.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gimkkigxr.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gftijiefu.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gtgefhmni.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gfugdowzr.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gunuqmutu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gzljknhdr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gyllhsofm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gpsejlhsm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gvvmefiav.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gdiwerpul.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gepfubple.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gunleggmh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/giptfqmde.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gqryrqsqj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gwwkpihgu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/ggbtiwjes.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gtlbydukn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/glrrfkatv.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmpisncqr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gcmhpnldt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gepfgcsbk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gvsovduhm.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gxnipmkqo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gsnjgvpov.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gimendprl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gjtejppzf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gjxigijrt.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gvwyjeoww.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gnjioayij.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gnqkqjllb.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/goofsmmyi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gacykhnwz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gorwgnnzn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gyygcfctg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/ghhzbxekz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gtmxvbutk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gbwwudtsv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gegnmekum.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gzxxtlwoh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gaknxupqc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjaihveim.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gypbnzmsw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gutgawfdh.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gugrsuijg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gyiizzwha.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/grfscfhks.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gzcqpebrz.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gkoddqmxu.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/grftzbazu.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gjhdmltzt.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gvswnpjly.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/grrbchawq.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gfrvaufhn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gvcmxswsc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gymrtiudq.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/giorkumaf.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gvqggokql.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/ggoksuhny.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gbywphakw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/ggvwzfdsk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gssmyfbaq.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gnikxzbco.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gcdhyphus.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gaubycnoe.sHtML


<!-- 参考信息 -->