代发 wailian999

TS:   resp.ok;  resp.status
来源：http://hz.fzhhl.top/gtlskydmzs.html

Java: resp.statusCode()
来源：http://hz.nanxuanxn.top/gttkaaupnu.html

Go:   resp.StatusCode
来源：http://hz.guowangkeji.top/gtduxaofml.html

Ruby: resp.code.to_i
来源：http://hz.aizwys.cn/gtttmuqqqw.html

C#:   (int)resp.StatusCode
来源：http://hz.cheryme.top/gtefanmnxa.html

[L08] 并发请求多个地址
来源：http://hz.vqdsnc.cn/gtigvadxug.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.andypj.xyz/gtuhahwxfw.html

PHP:  curl_multi_init() 系列
来源：http://hz.hammf.cn/gtbteapehc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cdnleiting.top/gtpleczqzd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shuidangran.top/gtkdalzlfh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zdqjudy.top/gtfwktupkf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tanke756.top/gtckjozxef.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.bjfxy.top/gtxanqatpf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cheryme.top/gtczivdvoc.html

================================================================================
来源：http://hz.gotoacloud.top/gtkwpkmgal.html

M. 命令行 / 进程 / 环境
来源：http://hz.meibo888.top/gtwvkcjahe.html

================================================================================
来源：http://hz.daxiang520.top/gtcrqzcsfm.html

[M01] 读取命令行参数
来源：http://hz.quarkkingdee.top/gtvipviavj.html

Py:   sys.argv[1:]
来源：http://hz.havefunace.top/gtjzdyvgsf.html

PHP:  $argv;  $argc;
来源：http://hz.wangdashe.top/gtlxgqsctx.html

JS:   process.argv.slice(2)
来源：http://hz.gaohongyu789.top/gtoksktpbf.html

TS:   process.argv.slice(2)
来源：http://hz.gogol.net.cn/gtxgipwdhh.html

Java: args 数组（main 方法参数）
来源：http://hz.hongshengwenyu.top/gtnxramseq.html

Go:   os.Args[1:]
来源：http://hz.gotoacloud.top/gtcaqrckxf.html

Ruby: ARGV
来源：http://hz.hnqzz.top/gtqfysfrnd.html

C#:   args 数组（Main 方法参数）
来源：http://hz.birdmap.top/gtwfvgsdfr.html

[M02] 读取环境变量
来源：http://hz.mhx1999.top/gtkgadfiqb.html

Py:   os.environ.get("HOME")
来源：http://hz.cdnleiting.top/gtochnbjmm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenzaomai.com/gtxakgqbdp.html

JS:   process.env.HOME
来源：http://hz.svipenyu.cn/gtvrmyncfj.html

TS:   process.env.HOME
来源：http://hz.snrcjt.cn/gthhmkldgo.html

Java: System.getenv("HOME")
来源：http://hz.zhaomingkeji.xyz/gtyjifrtos.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sxryk.cn/gtjixzjhxv.html

Ruby: ENV["HOME"]
来源：http://hz.havefunace.top/gtbpmrjyol.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xuetiantiany.cn/gtzvcbpilk.html

[M03] 执行外部命令
来源：http://hz.tanke756.top/gtkydvybif.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cashguo.top/gtakbdyfrl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.bjfxy.top/gtyomildfh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sufxvd.cn/gtxhgnqwrl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnqzz.top/gtwutxkaqy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinghuilouyu.cn/gtjsitwdqp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yueranfly.top/gtgfukfcdg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.tian-w.cn/gtxjncseva.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gaohongyu789.top/gtlyyxzego.html

[M04] 获取当前工作目录
来源：http://hz.aizwys.cn/gtiqbqntiu.html

Py:   os.getcwd()
来源：http://hz.nwbrower.top/gtlcoeujbq.html

PHP:  getcwd();
来源：http://hz.xylfe.cn/gtrxaxzrza.html

JS:   process.cwd()
来源：http://hz.guowangkeji.top/gtoepksctn.html

TS:   process.cwd()
来源：http://hz.zhongyouzk.top/gtsrtvdylh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.daria6918.cn/gtlcfrdegn.html

Go:   os.Getwd()
来源：http://hz.chenjidiqi.icu/gtrrirenlo.html

Ruby: Dir.pwd
来源：http://hz.ivvv.top/gthqkhufel.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.pengpengdd.cyou/gtafxeitrr.html

