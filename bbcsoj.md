代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.fengsongda.top/gtkqvflhrl.html

JS:   await fetch(url)
来源：http://hz.xuanzx.com/gteweuiadb.html

TS:   await fetch(url)
来源：http://hz.xuanzx.com/gtgkxmoelw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yangfankeji.com/gtcchzfxzo.html

Go:   resp, err := http.Get(url)
来源：http://hz.chenjidiqi.icu/gtvxpfwyez.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.kuanghao11.cn/gtyiumojcy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.andypj.xyz/gtyoilgbuo.html

[L02] 发送 POST JSON
来源：http://hz.ydzc1.top/gthpezpzde.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.tianlin.xyz/gtmivamhea.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.havefunace.top/gtqqmcseyw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aibaodan.cn/gtfmkgbfud.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yvedp.cn/gthgymndbd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.dianchejie.cn/gthjqghnou.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinqigufen.top/gtkbhievwd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.wangshuangyany.cn/gtpjwytbac.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.andypj.xyz/gtyynorokv.html

[L03] 设置自定义请求头
来源：http://hz.hywenlv.cn/gtrhojdqwr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yonumen.top/gtexmodhko.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.pycfn.com/gtwfendivn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.haohaochexian.top/gtocspgfxq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dashuyun.cn/gtjlwrqedb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shuidangran.top/gtfydkvtod.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.tian-w.cn/gtodxmqwuw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.chenlongwang.top/gtgowmrsfv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gotoacloud.top/gtjdfumlaw.html

[L04] 设置超时
来源：http://hz.aibaodan.cn/gthizkebff.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jinqigufen.top/gtwckykgbx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhijiandao.cn/gtbyowicnp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sweek.top/gtaqfqnvcg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgfzy.top/gtprutuilf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.havefunace.top/gtcpmgrosu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinyuanbaomall.cn/gtyxuspcga.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.iojbl.cn/gtrdmgocdq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gotoacloud.top/gtotnpdsua.html

[L05] 上传文件（multipart）
来源：http://hz.yongpay.top/gtskiczaqs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cashguo.top/gtgewqncnc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gotoacloud.top/gtavzdetgg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.gogol.net.cn/gtdxukbpwr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangtech.top/gtbtxprdvd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yvedp.cn/gtztorikyq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hnxiangtu.top/gtkjdnudxy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.316326.xyz/gtidpukmah.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cucudq.cn/gtcvcupdct.html

[L06] 解析响应为 JSON
来源：http://hz.nanxinkj.top/gtgsksshwn.html

Py:   resp.json()
来源：http://hz.zhijiandao.cn/gtjyxkmarx.html

PHP:  json_decode($body, true);
来源：http://hz.guowangkeji.top/gtsznpupgi.html

JS:   await resp.json()
来源：http://hz.cqqwz.cn/gtptzxvubu.html

TS:   await resp.json()
来源：http://hz.shzxlz.cn/gttviwjfcg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jqgufenzy.top/gtirrbbraz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hammf.cn/gteilvmtzj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenzaomai.com/gteyiqikgu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhijiandao.cn/gtqorsdlht.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhengqikj.top/gtanaypewm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.52xcode.cn/gtioyvlrav.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sweek.top/gtrrgyutvo.html

JS:   resp.ok;  resp.status
来源：http://hz.zhongyouzk.top/gthbbvkqjr.html

TS:   resp.ok;  resp.status
来源：http://hz.gzhubu.top/gtungxmnhv.html

Java: resp.statusCode()
来源：http://hz.yj20258888.top/gtuxnnvksb.html

Go:   resp.StatusCode
来源：http://hz.haohaochexian.top/gtvuoioxnj.html

Ruby: resp.code.to_i
来源：http://hz.nanxuanxn.top/gttlgqyjhp.html

C#:   (int)resp.StatusCode
来源：http://hz.zhoulong.xyz/gttfiqpeeb.html

[L08] 并发请求多个地址
来源：http://hz.zhaomingkeji.xyz/gtemzzlqth.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shanyushiyangkeji.top/gtlejgobnb.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangdashe.top/gtbwkxcnho.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinghuilouyu.cn/gteiqeluhk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yongpay.top/gtzwvuvaca.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gzhubu.top/gtragvixfj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shangyingyoupin.top/gtkxvnjoms.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jlsjyb.cn/gtjztbcwnl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yj202588.top/gtpzlfkkzy.html

