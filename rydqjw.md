代发 wailian999

L. 网络请求
来源：http://hz.iojbl.cn/gtxqgpjlvg.html

================================================================================
来源：http://hz.ydzc1.top/gtqliglsfy.html

[L01] 发送 GET 请求
来源：http://hz.pengpengdd.cyou/gttweisuzz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.pycfn.com/gtzkxfwujt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinqigfzy.top/gtswbcxssl.html

JS:   await fetch(url)
来源：http://hz.tanke756.top/gtbwemzeew.html

TS:   await fetch(url)
来源：http://hz.redwolf501.top/gttrjosyrl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.c1oappe.top/gtahfbrjzt.html

Go:   resp, err := http.Get(url)
来源：http://hz.c1oappe.top/gtkvbeuggh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhiwuduotai.top/gtcrzusrec.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shanyushiyangkeji.top/gtfyzpprjd.html

[L02] 发送 POST JSON
来源：http://hz.daria6918.cn/gtsivejtov.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shanyushiyangkeji.top/gtmowjsxps.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.haohaochexian.top/gtbpbmavbf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ydjk.org.cn/gttzhdxlpr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.svipenyu.cn/gtifbbbmqv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.chenzaomai.com/gtdzntqzwk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ybcxt.top/gtdfryfjpp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yangfankeji.com/gtthtbtmwc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.quarkkingdee.top/gtpbjueofy.html

[L03] 设置自定义请求头
来源：http://hz.jiagoushi.top/gtqgyoimpi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xingfuxueyuan.xyz/gtupbkvoaw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shuidangran.top/gtnkkdiyin.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.9152youxi.cn/gtqnugsgdf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yangfankeji.com/gtggixghdf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhaomingkeji.xyz/gtcsyqpyyu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hysaishi.cn/gtuivadboq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ydzc1.top/gtuocrmowh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.chenlongwang.top/gtiqzjbyzs.html

[L04] 设置超时
来源：http://hz.ydjk.org.cn/gtabawrzii.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jinghuilouyu.cn/gtvkkmfstv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.aibaodan.cn/gtsvgdxsul.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cucudq.cn/gtfcobgqwp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yongpay.top/gtsnkvmfhs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sxryk.cn/gtyuvafoja.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gaohongyu789.top/gtvmrmqtqt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.9152youxi.cn/gtfevygwty.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhixingplan.top/gtnkbwvjri.html

[L05] 上传文件（multipart）
来源：http://hz.zhengqikj.top/gtxtjjxnxq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.birdmap.top/gtjobrxaky.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jqgufenzy.top/gtpxmnwcnp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ywan-chungtsiang.top/gtqcyjcdzh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sysykeji.top/gtcktpjwds.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ppjwa.cn/gtwlinanql.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yonumen.top/gtnswrycfc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.pengpengdd.cyou/gtyisvtkkh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.vqdsnc.cn/gtrozhpaax.html

[L06] 解析响应为 JSON
来源：http://hz.hnqzz.top/gtxvohexay.html

Py:   resp.json()
来源：http://hz.redwolf501.top/gtygmsqqnt.html

PHP:  json_decode($body, true);
来源：http://hz.nwbrower.top/gtwydyffxz.html

JS:   await resp.json()
来源：http://hz.jinqigufen.top/gtrqitmpgk.html

TS:   await resp.json()
来源：http://hz.hywenlv.cn/gthhylytvs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.9152youxi.cn/gtqazzmnfc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinqigfzy.top/gthihdinmk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.c1oappe.top/gtdbpylhmv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hfpthk.cn/gttazqqbyn.html

[L07] 处理 HTTP 状态码
来源：http://hz.gzhubu.top/gtyfygvnna.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.mhx1999.top/gtpokssagn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hammf.cn/gtqvtrugnf.html

JS:   resp.ok;  resp.status
来源：http://hz.wangdashe.top/gtwuxmfnil.html

TS:   resp.ok;  resp.status
来源：http://hz.ivvv.top/gtyvnaoybn.html

Java: resp.statusCode()
来源：http://hz.hongshengwenyu.top/gtcdvqcvfz.html

Go:   resp.StatusCode
来源：http://hz.yj202588.top/gtsrlzfllo.html

Ruby: resp.code.to_i
来源：http://hz.cdnleiting.top/gtctxedxnp.html

