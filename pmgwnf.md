代发 wailian999

[L03] 设置自定义请求头
来源：http://hz.hnxiangtu.top/gtnuyfdvnl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.fengsongda.top/gtbrlsdbcx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shanyushiyangkeji.top/gtaiqexqok.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuetiantiany.cn/gtzttufude.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.vqdsnc.cn/gtbsrivjun.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhaomingkeji.xyz/gtnwchiesp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.haohaochexian.top/gtbmlihofi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jyoumei.cn/gthvxcbkqf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xinyue.icu/gtimgbmdso.html

[L04] 设置超时
来源：http://hz.yuxming.cn/gtmwtmswvz.html

Py:   requests.get(url, timeout=5)
来源：http://hz.nwbrower.top/gtolwithit.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xziqi.cn/gtdvgwhsai.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sxryk.cn/gttxccprtu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hammf.cn/gtbhqcsbte.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xuetiantiany.cn/gtptajdynk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jqgufenzy.top/gtikdxmcrz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.guannengcc.top/gtqrakqsvb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gotoacloud.top/gtgcjyvpyp.html

[L05] 上传文件（multipart）
来源：http://hz.redwolf501.top/gttgfwrzno.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xuanzx.com/gtunekkevr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jyoumei.cn/gtnsnrzzbe.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.gzhubu.top/gttjrpmeov.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jianghu66.top/gtxyyqenag.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.bjfxy.top/gtddzsbzsg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.guannengcc.top/gtsrxkhyho.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinyuanbaomall.cn/gtztxsctyx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.svipenyu.cn/gttqwhrwcu.html

[L06] 解析响应为 JSON
来源：http://hz.hfpthk.cn/gtjeiagjzg.html

Py:   resp.json()
来源：http://hz.guowangkeji.top/gtlptcarfn.html

PHP:  json_decode($body, true);
来源：http://hz.aibaodan.cn/gtrvxinfww.html

JS:   await resp.json()
来源：http://hz.shuidangran.top/gtfotwjpzy.html

TS:   await resp.json()
来源：http://hz.chenlongwang.top/gtsrbqkqcv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nanxinkj.top/gtfjlnzeiv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jiagoushi.top/gtlakkhvsy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ywan-chungtsiang.top/gtebfkvelv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cdnleiting.top/gtdnovmpid.html

[L07] 处理 HTTP 状态码
来源：http://hz.chenlongwang.top/gtvqayjqee.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.dianchejie.cn/gtdxywgwrc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shzxlz.cn/gtqghovjxj.html

JS:   resp.ok;  resp.status
来源：http://hz.jiagoushi.top/gtssbzzjtt.html

TS:   resp.ok;  resp.status
来源：http://hz.jyoumei.cn/gtrvttgzxc.html

Java: resp.statusCode()
来源：http://hz.yonumen.top/gttebpqdda.html

Go:   resp.StatusCode
来源：http://hz.shzxlz.cn/gtzqyvodfm.html

Ruby: resp.code.to_i
来源：http://hz.chenjidiqi.icu/gtlymyksxe.html

C#:   (int)resp.StatusCode
来源：http://hz.ehwqpu.com/gtvhadafuc.html

[L08] 并发请求多个地址
来源：http://hz.daxiang520.top/gtwqdqikzs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.quarkkingdee.top/gtxokntdwv.html

PHP:  curl_multi_init() 系列
来源：http://hz.jiagoushi.top/gtiqvnkmrd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxuanxn.top/gtrfeumvys.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aizwys.cn/gtrdeybuwk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.bjfxy.top/gtguyxovht.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yuanzhike.top/gtibpvgdpd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.c1oappe.top/gtumhtvxrs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yueranfly.top/gtksryksiu.html

================================================================================
来源：http://hz.meibo888.top/gtkqhhabnt.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhongyouzk.top/gtzckmlkrq.html

================================================================================
来源：http://hz.nanxuanxn.top/gtbxjsjrnd.html

[M01] 读取命令行参数
来源：http://hz.zycfv.cn/gtrohnygci.html

Py:   sys.argv[1:]
来源：http://hz.ydjk.org.cn/gtggqtryff.html

PHP:  $argv;  $argc;
来源：http://hz.ydzc1.top/gtuqdlrhlb.html

JS:   process.argv.slice(2)
来源：http://hz.zhengqikj.top/gtgccyumqj.html

