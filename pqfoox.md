代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://hz.jqgufenzy.top/gtxsqymbzr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhaomingkeji.xyz/gtyflpzsyi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zycfv.cn/gtqrzkchib.html

JS:   resp.ok;  resp.status
来源：http://hz.c1oappe.top/gtbtjsdase.html

TS:   resp.ok;  resp.status
来源：http://hz.yuanzhike.top/gtqfnnsxdk.html

Java: resp.statusCode()
来源：http://hz.yonumen.top/gtotguvqvv.html

Go:   resp.StatusCode
来源：http://hz.hnxiangtu.top/gtogttdazb.html

Ruby: resp.code.to_i
来源：http://hz.aizwys.cn/gtvyxulmke.html

C#:   (int)resp.StatusCode
来源：http://hz.jinqigfzy.top/gtwoyaiela.html

[L08] 并发请求多个地址
来源：http://hz.xingfuxueyuan.xyz/gtntflnjlb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.bjfxy.top/gtqzjkhfiz.html

PHP:  curl_multi_init() 系列
来源：http://hz.yongpay.top/gtzhaqikqr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gogol.net.cn/gtxvbnyres.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gzhubu.top/gtbuglwqym.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ivvv.top/gtivcqpcvm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tian-w.cn/gtihasttkj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.iojbl.cn/gtkzmitpoi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xinyue.icu/gttbajepiz.html

================================================================================
来源：http://hz.feifeiyinyue.top/gteptxkcxy.html

M. 命令行 / 进程 / 环境
来源：http://hz.hongshengwenyu.top/gtaftsyjjf.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtonngslxa.html

[M01] 读取命令行参数
来源：http://hz.feifeiyinyue.top/gtaeyakpuk.html

Py:   sys.argv[1:]
来源：http://hz.jinqigufen.top/gttkcejaxd.html

PHP:  $argv;  $argc;
来源：http://hz.jinqigufen.top/gtdjimsufu.html

JS:   process.argv.slice(2)
来源：http://hz.52xcode.cn/gtflkrqdta.html

TS:   process.argv.slice(2)
来源：http://hz.52xcode.cn/gtecleoelu.html

Java: args 数组（main 方法参数）
来源：http://hz.zhengqikj.top/gtqhtonxrb.html

Go:   os.Args[1:]
来源：http://hz.yanxiufei.cn/gtapilfgqa.html

Ruby: ARGV
来源：http://hz.nanxuanxn.top/gtntasmrcq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ehwqpu.com/gttrlfzbxz.html

[M02] 读取环境变量
来源：http://hz.yonumen.top/gtlxjzuyxb.html

Py:   os.environ.get("HOME")
来源：http://hz.xziqi.cn/gtmgdmskxq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shuidangran.top/gtysjycryr.html

JS:   process.env.HOME
来源：http://hz.zhijiandao.cn/gtyyfxpmvw.html

TS:   process.env.HOME
来源：http://hz.pengpengdd.cyou/gtawonnntm.html

Java: System.getenv("HOME")
来源：http://hz.wangdashe.top/gthpefbyku.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jianghu66.top/gtxazwbvlb.html

Ruby: ENV["HOME"]
来源：http://hz.zhijiandao.cn/gtmtilcffq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.iojbl.cn/gtjjzelbkn.html

[M03] 执行外部命令
来源：http://hz.haohaochexian.top/gtvuafmrdg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ybcxt.top/gtoyydvfhe.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yanxiufei.cn/gtjlrazjca.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigufen.top/gtfmprpssq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.316326.xyz/gtspyepeox.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.tianlin.xyz/gtegwsncop.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zdqjudy.top/gtjrfxfkjv.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.9152youxi.cn/gtuumrxshd.html

C#:   Process.Start("ls", "-l");
来源：http://hz.haohaochexian.top/gttuzgmqyf.html

[M04] 获取当前工作目录
来源：http://hz.chenzaomai.com/gtogybrvla.html

Py:   os.getcwd()
来源：http://hz.vqdsnc.cn/gtyhoegqnl.html

PHP:  getcwd();
来源：http://hz.sweek.top/gtjmkgypyo.html

JS:   process.cwd()
来源：http://hz.ydjk.org.cn/gtewbrlytf.html

TS:   process.cwd()
来源：http://hz.dianchejie.cn/gtpvshhrzd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sysykeji.top/gtkoujunfv.html

