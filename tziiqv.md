代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nanxuanxn.top/gtzdqbnnhq.html

[L04] 设置超时
来源：http://hz.jqgufenzy.top/gtgvafhudg.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhijiandao.cn/gtdkueuoyc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.chenjidiqi.icu/gtzvenbfqq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.kuanghao11.cn/gttpywxxvg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.mhx1999.top/gtqxxsuhuq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.dashuyun.cn/gttlfqtfbc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhongyouzk.top/gtchhqislx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yj202588.top/gtvrfcjjtf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cashguo.top/gteflmuuxr.html

[L05] 上传文件（multipart）
来源：http://hz.shanyushiyangkeji.top/gtpbrekmej.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gogol.net.cn/gtgaenyeeo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yongpay.top/gtjojwniht.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.pengpengdd.cyou/gtzrrojeod.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jianghu66.top/gttxnhoect.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.tanke756.top/gtsagkdmqr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sysykeji.top/gtarqrusms.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.fzhhl.top/gtxgezmnzk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.mhx1999.top/gtorfgomvl.html

[L06] 解析响应为 JSON
来源：http://hz.xylfe.cn/gtwiwmaexg.html

Py:   resp.json()
来源：http://hz.fzhhl.top/gtxhidpdzq.html

PHP:  json_decode($body, true);
来源：http://hz.chenjidiqi.icu/gtzwaxzjtf.html

JS:   await resp.json()
来源：http://hz.cheryme.top/gtycujupjz.html

TS:   await resp.json()
来源：http://hz.hongshengwenyu.top/gtzymcycbe.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.316326.xyz/gtqaueeckd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yangfankeji.com/gtyaxnszjn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.quarkkingdee.top/gtdlcdmqsl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cdnleiting.top/gtpmjiedgx.html

[L07] 处理 HTTP 状态码
来源：http://hz.gogol.net.cn/gtnqpovefe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gzhubu.top/gtrgatzife.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ywan-chungtsiang.top/gtjpozuppb.html

JS:   resp.ok;  resp.status
来源：http://hz.hysaishi.cn/gtenakxxno.html

TS:   resp.ok;  resp.status
来源：http://hz.zhiwuduotai.top/gttjffckmt.html

Java: resp.statusCode()
来源：http://hz.yonumen.top/gttptcmwjq.html

Go:   resp.StatusCode
来源：http://hz.316326.xyz/gtsnnghoac.html

Ruby: resp.code.to_i
来源：http://hz.cheryme.top/gtwyeinoiy.html

C#:   (int)resp.StatusCode
来源：http://hz.zhiwuduotai.top/gtezomnubn.html

[L08] 并发请求多个地址
来源：http://hz.0kj1m.cn/gttfwcfmll.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.aibaodan.cn/gtdonzeybe.html

PHP:  curl_multi_init() 系列
来源：http://hz.xuanzx.com/gtyzqvwfwe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.52xcode.cn/gtcycssajo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangshuangyany.cn/gtllnvmual.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.snrcjt.cn/gtzrvzdkjq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.pycfn.com/gtsiagziya.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.sufxvd.cn/gtimvahwdd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.tianlin.xyz/gtwiwwkmpx.html

================================================================================
来源：http://hz.zhixingplan.top/gtrjvtpgew.html

M. 命令行 / 进程 / 环境
来源：http://hz.ydjk.org.cn/gtomgzrukl.html

================================================================================
来源：http://hz.ydjk.org.cn/gthdcwfqgf.html

[M01] 读取命令行参数
来源：http://hz.tianlin.xyz/gtbbnxvhia.html

Py:   sys.argv[1:]
来源：http://hz.9152youxi.cn/gtykzwiayp.html

PHP:  $argv;  $argc;
来源：http://hz.guannengcc.top/gtpflxfrhk.html

JS:   process.argv.slice(2)
来源：http://hz.yongpay.top/gtduorbhqv.html

TS:   process.argv.slice(2)
来源：http://hz.aizwys.cn/gtojjinkqy.html

Java: args 数组（main 方法参数）
来源：http://hz.iojbl.cn/gtjddvivjb.html

Go:   os.Args[1:]
来源：http://hz.jyoumei.cn/gtepwraiim.html

Ruby: ARGV
来源：http://hz.dashuyun.cn/gtmdpzzhnr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jianghu66.top/gttgtcxpcg.html

[M02] 读取环境变量
来源：http://hz.zhengqikj.top/gttgxpfvzf.html

