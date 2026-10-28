代发 wailian999

TS:   resp.ok;  resp.status
来源：http://hz.nanxuanxn.top/gtjzmdbgcy.html

Java: resp.statusCode()
来源：http://hz.xuetiantiany.cn/gtaztubsrz.html

Go:   resp.StatusCode
来源：http://hz.chenzaomai.com/gtxzghnlbi.html

Ruby: resp.code.to_i
来源：http://hz.nanxuanxn.top/gtdqsddxkl.html

C#:   (int)resp.StatusCode
来源：http://hz.sysykeji.top/gtpvdhatim.html

[L08] 并发请求多个地址
来源：http://hz.aizwys.cn/gtxqogizyr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xziqi.cn/gtvmvqajbd.html

PHP:  curl_multi_init() 系列
来源：http://hz.birdmap.top/gtaqhpnktl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hammf.cn/gtykiyralu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daria6918.cn/gtjopljzus.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gogol.net.cn/gtjsnjhtpw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.meibo888.top/gtsrcakbdg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.gogol.net.cn/gttziwolta.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.andypj.xyz/gtszlvpizd.html

================================================================================
来源：http://hz.redwolf501.top/gtpiztzloj.html

M. 命令行 / 进程 / 环境
来源：http://hz.birdmap.top/gtwfowauig.html

================================================================================
来源：http://hz.sweek.top/gtzjsxztle.html

[M01] 读取命令行参数
来源：http://hz.jinqigfzy.top/gthkkuijes.html

Py:   sys.argv[1:]
来源：http://hz.yuxming.cn/gttvolfjco.html

PHP:  $argv;  $argc;
来源：http://hz.andypj.xyz/gtzcxzffyv.html

JS:   process.argv.slice(2)
来源：http://hz.hywenlv.cn/gtfadyvctn.html

TS:   process.argv.slice(2)
来源：http://hz.redwolf501.top/gturfrsmhy.html

Java: args 数组（main 方法参数）
来源：http://hz.9152youxi.cn/gttpkckxcp.html

Go:   os.Args[1:]
来源：http://hz.ehwqpu.com/gtpecnvjoo.html

Ruby: ARGV
来源：http://hz.c1oappe.top/gtfeobabzj.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhixingplan.top/gtswhqjfia.html

[M02] 读取环境变量
来源：http://hz.jinghuilouyu.cn/gtnsuqtcsm.html

Py:   os.environ.get("HOME")
来源：http://hz.svipenyu.cn/gtoaqapgkd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.daxiang520.top/gtksyipure.html

JS:   process.env.HOME
来源：http://hz.yangfankeji.com/gtmbrwdsek.html

TS:   process.env.HOME
来源：http://hz.ppjwa.cn/gtyuelymgs.html

Java: System.getenv("HOME")
来源：http://hz.jqgufenzy.top/gtznqyqwzf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.316326.xyz/gtfcizndlo.html

Ruby: ENV["HOME"]
来源：http://hz.shangyingyoupin.top/gttrytehdy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.feifeiyinyue.top/gtogsofqod.html

[M03] 执行外部命令
来源：http://hz.svipenyu.cn/gtzvyyqone.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj20258888.top/gtaaqznwnr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhiwuduotai.top/gtgwlzatin.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.dashuyun.cn/gtsootpzul.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.snrcjt.cn/gtzppezmvq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.meibo888.top/gtcrvgqvqz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.pycfn.com/gtrtpggtop.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xingfuxueyuan.xyz/gtinsqutwb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ydjk.org.cn/gtxijzekai.html

[M04] 获取当前工作目录
来源：http://hz.tian-w.cn/gtijkmxzlm.html

Py:   os.getcwd()
来源：http://hz.jyoumei.cn/gtyyhgwxse.html

PHP:  getcwd();
来源：http://hz.cheryme.top/gtsmmijstc.html

JS:   process.cwd()
来源：http://hz.mhx1999.top/gtfgrtwukl.html

TS:   process.cwd()
来源：http://hz.meibo888.top/gtneggoonz.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hammf.cn/gtbvahaiuo.html

Go:   os.Getwd()
来源：http://hz.zhoulong.xyz/gtriddyfke.html

Ruby: Dir.pwd
来源：http://hz.xuanzx.com/gtzyfjgzzy.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.fengsongda.top/gtvbljcfzw.html