================================================================================
来源：http://hz.shzxlz.cn/gtimaaoole.html

M. 命令行 / 进程 / 环境
来源：http://hz.xziqi.cn/gtnhngqzxu.html

================================================================================
来源：http://hz.cheryme.top/gtfgpwfpse.html

[M01] 读取命令行参数
来源：http://hz.ybcxt.top/gtyuxkcomy.html

Py:   sys.argv[1:]
来源：http://hz.ydzc1.top/gtfogltwrq.html

PHP:  $argv;  $argc;
来源：http://hz.aibaodan.cn/gtqcyylflc.html

JS:   process.argv.slice(2)
来源：http://hz.yongpay.top/gtzsbogupw.html

TS:   process.argv.slice(2)
来源：http://hz.sysykeji.top/gtrpeckmad.html

Java: args 数组（main 方法参数）
来源：http://hz.cheryme.top/gtrgvreiwr.html

Go:   os.Args[1:]
来源：http://hz.zhongyouzk.top/gtsnyreizq.html

Ruby: ARGV
来源：http://hz.dashuyun.cn/gtusrmtvbe.html

C#:   args 数组（Main 方法参数）
来源：http://hz.quarkkingdee.top/gtlzgylvgo.html

[M02] 读取环境变量
来源：http://hz.pengpengdd.cyou/gtvetbremg.html

Py:   os.environ.get("HOME")
来源：http://hz.zhengqikj.top/gtblknwegf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.redwolf501.top/gthiatbtao.html

JS:   process.env.HOME
来源：http://hz.gaohongyu789.top/gtpxjgknjs.html

TS:   process.env.HOME
来源：http://hz.zhoulong.xyz/gtmwjedrxv.html

Java: System.getenv("HOME")
来源：http://hz.cashguo.top/gtftdawcmc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yj202588.top/gtrhqmjwaj.html

Ruby: ENV["HOME"]
来源：http://hz.zhixingplan.top/gtrdizuxxv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhengqikj.top/gtprydxccf.html

[M03] 执行外部命令
来源：http://hz.xziqi.cn/gtdhapnbtg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.chenlongwang.top/gtrhoadxhm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hywenlv.cn/gtobydtfze.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sweek.top/gtxmdlrsxl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.c1oappe.top/gtzaefkhjo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hammf.cn/gtyervveit.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.smart0.xyz/gtfqarybka.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinqigfzy.top/gtakoewadb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shuidangran.top/gtvpdbejaz.html

[M04] 获取当前工作目录
来源：http://hz.feifeiyinyue.top/gtnwenzbjb.html

Py:   os.getcwd()
来源：http://hz.quarkkingdee.top/gtcobvtpxn.html

PHP:  getcwd();
来源：http://hz.9152youxi.cn/gtzsvebwor.html

JS:   process.cwd()
来源：http://hz.chenjidiqi.icu/gthmlwciez.html

TS:   process.cwd()
来源：http://hz.snrcjt.cn/gtxfmohaec.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.nanxinkj.top/gtjsanituz.html

Go:   os.Getwd()
来源：http://hz.shzxlz.cn/gtmppjkklg.html

Ruby: Dir.pwd
来源：http://hz.jianghu66.top/gtnbcpdwtm.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sweek.top/gtouuktard.html

[M05] 设置退出码
来源：http://hz.c1oappe.top/gtgztmwgoc.html

Py:   sys.exit(1)
来源：http://hz.zhixingplan.top/gtkqyvvxqr.html

PHP:  exit(1);
来源：http://hz.ppjwa.cn/gtgilenqqa.html

JS:   process.exit(1)
来源：http://hz.yongpay.top/gtkltkbtht.html

TS:   process.exit(1)
来源：http://hz.cqqwz.cn/gtechlltaw.html

Java: System.exit(1)
来源：http://hz.cheryme.top/gtsoylzaxd.html

Go:   os.Exit(1)
来源：http://hz.yuxming.cn/gtiwpixopm.html

Ruby: exit 1
来源：http://hz.ywan-chungtsiang.top/gtlglnhofg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.pycfn.com/gtqvaimbtu.html

