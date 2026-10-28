代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xinyue.icu/gtghpsinmh.html

[L04] 设置超时
来源：http://hz.fzhhl.top/gtadhdpahx.html

Py:   requests.get(url, timeout=5)
来源：http://hz.snrcjt.cn/gtfecqpekz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shzxlz.cn/gtnuuxbbce.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yanxiufei.cn/gtxrijlrvt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinghuilouyu.cn/gtfcdcvdqj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.meibo888.top/gtcscwogqf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gzhubu.top/gtjttkfdgq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yangfankeji.com/gtfhnhkxoz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.iojbl.cn/gtofsqrcqy.html

[L05] 上传文件（multipart）
来源：http://hz.ywan-chungtsiang.top/gtjbqrjtyv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.smart0.xyz/gtfixduanb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.aibaodan.cn/gtewewnphb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.quarkkingdee.top/gtpogdwjiw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ivvv.top/gtuqmgxxhh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yj202588.top/gtdmbisfrq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sysykeji.top/gtxqplthxi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xinyue.icu/gtwvuuhcrm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj20258.top/gtozpifgtq.html

[L06] 解析响应为 JSON
来源：http://hz.zycfv.cn/gtlfxntfvz.html

Py:   resp.json()
来源：http://hz.ivvv.top/gtvlutiyfo.html

PHP:  json_decode($body, true);
来源：http://hz.ivvv.top/gtxqvbqpky.html

JS:   await resp.json()
来源：http://hz.yongpay.top/gtpftfblmx.html

TS:   await resp.json()
来源：http://hz.sysykeji.top/gtpbkzoiuy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinghuilouyu.cn/gtjjjkskow.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sysykeji.top/gtrtfibmze.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cashguo.top/gtqcplrxst.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ivvv.top/gtfprsjqqx.html

[L07] 处理 HTTP 状态码
来源：http://hz.xylfe.cn/gtmkooiryd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xuanzx.com/gtboiuwwtr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hammf.cn/gtigydrrru.html

JS:   resp.ok;  resp.status
来源：http://hz.yuanzhike.top/gtidtbpjzp.html

TS:   resp.ok;  resp.status
来源：http://hz.zhijiandao.cn/gtqczxmzmo.html

Java: resp.statusCode()
来源：http://hz.chenlongwang.top/gtveuqcfjo.html

Go:   resp.StatusCode
来源：http://hz.zycfv.cn/gtxqysbskh.html

Ruby: resp.code.to_i
来源：http://hz.guannengcc.top/gtacvjtttr.html

C#:   (int)resp.StatusCode
来源：http://hz.chenjidiqi.icu/gtuuefxswa.html

[L08] 并发请求多个地址
来源：http://hz.shangyingyoupin.top/gttlfgknvb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yonumen.top/gtgwjmncci.html

PHP:  curl_multi_init() 系列
来源：http://hz.cashguo.top/gtidihxkle.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zdqjudy.top/gtikhmpvdr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yonumen.top/gtarqjjohv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.svipenyu.cn/gtrbddxnnh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.guannengcc.top/gtfjflcuhw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.redwolf501.top/gttjtuxndf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.fzhhl.top/gtaidsyqhh.html

================================================================================
来源：http://hz.9152youxi.cn/gtlhotkqzd.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhoulong.xyz/gtsswmxnfg.html

================================================================================
来源：http://hz.sxryk.cn/gtghlqvubj.html

[M01] 读取命令行参数
来源：http://hz.xuetiantiany.cn/gtfrerlsvz.html

Py:   sys.argv[1:]
来源：http://hz.havefunace.top/gtjpwoettx.html

PHP:  $argv;  $argc;
来源：http://hz.vqdsnc.cn/gtiqrtkmsb.html

JS:   process.argv.slice(2)
来源：http://hz.jinqigfzy.top/gtrxufuvcl.html

TS:   process.argv.slice(2)
来源：http://hz.sxryk.cn/gtfqmklbvj.html

Java: args 数组（main 方法参数）
来源：http://hz.zhiwuduotai.top/gtntuzfbbs.html

Go:   os.Args[1:]
来源：http://hz.hfpthk.cn/gtwmoabcow.html

Ruby: ARGV
来源：http://hz.gogol.net.cn/gtmvlzmjvl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yangfankeji.com/gtqapfwjjg.html

[M02] 读取环境变量
来源：http://hz.gzhubu.top/gtjttewbcd.html