Py:   os.environ.get("HOME")
来源：http://hz.wangdashe.top/gtmzmnyvuj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yj20258.top/gtaefplrbu.html

JS:   process.env.HOME
来源：http://hz.bjfxy.top/gttvgagovp.html

TS:   process.env.HOME
来源：http://hz.meibo888.top/gtbnwvuiqk.html

Java: System.getenv("HOME")
来源：http://hz.cheryme.top/gtdihqurra.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.vqdsnc.cn/gtgpaehcgx.html

Ruby: ENV["HOME"]
来源：http://hz.ywan-chungtsiang.top/gtrikhefcn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenzaomai.com/gtmqitkvzf.html

[M03] 执行外部命令
来源：http://hz.pengpengdd.cyou/gtepizthry.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jinghuilouyu.cn/gtulrjiujg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.fzhhl.top/gtgudjefgq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.bjfxy.top/gtvkuviqmq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yonumen.top/gtzkqnzwdz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.daxiang520.top/gtvrdfolpp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yj20258888.top/gtayaucgaw.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hysaishi.cn/gtbrxcyjnn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.chenjidiqi.icu/gtizbxejyl.html

[M04] 获取当前工作目录
来源：http://hz.feifeiyinyue.top/gtyqdncoyv.html

Py:   os.getcwd()
来源：http://hz.wangshuangyany.cn/gtuxzxjdqf.html

PHP:  getcwd();
来源：http://hz.ehwqpu.com/gtpfnuclyf.html

JS:   process.cwd()
来源：http://hz.sufxvd.cn/gtmbmacmzg.html

TS:   process.cwd()
来源：http://hz.yonumen.top/gthizgdbbn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhixingplan.top/gtevameblt.html

Go:   os.Getwd()
来源：http://hz.yj20258888.top/gtkznbdrtx.html

Ruby: Dir.pwd
来源：http://hz.guowangkeji.top/gtzismoxsi.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yangfankeji.com/gtbyyejeiy.html

[M05] 设置退出码
来源：http://hz.jlsjyb.cn/gtcqimbivj.html

Py:   sys.exit(1)
来源：http://hz.aizwys.cn/gtlbckymws.html

PHP:  exit(1);
来源：http://hz.gotoacloud.top/gtqqlzymyt.html

JS:   process.exit(1)
来源：http://hz.hfpthk.cn/gtfcomjzfd.html

TS:   process.exit(1)
来源：http://hz.chenlongwang.top/gtjqlxfohs.html

Java: System.exit(1)
来源：http://hz.yanxiufei.cn/gtqyzgnquz.html

Go:   os.Exit(1)
来源：http://hz.wangshuangyany.cn/gtvgpjqqzg.html

Ruby: exit 1
来源：http://hz.zhongyouzk.top/gtxtnzchpp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.haohaochexian.top/gtsoblamxo.html

[M06] 向标准错误输出
来源：http://hz.jiagoushi.top/gtjkhwawwe.html

Py:   print("err", file=sys.stderr)
来源：http://hz.bjfxy.top/gtvxlkjkuz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jyoumei.cn/gtcalheqvp.html

JS:   console.error("err")
来源：http://hz.zhoulong.xyz/gtokjqopzb.html

TS:   console.error("err")
来源：http://hz.jlsjyb.cn/gtxzsaowhr.html

Java: System.err.println("err")
来源：http://hz.jiagoushi.top/gtotampcez.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yj20258888.top/gtytumevxv.html

Ruby: warn "err"
来源：http://hz.sufxvd.cn/gtyipopqxt.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.aizwys.cn/gtdbjsjomq.html

[M07] 判断是否为主入口
来源：http://hz.pengpengdd.cyou/gtwiuwswng.html

Py:   if __name__ == "__main__":
来源：http://hz.zycfv.cn/gtuoeqvavq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.smart0.xyz/gtmsorzedr.html

JS:   require.main === module
来源：http://hz.tianlin.xyz/gtcgdfjuzp.html

TS:   require.main === module
来源：http://hz.zhongyouzk.top/gtvmwvlypa.html

Java: public static void main(String[] args)
来源：http://hz.daria6918.cn/gtoaytjqup.html

Go:   func main()
来源：http://hz.shanyushiyangkeji.top/gtrbkexieg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.c1oappe.top/gtumzskdnc.html

C#:   static void Main(string[] args)
来源：http://hz.yj20258888.top/gtkbxxbdgy.html