[M06] 向标准错误输出
来源：http://hz.dashuyun.cn/gtxzndtqhy.html

Py:   print("err", file=sys.stderr)
来源：http://hz.c1oappe.top/gtyulgtzvk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.redwolf501.top/gtrwwskvsf.html

JS:   console.error("err")
来源：http://hz.hysaishi.cn/gtmwrrqzzh.html

TS:   console.error("err")
来源：http://hz.shzxlz.cn/gtctdcpekf.html

Java: System.err.println("err")
来源：http://hz.hnxiangtu.top/gtovcnzmkm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.mhx1999.top/gtbiurcahc.html

Ruby: warn "err"
来源：http://hz.zhengqikj.top/gtuxcekdzd.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hysaishi.cn/gtetqrnezq.html

[M07] 判断是否为主入口
来源：http://hz.ywan-chungtsiang.top/gtqvvigxry.html

Py:   if __name__ == "__main__":
来源：http://hz.smart0.xyz/gttwjlmryj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cqqwz.cn/gtcoiiounb.html

JS:   require.main === module
来源：http://hz.aizwys.cn/gtcdxrjnmn.html

TS:   require.main === module
来源：http://hz.shanyushiyangtech.top/gtamixrclp.html

Java: public static void main(String[] args)
来源：http://hz.daxiang520.top/gtbrovfzag.html

Go:   func main()
来源：http://hz.pycfn.com/gtcyreumpg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.meibo888.top/gtzvogaswp.html

C#:   static void Main(string[] args)
来源：http://hz.xingfuxueyuan.xyz/gtaluacstq.html

[M08] 获取系统与运行时信息
来源：http://hz.zycfv.cn/gtfkwdcvfw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cashguo.top/gtrwfobwqe.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhengqikj.top/gtrvyvqmud.html

JS:   process.platform;  process.version
来源：http://hz.vqdsnc.cn/gtghibhiia.html

TS:   process.platform;  process.version
来源：http://hz.gzhubu.top/gtvgleuror.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yuxming.cn/gtpjzvkhyg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.c1oappe.top/gtbemdqcjj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cucudq.cn/gtpnzvoxid.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.bjfxy.top/gtjbeicrts.html

================================================================================
来源：http://hz.smart0.xyz/gtsqagnupl.html

N. 数据结构与算法
来源：http://hz.guannengcc.top/gtmhsconck.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtzemxwvec.html

[N01] 二分查找（有序数组）
来源：http://hz.yvedp.cn/gtaeydverg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hfpthk.cn/gtjocbplrg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ydjk.org.cn/gtqftrqwxn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ybcxt.top/gtxvertpzr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.meibo888.top/gtqjlzfovg.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jqgufenzy.top/gtampistxd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhixingplan.top/gtczbndnsv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.kuanghao11.cn/gtimpiqibb.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yuanzhike.top/gtfjdqkldz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.pengpengdd.cyou/gtrfvtinni.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sysykeji.top/gtzrrdgkus.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hysaishi.cn/gtevvdiwed.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.quarkkingdee.top/gtkgsmfido.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtmokrlbsu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.guannengcc.top/gtlqqahktk.html

Go:   slices.Sort(arr)
来源：http://hz.hongshengwenyu.top/gtvsglticu.html

Ruby: arr.sort
来源：http://hz.shanyushiyangkeji.top/gtbpzvetxa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhongyouzk.top/gtigsimzqe.html

[N03] 快速排序（分治示例）
来源：http://hz.guowangkeji.top/gtsbihapgd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.birdmap.top/gtdlxfxytn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cashguo.top/gtlkrgatin.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.haohaochexian.top/gtihaoqepl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guowangkeji.top/gtonvbluvp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yanxiufei.cn/gtdnajejlc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.sxryk.cn/gtrtueffmx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gotoacloud.top/gtlxfsvlxy.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.guowangkeji.top/gtyqdycxaz.html

[N04] 斐波那契数列
来源：http://hz.yueranfly.top/gtmqlreakw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.wangshuangyany.cn/gtbcdjiyut.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.nanxinkj.top/gtbzbedbei.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.guowangkeji.top/gtgybdlacv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.birdmap.top/gtauodihxb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hongshengwenyu.top/gtvludbhcc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.daria6918.cn/gtinolgknc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gotoacloud.top/gthsvxucfb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.bjfxy.top/gtlwdebcxq.html