Go:   os.Getwd()
来源：http://hz.jinghuilouyu.cn/gtcvqzocve.html

Ruby: Dir.pwd
来源：http://hz.kuanghao11.cn/gtwffscmdj.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shzxlz.cn/gtntpcesdn.html

[M05] 设置退出码
来源：http://hz.yj20258888.top/gtdebufdhs.html

Py:   sys.exit(1)
来源：http://hz.xinyue.icu/gtabjofvin.html

PHP:  exit(1);
来源：http://hz.cucudq.cn/gthuuvgzhl.html

JS:   process.exit(1)
来源：http://hz.sweek.top/gtdvbcoshn.html

TS:   process.exit(1)
来源：http://hz.xinyue.icu/gtqdyusomj.html

Java: System.exit(1)
来源：http://hz.ppjwa.cn/gtfccxbbva.html

Go:   os.Exit(1)
来源：http://hz.andypj.xyz/gtzudazfro.html

Ruby: exit 1
来源：http://hz.shangyingyoupin.top/gttsdvanwo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.dashuyun.cn/gtqoqnglnq.html

[M06] 向标准错误输出
来源：http://hz.wangshuangyany.cn/gtdkfqcwqb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cqqwz.cn/gtttlfwyqk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shuidangran.top/gtrfbgxqbi.html

JS:   console.error("err")
来源：http://hz.hfpthk.cn/gtatgktiru.html

TS:   console.error("err")
来源：http://hz.iojbl.cn/gtnmvvbdtc.html

Java: System.err.println("err")
来源：http://hz.cdnleiting.top/gtrzpwfety.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jlsjyb.cn/gtbnzitjwa.html

Ruby: warn "err"
来源：http://hz.meibo888.top/gtdjkihykb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xingfuxueyuan.xyz/gtkxturviz.html

[M07] 判断是否为主入口
来源：http://hz.mhx1999.top/gtqosqhxeg.html

Py:   if __name__ == "__main__":
来源：http://hz.daxiang520.top/gtcdvakfig.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jyoumei.cn/gtahntkccv.html

JS:   require.main === module
来源：http://hz.sysykeji.top/gtsowvuqoc.html

TS:   require.main === module
来源：http://hz.cucudq.cn/gtawzpkwwi.html

Java: public static void main(String[] args)
来源：http://hz.tianlin.xyz/gtwgjkyzgk.html

Go:   func main()
来源：http://hz.c1oappe.top/gtrmrbsnlh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jiagoushi.top/gtfeurmrdz.html

C#:   static void Main(string[] args)
来源：http://hz.xingfuxueyuan.xyz/gtlubrrmtf.html

[M08] 获取系统与运行时信息
来源：http://hz.zhoulong.xyz/gtovjtdyuu.html

Py:   platform.system();  platform.python_version()
来源：http://hz.daxiang520.top/gtgezaaest.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xuanzx.com/gtyjwtuyvj.html

JS:   process.platform;  process.version
来源：http://hz.tianlin.xyz/gtdfzluqqn.html

TS:   process.platform;  process.version
来源：http://hz.zhijiandao.cn/gtiqpzqpag.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ybcxt.top/gtfdwvansi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.0kj1m.cn/gtqseqzuly.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinqigufen.top/gtepqzazzi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ppjwa.cn/gtqpyzceld.html

================================================================================
来源：http://hz.52xcode.cn/gtpssfhwaj.html

N. 数据结构与算法
来源：http://hz.shangyingyoupin.top/gtlemwnzih.html

================================================================================
来源：http://hz.cdnleiting.top/gtubltbqba.html

[N01] 二分查找（有序数组）
来源：http://hz.fengsongda.top/gtstdryarm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shanyushiyangtech.top/gteagizcxk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jiagoushi.top/gtaqynltbi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.316326.xyz/gtgkehycrh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yonumen.top/gtywaavutq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.tianlin.xyz/gtofwxvgza.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.bjfxy.top/gtflofvnxk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jianghu66.top/gtglwhcvyx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtjeaqktzn.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jqgfzy.top/gtordslwbo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zdqjudy.top/gtcoaonnek.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.guowangkeji.top/gtvullejjp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xziqi.cn/gtjecvielp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxinkj.top/gtrgrcscvq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.vqdsnc.cn/gtkdjdxlwz.html

Go:   slices.Sort(arr)
来源：http://hz.hnqzz.top/gtxribffnp.html

