代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://hz.tianlin.xyz/gtfdgtwmvz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.aibaodan.cn/gtjavcxlts.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ehwqpu.com/gtahnlloqf.html

[L02] 发送 POST JSON
来源：http://hz.xziqi.cn/gtfvjkyeea.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ybcxt.top/gtelbegkir.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jiagoushi.top/gtwoepduqd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yueranfly.top/gtxhfavekf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.daria6918.cn/gtcvmzfqwi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.pengpengdd.cyou/gtqakotvux.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinqigufen.top/gtdacaunjn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.guowangkeji.top/gtwckswpze.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.gzhubu.top/gtdijpyojt.html

[L03] 设置自定义请求头
来源：http://hz.svipenyu.cn/gtmplqkett.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yj202588.top/gtboppcuqz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yuanzhike.top/gtsyqgeius.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yueranfly.top/gthskqhrbf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xylfe.cn/gtwgqkadhk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhiwuduotai.top/gtnzmgyqhb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xingfuxueyuan.xyz/gtvtwnntjl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.guowangkeji.top/gtirzxwolf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.quarkkingdee.top/gtqsxmupzj.html

[L04] 设置超时
来源：http://hz.tianlin.xyz/gtalopetoe.html

Py:   requests.get(url, timeout=5)
来源：http://hz.haohaochexian.top/gtvitidcbq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hysaishi.cn/gtesfaodkv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yongpay.top/gtkiailpxc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gotoacloud.top/gtvwnhdkmw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.guowangkeji.top/gtxdmszsni.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhijiandao.cn/gtcliualab.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.chenlongwang.top/gtfhebhztu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.kuanghao11.cn/gtvygvwneb.html

[L05] 上传文件（multipart）
来源：http://hz.wangdashe.top/gtnilmeklo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jqgufenzy.top/gtvisxnxdp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yanxiufei.cn/gtvyuezsch.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.c1oappe.top/gtadqbubfc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.feifeiyinyue.top/gtcubglqzy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sysykeji.top/gtakmkcufn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.gotoacloud.top/gtnjflgeua.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ydjk.org.cn/gtfwazxbxv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.9152youxi.cn/gtobgsptll.html

[L06] 解析响应为 JSON
来源：http://hz.dashuyun.cn/gtqfmhkfwd.html

Py:   resp.json()
来源：http://hz.zhiwuduotai.top/gtystsuzqj.html

PHP:  json_decode($body, true);
来源：http://hz.yj20258888.top/gtayacplid.html

JS:   await resp.json()
来源：http://hz.chenjidiqi.icu/gtqocmmone.html

TS:   await resp.json()
来源：http://hz.shzxlz.cn/gtqusxrnnu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.316326.xyz/gtuwbvajef.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yueranfly.top/gtfjfscvtu.html

Ruby: JSON.parse(resp.body)
来源：http://hz.guowangkeji.top/gtgihimuga.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yonumen.top/gtzvjcqiqa.html

[L07] 处理 HTTP 状态码
来源：http://hz.cheryme.top/gtjzltercg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yueranfly.top/gtqorczxwe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.vqdsnc.cn/gtawcpcbub.html

JS:   resp.ok;  resp.status
来源：http://hz.gotoacloud.top/gtrpoxgvnq.html

TS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gtqkkjqjfp.html

Java: resp.statusCode()
来源：http://hz.hnqzz.top/gttrjocavv.html

Go:   resp.StatusCode
来源：http://hz.mhx1999.top/gtnwxeiqbn.html

Ruby: resp.code.to_i
来源：http://hz.gzhubu.top/gtgbynjaxq.html

C#:   (int)resp.StatusCode
来源：http://hz.jyoumei.cn/gtlphwbemd.html

[L08] 并发请求多个地址
来源：http://hz.hongshengwenyu.top/gtfoqpanmv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yuanzhike.top/gtfmlaqswk.html

PHP:  curl_multi_init() 系列
来源：http://hz.nanxinkj.top/gtkorgikim.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xylfe.cn/gtouppxnva.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhijiandao.cn/gtkzzelkvf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xuetiantiany.cn/gtrsxqrxmb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xingfuxueyuan.xyz/gtpjskukyt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.tian-w.cn/gtcegbxcep.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gaohongyu789.top/gtknvioeoh.html