C#:   (int)resp.StatusCode
来源：http://hz.yuxming.cn/gtsaalciqx.html

[L08] 并发请求多个地址
来源：http://hz.0kj1m.cn/gtkxnooqns.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shuidangran.top/gtzkbthabp.html

PHP:  curl_multi_init() 系列
来源：http://hz.tanke756.top/gthpqullfb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenlongwang.top/gtnvpirrxm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenzaomai.com/gtqjuzmrkg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gzhubu.top/gtuvmvvjib.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cashguo.top/gtoyoqrtgz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.tianlin.xyz/gtdxvwcqwa.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yj20258888.top/gtopxdueer.html

================================================================================
来源：http://hz.yj20258888.top/gtxslzyliy.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhoulong.xyz/gtrdxyuofx.html

================================================================================
来源：http://hz.aibaodan.cn/gtaudceexx.html

[M01] 读取命令行参数
来源：http://hz.yueranfly.top/gtehcdyazn.html

Py:   sys.argv[1:]
来源：http://hz.jinqigfzy.top/gtuaebnxlm.html

PHP:  $argv;  $argc;
来源：http://hz.svipenyu.cn/gtxfqbwyhz.html

JS:   process.argv.slice(2)
来源：http://hz.yj20258888.top/gtrhiiiofq.html

TS:   process.argv.slice(2)
来源：http://hz.vqdsnc.cn/gtgfogtgrw.html

Java: args 数组（main 方法参数）
来源：http://hz.ydjk.org.cn/gtvbckpxcx.html

Go:   os.Args[1:]
来源：http://hz.jianghu66.top/gtpavrvyea.html

Ruby: ARGV
来源：http://hz.zhengqikj.top/gtufhmcuwe.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xziqi.cn/gtubrwqddt.html

[M02] 读取环境变量
来源：http://hz.haohaochexian.top/gtzvvbxifu.html

Py:   os.environ.get("HOME")
来源：http://hz.cucudq.cn/gtdfgaeisw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.smart0.xyz/gtqlcgknzb.html

JS:   process.env.HOME
来源：http://hz.gogol.net.cn/gtwqfzhiax.html

TS:   process.env.HOME
来源：http://hz.tianlin.xyz/gtqxfopdci.html

Java: System.getenv("HOME")
来源：http://hz.yuxming.cn/gtfnfqbgyx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xingfuxueyuan.xyz/gtksmethlt.html

Ruby: ENV["HOME"]
来源：http://hz.shangyingyoupin.top/gtbiuqomtl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.haohaochexian.top/gtlxxjdsqm.html

[M03] 执行外部命令
来源：http://hz.ppjwa.cn/gtthjmhgay.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ywan-chungtsiang.top/gtyqdjqysz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yanxiufei.cn/gtkqoufdle.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.mhx1999.top/gttcwfbfkf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhoulong.xyz/gtiqwslofe.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sysykeji.top/gtqjptqmvy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xylfe.cn/gtbwtmesoq.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jlsjyb.cn/gtzkdsldrn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhijiandao.cn/gttejcfxip.html

[M04] 获取当前工作目录
来源：http://hz.cashguo.top/gtrgktfnjy.html

Py:   os.getcwd()
来源：http://hz.aibaodan.cn/gtlabuozef.html

PHP:  getcwd();
来源：http://hz.gogol.net.cn/gtpqbrqssf.html

JS:   process.cwd()
来源：http://hz.zdqjudy.top/gtzqkkanfe.html

TS:   process.cwd()
来源：http://hz.feifeiyinyue.top/gtzblqnxdx.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhengqikj.top/gtvlnofapm.html

Go:   os.Getwd()
来源：http://hz.pycfn.com/gtfqxvjeft.html

Ruby: Dir.pwd
来源：http://hz.sufxvd.cn/gtyifbhlhq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhoulong.xyz/gtnqgrlgac.html

[M05] 设置退出码
来源：http://hz.jinqigufen.top/gtkjbywtbz.html

Py:   sys.exit(1)
来源：http://hz.jinqigufen.top/gtvqmjlrpl.html

PHP:  exit(1);
来源：http://hz.gzhubu.top/gtzvlxxcra.html

JS:   process.exit(1)
来源：http://hz.redwolf501.top/gtuozwbxht.html