Ruby: arr.sort
来源：http://hz.zycfv.cn/gtnetmmdqt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shanyushiyangtech.top/gtwyhuxyri.html

[N03] 快速排序（分治示例）
来源：http://hz.snrcjt.cn/gtwqkpgyjs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.wangshuangyany.cn/gtkrssyzbi.html

PHP:  // 递归实现，或用 usort
来源：http://hz.andypj.xyz/gtybwleccb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aizwys.cn/gtyagdfhpz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yonumen.top/gtblyybtil.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.dianchejie.cn/gtpjbtxlhu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhiwuduotai.top/gtsaykptrk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shanyushiyangtech.top/gtntkldpep.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tian-w.cn/gtdqfsczvi.html

[N04] 斐波那契数列
来源：http://hz.ydzc1.top/gtrduueaod.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jqgfzy.top/gtysdxwztb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinghuilouyu.cn/gtzfnkaejl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.52xcode.cn/gtxrzctswt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sysykeji.top/gtzcshglkn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.aizwys.cn/gtlrlnzvmw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shzxlz.cn/gttqtvphes.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.c1oappe.top/gtskdidiae.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.aibaodan.cn/gtojntjmmz.html

[N05] 最大公约数
来源：http://hz.zhongyouzk.top/gtrqwfugni.html

Py:   math.gcd(a, b)
来源：http://hz.mhx1999.top/gtfqspkemv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhoulong.xyz/gtnbpvnfso.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sufxvd.cn/gtvysqtvmi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.snrcjt.cn/gtjezhbtcr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.pengpengdd.cyou/gtxqbjmeej.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hammf.cn/gtdsbgwzxz.html

Ruby: a.gcd(b)
来源：http://hz.shuidangran.top/gtgdvgjunj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.sysykeji.top/gtfgopxute.html

[N06] 判断回文字符串
来源：http://hz.xylfe.cn/gtscedwiwa.html

Py:   s == s[::-1]
来源：http://hz.vqdsnc.cn/gtpxmewoib.html

PHP:  $s === strrev($s);
来源：http://hz.shanyushiyangtech.top/gtffbsqfkw.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hfpthk.cn/gtegcntdfr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gthczzxzvk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhongyouzk.top/gtlpoxbfeb.html

Go:   // 双指针从两端比较
来源：http://hz.zhoulong.xyz/gtawsrygin.html

Ruby: s == s.reverse
来源：http://hz.gogol.net.cn/gtaulyxvsj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.chenlongwang.top/gtzmieyaxs.html

[N07] 两数之和（返回下标）
来源：http://hz.zhongyouzk.top/gtengdioyv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jqgfzy.top/gtexapnzxu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.andypj.xyz/gthtcahuwh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.cdnleiting.top/gtyzzksjnh.html

TS:   // 手写 Map<string, number>
来源：http://hz.cucudq.cn/gtqrhykobf.html

Java: // 手写 HashMap
来源：http://hz.zhiwuduotai.top/gttbbjcxqk.html

Go:   // 手写 map[int]int
来源：http://hz.yvedp.cn/gtrdvsktup.html

Ruby: // 手写 Hash
来源：http://hz.hammf.cn/gtmkqktzjq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yonumen.top/gtcpbnorui.html

[N08] 生成全排列
来源：http://hz.wangdashe.top/gtrpgqljnn.html

Py:   itertools.permutations(arr)
来源：http://hz.gaohongyu789.top/gtbammlrmv.html

PHP:  // 手写递归交换
来源：http://hz.mhx1999.top/gtwogvzwuu.html

JS:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtrzxnyfvx.html

TS:   // 手写回溯递归
来源：http://hz.ivvv.top/gtlspslhvw.html

Java: // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtncfhrvie.html

Go:   // 手写回溯递归
来源：http://hz.cqqwz.cn/gtshvlcamj.html

Ruby: arr.permutation.to_a
来源：http://hz.cqqwz.cn/gtplnddpgk.html

C#:   // 手写回溯递归
来源：http://hz.bjfxy.top/gtyroeobro.html

[N09] 栈与队列
来源：http://hz.shanyushiyangkeji.top/gtlxplrdsu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hfpthk.cn/gtodjshvbc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.chenlongwang.top/gtmbeumaos.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xylfe.cn/gthhtbgipl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.sxryk.cn/gtmzeotvmr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yuanzhike.top/gtsawpnnnp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinqigfzy.top/gtcmotfumv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhixingplan.top/gtfqwoihct.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zycfv.cn/gttfrvgkro.html

