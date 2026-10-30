代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fanxiaobao.xyz/Article/details/gggsvzykb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxlkjrdv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fanxiaobao.xyz/Article/details/gngaehfue.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fanxiaobao.xyz/Article/details/gtwcxgmmn.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fanxiaobao.xyz/Article/details/gjplbkmli.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcpxhguy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gorpdsnfl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqtozfdu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fanxiaobao.xyz/Article/details/grikcznwb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fanxiaobao.xyz/Article/details/gufvblbja.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbphewwei.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fanxiaobao.xyz/Article/details/gpbiekepy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfircpnm.sHtML

[L04] 设置超时
来源：http://www.share.fanxiaobao.xyz/Article/details/gorbdxylz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsmajnwf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fanxiaobao.xyz/Article/details/glhibgzjk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gnndzjggn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmwsttkf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlffjonm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fanxiaobao.xyz/Article/details/gmxkfjoga.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gluksqunt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gkukltbnc.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkjeaose.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fanxiaobao.xyz/Article/details/gpoozeist.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fanxiaobao.xyz/Article/details/gaevviwrk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fanxiaobao.xyz/Article/details/gauhhysaf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmqxpqqr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fanxiaobao.xyz/Article/details/ggahnzcfv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gowhohngz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fanxiaobao.xyz/Article/details/gkynwuggr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdpvqojr.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gbruhbkui.sHtML

Py:   resp.json()
来源：http://m.share.fanxiaobao.xyz/Article/details/galzlxpdo.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqlynbuf.sHtML

JS:   await resp.json()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsktvfjvv.sHtML

TS:   await resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmupdcvm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxebjcyrg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fanxiaobao.xyz/Article/details/gufvuenhe.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fanxiaobao.xyz/Article/details/gwcnetzlg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fanxiaobao.xyz/Article/details/gihepulbp.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/guzpyyref.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fanxiaobao.xyz/Article/details/gsllcfhow.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fanxiaobao.xyz/Article/details/gtbwnmkpx.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbextehn.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkvtpzig.sHtML

Java: resp.statusCode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmynbcdgq.sHtML

Go:   resp.StatusCode
来源：http://read.share.fanxiaobao.xyz/Article/details/gksiykxgg.sHtML

Ruby: resp.code.to_i
来源：http://wap.fanxiaobao.xyz/Article/details/gvfznnrey.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsqdqcrm.sHtML

[L08] 并发请求多个地址
来源：http://baike.fanxiaobao.xyz/Article/details/gdmtnccyh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzblcrej.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fanxiaobao.xyz/Article/details/gdyquczwa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsczrfpha.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gmxnivzxd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fanxiaobao.xyz/Article/details/ggvxohaok.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fanxiaobao.xyz/Article/details/gzahveyxp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fanxiaobao.xyz/Article/details/gebcgvcez.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfijcuqit.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gekwvwihp.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fanxiaobao.xyz/Article/details/gzebvfbzh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmieqasm.sHtML

[M01] 读取命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gscviwxsc.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwgiysmi.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fanxiaobao.xyz/Article/details/gijrtvoji.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsogpfsiv.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgdbvzkp.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fanxiaobao.xyz/Article/details/gaklhokcr.sHtML