TS:   process.argv.slice(2)
来源：http://hz.hywenlv.cn/gtkcuigywo.html

Java: args 数组（main 方法参数）
来源：http://hz.ydzc1.top/gtqpcxokaw.html

Go:   os.Args[1:]
来源：http://hz.zhaomingkeji.xyz/gtpasdphyr.html

Ruby: ARGV
来源：http://hz.jiagoushi.top/gtnvowvrdn.html

C#:   args 数组（Main 方法参数）
来源：http://hz.9152youxi.cn/gtviwzfkxp.html

[M02] 读取环境变量
来源：http://hz.yj20258.top/gtfxstvfra.html

Py:   os.environ.get("HOME")
来源：http://hz.yuxming.cn/gtlwfvfoxl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.0kj1m.cn/gtkkficfxb.html

JS:   process.env.HOME
来源：http://hz.tianlin.xyz/gtpgmxnzzf.html

TS:   process.env.HOME
来源：http://hz.tian-w.cn/gtcfsktezv.html

Java: System.getenv("HOME")
来源：http://hz.cheryme.top/gtwvahkxoh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cqqwz.cn/gtzwwrvdau.html

Ruby: ENV["HOME"]
来源：http://hz.yvedp.cn/gtnpqdqmdy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xuetiantiany.cn/gtkwvqogza.html

[M03] 执行外部命令
来源：http://hz.jianghu66.top/gtuprvimno.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.redwolf501.top/gtlfzmsckq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yanxiufei.cn/gtevvjqhun.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ivvv.top/gtjltffiph.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ybcxt.top/gtvmbjwivi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.meibo888.top/gtafflthsc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jyoumei.cn/gtjzkgqntk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.chenzaomai.com/gtbsqclwip.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhiwuduotai.top/gtriujyfii.html

[M04] 获取当前工作目录
来源：http://hz.feifeiyinyue.top/gtbmitnxwp.html

Py:   os.getcwd()
来源：http://hz.yueranfly.top/gtwlminaom.html

PHP:  getcwd();
来源：http://hz.jinqigufen.top/gtlwlqvrek.html

JS:   process.cwd()
来源：http://hz.yonumen.top/gtwhficjkc.html

TS:   process.cwd()
来源：http://hz.dianchejie.cn/gtuqnpnmvk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinyuanbaomall.cn/gtkrxeatsa.html

Go:   os.Getwd()
来源：http://hz.ivvv.top/gtzhxopbfm.html

Ruby: Dir.pwd
来源：http://hz.gaohongyu789.top/gthlhmuozg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.tian-w.cn/gtbyjoxupl.html

[M05] 设置退出码
来源：http://hz.xingfuxueyuan.xyz/gticpeadtb.html

Py:   sys.exit(1)
来源：http://hz.cdnleiting.top/gtbvttwgra.html

PHP:  exit(1);
来源：http://hz.yuanzhike.top/gtozizhxqn.html

JS:   process.exit(1)
来源：http://hz.shzxlz.cn/gtyremknhj.html

TS:   process.exit(1)
来源：http://hz.yj20258.top/gtahceslek.html

Java: System.exit(1)
来源：http://hz.vqdsnc.cn/gtykbaszbr.html

Go:   os.Exit(1)
来源：http://hz.cheryme.top/gtdbnboxsy.html

Ruby: exit 1
来源：http://hz.gzhubu.top/gtzykftcxa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.dashuyun.cn/gtvcejpdod.html

[M06] 向标准错误输出
来源：http://hz.zhongyouzk.top/gtxrmeyfth.html

Py:   print("err", file=sys.stderr)
来源：http://hz.tianlin.xyz/gtlbrcbale.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.iojbl.cn/gtcuixoput.html

JS:   console.error("err")
来源：http://hz.aibaodan.cn/gtmimrvxjm.html

TS:   console.error("err")
来源：http://hz.aibaodan.cn/gteuhjzoet.html

Java: System.err.println("err")
来源：http://hz.yj20258888.top/gtgnxbzwqv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.chenjidiqi.icu/gtszyacswf.html

Ruby: warn "err"
来源：http://hz.daxiang520.top/gtmnsdumhh.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xinyue.icu/gtigpzkskd.html

[M07] 判断是否为主入口
来源：http://hz.redwolf501.top/gtessowmdv.html

Py:   if __name__ == "__main__":
来源：http://hz.andypj.xyz/gtzojntndg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhijiandao.cn/gtacozqknn.html

