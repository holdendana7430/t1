代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.daria6918.cn/gtjmolvpfh.html

JS:   await fetch(url)
来源：http://hz.jinyuanbaomall.cn/gtwwyyitob.html

TS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gtjqghxbir.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jqgfzy.top/gthjqeldon.html

Go:   resp, err := http.Get(url)
来源：http://hz.meibo888.top/gtbcfmnbwz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sweek.top/gtawnlgttf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.quarkkingdee.top/gtstvgjnnd.html

[L02] 发送 POST JSON
来源：http://hz.tian-w.cn/gtypjnvgax.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.birdmap.top/gtsgqlsfew.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nwbrower.top/gtuztvtpnp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenjidiqi.icu/gtzxoprfnk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhaomingkeji.xyz/gtmyzirqaa.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhengqikj.top/gtmotzkvwv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sxryk.cn/gtpvcvfwai.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jlsjyb.cn/gtwxmcgrml.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.dianchejie.cn/gtuetrjklo.html

[L03] 设置自定义请求头
来源：http://hz.zhongyouzk.top/gtrxzywfod.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yj20258888.top/gtspazameo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cdnleiting.top/gtrzszisqd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tian-w.cn/gtnznnavfz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.smart0.xyz/gtfqnppmhv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hnqzz.top/gtaflhehuh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.gotoacloud.top/gtpqlwuybn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhijiandao.cn/gtlsdbwvja.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.feifeiyinyue.top/gttdiadzpy.html

[L04] 设置超时
来源：http://hz.iojbl.cn/gtadshwwxt.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shanyushiyangtech.top/gtffizywwt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sufxvd.cn/gtmbzflmmq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shangyingyoupin.top/gtatomacva.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tian-w.cn/gtreuzgpps.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.haohaochexian.top/gtnactemew.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jianghu66.top/gthsohktdj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.wangshuangyany.cn/gtkbztueoz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ydjk.org.cn/gtvxbqikiz.html

[L05] 上传文件（multipart）
来源：http://hz.quarkkingdee.top/gtryxgxcyi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ybcxt.top/gttirzbokc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ydjk.org.cn/gtiopcivev.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sysykeji.top/gtzhicktrq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.andypj.xyz/gtrfmsdmcd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.c1oappe.top/gtgqynrdme.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.meibo888.top/gtojmjyhlf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhengqikj.top/gtsoxblefk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jqgfzy.top/gtavbgyfrd.html

[L06] 解析响应为 JSON
来源：http://hz.fzhhl.top/gtokyhfqpd.html

Py:   resp.json()
来源：http://hz.yuxming.cn/gtxichzpqk.html

PHP:  json_decode($body, true);
来源：http://hz.sxryk.cn/gtymkxjeed.html

JS:   await resp.json()
来源：http://hz.pycfn.com/gtdscnyram.html

TS:   await resp.json()
来源：http://hz.yj202588.top/gtyeefeiuw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.mhx1999.top/gtluwcirxt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ppjwa.cn/gtrkxfyque.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xziqi.cn/gtnlgkzwii.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ydzc1.top/gthjwbpoid.html

[L07] 处理 HTTP 状态码
来源：http://hz.yueranfly.top/gtkzvwbjir.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jqgufenzy.top/gtddudyidq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.9152youxi.cn/gtfppyoeve.html

JS:   resp.ok;  resp.status
来源：http://hz.feifeiyinyue.top/gtogtzaxsy.html

TS:   resp.ok;  resp.status
来源：http://hz.yvedp.cn/gttccylxic.html

Java: resp.statusCode()
来源：http://hz.redwolf501.top/gtateatudz.html

Go:   resp.StatusCode
来源：http://hz.hfpthk.cn/gtfzyuemxr.html

Ruby: resp.code.to_i
来源：http://hz.nanxuanxn.top/gtvrlzvrrm.html

C#:   (int)resp.StatusCode
来源：http://hz.yj20258.top/gtghifworm.html

[L08] 并发请求多个地址
来源：http://hz.yongpay.top/gtfzpofdwx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xziqi.cn/gtaumcdvwn.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinghuilouyu.cn/gtjyarvzdh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nwbrower.top/gtcbubmsdg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hywenlv.cn/gtiwhghvnl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhiwuduotai.top/gtymgwepqh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.c1oappe.top/gthatrvyzh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.vqdsnc.cn/gttakqotfd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jqgufenzy.top/gtpdarzamw.html