[N10] 链表节点定义
来源：http://hz.jinyuanbaomall.cn/gtlpncprho.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.guannengcc.top/gtwawpslue.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.chenlongwang.top/gtabohbiop.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.chenzaomai.com/gtxznkrdzu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yanxiufei.cn/gtmeiykbjs.html

Java: class Node { int v; Node next; }
来源：http://hz.zhongyouzk.top/gtefpdrqwt.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yangfankeji.com/gtwtlmzcbi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xylfe.cn/gtjilontff.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhiwuduotai.top/gtcqrppgnj.html

[N11] 二叉树中序遍历
来源：http://hz.yanxiufei.cn/gtyolyszyl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.vqdsnc.cn/gtbgrcmzhy.html

PHP:  // 手写递归函数
来源：http://hz.sysykeji.top/gtkjikpjag.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yongpay.top/gtajsizsct.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dianchejie.cn/gtiiyqzfyy.html

Java: // 手写递归
来源：http://hz.shangyingyoupin.top/gtncoezmia.html

Go:   // 手写递归
来源：http://hz.birdmap.top/gtclccyvqy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.c1oappe.top/gtsrkhrleo.html

C#:   // 手写递归
来源：http://hz.gaohongyu789.top/gtepbfordu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zdqjudy.top/gtfbrvsskg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.havefunace.top/gtugbdnogq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinqigufen.top/gtdmcttqbq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtccsapgiy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gotoacloud.top/gtdgbixvkn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.haohaochexian.top/gtodhugcnl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.316326.xyz/gtjffjluzl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sxryk.cn/gtepjzhgxm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangtech.top/gtqgkypimy.html

================================================================================
来源：http://hz.jqgufenzy.top/gtyjnbrvcd.html

O. 并发与异步
来源：http://hz.nwbrower.top/gtdrggcqqj.html

================================================================================
来源：http://hz.c1oappe.top/gthuqkfkql.html

[O01] 启动一个线程
来源：http://hz.birdmap.top/gtzidjydwm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ybcxt.top/gtterfhbvv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhijiandao.cn/gtsghasdwi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.sufxvd.cn/gtmkujuexc.html

TS:   // 同 JS
来源：http://hz.sufxvd.cn/gtfanpldqh.html

Java: new Thread(() -> f()).start()
来源：http://hz.hnxiangtu.top/gtljnfeeqd.html

Go:   go f()
来源：http://hz.yanxiufei.cn/gtljypybzk.html

Ruby: Thread.new { f }
来源：http://hz.zycfv.cn/gtfyxmcfgh.html

C#:   Task.Run(() => F());
来源：http://hz.yuanzhike.top/gtvhwcquto.html

[O02] 使用线程池
来源：http://hz.gzhubu.top/gtfjkfcwyw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cqqwz.cn/gtovuicalb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jiagoushi.top/gtwgastqwe.html

JS:   // worker_threads 线程池
来源：http://hz.yongpay.top/gtlswsfggs.html

TS:   // worker_threads 线程池
来源：http://hz.meibo888.top/gtmhqsxlrs.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yangfankeji.com/gtcpmwcajx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.dianchejie.cn/gteowmcplb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yvedp.cn/gtywqrhnnw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hywenlv.cn/gtwrfifrzz.html

[O03] 加锁保护共享数据
来源：http://hz.daria6918.cn/gthutamdjh.html

Py:   with lock: shared += 1
来源：http://hz.zhixingplan.top/gtunmfqxdc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xuanzx.com/gtmxabvokp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shzxlz.cn/gtbwqutnpe.html

TS:   // 同 JS
来源：http://hz.hysaishi.cn/gtxluvcgcw.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhoulong.xyz/gtrwewcajf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jinqigufen.top/gthcdurqfu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yuxming.cn/gtiduhmwwi.html

C#:   lock (gate) { shared++; }
来源：http://hz.tianlin.xyz/gtrolnjtyo.html

[O04] 定义异步函数并等待
来源：http://hz.ybcxt.top/gtbiaxovcg.html

Py:   async def f():⏎    await g()
来源：http://hz.yvedp.cn/gtqatqbjsr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cheryme.top/gtnxuryxbt.html