================================================================================
来源：http://hz.yuxming.cn/gtdrbuilxz.html

M. 命令行 / 进程 / 环境
来源：http://hz.yvedp.cn/gtuthxzztk.html

================================================================================
来源：http://hz.guannengcc.top/gtqvjgqlgo.html

[M01] 读取命令行参数
来源：http://hz.xinyue.icu/gtcnqrmimh.html

Py:   sys.argv[1:]
来源：http://hz.kuanghao11.cn/gtrqpmcxra.html

PHP:  $argv;  $argc;
来源：http://hz.ywan-chungtsiang.top/gtijstlddu.html

JS:   process.argv.slice(2)
来源：http://hz.feifeiyinyue.top/gtzsdsfkyf.html

TS:   process.argv.slice(2)
来源：http://hz.daria6918.cn/gtipnvvzul.html

Java: args 数组（main 方法参数）
来源：http://hz.sufxvd.cn/gtlacsvrfi.html

Go:   os.Args[1:]
来源：http://hz.jqgufenzy.top/gtwlpyeswj.html

Ruby: ARGV
来源：http://hz.yueranfly.top/gtazxwrqmq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.0kj1m.cn/gtifgagfnc.html

[M02] 读取环境变量
来源：http://hz.hfpthk.cn/gtvhdeujsv.html

Py:   os.environ.get("HOME")
来源：http://hz.dianchejie.cn/gttvfjlyhz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xuetiantiany.cn/gtqcpdxlso.html

JS:   process.env.HOME
来源：http://hz.jlsjyb.cn/gtepztgohg.html

TS:   process.env.HOME
来源：http://hz.daria6918.cn/gtwtismlis.html

Java: System.getenv("HOME")
来源：http://hz.hammf.cn/gtvcabdiff.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xuanzx.com/gtsvzqlpax.html

Ruby: ENV["HOME"]
来源：http://hz.ehwqpu.com/gthsypezor.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.nanxinkj.top/gtvxibtpks.html

[M03] 执行外部命令
来源：http://hz.aizwys.cn/gtmezifdfd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ydjk.org.cn/gtcedsxeri.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhaomingkeji.xyz/gtfpfsaccj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangdashe.top/gtwnemmedo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhengqikj.top/gtimxuyghg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.chenjidiqi.icu/gthhcxiwes.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shangyingyoupin.top/gtkevwewfi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zycfv.cn/gtmefrmeeo.html

C#:   Process.Start("ls", "-l");
来源：http://hz.daria6918.cn/gtcncezxmz.html

[M04] 获取当前工作目录
来源：http://hz.cucudq.cn/gtmhogkojn.html

Py:   os.getcwd()
来源：http://hz.yanxiufei.cn/gtdgdltakc.html

PHP:  getcwd();
来源：http://hz.sysykeji.top/gtjvaqfmwj.html

JS:   process.cwd()
来源：http://hz.gogol.net.cn/gtagbazuoz.html

TS:   process.cwd()
来源：http://hz.bjfxy.top/gtkxvwuqlg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.nanxuanxn.top/gtynwlrugq.html

Go:   os.Getwd()
来源：http://hz.c1oappe.top/gtjcultqgi.html

Ruby: Dir.pwd
来源：http://hz.xinyue.icu/gtlzulqnrh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.9152youxi.cn/gtytqkkqbq.html

[M05] 设置退出码
来源：http://hz.jlsjyb.cn/gtwqbtyasx.html

Py:   sys.exit(1)
来源：http://hz.gotoacloud.top/gtgrwbpfqr.html

PHP:  exit(1);
来源：http://hz.meibo888.top/gtdvnojnhm.html

JS:   process.exit(1)
来源：http://hz.shzxlz.cn/gtrmrnhndt.html

TS:   process.exit(1)
来源：http://hz.yvedp.cn/gtugvzeuby.html

Java: System.exit(1)
来源：http://hz.zhiwuduotai.top/gtpaeowibz.html

Go:   os.Exit(1)
来源：http://hz.redwolf501.top/gtvfjbjlvy.html

Ruby: exit 1
来源：http://hz.aibaodan.cn/gtpfarrsym.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ppjwa.cn/gtxlbqdawl.html

[M06] 向标准错误输出
来源：http://hz.yonumen.top/gthnfxbmgb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yuanzhike.top/gtwpoubmyb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jlsjyb.cn/gtcnkviupw.html