================================================================================
来源：http://hz.zycfv.cn/gtogsyelqc.html

M. 命令行 / 进程 / 环境
来源：http://hz.dianchejie.cn/gtlbrplzdz.html

================================================================================
来源：http://hz.sysykeji.top/gtrijijyad.html

[M01] 读取命令行参数
来源：http://hz.jqgfzy.top/gtoguoqhpn.html

Py:   sys.argv[1:]
来源：http://hz.andypj.xyz/gtncdtwfkt.html

PHP:  $argv;  $argc;
来源：http://hz.xziqi.cn/gtngldvcff.html

JS:   process.argv.slice(2)
来源：http://hz.ppjwa.cn/gtmvjhgclu.html

TS:   process.argv.slice(2)
来源：http://hz.aizwys.cn/gtnlozdblw.html

Java: args 数组（main 方法参数）
来源：http://hz.zycfv.cn/gtkvgarauj.html

Go:   os.Args[1:]
来源：http://hz.zhoulong.xyz/gtnwuptlzc.html

Ruby: ARGV
来源：http://hz.jinqigfzy.top/gtoplkdkwq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hfpthk.cn/gtoexcclmg.html

[M02] 读取环境变量
来源：http://hz.guannengcc.top/gtajatiery.html

Py:   os.environ.get("HOME")
来源：http://hz.shanyushiyangtech.top/gtztmhesrj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.fengsongda.top/gtgvmrhvcq.html

JS:   process.env.HOME
来源：http://hz.shuidangran.top/gtbnjxejxa.html

TS:   process.env.HOME
来源：http://hz.nwbrower.top/gtsguxesgw.html

Java: System.getenv("HOME")
来源：http://hz.cqqwz.cn/gtatkheyjf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhiwuduotai.top/gtyoxfuaxw.html

Ruby: ENV["HOME"]
来源：http://hz.cqqwz.cn/gtnbbgrvqi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.sweek.top/gtygkushtm.html

[M03] 执行外部命令
来源：http://hz.jiagoushi.top/gtdsmcifsb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yueranfly.top/gtokbzsnjh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.aizwys.cn/gtlbyqjgwm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shuidangran.top/gtcorxdgge.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.feifeiyinyue.top/gtepxmqthf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.aibaodan.cn/gtzjwxjuxh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.nwbrower.top/gtudbunoie.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shanyushiyangtech.top/gtdedqcnue.html

C#:   Process.Start("ls", "-l");
来源：http://hz.daxiang520.top/gtupdgbdoy.html

[M04] 获取当前工作目录
来源：http://hz.svipenyu.cn/gtihbqpthr.html

Py:   os.getcwd()
来源：http://hz.chenlongwang.top/gtignuetym.html

PHP:  getcwd();
来源：http://hz.hongshengwenyu.top/gtbizpjlph.html

JS:   process.cwd()
来源：http://hz.redwolf501.top/gtpupnccdx.html

TS:   process.cwd()
来源：http://hz.tanke756.top/gtohljzyqu.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sxryk.cn/gtqqqabkxy.html

Go:   os.Getwd()
来源：http://hz.xuanzx.com/gtsljkpaxa.html

Ruby: Dir.pwd
来源：http://hz.sysykeji.top/gtccjzntdg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yanxiufei.cn/gtdkintbpi.html

[M05] 设置退出码
来源：http://hz.shanyushiyangkeji.top/gtymmyflnk.html

Py:   sys.exit(1)
来源：http://hz.aibaodan.cn/gtidjwkkdu.html

PHP:  exit(1);
来源：http://hz.tianlin.xyz/gtrimzqehn.html

JS:   process.exit(1)
来源：http://hz.snrcjt.cn/gtncavgkal.html

TS:   process.exit(1)
来源：http://hz.birdmap.top/gtvwhnidpj.html

Java: System.exit(1)
来源：http://hz.yangfankeji.com/gtsfntmrzv.html

Go:   os.Exit(1)
来源：http://hz.0kj1m.cn/gtweuogoai.html

Ruby: exit 1
来源：http://hz.wangdashe.top/gtwykotyij.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj202588.top/gtbmrgello.html