Go:   os.Args[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/gadjplsgm.sHtML

Ruby: ARGV
来源：http://baike.fanxiaobao.xyz/Article/details/gyxhdewkb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fanxiaobao.xyz/Article/details/gqcrajsik.sHtML

[M02] 读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/glklryxbi.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/galnyothh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqqfvfdg.sHtML

JS:   process.env.HOME
来源：http://wap.fanxiaobao.xyz/Article/details/geatmlleo.sHtML

TS:   process.env.HOME
来源：http://blog.fanxiaobao.xyz/Article/details/ggzjonhkj.sHtML

Java: System.getenv("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gikpgwgeo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzqhxjyn.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fanxiaobao.xyz/Article/details/gmtzefcxk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/gliepaehb.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryjrdsmo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzvlnzur.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsvtfbga.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/glbsaohsd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjmerwih.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxfxlxkn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fanxiaobao.xyz/Article/details/gvxpzsqlr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fanxiaobao.xyz/Article/details/guauxpqgz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fanxiaobao.xyz/Article/details/gfcmgkfuk.sHtML

[M04] 获取当前工作目录
来源：http://baike.fanxiaobao.xyz/Article/details/gvuebdglb.sHtML

Py:   os.getcwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gemqhmhqc.sHtML

PHP:  getcwd();
来源：http://read.share.fanxiaobao.xyz/Article/details/geemcnzet.sHtML

JS:   process.cwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzltzaoa.sHtML

TS:   process.cwd()
来源：http://wap.fanxiaobao.xyz/Article/details/giapgsabj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwpnagjn.sHtML

Go:   os.Getwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdoecdbd.sHtML

Ruby: Dir.pwd
来源：http://mobile.fanxiaobao.xyz/Article/details/geadmpdkg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fanxiaobao.xyz/Article/details/giiwjcbhd.sHtML

[M05] 设置退出码
来源：http://baike.fanxiaobao.xyz/Article/details/gtgcdfkkd.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonypfamv.sHtML

PHP:  exit(1);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbpnfzkf.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohwpqefe.sHtML

TS:   process.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwchpffxc.sHtML

Java: System.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyeheazr.sHtML

Go:   os.Exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gawiqfbpx.sHtML

Ruby: exit 1
来源：http://3g.fanxiaobao.xyz/Article/details/gjiioxjad.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fanxiaobao.xyz/Article/details/gtioedeis.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviugkjlg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gossxeaff.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkngutwk.sHtML

JS:   console.error("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtokfupke.sHtML

TS:   console.error("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamkdndnc.sHtML

Java: System.err.println("err")
来源：http://blog.fanxiaobao.xyz/Article/details/gxupxevye.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fanxiaobao.xyz/Article/details/gmjjskibk.sHtML

Ruby: warn "err"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwjixsgj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaofpfpm.sHtML

[M07] 判断是否为主入口
来源：http://blog.fanxiaobao.xyz/Article/details/gujerfdul.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtewbybak.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fanxiaobao.xyz/Article/details/glxlzhibb.sHtML

JS:   require.main === module
来源：http://wap.fanxiaobao.xyz/Article/details/gfytyqbzi.sHtML

TS:   require.main === module
来源：http://m.share.fanxiaobao.xyz/Article/details/ggntemyjk.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxvsaewd.sHtML

Go:   func main()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkkxmscc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqsjmugo.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fanxiaobao.xyz/Article/details/getdhykvh.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fanxiaobao.xyz/Article/details/gwgujbxuo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fanxiaobao.xyz/Article/details/gozkwgvjd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fanxiaobao.xyz/Article/details/gzgkyzxan.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fanxiaobao.xyz/Article/details/gurktddif.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuprlhmr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fanxiaobao.xyz/Article/details/gbdwuhkbi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fanxiaobao.xyz/Article/details/gpllevqtq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fanxiaobao.xyz/Article/details/goxyatypd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fanxiaobao.xyz/Article/details/gwotlylot.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkqvoity.sHtML

N. 数据结构与算法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrrrhzrp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glmoonggt.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gksxcklvl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphfnszrd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhtfqnqi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctsixdlk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/guubojlgm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdddtgtgt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrbzwajo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fanxiaobao.xyz/Article/details/govphkmuq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gopncouky.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzgsfwon.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gkqteiujg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gspruyvrr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gmddilnwa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxeqylbur.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gidqmbjtu.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gibleyujt.sHtML

Ruby: arr.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqknohry.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fanxiaobao.xyz/Article/details/grmxxckyh.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fanxiaobao.xyz/Article/details/gbckpyzxr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fanxiaobao.xyz/Article/details/givasgclp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmqaiqbp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkakxeaz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fanxiaobao.xyz/Article/details/gezuvexou.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fanxiaobao.xyz/Article/details/goryhkmjx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fanxiaobao.xyz/Article/details/gbrksafzm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fanxiaobao.xyz/Article/details/gxdqpwryl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fanxiaobao.xyz/Article/details/gdjoegvdk.sHtML

[N04] 斐波那契数列
来源：http://m.share.fanxiaobao.xyz/Article/details/girwukfki.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipqwlpwy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fanxiaobao.xyz/Article/details/gzjwwrbix.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdtpxaai.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gqowshxdz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/galvevdtw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fanxiaobao.xyz/Article/details/glhuorfao.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gacpuvbsf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gutslosqp.sHtML

[N05] 最大公约数
来源：http://baike.fanxiaobao.xyz/Article/details/gwyfrcszz.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/gbdwsunow.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktmlksdp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/gomnxpzza.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusedhgta.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fanxiaobao.xyz/Article/details/gfhcidhnz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gndjeenxv.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprtlctuz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fanxiaobao.xyz/Article/details/gipqrnprl.sHtML

[N06] 判断回文字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gmymvpfar.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamqujgaf.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfklokht.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gbdhenssc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gfgbready.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fanxiaobao.xyz/Article/details/goqfmgznr.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fanxiaobao.xyz/Article/details/gcxytnitp.sHtML

Ruby: s == s.reverse
来源：http://wap.fanxiaobao.xyz/Article/details/gpjmbxhcn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fanxiaobao.xyz/Article/details/gxjzoerdl.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fanxiaobao.xyz/Article/details/ghcewcjmd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnvwbrhy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fanxiaobao.xyz/Article/details/gkolswcvs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fanxiaobao.xyz/Article/details/guyfxwtfo.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fanxiaobao.xyz/Article/details/gzthcisvd.sHtML

Java: // 手写 HashMap
来源：http://baike.fanxiaobao.xyz/Article/details/gykedfyft.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fanxiaobao.xyz/Article/details/gbrvfockf.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fanxiaobao.xyz/Article/details/gjybyfvje.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fanxiaobao.xyz/Article/details/ggrtbavec.sHtML

[N08] 生成全排列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznjewkts.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gijdczdfq.sHtML

PHP:  // 手写递归交换
来源：http://baike.fanxiaobao.xyz/Article/details/gdnofjuky.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbhginho.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerdjwslm.sHtML

Java: // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gpjammsus.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwryhutgw.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fanxiaobao.xyz/Article/details/gdmxvcyte.sHtML

C#:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gljbwupzw.sHtML

[N09] 栈与队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbqmznys.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/gmtrmihbk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gxjclmold.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gpfhlmszm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtkygjzz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkgksgyy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghibdrhpn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/glzbrfzjp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fanxiaobao.xyz/Article/details/ghtblmdbc.sHtML

[N10] 链表节点定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbwmmmgu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geagccetv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvmsntyx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvshjzks.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmqejewt.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfmepjbp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezzwrkho.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fanxiaobao.xyz/Article/details/gmecoqkud.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fanxiaobao.xyz/Article/details/glayrypew.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fanxiaobao.xyz/Article/details/giejyotgi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fanxiaobao.xyz/Article/details/gvogesuoq.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gubylsgam.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fanxiaobao.xyz/Article/details/gjknwwatb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fanxiaobao.xyz/Article/details/gfnpsbiyi.sHtML

Java: // 手写递归
来源：http://baike.fanxiaobao.xyz/Article/details/gcrfzkxfc.sHtML

Go:   // 手写递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gylhqlryn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fanxiaobao.xyz/Article/details/gnrypsxqe.sHtML

C#:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/gdojcymlm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fanxiaobao.xyz/Article/details/ggtofbmxi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fanxiaobao.xyz/Article/details/gupqbcqcy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhkbxkkn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskvwempl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlgmjjhw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fanxiaobao.xyz/Article/details/gaztfkjoo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fanxiaobao.xyz/Article/details/gbevwinhn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gqjlfjrcv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fanxiaobao.xyz/Article/details/gjppubqtt.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstgutlit.sHtML

O. 并发与异步
来源：http://blog.fanxiaobao.xyz/Article/details/glaobpizf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gromgiceb.sHtML

[O01] 启动一个线程
来源：http://baike.fanxiaobao.xyz/Article/details/glwxagnrw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueydcbuw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyniqiqu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fanxiaobao.xyz/Article/details/gayjdlupw.sHtML

TS:   // 同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/gtsojcvwt.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdzztacd.sHtML

Go:   go f()
来源：http://3g.fanxiaobao.xyz/Article/details/ggskvpfcv.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpbyidbp.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbbgvaof.sHtML

[O02] 使用线程池
来源：http://3g.fanxiaobao.xyz/Article/details/gnxqbbhyf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gluueyllk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fanxiaobao.xyz/Article/details/gzjjvwuio.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuqcxmks.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjzvwqck.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/glskuajnj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fanxiaobao.xyz/Article/details/gnrrhpoet.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fanxiaobao.xyz/Article/details/grniduqua.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnyfwuew.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fanxiaobao.xyz/Article/details/gozzisyxr.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjblllfx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcsmslip.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fanxiaobao.xyz/Article/details/gipfeleju.sHtML

TS:   // 同 JS
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjsrdceh.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gywadevli.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshasndrd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchilcuhw.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fanxiaobao.xyz/Article/details/grxatcstu.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gtsccofdk.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fanxiaobao.xyz/Article/details/gchdlvdzl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocnawofm.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/golutsvhd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gepbqefov.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowtyucea.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fanxiaobao.xyz/Article/details/gwpmycpwk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fanxiaobao.xyz/Article/details/grhcmsfjt.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuiukuam.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fanxiaobao.xyz/Article/details/gzosbwzib.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/gnrujuaih.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmdqkomk.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/gququysod.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcbuchsx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fanxiaobao.xyz/Article/details/gqmvkxlic.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fanxiaobao.xyz/Article/details/ggnkxnmrz.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvvpzkoj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fanxiaobao.xyz/Article/details/geoxycehh.sHtML

[O06] 使用进程池
来源：http://3g.fanxiaobao.xyz/Article/details/golkfhpzb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fanxiaobao.xyz/Article/details/gyxnbcedv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fanxiaobao.xyz/Article/details/grssjslwb.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxligrhi.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fanxiaobao.xyz/Article/details/gngxkxyfp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fanxiaobao.xyz/Article/details/gxhrsezbh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfucnnwr.sHtML

Ruby: // fork 块
来源：http://baike.fanxiaobao.xyz/Article/details/gurfdpkeh.sHtML


<!-- 参考信息 -->