[M05] 设置退出码
来源：http://hz.zhoulong.xyz/gtxaanxxbu.html

Py:   sys.exit(1)
来源：http://hz.tian-w.cn/gtrkafatrs.html

PHP:  exit(1);
来源：http://hz.316326.xyz/gtjgnxrnng.html

JS:   process.exit(1)
来源：http://hz.dashuyun.cn/gtzplxsnyu.html

TS:   process.exit(1)
来源：http://hz.hnqzz.top/gthxqynjkz.html

Java: System.exit(1)
来源：http://hz.sweek.top/gtthpzolqn.html

Go:   os.Exit(1)
来源：http://hz.cashguo.top/gtarbiidfv.html

Ruby: exit 1
来源：http://hz.ivvv.top/gtuelantqp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.pycfn.com/gtuaqvdvko.html

[M06] 向标准错误输出
来源：http://hz.iojbl.cn/gttbnmocgy.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xingfuxueyuan.xyz/gtzvdprckl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zdqjudy.top/gthuomcwvr.html

JS:   console.error("err")
来源：http://hz.hysaishi.cn/gtbyhurxdi.html

TS:   console.error("err")
来源：http://hz.yj20258.top/gtnthwidki.html

Java: System.err.println("err")
来源：http://hz.52xcode.cn/gttqtccvzd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.smart0.xyz/gtxdjlgcri.html

Ruby: warn "err"
来源：http://hz.jqgfzy.top/gtcjkanxnl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.snrcjt.cn/gtaevixiux.html

[M07] 判断是否为主入口
来源：http://hz.daria6918.cn/gtorrzvkoc.html

Py:   if __name__ == "__main__":
来源：http://hz.daria6918.cn/gtrwgmyett.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhijiandao.cn/gtmcejvfxm.html

JS:   require.main === module
来源：http://hz.sysykeji.top/gtzbjcyrbo.html

TS:   require.main === module
来源：http://hz.jiagoushi.top/gtclubtbne.html

Java: public static void main(String[] args)
来源：http://hz.snrcjt.cn/gthtiezauo.html

Go:   func main()
来源：http://hz.hysaishi.cn/gtjztzbcmk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.pycfn.com/gtxyncuyin.html

C#:   static void Main(string[] args)
来源：http://hz.wangdashe.top/gteeudusio.html

[M08] 获取系统与运行时信息
来源：http://hz.tianlin.xyz/gtfyiidums.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gotoacloud.top/gtdxxtmtvr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cucudq.cn/gtilcovmii.html

JS:   process.platform;  process.version
来源：http://hz.jyoumei.cn/gttmrdqquf.html

TS:   process.platform;  process.version
来源：http://hz.jinyuanbaomall.cn/gtcaeecdup.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hywenlv.cn/gtlcpkugtd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jyoumei.cn/gtrziosfrn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.sweek.top/gtuzrmyvkg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yueranfly.top/gtjyewlvsc.html

================================================================================
来源：http://hz.daria6918.cn/gtzwfikbiq.html

N. 数据结构与算法
来源：http://hz.xylfe.cn/gtejcspsyj.html

================================================================================
来源：http://hz.0kj1m.cn/gtijdutyqt.html

[N01] 二分查找（有序数组）
来源：http://hz.0kj1m.cn/gtdfrpjizz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xylfe.cn/gtcxlspuhd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.snrcjt.cn/gtubgviwue.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daxiang520.top/gtzxbhzsdm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hammf.cn/gtiyhrlzmp.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.mhx1999.top/gthvmrsbhu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zdqjudy.top/gtloinzikm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.c1oappe.top/gtrnsrcvsv.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.havefunace.top/gtbyahfsko.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yj20258.top/gtvgvdfuwa.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sufxvd.cn/gtkjmhxgwi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ppjwa.cn/gtddiyrlrh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ivvv.top/gtsvcbpbtf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tianlin.xyz/gtlrwyydij.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.316326.xyz/gtmdzqveae.html

Go:   slices.Sort(arr)
来源：http://hz.jinyuanbaomall.cn/gtgjghpqdm.html

Ruby: arr.sort
来源：http://hz.yongpay.top/gtbogsiyap.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.dashuyun.cn/gtrnllssni.html