[N05] 最大公约数
来源：http://hz.nwbrower.top/gtmdxlaped.html

Py:   math.gcd(a, b)
来源：http://hz.hysaishi.cn/gtogzeqvpv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.nanxuanxn.top/gtpgosqteh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cashguo.top/gtoouacdzz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shangyingyoupin.top/gtlgjaavyl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhoulong.xyz/gtzeckldnx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sxryk.cn/gtfolgbqwd.html

Ruby: a.gcd(b)
来源：http://hz.dianchejie.cn/gtixpnoprv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hysaishi.cn/gtaaxpcjfh.html

[N06] 判断回文字符串
来源：http://hz.shzxlz.cn/gtuuitwfok.html

Py:   s == s[::-1]
来源：http://hz.nwbrower.top/gtjdwzkqaw.html

PHP:  $s === strrev($s);
来源：http://hz.ywan-chungtsiang.top/gtgyikyxws.html

JS:   s === [...s].reverse().join("")
来源：http://hz.guannengcc.top/gttsuedimp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtlfjvqtqa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xziqi.cn/gtpabumezr.html

Go:   // 双指针从两端比较
来源：http://hz.nanxinkj.top/gtdszkfkcg.html

Ruby: s == s.reverse
来源：http://hz.xinyue.icu/gtpgsxvxql.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gogol.net.cn/gtuouahfqk.html

[N07] 两数之和（返回下标）
来源：http://hz.zycfv.cn/gtshncngli.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yj20258.top/gtacnnnopz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.nwbrower.top/gtjrenarzk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhijiandao.cn/gtjrxcizvv.html

TS:   // 手写 Map<string, number>
来源：http://hz.daxiang520.top/gtadvwtlve.html

Java: // 手写 HashMap
来源：http://hz.birdmap.top/gtaodppkmf.html

Go:   // 手写 map[int]int
来源：http://hz.hammf.cn/gtnvsvxfol.html

Ruby: // 手写 Hash
来源：http://hz.chenjidiqi.icu/gtrvlsgcan.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinghuilouyu.cn/gtinsmthsd.html

[N08] 生成全排列
来源：http://hz.gotoacloud.top/gtwnzuyarv.html

Py:   itertools.permutations(arr)
来源：http://hz.yvedp.cn/gtrmcstywj.html

PHP:  // 手写递归交换
来源：http://hz.yj202588.top/gtinogglna.html

JS:   // 手写回溯递归
来源：http://hz.yvedp.cn/gtluoliozs.html

TS:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtrshhdikr.html

Java: // 手写回溯递归
来源：http://hz.sysykeji.top/gtqtaxrxit.html

Go:   // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gtkrphiate.html

Ruby: arr.permutation.to_a
来源：http://hz.hnqzz.top/gtbpuukaka.html

C#:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtnnzowzdl.html

[N09] 栈与队列
来源：http://hz.yangfankeji.com/gtpfcqjpyg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.cdnleiting.top/gtzfrbiccg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.birdmap.top/gtvgxpxkaq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.tian-w.cn/gtmmojnrvv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ydjk.org.cn/gtvucgdkls.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhongyouzk.top/gtechanxmp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hfpthk.cn/gtopxckxbe.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.feifeiyinyue.top/gttqyftwkq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinqigufen.top/gtnzqaohdh.html

[N10] 链表节点定义
来源：http://hz.zhengqikj.top/gtvnpsozkv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ehwqpu.com/gtrwbjxajz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.mhx1999.top/gtsjwcctzg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.kuanghao11.cn/gtmvrubpuw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenzaomai.com/gtfsjutmvz.html

Java: class Node { int v; Node next; }
来源：http://hz.bjfxy.top/gtynxpwexl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yangfankeji.com/gtxrzxrljs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.gotoacloud.top/gtujlqfzgz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yvedp.cn/gtgqrghkfn.html

[N11] 二叉树中序遍历
来源：http://hz.zhongyouzk.top/gtofzmelms.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinqigfzy.top/gtdzaibqfy.html

PHP:  // 手写递归函数
来源：http://hz.gotoacloud.top/gthibilfyj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guannengcc.top/gtujylpjkl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jyoumei.cn/gtgoeqgntu.html