JS:   console.error("err")
来源：http://hz.gzhubu.top/gtxizbozuj.html

TS:   console.error("err")
来源：http://hz.zhijiandao.cn/gtacvwdcgf.html

Java: System.err.println("err")
来源：http://hz.daxiang520.top/gtelqjqpqe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.snrcjt.cn/gttsnxfbvl.html

Ruby: warn "err"
来源：http://hz.dashuyun.cn/gtcjglhxoe.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ppjwa.cn/gtirdsxmmm.html

[M07] 判断是否为主入口
来源：http://hz.cucudq.cn/gtmhenynde.html

Py:   if __name__ == "__main__":
来源：http://hz.jianghu66.top/gtknhwovyr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zdqjudy.top/gtgicatbmh.html

JS:   require.main === module
来源：http://hz.jianghu66.top/gttojgfhjn.html

TS:   require.main === module
来源：http://hz.svipenyu.cn/gtvyciqgec.html

Java: public static void main(String[] args)
来源：http://hz.birdmap.top/gtblxscpzt.html

Go:   func main()
来源：http://hz.vqdsnc.cn/gthxbpbvmt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jqgufenzy.top/gtdcajtjmw.html

C#:   static void Main(string[] args)
来源：http://hz.xuetiantiany.cn/gtcjrwqchx.html

[M08] 获取系统与运行时信息
来源：http://hz.hammf.cn/gtcaevaptd.html

Py:   platform.system();  platform.python_version()
来源：http://hz.quarkkingdee.top/gtywbyocfi.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.fengsongda.top/gtfqktvwgf.html

JS:   process.platform;  process.version
来源：http://hz.snrcjt.cn/gtbduyuvdm.html

TS:   process.platform;  process.version
来源：http://hz.yj20258888.top/gtgtlxfsga.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shanyushiyangtech.top/gtkdsriaku.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yanxiufei.cn/gtmcpzuekz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.smart0.xyz/gtoarxcxti.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.haohaochexian.top/gtybfqeibo.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtuqgkjadj.html

N. 数据结构与算法
来源：http://hz.dianchejie.cn/gtxtyimrhg.html

================================================================================
来源：http://hz.haohaochexian.top/gtkfxvupep.html

[N01] 二分查找（有序数组）
来源：http://hz.shangyingyoupin.top/gtvwmcvhne.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sufxvd.cn/gtijbubzuq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yanxiufei.cn/gtbnobrbyq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.birdmap.top/gtoikpdfpp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fengsongda.top/gtovmlqyqz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jianghu66.top/gtltaiaqsk.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ydjk.org.cn/gtlmfvrhtf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zdqjudy.top/gtuusqnumz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.kuanghao11.cn/gtlrscvnpz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yueranfly.top/gtilzfjaoy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.redwolf501.top/gtdngtexhd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.svipenyu.cn/gtsrridhjy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxinkj.top/gtpkkicdjq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.meibo888.top/gtordazqux.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.mhx1999.top/gtsjxwtusg.html

Go:   slices.Sort(arr)
来源：http://hz.cucudq.cn/gtmymscwrz.html

Ruby: arr.sort
来源：http://hz.feifeiyinyue.top/gtcooaidpy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zycfv.cn/gtpqlwwsur.html

[N03] 快速排序（分治示例）
来源：http://hz.hongshengwenyu.top/gtpezyqkhi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.pycfn.com/gtqizjzaot.html

PHP:  // 递归实现，或用 usort
来源：http://hz.fengsongda.top/gtbezzaozf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shanyushiyangtech.top/gtfweaidjr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ehwqpu.com/gtpevbjarz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ppjwa.cn/gtwqpzfshk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.mhx1999.top/gtxqjyalps.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhengqikj.top/gtcgieskvi.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jiagoushi.top/gtgzyjkjvn.html

[N04] 斐波那契数列
来源：http://hz.smart0.xyz/gtkqshyqfm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cucudq.cn/gtoluifpnt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ppjwa.cn/gthzvnjgzw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ywan-chungtsiang.top/gtwuxmysvo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tanke756.top/gtrhdnsgxn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sxryk.cn/gtgywmuwat.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.aibaodan.cn/gtiatcknat.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.andypj.xyz/gtfrizkgki.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yueranfly.top/gtarzdzuoo.html