[N03] 快速排序（分治示例）
来源：http://hz.guowangkeji.top/gtpqrshqso.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.havefunace.top/gteymqahmn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yj20258.top/gtgxieaeas.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhaomingkeji.xyz/gtzuaoswll.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yonumen.top/gtfrjmnunp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tanke756.top/gthapprwse.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jianghu66.top/gtbqneskgg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sweek.top/gtqyhbzqyl.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.52xcode.cn/gtfbihnqxc.html

[N04] 斐波那契数列
来源：http://hz.jyoumei.cn/gtyhdgdvey.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.aibaodan.cn/gtjbzxramj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.gotoacloud.top/gtybfrzkpx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gtztrpatcb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ybcxt.top/gtncthfsfy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhijiandao.cn/gtaapyzzuw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gogol.net.cn/gthwewezsy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cucudq.cn/gtgzakqlye.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.aibaodan.cn/gtbbrafrzi.html

[N05] 最大公约数
来源：http://hz.yangfankeji.com/gtdastaxsk.html

Py:   math.gcd(a, b)
来源：http://hz.haohaochexian.top/gtmsssgzry.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.wangshuangyany.cn/gtxxsvkgrm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.kuanghao11.cn/gtjmxddvpi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.havefunace.top/gtcmumuwtl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.tian-w.cn/gtrebxjvsg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhengqikj.top/gtkgqmwfmc.html

Ruby: a.gcd(b)
来源：http://hz.nanxinkj.top/gttjrxjqyz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xingfuxueyuan.xyz/gtivcgmdia.html

[N06] 判断回文字符串
来源：http://hz.sysykeji.top/gtnwktsdyf.html

Py:   s == s[::-1]
来源：http://hz.redwolf501.top/gtdiyzngzo.html

PHP:  $s === strrev($s);
来源：http://hz.svipenyu.cn/gtjpmsazwm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.guannengcc.top/gtvaibuyes.html

TS:   s === [...s].reverse().join("")
来源：http://hz.pycfn.com/gtbfhihyvy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhengqikj.top/gtcdnspzra.html

Go:   // 双指针从两端比较
来源：http://hz.gaohongyu789.top/gtloizjuld.html

Ruby: s == s.reverse
来源：http://hz.chenjidiqi.icu/gtvdzuqrsy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yanxiufei.cn/gtcbtenfeg.html

[N07] 两数之和（返回下标）
来源：http://hz.cqqwz.cn/gtuolzfwvc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xziqi.cn/gtgsayiebp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.bjfxy.top/gtazvfvpfw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nwbrower.top/gtkujivtbx.html

TS:   // 手写 Map<string, number>
来源：http://hz.ywan-chungtsiang.top/gtxuxqjinv.html

Java: // 手写 HashMap
来源：http://hz.zhoulong.xyz/gtrdrirxjo.html

Go:   // 手写 map[int]int
来源：http://hz.andypj.xyz/gtdnfqifbw.html

Ruby: // 手写 Hash
来源：http://hz.0kj1m.cn/gtiirjewkh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.316326.xyz/gtoysgkifm.html

[N08] 生成全排列
来源：http://hz.jqgufenzy.top/gtivqotavo.html

Py:   itertools.permutations(arr)
来源：http://hz.ywan-chungtsiang.top/gtiygauold.html

PHP:  // 手写递归交换
来源：http://hz.zhongyouzk.top/gtgmnfieck.html

JS:   // 手写回溯递归
来源：http://hz.cheryme.top/gtreuwegpi.html

TS:   // 手写回溯递归
来源：http://hz.yuxming.cn/gtmemsxzwr.html

Java: // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtioajslpv.html

Go:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtslxwgdhp.html

Ruby: arr.permutation.to_a
来源：http://hz.vqdsnc.cn/gtcqigrxef.html

C#:   // 手写回溯递归
来源：http://hz.meibo888.top/gtmnyqehip.html

[N09] 栈与队列
来源：http://hz.tanke756.top/gtahmlkmvt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.aibaodan.cn/gthwmifrhz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hysaishi.cn/gtmvyoidcp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ybcxt.top/gtyojcvonb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.fengsongda.top/gtalbzotfe.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xziqi.cn/gtqvgvvntv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tian-w.cn/gtcoazglfl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.9152youxi.cn/gtivawiyvx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.0kj1m.cn/gtzcyfftvz.html

[N10] 链表节点定义
来源：http://hz.guowangkeji.top/gtbxuaupos.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hywenlv.cn/gtpxufzojb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jlsjyb.cn/gtbxyvlbls.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.mhx1999.top/gthslebonb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.meibo888.top/gtuowrnhol.html