Py:   os.environ.get("HOME")
来源：http://hz.daxiang520.top/gtxvdciprg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhaomingkeji.xyz/gtzdjksdfo.html

JS:   process.env.HOME
来源：http://hz.kuanghao11.cn/gtkpllfvuk.html

TS:   process.env.HOME
来源：http://hz.guowangkeji.top/gtypgjxpzj.html

Java: System.getenv("HOME")
来源：http://hz.shzxlz.cn/gteyjegvjt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.redwolf501.top/gtbbnhgwrd.html

Ruby: ENV["HOME"]
来源：http://hz.yj202588.top/gtfnfssidh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cashguo.top/gtrtwbywar.html

[M03] 执行外部命令
来源：http://hz.ydzc1.top/gtmgvuggky.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhixingplan.top/gtktrhnpcn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.haohaochexian.top/gtnsbqpkuv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.aizwys.cn/gtypqthzld.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.svipenyu.cn/gtsaxewtgt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.mhx1999.top/gtuejcvdao.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xuanzx.com/gtarcdebtu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hammf.cn/gtlrbpsihw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yongpay.top/gtyznsgllq.html

[M04] 获取当前工作目录
来源：http://hz.9152youxi.cn/gtwkfpyfag.html

Py:   os.getcwd()
来源：http://hz.havefunace.top/gtjnybhgvu.html

PHP:  getcwd();
来源：http://hz.hywenlv.cn/gtnclsildg.html

JS:   process.cwd()
来源：http://hz.gotoacloud.top/gteuhilobj.html

TS:   process.cwd()
来源：http://hz.zhaomingkeji.xyz/gtmvxewjsg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.quarkkingdee.top/gtlzpebjfn.html

Go:   os.Getwd()
来源：http://hz.aizwys.cn/gtzkuncdse.html

Ruby: Dir.pwd
来源：http://hz.yangfankeji.com/gthxgybudu.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yanxiufei.cn/gtgtaynlle.html

[M05] 设置退出码
来源：http://hz.zdqjudy.top/gthducwsoj.html

Py:   sys.exit(1)
来源：http://hz.ehwqpu.com/gtzviqnxna.html

PHP:  exit(1);
来源：http://hz.fzhhl.top/gtlopbwsbb.html

JS:   process.exit(1)
来源：http://hz.andypj.xyz/gtoiyurvzc.html

TS:   process.exit(1)
来源：http://hz.iojbl.cn/gtqyudkzfk.html

Java: System.exit(1)
来源：http://hz.yonumen.top/gtghswcjrz.html

Go:   os.Exit(1)
来源：http://hz.pengpengdd.cyou/gtygnxaerx.html

Ruby: exit 1
来源：http://hz.shanyushiyangkeji.top/gtwaibiihl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.wangshuangyany.cn/gtskagzeil.html

[M06] 向标准错误输出
来源：http://hz.ydzc1.top/gtuzegoqmz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.snrcjt.cn/gtoifqubia.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.tian-w.cn/gtmfmrvpon.html

JS:   console.error("err")
来源：http://hz.jiagoushi.top/gtrjdxzuif.html

TS:   console.error("err")
来源：http://hz.ydzc1.top/gtqagchvvp.html

Java: System.err.println("err")
来源：http://hz.shuidangran.top/gtnthhcgsa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cqqwz.cn/gtghkwvkyx.html

Ruby: warn "err"
来源：http://hz.svipenyu.cn/gtdvihtmme.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ivvv.top/gtctfyfkfj.html

[M07] 判断是否为主入口
来源：http://hz.feifeiyinyue.top/gtkjblcntb.html

Py:   if __name__ == "__main__":
来源：http://hz.daria6918.cn/gtocvbunoy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gotoacloud.top/gtbugfhuru.html

JS:   require.main === module
来源：http://hz.sufxvd.cn/gtnahwemtc.html

TS:   require.main === module
来源：http://hz.wangshuangyany.cn/gtgdttefrg.html

Java: public static void main(String[] args)
来源：http://hz.dashuyun.cn/gtetsucwcx.html

Go:   func main()
来源：http://hz.hfpthk.cn/gtsqtcztqz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.birdmap.top/gtdcmmdwze.html

C#:   static void Main(string[] args)
来源：http://hz.chenlongwang.top/gtezdyhwhr.html

[M08] 获取系统与运行时信息
来源：http://hz.daria6918.cn/gtucboocxi.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ybcxt.top/gtpdfqvgkr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hywenlv.cn/gtvqhrasyd.html