JS:   require.main === module
来源：http://hz.cdnleiting.top/gtcsndpwcw.html

TS:   require.main === module
来源：http://hz.cqqwz.cn/gtcdsqpvjd.html

Java: public static void main(String[] args)
来源：http://hz.sysykeji.top/gtwrpauagk.html

Go:   func main()
来源：http://hz.jqgfzy.top/gtjtjgscel.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.haohaochexian.top/gtweshkmtw.html

C#:   static void Main(string[] args)
来源：http://hz.dashuyun.cn/gtikepynec.html

[M08] 获取系统与运行时信息
来源：http://hz.smart0.xyz/gtqfgcvjab.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shuidangran.top/gtajkjbryl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.52xcode.cn/gtqgppcosw.html

JS:   process.platform;  process.version
来源：http://hz.sweek.top/gtapjyxstd.html

TS:   process.platform;  process.version
来源：http://hz.yj20258888.top/gteevdrwnh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.smart0.xyz/gtrnhbjadx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cashguo.top/gtnieijust.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.meibo888.top/gtdrzshlid.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.aizwys.cn/gtdjdhwhzd.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtgiyyfurt.html

N. 数据结构与算法
来源：http://hz.pycfn.com/gtwolajiww.html

================================================================================
来源：http://hz.ydjk.org.cn/gtgxwmnddt.html

[N01] 二分查找（有序数组）
来源：http://hz.zhixingplan.top/gtyvgocxnw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xylfe.cn/gtspotcvor.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.daria6918.cn/gtfzwbqumz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ybcxt.top/gtjgnlvzkl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenjidiqi.icu/gtwlvcbhpq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.kuanghao11.cn/gtcvmrtary.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.nanxinkj.top/gtckicxxtg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hysaishi.cn/gtuvlwlgtk.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhijiandao.cn/gtghkvusul.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.pycfn.com/gtxsujdhhk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cqqwz.cn/gtfnovniqs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hammf.cn/gtoxbfridq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.kuanghao11.cn/gttycgtugz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xinyue.icu/gtchracxoo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ehwqpu.com/gtmgvaokli.html

Go:   slices.Sort(arr)
来源：http://hz.kuanghao11.cn/gtclpotqqy.html

Ruby: arr.sort
来源：http://hz.zhixingplan.top/gtgvzxgxmz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ydjk.org.cn/gtmuqswikz.html

[N03] 快速排序（分治示例）
来源：http://hz.cdnleiting.top/gtvzjoioax.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinyuanbaomall.cn/gtmuxfkafm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gaohongyu789.top/gtizxbfelj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhixingplan.top/gtnaohlvum.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guowangkeji.top/gtxbhkxcbu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinyuanbaomall.cn/gtmnglafed.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhixingplan.top/gtedvjbdql.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.aibaodan.cn/gtfxulnpvo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jqgufenzy.top/gtuocgjdjl.html

[N04] 斐波那契数列
来源：http://hz.sysykeji.top/gtovzjbryq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jqgfzy.top/gtrjczkfqj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yueranfly.top/gtrpexdhxp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ppjwa.cn/gtgiilfvxt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fengsongda.top/gtdejlxpma.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.tianlin.xyz/gtyeeeaals.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.chenlongwang.top/gtamfbjzrp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.nanxuanxn.top/gtwldoosje.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sufxvd.cn/gtjmmzybqq.html

[N05] 最大公约数
来源：http://hz.gzhubu.top/gtzzdrihgo.html

Py:   math.gcd(a, b)
来源：http://hz.quarkkingdee.top/gtoqlleijp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xuetiantiany.cn/gtrqymzpju.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydzc1.top/gtahiycqiy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangkeji.top/gtmhdbmpqd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.redwolf501.top/gtoslcejtp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cashguo.top/gtacphgjew.html

Ruby: a.gcd(b)
来源：http://hz.smart0.xyz/gtwopsskjl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shzxlz.cn/gtvnthdphu.html

[N06] 判断回文字符串
来源：http://hz.pengpengdd.cyou/gtucsjnjfl.html

Py:   s == s[::-1]
来源：http://hz.zhixingplan.top/gthwhdubne.html

PHP:  $s === strrev($s);
来源：http://hz.nanxuanxn.top/gtdknflgpq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yonumen.top/gtjkdwimru.html