Java: class Node { int v; Node next; }
来源：http://hz.haohaochexian.top/gtqifamckc.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jiagoushi.top/gtwzfqglev.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.gzhubu.top/gtedcgjvce.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.pycfn.com/gtnbdwukcg.html

[N11] 二叉树中序遍历
来源：http://hz.chenjidiqi.icu/gtpfajfcex.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhengqikj.top/gtkcdkrefn.html

PHP:  // 手写递归函数
来源：http://hz.jinghuilouyu.cn/gtfxurwibw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xylfe.cn/gtvyevpuve.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnqzz.top/gtpbymxpza.html

Java: // 手写递归
来源：http://hz.yonumen.top/gtufhaytow.html

Go:   // 手写递归
来源：http://hz.yongpay.top/gtoksumido.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.sweek.top/gtmuxaxbas.html

C#:   // 手写递归
来源：http://hz.yj202588.top/gtzeuatmof.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.316326.xyz/gtjekaypkr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ybcxt.top/gtvmusgxcr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.guannengcc.top/gtexdzpjnr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cdnleiting.top/gtrupuuxhu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gogol.net.cn/gtjbqziver.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.aibaodan.cn/gtpculjulf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.vqdsnc.cn/gtqjahlxsx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sysykeji.top/gtxsthgust.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.aibaodan.cn/gtuqjeexul.html

================================================================================
来源：http://hz.gzhubu.top/gtlbrenwkk.html

O. 并发与异步
来源：http://hz.52xcode.cn/gtlbhfmket.html

================================================================================
来源：http://hz.aizwys.cn/gtmlfjfyjl.html

[O01] 启动一个线程
来源：http://hz.yuxming.cn/gtlpveetol.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.wangdashe.top/gtanwpimvs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cheryme.top/gtaaeewvzb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhaomingkeji.xyz/gtbtwsfylv.html

TS:   // 同 JS
来源：http://hz.daxiang520.top/gtangfiltz.html

Java: new Thread(() -> f()).start()
来源：http://hz.jlsjyb.cn/gtvlnopbru.html

Go:   go f()
来源：http://hz.zhongyouzk.top/gtvztuqwqw.html

Ruby: Thread.new { f }
来源：http://hz.jinqigfzy.top/gtuyjfvfvf.html

C#:   Task.Run(() => F());
来源：http://hz.zhoulong.xyz/gthpdnvwsh.html

[O02] 使用线程池
来源：http://hz.sweek.top/gtjwrwvkmr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.daxiang520.top/gtamqbtluj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ywan-chungtsiang.top/gtgmscnsqp.html

JS:   // worker_threads 线程池
来源：http://hz.smart0.xyz/gttkpfezao.html

TS:   // worker_threads 线程池
来源：http://hz.kuanghao11.cn/gtdbigmgwl.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.daria6918.cn/gtyeovpket.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.birdmap.top/gtpqzhtmbv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yvedp.cn/gtifszwtvv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yueranfly.top/gtlxyylhll.html

[O03] 加锁保护共享数据
来源：http://hz.jinghuilouyu.cn/gthupqgngb.html

Py:   with lock: shared += 1
来源：http://hz.zhaomingkeji.xyz/gtsozsyiew.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.nwbrower.top/gtssybpwcb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.andypj.xyz/gtddkybvpt.html

TS:   // 同 JS
来源：http://hz.pycfn.com/gtgrvehwxf.html

Java: synchronized (this) { shared++; }
来源：http://hz.jyoumei.cn/gtujenyzic.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yvedp.cn/gtmjozqkdh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.316326.xyz/gtsrrxmina.html

C#:   lock (gate) { shared++; }
来源：http://hz.andypj.xyz/gtcgkokytf.html

[O04] 定义异步函数并等待
来源：http://hz.gaohongyu789.top/gtucxwmpvy.html

Py:   async def f():⏎    await g()
来源：http://hz.wangshuangyany.cn/gtleyywxgw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.pengpengdd.cyou/gtnnnapatf.html

JS:   async function f() { await g(); }
来源：http://hz.xinyue.icu/gtncbotzqa.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ppjwa.cn/gtayyiykkn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.dianchejie.cn/gtlbwluxfa.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yonumen.top/gtmiuxxofp.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.daria6918.cn/gtbwnkmdqs.html

