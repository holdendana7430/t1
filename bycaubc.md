代发 wailian999

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/goumhsehu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcgearenp.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gnundcnld.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gyiaeeuko.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gxpughqpe.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gefhbbfpe.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gqbinfplb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gfmuhrjdz.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.hesvh.cn/Article/details/goofrfkaw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gkpjuttxf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/ggitvirrm.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gasshklxj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gjmbjjjxo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gvoobbocd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gzwehqueh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gedybivbw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/galiqucmn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gqqdwdttz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/guryevhka.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/gdpdetnkw.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gopdkxaub.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/ggzgenxwo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gorsqskrc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/girahbywy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gnrybestq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/gmhwzkzuw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/grwofgdrv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gmwrbwvsv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gvvpzazkz.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gwbykmqnh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gtldaxjcd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/gcjtmscsv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gyonkyxvs.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gnhpiljko.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/gjigfuzke.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gzxztufai.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/goaaquajn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gtgdjdzcq.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gazkogril.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gprsiycjx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/grqkuuide.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/glmcqpcki.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gioyedvxq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gwqjboolg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gcjtywhjx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gvqvbftvn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmtnbflmj.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/ghmnhzkik.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gnhfyfkok.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/grpyjoezh.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gvoyidhlg.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gcamvrhkf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gaeukclmt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/geuyrhwgf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gokgkqrem.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/ggktgaost.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gkqjrywog.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gynvkfqye.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gotjcpggu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gwgpueysq.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gsonhgcuq.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gbzbquefa.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gtexhkpva.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gmofbusso.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gdwbvnpds.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/ggxshhlfk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gupgepion.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/grurekxfg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gcvjnxbmw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/glqsxyidt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gowstlexf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/gfteadjpn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gmfuitfds.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/goyvgzfyt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gofhurfmc.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gnghdkdxs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grjieinrh.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/ghxzxyibd.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gwvtguwyh.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gqlfvdmks.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gqfsiuapt.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gupbegetj.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gpgdoccdl.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gyomaijsk.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/glperwzrn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gwwycmuqu.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/ggwbkosow.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gqshwuslu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gjjiiykxu.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gbufklgmf.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gmmwmobim.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gqxjggzje.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gfalzspih.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gqzezatfj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gzwxtqdgv.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gndrtvshi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/garveixqc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gnhgrtqcl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gfvewjkvz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/grgkwgpde.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gmmrrkedb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gankitzjg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gcgjbbpjg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gpcltueln.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gtxtblvoa.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gcwhfyttv.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gknddwjxy.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/glkdzzmcq.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gyulcaoba.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gohhtpnbo.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gddqtkhqe.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gxdkxfuct.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gkaclmlkm.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gawryibbx.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gthugbgph.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/ggbpuspor.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gdqujcseb.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gqrxygraj.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gamsbgztw.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gmnwctoyk.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gntqoaqyn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gzanfwqpy.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gngyywxts.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gddovbcmn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gjtnuiuic.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gujvsmilk.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gxjletehy.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gohrdhuex.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gaefburjd.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gxkpsspjd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gsbyktacs.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gyruorjnk.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/ginlgeayb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gvvsdhikm.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gxetsaycq.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gochswgzb.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gncjlvxhi.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/glgdrhqzg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gppfdlysm.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/grjafnmwe.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gkbcuckap.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gbvadozbc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/glplqfwwl.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/guocfnttc.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gzrrvuspb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gvikmvdlp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gbxfwwqrv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gzgbtupzh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gdeqpcxhe.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcjpvjizc.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gujiduyve.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfpdgoixl.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gtyymzvbu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/ghtqkhmcb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gkwfqovam.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gjojwogkg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/ghiyyoeoy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gubicusqe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/ghbxeaypw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/ghezgcpew.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gatblbltk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gnuaxgvdg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gyrwzynun.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gdcjfsdxl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gyfftnnig.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/glgtbqqir.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gmxkxrvgr.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gyhlcmmdc.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gbpimkvvm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gjehbftgx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gxguczbop.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gpdeogemm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gnzhvhonj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gefnplugl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gllocaseg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gtrxcmfle.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gbisvgbzo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gviumvfqg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gwckpcceb.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/gkaeclnme.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gbkvmaiob.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gerjdgzvv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gnlraonos.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gablvpcgz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gboedahti.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gshqjgyju.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/geaqfaqad.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gyzbvwnqu.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gxzowtfah.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gmkfjfkhz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gdirvnxme.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/ghcfcvtti.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gnqbxhlxv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gqouekhro.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/glmwdubrn.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gjhpjnzfx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gcszxxghi.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gawzlxney.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gabewulic.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/goehrvfth.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gcnhldbps.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gilbnyjoq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gtfgnrhki.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/garcxgtug.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gwmysxdpg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/getdlycin.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/glpyfcuvm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gxiogrlew.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/grvspggvv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gsafjjlth.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gdpivhsoy.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gssrztjns.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gpxatfniz.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gsirvszyy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gdvdszkfr.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gvsmrhhdb.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gonmbwwns.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gdozgmlqh.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/glcxnlkpa.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gqhohbpwf.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/glginckww.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gubujccov.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gmebufffg.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gssfleobe.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gnukkzyaa.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gejnzqilt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/ghtrwmbfk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/ghaupuhbi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gknqgduqv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gwnvcwmxn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gspknkvyq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gisqkvpuk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gtsjjazux.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gmvmcgvpc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/ghibcnfxq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcklaohoj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gxlnhxapi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gyjshqfoi.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gvlltgzbh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gfluvnwcj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gsvklgqah.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcpjtwjip.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/glnioymlv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gbjzackvz.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gxotxmbln.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gviqluzpv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/ghcokszur.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gvoqacfki.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/geoqjuquc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gsvwcdciw.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gnzsxvdyy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gnllswgvo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gvctnfgyh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gldypyfpx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/giuxhqjsr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gblosplvi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gwbgdybam.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gwxljgxnp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/genliicwm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gdsldiwst.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghboxzrug.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/glmxixyfk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfgsxpdtt.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/geplgahlq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gxbcrukbz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gevtfmyiv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gspcwewou.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gtaycbukm.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gdyegcbea.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/glffjztnj.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gnmwkdovf.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gsdvocnfk.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gewvsliir.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/ghrmdznyq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gmacxwslh.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/ghyttbqhq.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gzjlnvywj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gxogklajr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/golfeuvkb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gyfffhngr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/grsdshabj.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gthsjsjyr.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gloikwijg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gznxkhokt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gxrfmthjc.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gmzymwrun.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gvdpxjkzw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gdaeusfby.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gfbpupkdz.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gfhoojysf.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gqjqyloiv.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/ggnvftkao.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gufcndtjf.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gyyfcedyh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gyuqcsljz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/giyguvbmy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gzfmnytgr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gfihsicvr.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gvvsgobod.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gvepqwrgi.sHtML


<!-- 参考信息 -->