[M05] 设置退出码
来源：http://hz.cheryme.top/gtlxkhyacq.html

Py:   sys.exit(1)
来源：http://hz.zhixingplan.top/gtrtuospcz.html

PHP:  exit(1);
来源：http://hz.sxryk.cn/gtndybikqb.html

JS:   process.exit(1)
来源：http://hz.316326.xyz/gtexzeeccu.html

TS:   process.exit(1)
来源：http://hz.zhongyouzk.top/gtydigctvo.html

Java: System.exit(1)
来源：http://hz.0kj1m.cn/gtbsyppvyr.html

Go:   os.Exit(1)
来源：http://hz.chenlongwang.top/gtpqycztzo.html

Ruby: exit 1
来源：http://hz.tanke756.top/gtbnwsoezx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.meibo888.top/gtxuohsajk.html

[M06] 向标准错误输出
来源：http://hz.cdnleiting.top/gtlptcfedm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.c1oappe.top/gtvbbxldoc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shanyushiyangkeji.top/gtzitylfli.html

JS:   console.error("err")
来源：http://hz.xuanzx.com/gtukgmyrbe.html

TS:   console.error("err")
来源：http://hz.jqgufenzy.top/gttxpkfqbw.html

Java: System.err.println("err")
来源：http://hz.zhijiandao.cn/gtscgfnugu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.chenzaomai.com/gtqqbrqriw.html

Ruby: warn "err"
来源：http://hz.ybcxt.top/gtdibnwwzj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.wangshuangyany.cn/gtwxuurbcw.html

[M07] 判断是否为主入口
来源：http://hz.yj20258.top/gthptqdjyi.html

Py:   if __name__ == "__main__":
来源：http://hz.guowangkeji.top/gtmqkmdoyp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hnqzz.top/gtocsuzpvy.html

JS:   require.main === module
来源：http://hz.zdqjudy.top/gtlewgzuca.html

TS:   require.main === module
来源：http://hz.birdmap.top/gtgebekwqm.html

Java: public static void main(String[] args)
来源：http://hz.fengsongda.top/gtvtofouyu.html

Go:   func main()
来源：http://hz.cheryme.top/gtspvgdoxt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.aibaodan.cn/gtpwnnskpx.html

C#:   static void Main(string[] args)
来源：http://hz.zhongyouzk.top/gtafkblorb.html

[M08] 获取系统与运行时信息
来源：http://hz.wangdashe.top/gteqnietdp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.316326.xyz/gtwunqlkgg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ybcxt.top/gtidretmhq.html

JS:   process.platform;  process.version
来源：http://hz.zhixingplan.top/gttoiyupmv.html

TS:   process.platform;  process.version
来源：http://hz.hnxiangtu.top/gtwnkssuuy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhengqikj.top/gtadkqxuay.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.fzhhl.top/gtlzvptlyc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ybcxt.top/gtvktuedts.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhoulong.xyz/gtrmvrijpy.html

================================================================================
来源：http://hz.yuanzhike.top/gtyxzirgqf.html

N. 数据结构与算法
来源：http://hz.ybcxt.top/gtxowqmhlj.html

================================================================================
来源：http://hz.jiagoushi.top/gtlagcmens.html

[N01] 二分查找（有序数组）
来源：http://hz.ybcxt.top/gtqgwiuiko.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ivvv.top/gtooaxjvlo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.pengpengdd.cyou/gtopbngkdi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhoulong.xyz/gtgwoortpy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xziqi.cn/gtvxjglfff.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cdnleiting.top/gtrfyqypig.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.guowangkeji.top/gtaffjtjqe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ydjk.org.cn/gtokwxnphh.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jqgfzy.top/gtumwousdv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.chenzaomai.com/gtnionxkby.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sweek.top/gtqmxiehmb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.kuanghao11.cn/gtzlptyyqk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shangyingyoupin.top/gtyzcitgin.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gzhubu.top/gtblvuqkwm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.chenzaomai.com/gtuhhqcijz.html

Go:   slices.Sort(arr)
来源：http://hz.snrcjt.cn/gtqiisutbc.html

Ruby: arr.sort
来源：http://hz.ivvv.top/gtsoljfuni.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.tanke756.top/gtielbtqfy.html