C#:   async Task F() { await G(); }
来源：http://hz.wangshuangyany.cn/gtteqayjut.html

[O05] 并发执行并等待全部完成
来源：http://hz.zycfv.cn/gtopbcsrqb.html

Py:   asyncio.gather(*tasks)
来源：http://hz.daria6918.cn/gtwedscfzj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zdqjudy.top/gtzbnhqzag.html

JS:   await Promise.all(tasks)
来源：http://hz.gaohongyu789.top/gthimmlgoi.html

TS:   await Promise.all(tasks)
来源：http://hz.dashuyun.cn/gtughqtnaq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.pycfn.com/gtacnesbhy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hfpthk.cn/gthmmdakau.html

Ruby: threads.map(&:join)
来源：http://hz.vqdsnc.cn/gtujzjqmwb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.nwbrower.top/gtcnmldyyq.html

[O06] 使用进程池
来源：http://hz.ehwqpu.com/gtleclqmgl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ydzc1.top/gtimtlgcel.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shuidangran.top/gtcjpyuaeg.html

JS:   // child_process / cluster 模块
来源：http://hz.feifeiyinyue.top/gtfkrfhhuo.html

TS:   // child_process / cluster 模块
来源：http://hz.xuetiantiany.cn/gtizteaixr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.dianchejie.cn/gtirduoiyf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shuidangran.top/gthgbajdky.html

Ruby: // fork 块
来源：http://hz.andypj.xyz/gttnigpkta.html

C#:   Parallel.For
来源：http://hz.xziqi.cn/gtibcyssmb.html

================================================================================
来源：http://hz.jqgufenzy.top/gtfxjjbbul.html

P. 常用工具函数
来源：http://hz.316326.xyz/gteiignozk.html

================================================================================
来源：http://hz.guannengcc.top/gtpmgidajd.html

[P01] 生成 UUID
来源：http://hz.yanxiufei.cn/gtpcfhyhiq.html

Py:   str(uuid.uuid4())
来源：http://hz.0kj1m.cn/gtpuexdgog.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.wangdashe.top/gthekyysoe.html

JS:   crypto.randomUUID()
来源：http://hz.xinyue.icu/gtyfmykljs.html

TS:   crypto.randomUUID()
来源：http://hz.fengsongda.top/gtarytlcyw.html

Java: UUID.randomUUID().toString()
来源：http://hz.hongshengwenyu.top/gtsrnxfwfr.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhixingplan.top/gtemxieeyx.html

Ruby: SecureRandom.uuid
来源：http://hz.ydzc1.top/gtybvvxxpu.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ehwqpu.com/gtjdxnjylr.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinghuilouyu.cn/gtirfakkhw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.aizwys.cn/gtvlsjqksa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.aibaodan.cn/gtpskdbkhn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinqigfzy.top/gtrftecqnt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shangyingyoupin.top/gtitolcckr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jqgufenzy.top/gtiuovakcd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gotoacloud.top/gtzuauviqj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.fengsongda.top/gteyvbirri.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhijiandao.cn/gtjbhgcqls.html

[P03] 生成短随机字符串
来源：http://hz.dianchejie.cn/gtkovsxjel.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shanyushiyangtech.top/gtjdfbmndg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hysaishi.cn/gtmcwmsczg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj202588.top/gtwrcgdfca.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.52xcode.cn/gtgguxwmbg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhoulong.xyz/gtkywhkars.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.feifeiyinyue.top/gtlytkhrkl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.pycfn.com/gtkzcjkndk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yanxiufei.cn/gtbiuspqle.html

[P04] 求长度
来源：http://hz.nanxuanxn.top/gtmbgsgolf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.sweek.top/gtjewrdpob.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gaohongyu789.top/gtlpuozwrb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhiwuduotai.top/gtbydcaogw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinqigfzy.top/gtiqhbeahr.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhijiandao.cn/gtnjwsmbyz.html

Go:   len(arr);  len(m)
来源：http://hz.chenzaomai.com/gtbuvvhyla.html

Ruby: x.length;  x.size
来源：http://hz.yanxiufei.cn/gtgqrlunup.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gogol.net.cn/gtqsyllwea.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shanyushiyangkeji.top/gtuooormxp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jqgufenzy.top/gtlyaczaga.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ywan-chungtsiang.top/gtqijvhctx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.52xcode.cn/gtsxemfjge.html


<!-- 参考信息 -->