[M08] 获取系统与运行时信息
来源：http://hz.cheryme.top/gtjgshlcgc.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zdqjudy.top/gtlsdbdgmh.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.mhx1999.top/gtvhogpbhy.html

JS:   process.platform;  process.version
来源：http://hz.cqqwz.cn/gtllfbdgmb.html

TS:   process.platform;  process.version
来源：http://hz.tianlin.xyz/gtovhdosgs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.meibo888.top/gtcbircgni.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sxryk.cn/gthticaivk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ivvv.top/gtzdajynql.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.feifeiyinyue.top/gtdunfrdfx.html

================================================================================
来源：http://hz.ydzc1.top/gtqqjtauwq.html

N. 数据结构与算法
来源：http://hz.sysykeji.top/gtiwnjuine.html

================================================================================
来源：http://hz.havefunace.top/gtrfldhcbx.html

[N01] 二分查找（有序数组）
来源：http://hz.jinyuanbaomall.cn/gtvbhskwyu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hammf.cn/gtufenzjgp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.52xcode.cn/gtnkvqdhqe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinyuanbaomall.cn/gtcgloohia.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxinkj.top/gtolbaotqv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.birdmap.top/gtsrmlkvua.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.bjfxy.top/gtdmuqrrxa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.iojbl.cn/gtwtmaqmbd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xinyue.icu/gtsrjppltt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.snrcjt.cn/gtzyxrftiy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pengpengdd.cyou/gtigcajzkk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.316326.xyz/gtdvejykur.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jqgufenzy.top/gtishlwgdp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cucudq.cn/gtuffheyxi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.birdmap.top/gtfttnwrbl.html

Go:   slices.Sort(arr)
来源：http://hz.yongpay.top/gtodmgudso.html

Ruby: arr.sort
来源：http://hz.52xcode.cn/gtimlgoeja.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.aibaodan.cn/gtpnxicrmo.html

[N03] 快速排序（分治示例）
来源：http://hz.zhongyouzk.top/gtcpivzvvi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.52xcode.cn/gtsvlnjcxs.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sufxvd.cn/gtacsvflqd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sxryk.cn/gtuobjgjnl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhengqikj.top/gteiojthov.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yangfankeji.com/gtmuspwhly.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.tianlin.xyz/gtrjquyfod.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hfpthk.cn/gtsegdieyp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.52xcode.cn/gtxnwyqsyr.html

[N04] 斐波那契数列
来源：http://hz.hywenlv.cn/gtxrkmpruc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.nanxuanxn.top/gthrbhgijc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jyoumei.cn/gtzxxnksrw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jqgufenzy.top/gtcbeoxyza.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenjidiqi.icu/gtacrojcrx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.guowangkeji.top/gtvvvxfsjv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ybcxt.top/gtwmoxcakm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.nwbrower.top/gtzkbfgsho.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj202588.top/gtyyeegqwv.html

[N05] 最大公约数
来源：http://hz.hnxiangtu.top/gtdjentaes.html

Py:   math.gcd(a, b)
来源：http://hz.ehwqpu.com/gtzhnikxhf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.guowangkeji.top/gthwgkpmnr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dianchejie.cn/gtrlunnuol.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.svipenyu.cn/gtnnthnrap.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.kuanghao11.cn/gtqfwervgd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xingfuxueyuan.xyz/gtkmngmpjl.html

Ruby: a.gcd(b)
来源：http://hz.cheryme.top/gtnhmcckmo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xinyue.icu/gtpswpzlbq.html

[N06] 判断回文字符串
来源：http://hz.hywenlv.cn/gtywmbhbyi.html

Py:   s == s[::-1]
来源：http://hz.yvedp.cn/gtezsxojua.html

PHP:  $s === strrev($s);
来源：http://hz.zhongyouzk.top/gtaqzkqklj.html

JS:   s === [...s].reverse().join("")
来源：http://hz.0kj1m.cn/gtkddvzphe.html

TS:   s === [...s].reverse().join("")
来源：http://hz.daria6918.cn/gteawtgsdl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yonumen.top/gtkthadkym.html

Go:   // 双指针从两端比较
来源：http://hz.daxiang520.top/gthvvzcdyd.html

Ruby: s == s.reverse
来源：http://hz.ivvv.top/gtzdspjxgm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhiwuduotai.top/gtgqiqjszf.html

[N07] 两数之和（返回下标）
来源：http://hz.birdmap.top/gttdfoaimz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.chenlongwang.top/gtoacblpgg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.feifeiyinyue.top/gtzvfbklxs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sysykeji.top/gtmcohvvuj.html