TS:   process.exit(1)
来源：http://hz.gogol.net.cn/gtorbaihpe.html

Java: System.exit(1)
来源：http://hz.ydzc1.top/gtgnlryyky.html

Go:   os.Exit(1)
来源：http://hz.zycfv.cn/gtgzqisdul.html

Ruby: exit 1
来源：http://hz.ehwqpu.com/gtzqjwpwtv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gaohongyu789.top/gtnaahoyhj.html

[M06] 向标准错误输出
来源：http://hz.pengpengdd.cyou/gtdnretpml.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinyuanbaomall.cn/gtzwhsaiqc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gotoacloud.top/gtxnuuwezs.html

JS:   console.error("err")
来源：http://hz.316326.xyz/gtnzgobria.html

TS:   console.error("err")
来源：http://hz.quarkkingdee.top/gtsuzsfyck.html

Java: System.err.println("err")
来源：http://hz.pengpengdd.cyou/gtmtmzpipd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ppjwa.cn/gtfrepiewf.html

Ruby: warn "err"
来源：http://hz.cqqwz.cn/gtpxvjyvjm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ydjk.org.cn/gtdwdfxjuz.html

[M07] 判断是否为主入口
来源：http://hz.hysaishi.cn/gtyoqazegi.html

Py:   if __name__ == "__main__":
来源：http://hz.havefunace.top/gttsazslzf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jianghu66.top/gtkdcfkygb.html

JS:   require.main === module
来源：http://hz.vqdsnc.cn/gtraxuaint.html

TS:   require.main === module
来源：http://hz.daria6918.cn/gtvnyysbxi.html

Java: public static void main(String[] args)
来源：http://hz.zycfv.cn/gtahkcazng.html

Go:   func main()
来源：http://hz.hywenlv.cn/gtinifqzsr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.wangshuangyany.cn/gtztjpacuh.html

C#:   static void Main(string[] args)
来源：http://hz.sysykeji.top/gtzqtiwvyh.html

[M08] 获取系统与运行时信息
来源：http://hz.yj20258888.top/gtdlnpslng.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ywan-chungtsiang.top/gtshtopdlr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hongshengwenyu.top/gtdikiukgk.html

JS:   process.platform;  process.version
来源：http://hz.gogol.net.cn/gtknfnyeir.html

TS:   process.platform;  process.version
来源：http://hz.yj202588.top/gtuxssqixk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jqgufenzy.top/gtdmwjflor.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.0kj1m.cn/gtlsxooryx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.vqdsnc.cn/gtczqptfqy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hfpthk.cn/gtbdzpubji.html

================================================================================
来源：http://hz.yvedp.cn/gtugpgoqia.html

N. 数据结构与算法
来源：http://hz.daria6918.cn/gtyrnutdhg.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtghyeinqf.html

[N01] 二分查找（有序数组）
来源：http://hz.cqqwz.cn/gtlagrrntk.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.andypj.xyz/gtxfoimqac.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.9152youxi.cn/gtwledjmpg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.guannengcc.top/gtesrdulis.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258.top/gtajdobmfl.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.fengsongda.top/gtfnbvnynl.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.fzhhl.top/gtnpavjhpo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.cdnleiting.top/gtcrtxeemh.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.pengpengdd.cyou/gtaopxvdpm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.52xcode.cn/gtmllmtxdc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yueranfly.top/gtdwsjzojy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ydzc1.top/gtbhggaqwp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ehwqpu.com/gtnldkywfx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gtsnazbcwt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shzxlz.cn/gtyuweqcdf.html

Go:   slices.Sort(arr)
来源：http://hz.ywan-chungtsiang.top/gtdooydiji.html

Ruby: arr.sort
来源：http://hz.zhengqikj.top/gttzddotcd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.pycfn.com/gtkyubpomk.html

[N03] 快速排序（分治示例）
来源：http://hz.aibaodan.cn/gtfntouqqi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cdnleiting.top/gtaccjclua.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hammf.cn/gtzihxkjqp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hongshengwenyu.top/gtjkdvwjqg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.meibo888.top/gttozskkcm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.dashuyun.cn/gtvlphjodz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shanyushiyangtech.top/gtioyhbvfd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.svipenyu.cn/gtqwwlyfml.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.haohaochexian.top/gtyntpnlec.html