[N03] 快速排序（分治示例）
来源：http://hz.tian-w.cn/gtjqflcyou.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hysaishi.cn/gtffbdxjdu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinghuilouyu.cn/gtfynppell.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.fengsongda.top/gtwfcsxolv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenlongwang.top/gtellauixa.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.havefunace.top/gtlqjjlqor.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.fzhhl.top/gtkcjspcgh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yanxiufei.cn/gtatkqgvyo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.chenlongwang.top/gtjhzwsnsq.html

[N04] 斐波那契数列
来源：http://hz.cucudq.cn/gtfskqiyuu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tanke756.top/gtdtmnlocd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.52xcode.cn/gtdhrhalra.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tanke756.top/gttyhjwcbe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.0kj1m.cn/gtksknvejm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gaohongyu789.top/gthzudjlzm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.svipenyu.cn/gtfsfokaqs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.nwbrower.top/gtryrwzyay.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenzaomai.com/gtmrhmfpmg.html

[N05] 最大公约数
来源：http://hz.shzxlz.cn/gtbfkvfgus.html

Py:   math.gcd(a, b)
来源：http://hz.yj202588.top/gtfkcofqtr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yueranfly.top/gtmabmdpul.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sweek.top/gthtfcykzn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gotoacloud.top/gthlbqjevs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hfpthk.cn/gttqhvqjju.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yangfankeji.com/gtfbchxvzr.html

Ruby: a.gcd(b)
来源：http://hz.yanxiufei.cn/gtfbsonxsi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yanxiufei.cn/gtcuzodmkm.html

[N06] 判断回文字符串
来源：http://hz.iojbl.cn/gtgjsiwrmr.html

Py:   s == s[::-1]
来源：http://hz.havefunace.top/gtsjisuvqn.html

PHP:  $s === strrev($s);
来源：http://hz.xylfe.cn/gtahemvdpo.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hongshengwenyu.top/gtkdwliwsf.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gttxabgsde.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xylfe.cn/gtmlyhccha.html

Go:   // 双指针从两端比较
来源：http://hz.xziqi.cn/gtuiynkjga.html

Ruby: s == s.reverse
来源：http://hz.shanyushiyangkeji.top/gtyldziybx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jlsjyb.cn/gtgujpuqpe.html

[N07] 两数之和（返回下标）
来源：http://hz.tanke756.top/gtoonvifsq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shanyushiyangkeji.top/gttllbbzal.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.c1oappe.top/gtaftyirtj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gogol.net.cn/gtrdgtxrxz.html

TS:   // 手写 Map<string, number>
来源：http://hz.xylfe.cn/gtiompfesr.html

Java: // 手写 HashMap
来源：http://hz.pengpengdd.cyou/gtmcmaesem.html

Go:   // 手写 map[int]int
来源：http://hz.ydjk.org.cn/gtuhoobtkl.html

Ruby: // 手写 Hash
来源：http://hz.xuetiantiany.cn/gtnjguhxnj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.feifeiyinyue.top/gtlomqfgcf.html

[N08] 生成全排列
来源：http://hz.guannengcc.top/gtnggoohkb.html

Py:   itertools.permutations(arr)
来源：http://hz.shanyushiyangtech.top/gtrtltlkel.html

PHP:  // 手写递归交换
来源：http://hz.ydjk.org.cn/gtzyspgmbk.html

JS:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtknhxxliy.html

TS:   // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtkqpxzsfc.html

Java: // 手写回溯递归
来源：http://hz.xinyue.icu/gtmevoovrz.html

Go:   // 手写回溯递归
来源：http://hz.fengsongda.top/gtrfzohngp.html

Ruby: arr.permutation.to_a
来源：http://hz.shuidangran.top/gttorahqmv.html

C#:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtaaqdmkle.html

[N09] 栈与队列
来源：http://hz.andypj.xyz/gtvgmibuku.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jqgfzy.top/gtyltubrnv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.haohaochexian.top/gtdhsymwfr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ivvv.top/gtvuotsyhm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.guannengcc.top/gtlknftmcw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yuxming.cn/gtscurfaqb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jlsjyb.cn/gtxwstgkqp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.9152youxi.cn/gtzecirfjv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gzhubu.top/gtssmollvp.html

[N10] 链表节点定义
来源：http://hz.yvedp.cn/gttltbuiss.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yj20258888.top/gtlikacxqe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cashguo.top/gtoplomvri.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.birdmap.top/gtpxewfkoa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.meibo888.top/gtkxzbifeq.html