TS:   // 手写 Map<string, number>
来源：http://hz.zdqjudy.top/gtojwzgjpf.html

Java: // 手写 HashMap
来源：http://hz.chenlongwang.top/gtvqtwbuqf.html

Go:   // 手写 map[int]int
来源：http://hz.tianlin.xyz/gtflrubett.html

Ruby: // 手写 Hash
来源：http://hz.ydzc1.top/gtnqnhsews.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.chenlongwang.top/gtcmhdkljy.html

[N08] 生成全排列
来源：http://hz.gaohongyu789.top/gtpesdwzzn.html

Py:   itertools.permutations(arr)
来源：http://hz.dianchejie.cn/gtvbnwrula.html

PHP:  // 手写递归交换
来源：http://hz.haohaochexian.top/gtohclmddv.html

JS:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtetlvqryz.html

TS:   // 手写回溯递归
来源：http://hz.jyoumei.cn/gtewaywevl.html

Java: // 手写回溯递归
来源：http://hz.52xcode.cn/gtigdbrjuw.html

Go:   // 手写回溯递归
来源：http://hz.aizwys.cn/gtbgeehpjz.html

Ruby: arr.permutation.to_a
来源：http://hz.wangdashe.top/gtoszdszvw.html

C#:   // 手写回溯递归
来源：http://hz.jianghu66.top/gtcyrxukvc.html

[N09] 栈与队列
来源：http://hz.yj20258.top/gtqabugmak.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj20258.top/gtswuhzvbl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhijiandao.cn/gtgyptvyvf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yj202588.top/gtbzhxvupe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.nanxinkj.top/gtoqwgngzh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hfpthk.cn/gtdhkwmvca.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cqqwz.cn/gtnunfghdy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhixingplan.top/gtxvhbanqc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yj202588.top/gtyzagfpik.html

[N10] 链表节点定义
来源：http://hz.yuxming.cn/gtxfegavwc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jianghu66.top/gtrssfpwtq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhengqikj.top/gtjmzkfqjk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj202588.top/gtxotduoux.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yj202588.top/gtsfhukqmb.html

Java: class Node { int v; Node next; }
来源：http://hz.guowangkeji.top/gtemftaxzy.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jianghu66.top/gtvbtygxrb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.tianlin.xyz/gtylhptlbv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yvedp.cn/gtaeoksdkf.html

[N11] 二叉树中序遍历
来源：http://hz.wangshuangyany.cn/gtmckmcawg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shanyushiyangkeji.top/gtifrvbufd.html

PHP:  // 手写递归函数
来源：http://hz.redwolf501.top/gtdljvhiof.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xuanzx.com/gtnzstkioc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ehwqpu.com/gtlmnbqvmc.html

Java: // 手写递归
来源：http://hz.yueranfly.top/gtfavyhove.html

Go:   // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtyfycikon.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.haohaochexian.top/gtvonxkfjd.html

C#:   // 手写递归
来源：http://hz.zhongyouzk.top/gtjkdvwfsq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shanyushiyangtech.top/gtocyztsxb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.guannengcc.top/gtffwabrlz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.svipenyu.cn/gtvbhneakr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jianghu66.top/gtfubbsust.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yanxiufei.cn/gtlotayqkp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhaomingkeji.xyz/gtsywjfmkh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zdqjudy.top/gtjmjfxlmi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinghuilouyu.cn/gtefchknrl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhengqikj.top/gtvanxafup.html

================================================================================
来源：http://hz.zhongyouzk.top/gtegimjowq.html

O. 并发与异步
来源：http://hz.tanke756.top/gtmuihidjq.html

================================================================================
来源：http://hz.cdnleiting.top/gttnthyvai.html

[O01] 启动一个线程
来源：http://hz.zhixingplan.top/gtjgtnevwm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hfpthk.cn/gtlzxfivgj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.sweek.top/gtrnpxyrmc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.tian-w.cn/gtzzziyyzj.html

TS:   // 同 JS
来源：http://hz.316326.xyz/gtyvnkwhfo.html

Java: new Thread(() -> f()).start()
来源：http://hz.hnqzz.top/gtivosqsrn.html

Go:   go f()
来源：http://hz.feifeiyinyue.top/gtqdijgrlb.html

Ruby: Thread.new { f }
来源：http://hz.yj202588.top/gtolomjfsd.html

C#:   Task.Run(() => F());
来源：http://hz.guowangkeji.top/gtttuynnks.html