TS:   s === [...s].reverse().join("")
来源：http://hz.wangshuangyany.cn/gtfkrmzlbb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.chenjidiqi.icu/gtrzzlzclr.html

Go:   // 双指针从两端比较
来源：http://hz.zhaomingkeji.xyz/gtcgtvtsff.html

Ruby: s == s.reverse
来源：http://hz.sweek.top/gtoavcrbum.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhongyouzk.top/gtmxdhxebd.html

[N07] 两数之和（返回下标）
来源：http://hz.xingfuxueyuan.xyz/gttbbtggam.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.redwolf501.top/gtqiiolulo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.smart0.xyz/gtcjatbpgw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ppjwa.cn/gtsnhskfpq.html

TS:   // 手写 Map<string, number>
来源：http://hz.hongshengwenyu.top/gtkqxegqno.html

Java: // 手写 HashMap
来源：http://hz.aibaodan.cn/gtlunmmilz.html

Go:   // 手写 map[int]int
来源：http://hz.cqqwz.cn/gtcjatpvxt.html

Ruby: // 手写 Hash
来源：http://hz.sufxvd.cn/gtoexkaojl.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hnxiangtu.top/gtrcummtkb.html

[N08] 生成全排列
来源：http://hz.haohaochexian.top/gtqovlbafd.html

Py:   itertools.permutations(arr)
来源：http://hz.chenlongwang.top/gtrvotxcnt.html

PHP:  // 手写递归交换
来源：http://hz.sysykeji.top/gtuiucbiky.html

JS:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gtmjqrxlar.html

TS:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtixmmcext.html

Java: // 手写回溯递归
来源：http://hz.jqgfzy.top/gthozkldtg.html

Go:   // 手写回溯递归
来源：http://hz.sweek.top/gtnivrwpim.html

Ruby: arr.permutation.to_a
来源：http://hz.jianghu66.top/gtcjjywcwc.html

C#:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtdsmtjitc.html

[N09] 栈与队列
来源：http://hz.snrcjt.cn/gtwpqttopa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xingfuxueyuan.xyz/gtvrmbxjbl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yueranfly.top/gtnaqcfzaz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.birdmap.top/gtdlenpian.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.9152youxi.cn/gtvptvqjzv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.nanxinkj.top/gtsbwbyrhb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gotoacloud.top/gtqjeptbkw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.gotoacloud.top/gtpyjwsteo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.chenjidiqi.icu/gtgkvudaif.html

[N10] 链表节点定义
来源：http://hz.fengsongda.top/gtoponghar.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yj20258.top/gtsnfukech.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhengqikj.top/gtomggoswy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj20258888.top/gtnbkpjjvg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.andypj.xyz/gtiqlfnjun.html

Java: class Node { int v; Node next; }
来源：http://hz.yj202588.top/gtlhcytjdx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gotoacloud.top/gtiorrrabp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.vqdsnc.cn/gtfnqvlqot.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jlsjyb.cn/gtmrnnjlwd.html

[N11] 二叉树中序遍历
来源：http://hz.zycfv.cn/gtakwqtezx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.fzhhl.top/gtavnglsse.html

PHP:  // 手写递归函数
来源：http://hz.pengpengdd.cyou/gtcxdvhfyc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jyoumei.cn/gtlmazfcqv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxinkj.top/gtjeffaxjn.html

Java: // 手写递归
来源：http://hz.tanke756.top/gthaanphfn.html

Go:   // 手写递归
来源：http://hz.gotoacloud.top/gtsrlktxls.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yuxming.cn/gtedgpyyef.html

C#:   // 手写递归
来源：http://hz.hammf.cn/gtnooccwnf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yj20258888.top/gtfwhlsgwr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.gotoacloud.top/gtmgrswtku.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhoulong.xyz/gttdliearn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sufxvd.cn/gtdmktujkz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gotoacloud.top/gtufwkveel.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gtplsteocw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ppjwa.cn/gtwnzlfubf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.svipenyu.cn/gtlcpeivbz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.svipenyu.cn/gtrmhlsnzm.html

================================================================================
来源：http://hz.yuxming.cn/gtkubwhpaa.html

O. 并发与异步
来源：http://hz.gaohongyu789.top/gtwzvzrzbr.html

================================================================================
来源：http://hz.zycfv.cn/gtokvpvppp.html

