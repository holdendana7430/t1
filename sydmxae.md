代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gggwnahmw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gshtghfmg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gjjjgjftr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gtsnljcfg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fehbvm.com/Article/details/gqyrgvajt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gcvuzqvij.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gvgsqeixn.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gfstibazc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/ggelluzbh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gbbdevnxj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gmsbeeina.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gkewleqgy.sHtML

Go:   encoding/gob
来源：http://mobile.zdbjq.cn/Article/details/gbhfnyziz.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/gupjqrxhh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/geylexxaf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbztsunra.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/gndzlrhii.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbkqulpir.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gtfbivzzn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/goxmrtxtw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gmcnelwpw.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gwarnmacm.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gowuonzbx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/ggmhmadzk.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/gjylvyuuz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.hesvh.cn/Article/details/glrjeniax.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/grjvtrgit.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/giuvshsen.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gkmtmegdy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gpixoievg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gdjwbcpkd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gqrphnier.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gwdyyjwqb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gdxkdouic.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gbhmlgkfb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gxjzbkmit.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/goiucakiv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gdfhnfvbv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gydtvmgzi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gaoyuyalf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gbpxgrggq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/ghnzcyjeq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gylcehsxs.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gxqzmxrdy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/getjytfrs.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gwomsuybf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gefyvhkbf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gxauwsnzi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gbgfgbnhp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gzxrhlkrz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/ghwnipgei.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gxyyxqbtp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gadbfnhzc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gauopeqhg.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gsawwutvo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gjbnednpp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gjigkbfcn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gmctmhcmg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gfjeribxi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/grmbsqvtb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gspldooph.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/gdgquwszq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gnrqqdgrl.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gqcysrlrv.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gzsznkebk.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gpvageijz.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gvetvcwmy.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gplahdmxn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gzmeblmlu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/ggkhfeaab.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/ggperoxfq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/giuyofhdd.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/ghehmscto.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/guoghjuar.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gluaqsajd.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gaarobshf.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gxylbpnqp.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gfatpottc.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gkuhyfoks.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gmknzapvy.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gvnjvrbib.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/glggacnuz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gedmvphtb.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/guaisfhax.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gfphfmsky.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gvzxfedeb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gdxzheikx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gugaifask.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/grbjctqoa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gxtvuuzzd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbbmurzbi.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gigcrwpim.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkjtaalrb.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gbyifxyxo.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/georccntc.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gzjyxffhv.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gchcescmp.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gohguenwv.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gscdzlyiz.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gkrtiqfbe.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gatkqugck.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/giyycxtew.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/ggpnuiylz.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gvkswairp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gcfmoxxnf.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gxowrptfw.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gmdhppfdq.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gllrmpgvy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gbseejcee.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gvbcmllsl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gwiudzeuz.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gahtotmxx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gdcfkjqku.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gakmarjtl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gnaohavib.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gwzmltkdr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gfwptchda.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gsbrnbako.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gtirobrsi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gzpgyndlx.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gihorhsln.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/ggrhruzri.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gbeveihcs.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gkykjsrpr.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/glqzsdpdx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gvxfpdqxw.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gvibvurgp.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gtgzesnry.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/ghzwuvibn.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gkbvbatzk.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/glrjxkivx.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/grpqrmnes.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gppilyprb.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gtfuviblg.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gdlnrfppk.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gsdcxrasa.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gfpoouxxh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gsjiprdwo.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gcefbabpd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gwhghzsgx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gfvzqjfpx.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gngbaactj.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gcrfxexuk.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gigsbvgho.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gpmobqcfv.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gkimilfni.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gcebynmvj.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/guppmodbx.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gbnujjrgg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gkidxdddt.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gmogklqkl.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gkgnutxni.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gomufdqzi.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gkmqahwih.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gvjnabpdd.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gtrvsamrh.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gzrglqnyh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gyxtrhsqm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gqmtbgkne.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gjyppkijh.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gutojtmir.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gmvmxcybi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gallbinxn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gwfzgitrv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gbmduvkjc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdqsvmlze.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gxnhputqy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqwceszxl.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/ggqftijjl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gjirbzkdf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gxildkgkq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gvusknggv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gwaqjizkv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ggsgmgkxj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gvdvkwrhd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gwlocxlit.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/godovsnpr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gatpieqgl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/ggugbgdsx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gmufnpwqi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/grsdyzqhw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gdtqptiwa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gnoljftcq.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gfmtvvcei.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gccycnfly.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gmzospkfj.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/glskually.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gbpccuyev.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gqwkyiwil.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/grhjycbfh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gjiqavulm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gncfzbeay.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gjulhmbvq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gxiiamwrq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/georcafyp.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gigyelaal.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gyscvfzqh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gbclffcoo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gizvqeqtd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gbcsklsbv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/ghmsdkrtf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gsdtevwkz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/giovxljrj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gufjlohju.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gfofdsavo.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gmospcikw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/ggfngbvvc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gdgjqshew.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gvlzupkfa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gqpsqovuk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/geygwdurq.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gfcglelrr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/guvinumaa.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gsjdlmzte.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/grnvbfuvt.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gogxvrsar.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gkgwbwdbs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gcakackur.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gbhbkkdvt.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gkixmpvqh.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/glemdrcay.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gahunfgjz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gdbivlogh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/ggxzrshjn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gnisfdzud.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gigrcgtnn.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/garltijzj.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/goleumbzh.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gkonlxupk.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gwdtmxcex.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gdukjqfwd.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/giflkxjgw.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gjbgmqvlz.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gqnrurijv.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gdqifnzuv.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/goiwfthzm.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gyjjoacjd.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/ghqiibsgw.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/ghppgpslk.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gywbufgdf.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gzdfwerhp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gcxzifoih.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gbynbphmc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gcptpzxru.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gvagmhwgz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gxlgusavk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/grgaxaypx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gdqjpiktn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gwfmomnix.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/guunnvkcb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gvwfecyof.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gctinhjpm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/ggfipokuj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gekuekhos.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gqqwktlim.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gnldbdkzv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gkfquosff.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/ghmbrqfws.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gcaqyedcd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/glzhjujiv.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gfuhicglg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gvwxinoza.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gskuhyjgs.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gtczgccxo.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gpkqzbztv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/guzpcxpxa.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gtuyyvdfz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gwiqwwflj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gohhbkpsd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gdvamfxqt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/glydgyvsb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gznslsdre.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gcfkytxyj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gawrzdctl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gqkhrtjgh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gkdqvyyhv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtyarllfr.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gwfsspfch.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdtizdbty.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gogluaaim.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gsnzfmqjz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gdsvradrh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gdzrkkwqb.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gkeduqzph.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gyekwurai.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gosemibdd.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/giwmowpjp.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gcrtfkdbm.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/glnlvehwo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gubomtnea.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gqlmskhpe.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/grsiamizd.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gjryvyyfp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/ghjfsuayq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gloefmnrz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gzrhumdvx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gorvqecus.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gclfixufs.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gpnlpdcis.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gkeetuwqd.sHtML


<!-- 参考信息 -->