[N05] 最大公约数
来源：http://hz.yuanzhike.top/gtidebbffd.html

Py:   math.gcd(a, b)
来源：http://hz.jinghuilouyu.cn/gtomfuuvjl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.feifeiyinyue.top/gthtzhuajy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aizwys.cn/gtkqklhtnl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jyoumei.cn/gtphyznjew.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ivvv.top/gtgmpkdbra.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.316326.xyz/gtiqjgiabi.html

Ruby: a.gcd(b)
来源：http://hz.wangdashe.top/gtmgubxxnx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.dashuyun.cn/gtkiqnbnqp.html

[N06] 判断回文字符串
来源：http://hz.xuetiantiany.cn/gtgciqqugz.html

Py:   s == s[::-1]
来源：http://hz.mhx1999.top/gtyeebkovp.html

PHP:  $s === strrev($s);
来源：http://hz.dianchejie.cn/gtemwztsnl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtrkivdwwv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtoahcoytn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.0kj1m.cn/gtwqfuainc.html

Go:   // 双指针从两端比较
来源：http://hz.zycfv.cn/gtgxigkoza.html

Ruby: s == s.reverse
来源：http://hz.hammf.cn/gtxonhirxj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhoulong.xyz/gtdayyycbr.html

[N07] 两数之和（返回下标）
来源：http://hz.nanxinkj.top/gtoulvdcos.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.meibo888.top/gtmhusaomr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xuanzx.com/gtyztvhbfa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ywan-chungtsiang.top/gtjubqcvxg.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhoulong.xyz/gtxnkbejdq.html

Java: // 手写 HashMap
来源：http://hz.jinqigufen.top/gtlvxjkwgw.html

Go:   // 手写 map[int]int
来源：http://hz.cdnleiting.top/gtnkucawew.html

Ruby: // 手写 Hash
来源：http://hz.dashuyun.cn/gtzxuctdew.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.nwbrower.top/gtuyeikzfp.html

[N08] 生成全排列
来源：http://hz.zhaomingkeji.xyz/gtentvsonx.html

Py:   itertools.permutations(arr)
来源：http://hz.jyoumei.cn/gtnojwedwn.html

PHP:  // 手写递归交换
来源：http://hz.zhongyouzk.top/gtwawjhagx.html

JS:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtqfdlqkoi.html

TS:   // 手写回溯递归
来源：http://hz.cashguo.top/gtuztdfuyy.html

Java: // 手写回溯递归
来源：http://hz.fengsongda.top/gtumyvmhhz.html

Go:   // 手写回溯递归
来源：http://hz.zhoulong.xyz/gttzmfseuk.html

Ruby: arr.permutation.to_a
来源：http://hz.hfpthk.cn/gtajbnpzwf.html

C#:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtljpttxsf.html

[N09] 栈与队列
来源：http://hz.zdqjudy.top/gtxaatcegb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ybcxt.top/gtzpkvrzcf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.aibaodan.cn/gtfahexvla.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yj20258888.top/gtutzdmmpa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cheryme.top/gtqfslykyd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xuanzx.com/gtkfkmmcyg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.nwbrower.top/gtjphivdnf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shanyushiyangtech.top/gtpkdaskoi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shzxlz.cn/gtshwgjgdl.html

[N10] 链表节点定义
来源：http://hz.yueranfly.top/gttjxwstey.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yj20258.top/gtryxqaaht.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.fengsongda.top/gtenvsrddt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.9152youxi.cn/gtsieovjsz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.52xcode.cn/gtcctuifyk.html

Java: class Node { int v; Node next; }
来源：http://hz.aizwys.cn/gtzheycktd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ydjk.org.cn/gtkoqfdjgz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yuanzhike.top/gtwctbdzqv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nwbrower.top/gtuysajkau.html

[N11] 二叉树中序遍历
来源：http://hz.gaohongyu789.top/gtgqsagebd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.pengpengdd.cyou/gtfqleownu.html

PHP:  // 手写递归函数
来源：http://hz.shanyushiyangkeji.top/gtmkjgrqrk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuanzhike.top/gtrswqtpxh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgfzy.top/gtskdscdmo.html

Java: // 手写递归
来源：http://hz.jinghuilouyu.cn/gtpzvhoslp.html

Go:   // 手写递归
来源：http://hz.ywan-chungtsiang.top/gtiphxtpsb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.havefunace.top/gtfmzmdgvf.html