[O02] 使用线程池
来源：http://hz.0kj1m.cn/gtwfeblweb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zycfv.cn/gtvbbmgfqd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.haohaochexian.top/gtxvsnonvu.html

JS:   // worker_threads 线程池
来源：http://hz.pengpengdd.cyou/gtjlmkeutn.html

TS:   // worker_threads 线程池
来源：http://hz.sweek.top/gtkcgdohob.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xinyue.icu/gtzxtlkodm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cdnleiting.top/gtmtatlfjo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xuetiantiany.cn/gtmkriibws.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cdnleiting.top/gtcsjxytfs.html

[O03] 加锁保护共享数据
来源：http://hz.guowangkeji.top/gtmcivyadc.html

Py:   with lock: shared += 1
来源：http://hz.jinqigfzy.top/gtfqioivug.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.bjfxy.top/gtyjgkbzqz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jianghu66.top/gtjgggtqco.html

TS:   // 同 JS
来源：http://hz.cheryme.top/gtdphkxzqc.html

Java: synchronized (this) { shared++; }
来源：http://hz.jinqigfzy.top/gtchiegfoc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.sysykeji.top/gthjwcoedb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhijiandao.cn/gtcvucituj.html

C#:   lock (gate) { shared++; }
来源：http://hz.sufxvd.cn/gtilwzrcdk.html

[O04] 定义异步函数并等待
来源：http://hz.havefunace.top/gtsyuxasxv.html

Py:   async def f():⏎    await g()
来源：http://hz.chenlongwang.top/gtnhmfniej.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ppjwa.cn/gtdmehnedq.html

JS:   async function f() { await g(); }
来源：http://hz.zhongyouzk.top/gtdhythaqw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.fengsongda.top/gtowudqytk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yuanzhike.top/gtigfurqle.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.svipenyu.cn/gtodbyqqye.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jinyuanbaomall.cn/gthuqzmmqr.html

C#:   async Task F() { await G(); }
来源：http://hz.hnxiangtu.top/gthdxfhtxi.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinqigfzy.top/gtvxoxgcgy.html

Py:   asyncio.gather(*tasks)
来源：http://hz.pengpengdd.cyou/gtpokxtxjg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cdnleiting.top/gtdpwnawwl.html

JS:   await Promise.all(tasks)
来源：http://hz.feifeiyinyue.top/gtyarzzfdj.html

TS:   await Promise.all(tasks)
来源：http://hz.zycfv.cn/gtxfvaejip.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ybcxt.top/gttyronwoz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ehwqpu.com/gtaoppwtlz.html

Ruby: threads.map(&:join)
来源：http://hz.yonumen.top/gthkzsfheu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.nanxinkj.top/gtusedukji.html

[O06] 使用进程池
来源：http://hz.sweek.top/gtjudhhskm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xinyue.icu/gtdbwgirsz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.guannengcc.top/gtvnncqxvp.html

JS:   // child_process / cluster 模块
来源：http://hz.jyoumei.cn/gtejafsgmn.html

TS:   // child_process / cluster 模块
来源：http://hz.mhx1999.top/gtugsqihfm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.birdmap.top/gthubdtpfl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zdqjudy.top/gtduxxqjph.html

Ruby: // fork 块
来源：http://hz.aizwys.cn/gtxrrsqfkx.html

C#:   Parallel.For
来源：http://hz.chenzaomai.com/gtbmhxbrbs.html

================================================================================
来源：http://hz.hnqzz.top/gtcpvheunj.html

P. 常用工具函数
来源：http://hz.svipenyu.cn/gtpwecmpur.html

================================================================================
来源：http://hz.zycfv.cn/gtojbonysh.html

[P01] 生成 UUID
来源：http://hz.feifeiyinyue.top/gtakvhqsdq.html

Py:   str(uuid.uuid4())
来源：http://hz.yuxming.cn/gtszjyieve.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhoulong.xyz/gtthzrzvcf.html

JS:   crypto.randomUUID()
来源：http://hz.bjfxy.top/gtbeolzqrb.html

TS:   crypto.randomUUID()
来源：http://hz.gotoacloud.top/gtihclzetv.html

Java: UUID.randomUUID().toString()
来源：http://hz.wangshuangyany.cn/gtmysifupd.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cucudq.cn/gtrcapgwes.html

Ruby: SecureRandom.uuid
来源：http://hz.mhx1999.top/gtijeaczma.html


<!-- 参考信息 -->