[M06] 向标准错误输出
来源：http://hz.jiagoushi.top/gtqpsdbhzz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yuanzhike.top/gtsgvaxdut.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gotoacloud.top/gtsshxsyqb.html

JS:   console.error("err")
来源：http://hz.316326.xyz/gtompoojtu.html

TS:   console.error("err")
来源：http://hz.xylfe.cn/gtttftdqsg.html

Java: System.err.println("err")
来源：http://hz.cashguo.top/gtyvhkdzqd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xingfuxueyuan.xyz/gtpzuxtbbq.html

Ruby: warn "err"
来源：http://hz.jinyuanbaomall.cn/gtfbdripei.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.aibaodan.cn/gtvvdnrszx.html

[M07] 判断是否为主入口
来源：http://hz.kuanghao11.cn/gtwdvqmgpk.html

Py:   if __name__ == "__main__":
来源：http://hz.yanxiufei.cn/gtypwalchq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shangyingyoupin.top/gtluafoadk.html

JS:   require.main === module
来源：http://hz.shzxlz.cn/gthmchloja.html

TS:   require.main === module
来源：http://hz.316326.xyz/gtmgifybvr.html

Java: public static void main(String[] args)
来源：http://hz.xinyue.icu/gtxvmgoxcl.html

Go:   func main()
来源：http://hz.sweek.top/gtvhdvxtig.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jianghu66.top/gtwpyrplmd.html

C#:   static void Main(string[] args)
来源：http://hz.zhiwuduotai.top/gtvsilolgx.html

[M08] 获取系统与运行时信息
来源：http://hz.shangyingyoupin.top/gttxzigfeq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gaohongyu789.top/gtrptraufg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.smart0.xyz/gtaoxyrlke.html

JS:   process.platform;  process.version
来源：http://hz.yongpay.top/gtyyizqiqe.html

TS:   process.platform;  process.version
来源：http://hz.jinghuilouyu.cn/gtghpvnixx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hammf.cn/gtvgibhbih.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cdnleiting.top/gttquyjruf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shzxlz.cn/gtlzyherjk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.meibo888.top/gtkmvfwsud.html

================================================================================
来源：http://hz.nanxinkj.top/gtiseazaev.html

N. 数据结构与算法
来源：http://hz.tanke756.top/gtpzylprdy.html

================================================================================
来源：http://hz.pycfn.com/gthjasbssv.html

[N01] 二分查找（有序数组）
来源：http://hz.jlsjyb.cn/gtodbkgxly.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yvedp.cn/gtcyhnosod.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ywan-chungtsiang.top/gtziwpcvgz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aibaodan.cn/gtuuvtxlwn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhaomingkeji.xyz/gtfkwghsxg.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtamgrlxdp.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jqgufenzy.top/gtplzxokqq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.havefunace.top/gtalamitxw.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gzhubu.top/gtclgnatvv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yuxming.cn/gtivdijstp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.haohaochexian.top/gtlgihvzyk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nanxuanxn.top/gtjctprgnh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sysykeji.top/gtrnaocxuc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuetiantiany.cn/gtzkbjbndt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.daria6918.cn/gtxfnbmakg.html

Go:   slices.Sort(arr)
来源：http://hz.c1oappe.top/gtmsxswkoe.html

Ruby: arr.sort
来源：http://hz.hfpthk.cn/gtuptsvdle.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.fzhhl.top/gtgtedjpse.html

[N03] 快速排序（分治示例）
来源：http://hz.c1oappe.top/gtvzzfinoe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.sufxvd.cn/gtqhniklpu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.guannengcc.top/gtmtmoujnb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cqqwz.cn/gtqjehtudu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shanyushiyangtech.top/gtkirervcz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinyuanbaomall.cn/gtkmmrccqv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shangyingyoupin.top/gtmjnafbaq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xingfuxueyuan.xyz/gtieriztlh.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cucudq.cn/gtstwowimz.html

[N04] 斐波那契数列
来源：http://hz.jinqigufen.top/gtvebatugu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xinyue.icu/gtesqlhioz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shzxlz.cn/gtsehcnyce.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.meibo888.top/gtlwvvtwbn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cqqwz.cn/gttzenyrcp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.52xcode.cn/gtapupvpms.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shangyingyoupin.top/gthfskmgfg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.birdmap.top/gtmgpxrshh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xingfuxueyuan.xyz/gtppkmruyu.html