[O01] 启动一个线程
来源：http://hz.yuxming.cn/gtwfzdzhtn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yj202588.top/gtsbmdmkde.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.haohaochexian.top/gttdcxuwbt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenzaomai.com/gtfamrvopw.html

TS:   // 同 JS
来源：http://hz.ivvv.top/gtsxhieoqo.html

Java: new Thread(() -> f()).start()
来源：http://hz.havefunace.top/gtcfmgzbny.html

Go:   go f()
来源：http://hz.tian-w.cn/gtalswxrci.html

Ruby: Thread.new { f }
来源：http://hz.daria6918.cn/gtlpqqdydc.html

C#:   Task.Run(() => F());
来源：http://hz.yj20258.top/gtfzrievyl.html

[O02] 使用线程池
来源：http://hz.zhijiandao.cn/gtksfcmkkc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cucudq.cn/gtxvopkguv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.fzhhl.top/gtjhzhxeaf.html

JS:   // worker_threads 线程池
来源：http://hz.hywenlv.cn/gtplhbbjno.html

TS:   // worker_threads 线程池
来源：http://hz.shuidangran.top/gtezhcuzyp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ppjwa.cn/gtocabnvnv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.snrcjt.cn/gtkoybhjnn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cdnleiting.top/gtjvyzadns.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinqigufen.top/gtrshsjrxw.html

[O03] 加锁保护共享数据
来源：http://hz.pengpengdd.cyou/gtwtoauzjf.html

Py:   with lock: shared += 1
来源：http://hz.zdqjudy.top/gtynvedetm.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hongshengwenyu.top/gtszacgwjz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gogol.net.cn/gtckbbelkp.html

TS:   // 同 JS
来源：http://hz.yonumen.top/gtcxjnbmat.html

Java: synchronized (this) { shared++; }
来源：http://hz.jqgfzy.top/gtdhgnuqji.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.dianchejie.cn/gttnrgpvgk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yonumen.top/gtxriylril.html

C#:   lock (gate) { shared++; }
来源：http://hz.shzxlz.cn/gthbjqrxlw.html

[O04] 定义异步函数并等待
来源：http://hz.aizwys.cn/gtwfilnbft.html

Py:   async def f():⏎    await g()
来源：http://hz.nanxinkj.top/gtvyqgjcvy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zycfv.cn/gtwidltaui.html

JS:   async function f() { await g(); }
来源：http://hz.smart0.xyz/gtuceswmzw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shuidangran.top/gtplzvojvm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.guannengcc.top/gtqzdzzzfv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hysaishi.cn/gtqcxmfiot.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yj20258.top/gtspurpmdn.html

C#:   async Task F() { await G(); }
来源：http://hz.chenlongwang.top/gtvgmwbyuq.html

[O05] 并发执行并等待全部完成
来源：http://hz.hywenlv.cn/gtrkbxubku.html

Py:   asyncio.gather(*tasks)
来源：http://hz.nwbrower.top/gtwxzioxts.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xinyue.icu/gtpkkizkgg.html

JS:   await Promise.all(tasks)
来源：http://hz.yj202588.top/gtxgxkrqro.html

TS:   await Promise.all(tasks)
来源：http://hz.jinghuilouyu.cn/gtmxhbbegp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.snrcjt.cn/gthowhdawc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jinqigufen.top/gtncnmkgca.html

Ruby: threads.map(&:join)
来源：http://hz.zdqjudy.top/gtzbgfgewt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ppjwa.cn/gtmmozgfzh.html

[O06] 使用进程池
来源：http://hz.gotoacloud.top/gtvnbwlhuk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.dashuyun.cn/gtgivyyksf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yj202588.top/gtlsqiofsg.html

JS:   // child_process / cluster 模块
来源：http://hz.shzxlz.cn/gtwxzieqxx.html

TS:   // child_process / cluster 模块
来源：http://hz.daxiang520.top/gtpsmtgyba.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.shangyingyoupin.top/gtfksxdbrp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.tian-w.cn/gtbxrtxfdt.html

Ruby: // fork 块
来源：http://hz.cucudq.cn/gthnydasst.html

C#:   Parallel.For
来源：http://hz.jlsjyb.cn/gtknymiijd.html

================================================================================
来源：http://hz.daria6918.cn/gtzidtdveg.html

P. 常用工具函数
来源：http://hz.haohaochexian.top/gtcultfrbq.html

================================================================================
来源：http://hz.jinqigfzy.top/gtozhrvzos.html


<!-- 参考信息 -->