[N04] 斐波那契数列
来源：http://hz.dianchejie.cn/gtbwdfcwxb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cqqwz.cn/gtlchkosxh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.0kj1m.cn/gtaynjpnku.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangtech.top/gtrdynkogw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinyuanbaomall.cn/gtphgfozih.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.svipenyu.cn/gticajagzk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hysaishi.cn/gtksqqvsrx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhijiandao.cn/gtxenylsjg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.nanxinkj.top/gtaoppydra.html

[N05] 最大公约数
来源：http://hz.aibaodan.cn/gthuknkrfk.html

Py:   math.gcd(a, b)
来源：http://hz.jianghu66.top/gtaapsgmbp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shanyushiyangtech.top/gtltgkhwze.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xinyue.icu/gtzikwzufx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hfpthk.cn/gtlrghxqkf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.dianchejie.cn/gthomfumsv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhongyouzk.top/gtkvxjtxoe.html

Ruby: a.gcd(b)
来源：http://hz.svipenyu.cn/gtezarubaq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinqigufen.top/gtmsowwpvj.html

[N06] 判断回文字符串
来源：http://hz.cheryme.top/gtyovxokaw.html

Py:   s == s[::-1]
来源：http://hz.jqgufenzy.top/gtnneztbcy.html

PHP:  $s === strrev($s);
来源：http://hz.c1oappe.top/gteenfwvur.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenjidiqi.icu/gthvzdsuai.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yonumen.top/gtacprmfmz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zdqjudy.top/gttaxlqlbs.html

Go:   // 双指针从两端比较
来源：http://hz.chenjidiqi.icu/gticnopsrk.html

Ruby: s == s.reverse
来源：http://hz.cqqwz.cn/gtlybihbro.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.redwolf501.top/gtsnriipxm.html

[N07] 两数之和（返回下标）
来源：http://hz.316326.xyz/gtvftlxnlq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhaomingkeji.xyz/gteagxrkny.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.aizwys.cn/gthcboivhz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hysaishi.cn/gtsbamjplh.html

TS:   // 手写 Map<string, number>
来源：http://hz.chenlongwang.top/gtedtjvhhn.html

Java: // 手写 HashMap
来源：http://hz.smart0.xyz/gtvzadxjxx.html

Go:   // 手写 map[int]int
来源：http://hz.gzhubu.top/gtzxnlehoe.html

Ruby: // 手写 Hash
来源：http://hz.pengpengdd.cyou/gtwehuarho.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.dashuyun.cn/gtmnibqinr.html

[N08] 生成全排列
来源：http://hz.yongpay.top/gttljddeom.html

Py:   itertools.permutations(arr)
来源：http://hz.daxiang520.top/gtymqrikwl.html

PHP:  // 手写递归交换
来源：http://hz.vqdsnc.cn/gtvfcwyalp.html

JS:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtpebjokur.html

TS:   // 手写回溯递归
来源：http://hz.xziqi.cn/gtlootnypg.html

Java: // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gtvnldsazn.html

Go:   // 手写回溯递归
来源：http://hz.52xcode.cn/gtrsfrizev.html

Ruby: arr.permutation.to_a
来源：http://hz.ywan-chungtsiang.top/gtiazvhcgy.html

C#:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtzwljtiew.html

[N09] 栈与队列
来源：http://hz.xuetiantiany.cn/gtelqawado.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jianghu66.top/gtqgogsqfq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.bjfxy.top/gtwdkbuurh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yongpay.top/gtafgfkqdh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xinyue.icu/gtutrziwcm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gogol.net.cn/gtonvmqjep.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ydjk.org.cn/gtutlskeyy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhixingplan.top/gtimosnerg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yueranfly.top/gtgxfudgaj.html

[N10] 链表节点定义
来源：http://hz.hfpthk.cn/gtzyvieihd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yvedp.cn/gtxjafqjhy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.nwbrower.top/gtwrwiccxn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jqgfzy.top/gtjipjkpxc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jinqigufen.top/gtxdzjgqon.html

Java: class Node { int v; Node next; }
来源：http://hz.yongpay.top/gtykbuzhna.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yj202588.top/gttpijihvw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jqgufenzy.top/gtlpacyoyz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hongshengwenyu.top/gtcmfkbhnl.html