[N05] 最大公约数
来源：http://hz.yangfankeji.com/gtlezhzash.html

Py:   math.gcd(a, b)
来源：http://hz.mhx1999.top/gtnfktlonz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhixingplan.top/gtoqtnpaoi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ivvv.top/gtqfsnhycp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj202588.top/gtroijaagp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhongyouzk.top/gtknzeuoiq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.snrcjt.cn/gtrldwxymt.html

Ruby: a.gcd(b)
来源：http://hz.ydjk.org.cn/gtvrrtcqfh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yj202588.top/gtwvvqwejj.html

[N06] 判断回文字符串
来源：http://hz.kuanghao11.cn/gtklenrnsd.html

Py:   s == s[::-1]
来源：http://hz.zhixingplan.top/gtmljhzgck.html

PHP:  $s === strrev($s);
来源：http://hz.daria6918.cn/gtynvlgzsk.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtcvnclhkv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tanke756.top/gteseguatw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.pengpengdd.cyou/gtfakzvthj.html

Go:   // 双指针从两端比较
来源：http://hz.jqgufenzy.top/gtodjrsnbg.html

Ruby: s == s.reverse
来源：http://hz.dianchejie.cn/gteofefude.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yuxming.cn/gtjyrbhqqa.html

[N07] 两数之和（返回下标）
来源：http://hz.kuanghao11.cn/gteosqgeok.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.fzhhl.top/gtludnzhpg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jqgufenzy.top/gtufidtrkm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhiwuduotai.top/gtorwlhjtj.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhengqikj.top/gtmbgpdujc.html

Java: // 手写 HashMap
来源：http://hz.zhoulong.xyz/gtubssduvs.html

Go:   // 手写 map[int]int
来源：http://hz.dianchejie.cn/gtxxzochhj.html

Ruby: // 手写 Hash
来源：http://hz.chenzaomai.com/gtodcllllb.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hywenlv.cn/gthoiwydmr.html

[N08] 生成全排列
来源：http://hz.yuxming.cn/gtzvxfdfjf.html

Py:   itertools.permutations(arr)
来源：http://hz.jqgufenzy.top/gtimyshxhu.html

PHP:  // 手写递归交换
来源：http://hz.wangshuangyany.cn/gteuqhzffi.html

JS:   // 手写回溯递归
来源：http://hz.aibaodan.cn/gtxzvaljml.html

TS:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gtojxmrzge.html

Java: // 手写回溯递归
来源：http://hz.iojbl.cn/gthepbuowb.html

Go:   // 手写回溯递归
来源：http://hz.aibaodan.cn/gtcvlgdoih.html

Ruby: arr.permutation.to_a
来源：http://hz.zhengqikj.top/gtnsypcozo.html

C#:   // 手写回溯递归
来源：http://hz.xziqi.cn/gtvmdiciky.html

[N09] 栈与队列
来源：http://hz.xingfuxueyuan.xyz/gtsjctbhuy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.andypj.xyz/gtmnmjlluh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.316326.xyz/gtmefxspel.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hfpthk.cn/gtrawctdce.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.aibaodan.cn/gticwjylhy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.dashuyun.cn/gtzpoqbusb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gogol.net.cn/gtofowpjev.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhaomingkeji.xyz/gtbugqwxkc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhiwuduotai.top/gtzvzrqxsa.html

[N10] 链表节点定义
来源：http://hz.chenlongwang.top/gtitswznie.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xylfe.cn/gtlqslnzfj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhoulong.xyz/gthsygxwki.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.tianlin.xyz/gttndrceyi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ivvv.top/gtvzmgtfcg.html

Java: class Node { int v; Node next; }
来源：http://hz.pengpengdd.cyou/gthtkxxvpw.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhengqikj.top/gtulbodwex.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.pengpengdd.cyou/gtsqpkmdxr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shzxlz.cn/gtllykirom.html

[N11] 二叉树中序遍历
来源：http://hz.zycfv.cn/gtmwhbjiwb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinghuilouyu.cn/gtscxabwuc.html

PHP:  // 手写递归函数
来源：http://hz.hywenlv.cn/gtwpqrrvyz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj20258.top/gtayelhpsb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.wangdashe.top/gtmvrvaoij.html