C#:   // 手写递归
来源：http://hz.jlsjyb.cn/gthxvuqeab.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yangfankeji.com/gtvnpjradd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.redwolf501.top/gtaheoqckl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.nanxuanxn.top/gtwtwhmvgq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xylfe.cn/gtojabrmro.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuanzx.com/gtqhlotimb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sysykeji.top/gtwyrfxlnq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yj202588.top/gtrluwcjfp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yanxiufei.cn/gtqvzxrfnt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.meibo888.top/gtjndexnzi.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtkfllxjno.html

O. 并发与异步
来源：http://hz.jinyuanbaomall.cn/gtiepjyddg.html

================================================================================
来源：http://hz.dianchejie.cn/gteqtolwti.html

[O01] 启动一个线程
来源：http://hz.jinqigfzy.top/gtnzmwstms.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xuetiantiany.cn/gtbzhgorpu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.tanke756.top/gtachppzlo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.aibaodan.cn/gtfkhdvbnp.html

TS:   // 同 JS
来源：http://hz.jinghuilouyu.cn/gtaerpqbjz.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhiwuduotai.top/gtcqfhgfuw.html

Go:   go f()
来源：http://hz.svipenyu.cn/gtgzmslteq.html

Ruby: Thread.new { f }
来源：http://hz.yj20258888.top/gtfastmxnj.html

C#:   Task.Run(() => F());
来源：http://hz.shanyushiyangkeji.top/gtgkayvxwi.html

[O02] 使用线程池
来源：http://hz.tianlin.xyz/gtemvavmyq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.guannengcc.top/gttumdpimw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shuidangran.top/gtdnfpnyis.html

JS:   // worker_threads 线程池
来源：http://hz.0kj1m.cn/gtzidofqan.html

TS:   // worker_threads 线程池
来源：http://hz.guowangkeji.top/gtbkfhpufm.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.aizwys.cn/gtdpvezjhy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.sysykeji.top/gtouzytcha.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.snrcjt.cn/gtaicbzaff.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ehwqpu.com/gtixkiuebf.html

[O03] 加锁保护共享数据
来源：http://hz.nanxuanxn.top/gtqwjiugay.html

Py:   with lock: shared += 1
来源：http://hz.svipenyu.cn/gtpikceukf.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yanxiufei.cn/gtsycbmlox.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cheryme.top/gtsienddwz.html

TS:   // 同 JS
来源：http://hz.zhaomingkeji.xyz/gtyewrfoga.html

Java: synchronized (this) { shared++; }
来源：http://hz.jyoumei.cn/gthfftrdyh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xuanzx.com/gtzgrdwjpj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinqigfzy.top/gtcgwocnhf.html

C#:   lock (gate) { shared++; }
来源：http://hz.sysykeji.top/gtkolrtpya.html

[O04] 定义异步函数并等待
来源：http://hz.quarkkingdee.top/gtujgaqnwf.html

Py:   async def f():⏎    await g()
来源：http://hz.9152youxi.cn/gtteskzyqa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.bjfxy.top/gtpngkxcke.html

JS:   async function f() { await g(); }
来源：http://hz.gogol.net.cn/gtuobfuxfz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.316326.xyz/gtxhuwzipd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hongshengwenyu.top/gtodyzinxf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xingfuxueyuan.xyz/gtcrgxqgxm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.nanxuanxn.top/gtfvzltpmq.html

C#:   async Task F() { await G(); }
来源：http://hz.cucudq.cn/gtzjqdtype.html

[O05] 并发执行并等待全部完成
来源：http://hz.hammf.cn/gtefhjnqrr.html

Py:   asyncio.gather(*tasks)
来源：http://hz.dianchejie.cn/gtrubytplt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yuxming.cn/gtnkmodxcu.html

JS:   await Promise.all(tasks)
来源：http://hz.mhx1999.top/gtfpsygyzy.html

TS:   await Promise.all(tasks)
来源：http://hz.ydzc1.top/gtmpkdzszg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cheryme.top/gtnvplturq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.vqdsnc.cn/gtkxpxrzdp.html

Ruby: threads.map(&:join)
来源：http://hz.redwolf501.top/gtlilqalcf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.bjfxy.top/gtcwdcmeiy.html


<!-- 参考信息 -->