JS:   async function f() { await g(); }
来源：http://hz.gaohongyu789.top/gtrcxccyke.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.redwolf501.top/gttcovcygx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ywan-chungtsiang.top/gtqfodsxsq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.tian-w.cn/gtuskavpnv.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yuanzhike.top/gtatpoxoci.html

C#:   async Task F() { await G(); }
来源：http://hz.yueranfly.top/gtomjlskyl.html

[O05] 并发执行并等待全部完成
来源：http://hz.chenlongwang.top/gtxowlhajq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shanyushiyangtech.top/gtsqgzjjtx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.0kj1m.cn/gtbsravddv.html

JS:   await Promise.all(tasks)
来源：http://hz.snrcjt.cn/gtzgxyfgbe.html

TS:   await Promise.all(tasks)
来源：http://hz.xuetiantiany.cn/gtvhhzynyi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.c1oappe.top/gtfwtrjkim.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.gotoacloud.top/gtxnffhkvl.html

Ruby: threads.map(&:join)
来源：http://hz.vqdsnc.cn/gtiuvlbswe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.sxryk.cn/gtpezkaqdi.html

[O06] 使用进程池
来源：http://hz.daxiang520.top/gtgduguabt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xuanzx.com/gtoxkdjxdn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhiwuduotai.top/gtkjgvshlz.html

JS:   // child_process / cluster 模块
来源：http://hz.chenzaomai.com/gtqrramydv.html

TS:   // child_process / cluster 模块
来源：http://hz.daria6918.cn/gtyuuhylzd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.iojbl.cn/gtkshgwcoj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.guannengcc.top/gtbqsortsd.html

Ruby: // fork 块
来源：http://hz.shuidangran.top/gtjbhjvzpw.html

C#:   Parallel.For
来源：http://hz.jqgufenzy.top/gtarrnjlkw.html

================================================================================
来源：http://hz.snrcjt.cn/gtscsojmab.html

P. 常用工具函数
来源：http://hz.sweek.top/gtpbgtqpch.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gthswxcflb.html

[P01] 生成 UUID
来源：http://hz.hfpthk.cn/gtilfiuquj.html

Py:   str(uuid.uuid4())
来源：http://hz.zycfv.cn/gtigllwnol.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sysykeji.top/gtvnychsnr.html

JS:   crypto.randomUUID()
来源：http://hz.xinyue.icu/gtxsyfgtxe.html

TS:   crypto.randomUUID()
来源：http://hz.havefunace.top/gtjbmwwnli.html

Java: UUID.randomUUID().toString()
来源：http://hz.xylfe.cn/gtoislremx.html

Go:   // 用 github.com/google/uuid
来源：http://hz.feifeiyinyue.top/gturhomwnn.html

Ruby: SecureRandom.uuid
来源：http://hz.ydjk.org.cn/gtuskifoia.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinqigfzy.top/gtjbdqiuce.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sweek.top/gtxkuqikgk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ybcxt.top/gtxhvzpvhm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.aizwys.cn/gtcqydjyhc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.snrcjt.cn/gtzntfecmw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ywan-chungtsiang.top/gtqqumkhvp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jinghuilouyu.cn/gtfronctjj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.pycfn.com/gtnbkvgffr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cdnleiting.top/gtvsqmardg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.tian-w.cn/gtcssjzfag.html

[P03] 生成短随机字符串
来源：http://hz.shuidangran.top/gtoirhhzmq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xziqi.cn/gtiyxfmfte.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hfpthk.cn/gtixmpilny.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.iojbl.cn/gtplugioex.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.kuanghao11.cn/gtwncueyrx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yangfankeji.com/gtlfonzztt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nanxinkj.top/gtqfrbfitv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sxryk.cn/gtnuoejmbi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shuidangran.top/gtwhxzvels.html

[P04] 求长度
来源：http://hz.shangyingyoupin.top/gtvkgdqaul.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yvedp.cn/gteqmrgxgb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.dashuyun.cn/gtftcwpual.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydjk.org.cn/gtuclbvxgo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xziqi.cn/gtrebrkvgs.html

Java: list.size();  map.size();  s.length()
来源：http://hz.kuanghao11.cn/gtgecjfidm.html

Go:   len(arr);  len(m)
来源：http://hz.sxryk.cn/gtymcgjijx.html

Ruby: x.length;  x.size
来源：http://hz.cheryme.top/gtsassjgbk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.pycfn.com/gtpqrcvhav.html


<!-- 参考信息 -->