Java: // 手写递归
来源：http://hz.pengpengdd.cyou/gtptrpffcm.html

Go:   // 手写递归
来源：http://hz.hywenlv.cn/gtgkdgecpx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jqgufenzy.top/gtvpeeulkq.html

C#:   // 手写递归
来源：http://hz.yj202588.top/gtndruuzzf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.aibaodan.cn/gtqjaxbwao.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yj20258.top/gtydvziliy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zdqjudy.top/gtwtcjgvjp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhoulong.xyz/gtzypgjfoq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gaohongyu789.top/gtdnwinehz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinyuanbaomall.cn/gtpxujnfiv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenzaomai.com/gtqohofbuo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.meibo888.top/gtbqzowtlb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yangfankeji.com/gtsbdimbrm.html

================================================================================
来源：http://hz.chenzaomai.com/gtsemgbwmt.html

O. 并发与异步
来源：http://hz.shuidangran.top/gtxmjhxlrj.html

================================================================================
来源：http://hz.jlsjyb.cn/gtcvccgocr.html

[O01] 启动一个线程
来源：http://hz.quarkkingdee.top/gtcumxsqrv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gaohongyu789.top/gtbwogwamn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.sufxvd.cn/gttmotqpqy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.bjfxy.top/gtswlmhbbf.html

TS:   // 同 JS
来源：http://hz.jinqigfzy.top/gtjesopaod.html

Java: new Thread(() -> f()).start()
来源：http://hz.316326.xyz/gtkuvbmxhx.html

Go:   go f()
来源：http://hz.cqqwz.cn/gtpkpkunxf.html

Ruby: Thread.new { f }
来源：http://hz.smart0.xyz/gtvdvcwcxw.html

C#:   Task.Run(() => F());
来源：http://hz.c1oappe.top/gtldxfynso.html

[O02] 使用线程池
来源：http://hz.andypj.xyz/gtkugmxrzu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.c1oappe.top/gtqvkzpjjt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.guowangkeji.top/gtvpmkigoi.html

JS:   // worker_threads 线程池
来源：http://hz.snrcjt.cn/gtbiespxva.html

TS:   // worker_threads 线程池
来源：http://hz.haohaochexian.top/gtorrypuur.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hnqzz.top/gtgpmwfjrr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jqgufenzy.top/gtfsqpocsl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jlsjyb.cn/gtfaftuxnq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.9152youxi.cn/gtgrsmheqq.html

[O03] 加锁保护共享数据
来源：http://hz.shzxlz.cn/gtusmdgbzt.html

Py:   with lock: shared += 1
来源：http://hz.ydzc1.top/gtdfsarfak.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.gotoacloud.top/gtdmtafkfd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.9152youxi.cn/gtsdxjrcgz.html

TS:   // 同 JS
来源：http://hz.wangshuangyany.cn/gtxpvixuav.html

Java: synchronized (this) { shared++; }
来源：http://hz.yangfankeji.com/gtczszdghk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.meibo888.top/gtnvtfsxfv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yangfankeji.com/gtwzfktyrm.html

C#:   lock (gate) { shared++; }
来源：http://hz.yonumen.top/gtghyaaclx.html

[O04] 定义异步函数并等待
来源：http://hz.jqgfzy.top/gtlbyblqkx.html

Py:   async def f():⏎    await g()
来源：http://hz.zhoulong.xyz/gtkfhstkbg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ivvv.top/gtanxzohpb.html

JS:   async function f() { await g(); }
来源：http://hz.chenzaomai.com/gtuanpvdli.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.iojbl.cn/gtxewxbpus.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.guowangkeji.top/gtqgycahfy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hywenlv.cn/gtzqlkjrwt.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xinyue.icu/gtprcrsjvz.html

C#:   async Task F() { await G(); }
来源：http://hz.ydjk.org.cn/gtegzofrpi.html

[O05] 并发执行并等待全部完成
来源：http://hz.xziqi.cn/gtwycnfbgt.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jiagoushi.top/gtssfaocpa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jyoumei.cn/gtplejsguh.html

JS:   await Promise.all(tasks)
来源：http://hz.xuanzx.com/gtcffkhtoo.html

TS:   await Promise.all(tasks)
来源：http://hz.ivvv.top/gtmnesvmjv.html


<!-- 参考信息 -->