Java: // 手写递归
来源：http://hz.svipenyu.cn/gtywejyrwu.html

Go:   // 手写递归
来源：http://hz.jinyuanbaomall.cn/gtteqjlisx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yueranfly.top/gtndvzafui.html

C#:   // 手写递归
来源：http://hz.yvedp.cn/gtejycsuvs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xziqi.cn/gtkyxathhw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.nanxuanxn.top/gtaqzakrqc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhoulong.xyz/gtioxbwctz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dianchejie.cn/gtankrnbau.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.c1oappe.top/gttrdckwym.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nanxinkj.top/gtumntadhq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ybcxt.top/gtyqegtuad.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.chenlongwang.top/gtshfxoaqq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guowangkeji.top/gtjhawvwko.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtxwvcagmu.html

O. 并发与异步
来源：http://hz.hfpthk.cn/gtrbskzvkp.html

================================================================================
来源：http://hz.yangfankeji.com/gtyohjfsht.html

[O01] 启动一个线程
来源：http://hz.sxryk.cn/gtgcjomymd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cheryme.top/gtkeeebbax.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yonumen.top/gtmsyhlewj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xziqi.cn/gtzutwaiii.html

TS:   // 同 JS
来源：http://hz.daxiang520.top/gtmquuqivf.html

Java: new Thread(() -> f()).start()
来源：http://hz.sweek.top/gtwjnvkqcv.html

Go:   go f()
来源：http://hz.haohaochexian.top/gtcjdmbbwn.html

Ruby: Thread.new { f }
来源：http://hz.zycfv.cn/gtjvqrpsuv.html

C#:   Task.Run(() => F());
来源：http://hz.316326.xyz/gtcvzesfsh.html

[O02] 使用线程池
来源：http://hz.redwolf501.top/gtosfobtao.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.gaohongyu789.top/gttwxwetid.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.svipenyu.cn/gtoxmmdsbc.html

JS:   // worker_threads 线程池
来源：http://hz.zhiwuduotai.top/gthspqtmvp.html

TS:   // worker_threads 线程池
来源：http://hz.pengpengdd.cyou/gtakttcmcv.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jyoumei.cn/gtdspbhjdr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhengqikj.top/gtyiuhizof.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.wangdashe.top/gtpclhdwas.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cucudq.cn/gtjnjkkgaz.html

[O03] 加锁保护共享数据
来源：http://hz.pengpengdd.cyou/gtwxqeofgn.html

Py:   with lock: shared += 1
来源：http://hz.fzhhl.top/gtjllpcxpg.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.aizwys.cn/gtarhhnupz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.aizwys.cn/gtmgxangyx.html

TS:   // 同 JS
来源：http://hz.hammf.cn/gtgpfhhvux.html

Java: synchronized (this) { shared++; }
来源：http://hz.gogol.net.cn/gtvtessyzm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yj202588.top/gtjukcynml.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.snrcjt.cn/gtlsbqnmts.html

C#:   lock (gate) { shared++; }
来源：http://hz.52xcode.cn/gtxeokmkie.html

[O04] 定义异步函数并等待
来源：http://hz.jinqigfzy.top/gtohkkpdzi.html

Py:   async def f():⏎    await g()
来源：http://hz.hnxiangtu.top/gtswrzjjrk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ydzc1.top/gtzrhsasxe.html

JS:   async function f() { await g(); }
来源：http://hz.svipenyu.cn/gttfprigbu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yuxming.cn/gtiipzwbuz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.dashuyun.cn/gtaeseovob.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.nanxuanxn.top/gtduwystuz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.vqdsnc.cn/gtlghtcppu.html

C#:   async Task F() { await G(); }
来源：http://hz.sxryk.cn/gtwvqmxwks.html

[O05] 并发执行并等待全部完成
来源：http://hz.hfpthk.cn/gtqdnulxvl.html

Py:   asyncio.gather(*tasks)
来源：http://hz.fengsongda.top/gtzhegmaih.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.meibo888.top/gtzgzlmyar.html

JS:   await Promise.all(tasks)
来源：http://hz.zhiwuduotai.top/gthjldmfno.html

TS:   await Promise.all(tasks)
来源：http://hz.vqdsnc.cn/gtnendsiyz.html


<!-- 参考信息 -->