Java: class Node { int v; Node next; }
来源：http://hz.gogol.net.cn/gtxuqeefka.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xinyue.icu/gtqbtwuthx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ppjwa.cn/gtecpvvuwf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.52xcode.cn/gtvywyehyi.html

[N11] 二叉树中序遍历
来源：http://hz.52xcode.cn/gttuawvnyq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.gogol.net.cn/gtwcuoxyob.html

PHP:  // 手写递归函数
来源：http://hz.ydzc1.top/gtaoajtzpo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guowangkeji.top/gtzzkvotwk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zycfv.cn/gtgbgmyidu.html

Java: // 手写递归
来源：http://hz.shanyushiyangkeji.top/gtezwvrxcv.html

Go:   // 手写递归
来源：http://hz.chenlongwang.top/gtmpdjhtdv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhongyouzk.top/gtjhcfbfvm.html

C#:   // 手写递归
来源：http://hz.cdnleiting.top/gtcagtoors.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yongpay.top/gtzehxfrvo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.vqdsnc.cn/gtqmlxkxpl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hfpthk.cn/gtxoxgdlfn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtdtpskavo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ybcxt.top/gtyujzglqz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hfpthk.cn/gtqxhlkbpj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.snrcjt.cn/gtnyjlymxz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xuanzx.com/gtsirtrewd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhongyouzk.top/gtmtjyljot.html

================================================================================
来源：http://hz.ydzc1.top/gtcyrjyuip.html

O. 并发与异步
来源：http://hz.jinqigfzy.top/gtxpazbhiv.html

================================================================================
来源：http://hz.quarkkingdee.top/gttozytegx.html

[O01] 启动一个线程
来源：http://hz.ivvv.top/gtebngqpwe.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.bjfxy.top/gtbuupnnzj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hongshengwenyu.top/gterazozef.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.sxryk.cn/gtegrnahfl.html

TS:   // 同 JS
来源：http://hz.wangshuangyany.cn/gtfprvcfkp.html

Java: new Thread(() -> f()).start()
来源：http://hz.cucudq.cn/gtfkmvfdqk.html

Go:   go f()
来源：http://hz.dashuyun.cn/gtpneoxndl.html

Ruby: Thread.new { f }
来源：http://hz.zhijiandao.cn/gtcfpvcugh.html

C#:   Task.Run(() => F());
来源：http://hz.316326.xyz/gtheqtetnv.html

[O02] 使用线程池
来源：http://hz.zhengqikj.top/gtpwxmitfw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinqigufen.top/gtkcbmxyrh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.chenlongwang.top/gtmecodrux.html

JS:   // worker_threads 线程池
来源：http://hz.hysaishi.cn/gtqywpljef.html

TS:   // worker_threads 线程池
来源：http://hz.0kj1m.cn/gtbqmugxep.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ivvv.top/gtkpgsamol.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gzhubu.top/gtolwwxsft.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinghuilouyu.cn/gtyndzqxfh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cqqwz.cn/gtzcokfpty.html

[O03] 加锁保护共享数据
来源：http://hz.snrcjt.cn/gtonrcczys.html

Py:   with lock: shared += 1
来源：http://hz.dianchejie.cn/gtvbftlfno.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xuetiantiany.cn/gtqbhckvhh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yongpay.top/gtjzzthexr.html

TS:   // 同 JS
来源：http://hz.yanxiufei.cn/gtiexsymsi.html

Java: synchronized (this) { shared++; }
来源：http://hz.c1oappe.top/gtlmbeannz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.aizwys.cn/gteglqlhgz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hnqzz.top/gtphlcxahm.html

C#:   lock (gate) { shared++; }
来源：http://hz.jinqigfzy.top/gtfgqjtnbb.html

[O04] 定义异步函数并等待
来源：http://hz.sufxvd.cn/gtglpzcyoz.html

Py:   async def f():⏎    await g()
来源：http://hz.zhiwuduotai.top/gtxawnsyqu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yj20258.top/gtoffrcroj.html

JS:   async function f() { await g(); }
来源：http://hz.gaohongyu789.top/gtulwvhnvu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.nanxuanxn.top/gtbuvvlpdk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.daxiang520.top/gthynswpwp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.kuanghao11.cn/gtislnhnsd.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.tian-w.cn/gtnckpvrpy.html