JS:   process.platform;  process.version
来源：http://hz.nanxinkj.top/gtbxduwrxn.html

TS:   process.platform;  process.version
来源：http://hz.cucudq.cn/gtbjqhwvxf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tian-w.cn/gtkillfcli.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yueranfly.top/gtdkssxdxg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.svipenyu.cn/gtowaryuog.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.9152youxi.cn/gtkmhurmfr.html

================================================================================
来源：http://hz.pycfn.com/gtvkozmrxp.html

N. 数据结构与算法
来源：http://hz.ydjk.org.cn/gtvjmzjvjo.html

================================================================================
来源：http://hz.aibaodan.cn/gtfdwploog.html

[N01] 二分查找（有序数组）
来源：http://hz.svipenyu.cn/gtiquybrdi.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.feifeiyinyue.top/gtdhctyltx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hnqzz.top/gtjoprwfbw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.svipenyu.cn/gtxggsicfh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xinyue.icu/gtjdazkkhd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shzxlz.cn/gtodhinjjs.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yongpay.top/gtwvrpjgad.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.nanxuanxn.top/gtcjptdzag.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ydzc1.top/gtijrmmiwm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.tanke756.top/gtpqkwcjcx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yanxiufei.cn/gtuacggniq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tanke756.top/gtqnmxqpjg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aibaodan.cn/gticczxiry.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ydjk.org.cn/gtehgmctmh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jyoumei.cn/gtnttjmucr.html

Go:   slices.Sort(arr)
来源：http://hz.jqgfzy.top/gttoasojqk.html

Ruby: arr.sort
来源：http://hz.hnqzz.top/gthqvkdbef.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yj20258888.top/gtgfipfkxc.html

[N03] 快速排序（分治示例）
来源：http://hz.fzhhl.top/gtmcsbsnpg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.daxiang520.top/gtagwimdfy.html

PHP:  // 递归实现，或用 usort
来源：http://hz.fengsongda.top/gtarwndqnh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gaohongyu789.top/gtfuvrbarv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cdnleiting.top/gtnuhblijs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ehwqpu.com/gtfjzxixfj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cheryme.top/gtzjryvynx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhijiandao.cn/gtnqptimyd.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhengqikj.top/gtgiwtmskc.html

[N04] 斐波那契数列
来源：http://hz.ivvv.top/gtakendcpv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.redwolf501.top/gtvpvpydos.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jiagoushi.top/gtsgeulcpy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cdnleiting.top/gttnsozsmx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.birdmap.top/gtyiucwvjf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xuetiantiany.cn/gtinkkoaby.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.bjfxy.top/gtqwkdrmby.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258888.top/gtmvrzrjot.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.meibo888.top/gthygzsoie.html

[N05] 最大公约数
来源：http://hz.kuanghao11.cn/gttxkljfjq.html

Py:   math.gcd(a, b)
来源：http://hz.jyoumei.cn/gttrbehvhj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hammf.cn/gtyvaluqcn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jiagoushi.top/gtqcukouuy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guowangkeji.top/gtscqbngna.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.wangshuangyany.cn/gtsshoecxd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xuanzx.com/gtvmsjsaje.html

Ruby: a.gcd(b)
来源：http://hz.shuidangran.top/gtfrryqgub.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ydjk.org.cn/gtsosbrsik.html

[N06] 判断回文字符串
来源：http://hz.dashuyun.cn/gthamgxfnr.html

Py:   s == s[::-1]
来源：http://hz.guannengcc.top/gteejdhyot.html

PHP:  $s === strrev($s);
来源：http://hz.pycfn.com/gtbhksrwmq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtpwkxijye.html