[N11] 二叉树中序遍历
来源：http://hz.hnxiangtu.top/gtcaikskan.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hammf.cn/gtytmlugks.html

PHP:  // 手写递归函数
来源：http://hz.chenjidiqi.icu/gtcqwcwzcm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxinkj.top/gtoxhljioa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jlsjyb.cn/gteoxpmdra.html

Java: // 手写递归
来源：http://hz.xylfe.cn/gtnjfpsqin.html

Go:   // 手写递归
来源：http://hz.xuanzx.com/gtcrpyrdyl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.guowangkeji.top/gtgowioule.html

C#:   // 手写递归
来源：http://hz.ydjk.org.cn/gttfbjuegn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.chenzaomai.com/gtbdzrkyzz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhongyouzk.top/gtoncwlami.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zdqjudy.top/gtatwpsvek.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xingfuxueyuan.xyz/gtknjildtw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.pengpengdd.cyou/gtencteoxd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yvedp.cn/gtvuzrhfbb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.cheryme.top/gtaploiudn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhiwuduotai.top/gtnhmmqgqy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydjk.org.cn/gthgpupfer.html

================================================================================
来源：http://hz.nanxinkj.top/gtaeajqtzx.html

O. 并发与异步
来源：http://hz.yongpay.top/gtiogowotn.html

================================================================================
来源：http://hz.mhx1999.top/gtmcpjqitd.html

[O01] 启动一个线程
来源：http://hz.fzhhl.top/gtrrycnmjx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yuxming.cn/gtlzudgjmk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.fengsongda.top/gtzvaowkfc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yanxiufei.cn/gtpidldkvt.html

TS:   // 同 JS
来源：http://hz.zhijiandao.cn/gtjrueohtf.html

Java: new Thread(() -> f()).start()
来源：http://hz.guowangkeji.top/gtebdgglvt.html

Go:   go f()
来源：http://hz.pycfn.com/gtnwatwgku.html

Ruby: Thread.new { f }
来源：http://hz.jinyuanbaomall.cn/gtcahxkmho.html

C#:   Task.Run(() => F());
来源：http://hz.feifeiyinyue.top/gtkjgexndf.html

[O02] 使用线程池
来源：http://hz.gaohongyu789.top/gtiritdlyk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hysaishi.cn/gttgejqjmy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhaomingkeji.xyz/gtloembjqq.html

JS:   // worker_threads 线程池
来源：http://hz.yonumen.top/gtbsjhoxbj.html

TS:   // worker_threads 线程池
来源：http://hz.ppjwa.cn/gtctnxdrqe.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shuidangran.top/gtolxusrdl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yanxiufei.cn/gthqkewhbq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.birdmap.top/gtvvtyjutb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yangfankeji.com/gtjbepktvm.html

[O03] 加锁保护共享数据
来源：http://hz.xinyue.icu/gtgenelvta.html

Py:   with lock: shared += 1
来源：http://hz.dianchejie.cn/gtqjzlegih.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.chenlongwang.top/gtsfhjihml.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shuidangran.top/gtnablsrri.html

TS:   // 同 JS
来源：http://hz.cucudq.cn/gtxbdffabc.html

Java: synchronized (this) { shared++; }
来源：http://hz.ppjwa.cn/gthveniyon.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.mhx1999.top/gtccchuxyq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.andypj.xyz/gtbzkcrmoj.html

C#:   lock (gate) { shared++; }
来源：http://hz.havefunace.top/gtlwxlgicn.html

[O04] 定义异步函数并等待
来源：http://hz.xuanzx.com/gtxdenoesg.html

Py:   async def f():⏎    await g()
来源：http://hz.hongshengwenyu.top/gtqhvhdkob.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.feifeiyinyue.top/gtpyrojpkj.html

JS:   async function f() { await g(); }
来源：http://hz.xuetiantiany.cn/gtgbtqkmuq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ywan-chungtsiang.top/gtcgioamop.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cqqwz.cn/gtjseszxek.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xylfe.cn/gtcpwjmapn.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ybcxt.top/gtneupqppt.html

C#:   async Task F() { await G(); }
来源：http://hz.jinqigufen.top/gtjsglmskj.html

[O05] 并发执行并等待全部完成
来源：http://hz.gaohongyu789.top/gtkmclvocz.html


<!-- 参考信息 -->