C#:   async Task F() { await G(); }
来源：http://hz.ehwqpu.com/gtoksqupgf.html

[O05] 并发执行并等待全部完成
来源：http://hz.ydjk.org.cn/gtfvlkqrqv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.tanke756.top/gtersvjfcu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.svipenyu.cn/gtapvplnqd.html

JS:   await Promise.all(tasks)
来源：http://hz.shuidangran.top/gtaazpycoe.html

TS:   await Promise.all(tasks)
来源：http://hz.yonumen.top/gtoipscrrh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yanxiufei.cn/gtlxkixink.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shzxlz.cn/gtndquvwwq.html

Ruby: threads.map(&:join)
来源：http://hz.havefunace.top/gtbqlhltey.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.sysykeji.top/gtuiczmfhk.html

[O06] 使用进程池
来源：http://hz.ybcxt.top/gtwwgtxyfs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.guowangkeji.top/gtxpwzbcdm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yj20258888.top/gtmeaarweq.html

JS:   // child_process / cluster 模块
来源：http://hz.redwolf501.top/gtawwwclrw.html

TS:   // child_process / cluster 模块
来源：http://hz.yuxming.cn/gtcabryhfz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ywan-chungtsiang.top/gttceawwxe.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yuxming.cn/gtxhkpljtw.html

Ruby: // fork 块
来源：http://hz.shanyushiyangtech.top/gtqgbgjrvb.html

C#:   Parallel.For
来源：http://hz.gaohongyu789.top/gtrprpknnl.html

================================================================================
来源：http://hz.chenzaomai.com/gtqsfvbill.html

P. 常用工具函数
来源：http://hz.shangyingyoupin.top/gtprszihwu.html

================================================================================
来源：http://hz.wangdashe.top/gtpuriunrg.html

[P01] 生成 UUID
来源：http://hz.jinyuanbaomall.cn/gtzzgktlht.html

Py:   str(uuid.uuid4())
来源：http://hz.sweek.top/gtytdbmoik.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.aibaodan.cn/gtmjlxuruv.html

JS:   crypto.randomUUID()
来源：http://hz.smart0.xyz/gtjtqubqom.html

TS:   crypto.randomUUID()
来源：http://hz.meibo888.top/gtcjiwwtic.html

Java: UUID.randomUUID().toString()
来源：http://hz.kuanghao11.cn/gtdbwehrjt.html

Go:   // 用 github.com/google/uuid
来源：http://hz.daxiang520.top/gtmjodwujy.html

Ruby: SecureRandom.uuid
来源：http://hz.pycfn.com/gtvvxlpfgf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sysykeji.top/gtkzxsqqbc.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sweek.top/gthsweyiut.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenzaomai.com/gtrillnnpz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.wangdashe.top/gtpsolphpe.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.sweek.top/gtiuqmmpga.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shzxlz.cn/gtdjfutjqt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.316326.xyz/gtuvylnrfe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hywenlv.cn/gtxjxrzkll.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhiwuduotai.top/gtvtgxrqdz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhongyouzk.top/gtztvnehjp.html

[P03] 生成短随机字符串
来源：http://hz.fzhhl.top/gteextgeos.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.pengpengdd.cyou/gtldxzoyct.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yuanzhike.top/gtakmrsttc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ehwqpu.com/gtxybhbkow.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xingfuxueyuan.xyz/gtdrssvznn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gzhubu.top/gtjxtgpyff.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.tian-w.cn/gtiwoyxhma.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.wangdashe.top/gtmkwfxyig.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinyuanbaomall.cn/gtxoxtgjco.html

[P04] 求长度
来源：http://hz.yueranfly.top/gtveeojdpn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shangyingyoupin.top/gtggcdxblp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhiwuduotai.top/gtdwnugaiz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cashguo.top/gtrcmeugsp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sufxvd.cn/gtgdcwzupj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xuetiantiany.cn/gtggnnalzg.html

Go:   len(arr);  len(m)
来源：http://hz.zhijiandao.cn/gtyuzgynxm.html

Ruby: x.length;  x.size
来源：http://hz.yj20258888.top/gtadrknzrm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jlsjyb.cn/gtiwsajwkq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.tianlin.xyz/gtkacmxoii.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhaomingkeji.xyz/gtkocqaarq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.vqdsnc.cn/gtauwrcrzr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenjidiqi.icu/gtmfuljdav.html


<!-- 参考信息 -->