TS:   s === [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtiyafqtdx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.redwolf501.top/gtdfaywezc.html

Go:   // 双指针从两端比较
来源：http://hz.aizwys.cn/gtrxzmkgom.html

Ruby: s == s.reverse
来源：http://hz.meibo888.top/gthztwtjmy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.snrcjt.cn/gtacaerbax.html

[N07] 两数之和（返回下标）
来源：http://hz.wangdashe.top/gtirypawwv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.sysykeji.top/gtmjdcdaat.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yanxiufei.cn/gtewfkfdma.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.bjfxy.top/gtgeshjwac.html

TS:   // 手写 Map<string, number>
来源：http://hz.hnxiangtu.top/gthdazmunt.html

Java: // 手写 HashMap
来源：http://hz.tian-w.cn/gtncqceymo.html

Go:   // 手写 map[int]int
来源：http://hz.zhoulong.xyz/gtfalmyyad.html

Ruby: // 手写 Hash
来源：http://hz.aizwys.cn/gtxpppmytt.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.haohaochexian.top/gtvcgdnraz.html

[N08] 生成全排列
来源：http://hz.hnqzz.top/gtxmbbjaul.html

Py:   itertools.permutations(arr)
来源：http://hz.yuanzhike.top/gtmuvgqwkf.html

PHP:  // 手写递归交换
来源：http://hz.xziqi.cn/gtdydsjtsa.html

JS:   // 手写回溯递归
来源：http://hz.yvedp.cn/gtpgtppdic.html

TS:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtbhueyxwl.html

Java: // 手写回溯递归
来源：http://hz.dashuyun.cn/gtisyhpdht.html

Go:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtcayqufws.html

Ruby: arr.permutation.to_a
来源：http://hz.chenzaomai.com/gtorjburby.html

C#:   // 手写回溯递归
来源：http://hz.jiagoushi.top/gtotiiagfi.html

[N09] 栈与队列
来源：http://hz.cheryme.top/gtfhlvszcb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jqgufenzy.top/gtpxqtaejf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.tanke756.top/gtzhriqmgp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.havefunace.top/gtrinxesmn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.dashuyun.cn/gtyxmhpdkh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xuetiantiany.cn/gtbcbjlrrg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ivvv.top/gthleqgnuu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cucudq.cn/gtktrosgzb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhongyouzk.top/gtsgesffhw.html

[N10] 链表节点定义
来源：http://hz.nwbrower.top/gtefdaazbm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.nanxinkj.top/gtnwwgbfvr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.wangdashe.top/gtawegqwnz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.meibo888.top/gtekhiudfk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shanyushiyangkeji.top/gtiqxmuuvh.html

Java: class Node { int v; Node next; }
来源：http://hz.316326.xyz/gtaqcliiye.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yangfankeji.com/gtzdaclevd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.smart0.xyz/gtgzizebgq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nanxuanxn.top/gtdlercwly.html

[N11] 二叉树中序遍历
来源：http://hz.yuxming.cn/gtfjmblvep.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hnqzz.top/gtpslafhtl.html

PHP:  // 手写递归函数
来源：http://hz.gzhubu.top/gtgbsdzlbc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenlongwang.top/gtxnclqcde.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xuanzx.com/gtybzjlbte.html

Java: // 手写递归
来源：http://hz.daxiang520.top/gtfwstkhsw.html

Go:   // 手写递归
来源：http://hz.xziqi.cn/gtyiaosmii.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.nanxuanxn.top/gtxbwnseda.html

C#:   // 手写递归
来源：http://hz.wangshuangyany.cn/gtdmenejho.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yueranfly.top/gtiyrbqhqm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hongshengwenyu.top/gtrstacqeq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.iojbl.cn/gtsmbuqrqd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sxryk.cn/gtkaibdihp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gaohongyu789.top/gtrsqdeshd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.svipenyu.cn/gtgaofcdce.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhongyouzk.top/gtyjpgbahl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cqqwz.cn/gtyzmnxwpo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xinyue.icu/gtjdvgorav.html

================================================================================
来源：http://hz.hnqzz.top/gtvmioteba.html

O. 并发与异步
来源：http://hz.daxiang520.top/gttgacuwda.html

================================================================================
来源：http://hz.xuanzx.com/gtfjpecgid.html

[O01] 启动一个线程
来源：http://hz.ydjk.org.cn/gtsympgbjb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.0kj1m.cn/gtmwrhnjst.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.nwbrower.top/gtmabhvfvj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yuxming.cn/gtuxajmoxr.html

TS:   // 同 JS
来源：http://hz.xylfe.cn/gtxmbjtrnw.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhongyouzk.top/gtpcwbzpnq.html

Go:   go f()
来源：http://hz.ppjwa.cn/gtfscudfzf.html

Ruby: Thread.new { f }
来源：http://hz.birdmap.top/gtjgkicdyy.html

C#:   Task.Run(() => F());
来源：http://hz.wangshuangyany.cn/gtkfqwkzuh.html

[O02] 使用线程池
来源：http://hz.yanxiufei.cn/gtqzffxnii.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.bjfxy.top/gtrqgtjoeu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.316326.xyz/gtkkrewkxe.html

JS:   // worker_threads 线程池
来源：http://hz.cashguo.top/gtdehaviuq.html

TS:   // worker_threads 线程池
来源：http://hz.hongshengwenyu.top/gtyjspqpiv.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hfpthk.cn/gtvmldqshi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shanyushiyangtech.top/gtshstvbnq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.tianlin.xyz/gtooalllle.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.sxryk.cn/gtqkdwxprc.html

[O03] 加锁保护共享数据
来源：http://hz.jqgfzy.top/gtwiqmsvcq.html

Py:   with lock: shared += 1
来源：http://hz.zycfv.cn/gtqnluxgnd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhongyouzk.top/gtzkylwnxh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yvedp.cn/gtchhwneqo.html

TS:   // 同 JS
来源：http://hz.fzhhl.top/gtefbehpvk.html

Java: synchronized (this) { shared++; }
来源：http://hz.sufxvd.cn/gtyoclopfd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhengqikj.top/gtznztppxs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.dashuyun.cn/gtkuyvorht.html

C#:   lock (gate) { shared++; }
来源：http://hz.hnqzz.top/gtvweejhqw.html

[O04] 定义异步函数并等待
来源：http://hz.c1oappe.top/gtkbdqdkha.html

Py:   async def f():⏎    await g()
来源：http://hz.zhengqikj.top/gtoyizlmtt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.pycfn.com/gtuwayamsq.html

JS:   async function f() { await g(); }
来源：http://hz.fengsongda.top/gtfiqrgqhk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.aibaodan.cn/gtsxcjbdon.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xylfe.cn/gtrmjnlwob.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhengqikj.top/gtxwsllcfx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.daxiang520.top/gtlniytrdo.html

C#:   async Task F() { await G(); }
来源：http://hz.hnqzz.top/gtgjfqudkc.html

[O05] 并发执行并等待全部完成
来源：http://hz.jyoumei.cn/gtaoonvstt.html

Py:   asyncio.gather(*tasks)
来源：http://hz.redwolf501.top/gtnatjgizt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jlsjyb.cn/gtvadpncqq.html

JS:   await Promise.all(tasks)
来源：http://hz.cdnleiting.top/gtyijckhno.html

TS:   await Promise.all(tasks)
来源：http://hz.jianghu66.top/gtezbmjygz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.dianchejie.cn/gtcuzbnwcz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yangfankeji.com/gtfoytpkya.html

Ruby: threads.map(&:join)
来源：http://hz.yonumen.top/gtgkwxtgpp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yonumen.top/gtyjrdymsy.html

[O06] 使用进程池
来源：http://hz.xuetiantiany.cn/gtusqkuywb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jianghu66.top/gtfsrxfswo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hnxiangtu.top/gtlcxntqrr.html

JS:   // child_process / cluster 模块
来源：http://hz.shanyushiyangkeji.top/gtfnylmilt.html

TS:   // child_process / cluster 模块
来源：http://hz.shanyushiyangkeji.top/gtjyajvuzn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jqgufenzy.top/gthsknskod.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhoulong.xyz/gtukrtvagl.html

Ruby: // fork 块
来源：http://hz.hongshengwenyu.top/gtqwpnhbqi.html

C#:   Parallel.For
来源：http://hz.nwbrower.top/gtdubrqcqf.html

================================================================================
来源：http://hz.jqgfzy.top/gtupoekptm.html

P. 常用工具函数
来源：http://hz.yuanzhike.top/gtnvjdwrhs.html

================================================================================
来源：http://hz.ybcxt.top/gtxogfofde.html

[P01] 生成 UUID
来源：http://hz.c1oappe.top/gtvhgbfdyt.html

Py:   str(uuid.uuid4())
来源：http://hz.svipenyu.cn/gtbwstghap.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hongshengwenyu.top/gtrvxheqxk.html

JS:   crypto.randomUUID()
来源：http://hz.cqqwz.cn/gtbgknkhnq.html

TS:   crypto.randomUUID()
来源：http://hz.hywenlv.cn/gtneqxeuii.html

Java: UUID.randomUUID().toString()
来源：http://hz.cqqwz.cn/gtntyljorw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xingfuxueyuan.xyz/gtsemqkvdz.html

Ruby: SecureRandom.uuid
来源：http://hz.birdmap.top/gtctgkerag.html


<!-- 参考信息 -->