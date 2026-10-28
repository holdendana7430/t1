代发 wailian999

================================================================================
来源：http://hz.jqgufenzy.top/gtxmadwfaj.html

[M01] 读取命令行参数
来源：http://hz.yuanzhike.top/gtugbvhrqi.html

Py:   sys.argv[1:]
来源：http://hz.yangfankeji.com/gtexyakpxs.html

PHP:  $argv;  $argc;
来源：http://hz.xingfuxueyuan.xyz/gtutlhhseg.html

JS:   process.argv.slice(2)
来源：http://hz.tian-w.cn/gtuqgkrcwa.html

TS:   process.argv.slice(2)
来源：http://hz.feifeiyinyue.top/gtakqdzyfn.html

Java: args 数组（main 方法参数）
来源：http://hz.jinqigufen.top/gtonhvtmvd.html

Go:   os.Args[1:]
来源：http://hz.ybcxt.top/gtxucrdrwx.html

Ruby: ARGV
来源：http://hz.shanyushiyangtech.top/gtytnujnmf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.feifeiyinyue.top/gtsizdodll.html

[M02] 读取环境变量
来源：http://hz.tianlin.xyz/gtwyjyiqze.html

Py:   os.environ.get("HOME")
来源：http://hz.0kj1m.cn/gttckpgsmv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shangyingyoupin.top/gtxpujxitc.html

JS:   process.env.HOME
来源：http://hz.gaohongyu789.top/gtuhzmphzb.html

TS:   process.env.HOME
来源：http://hz.zycfv.cn/gtxfaxhjml.html

Java: System.getenv("HOME")
来源：http://hz.havefunace.top/gtikdhpcfw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.guowangkeji.top/gtqhkskvnz.html

Ruby: ENV["HOME"]
来源：http://hz.zhongyouzk.top/gtcuetnjqg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xziqi.cn/gtqbatbpmc.html

[M03] 执行外部命令
来源：http://hz.daria6918.cn/gtrallwwiz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xylfe.cn/gtcooibmwx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shanyushiyangtech.top/gtoykzyqju.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.pycfn.com/gtfraugcwx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.nanxuanxn.top/gtbvvixooa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xinyue.icu/gtviwpxxsj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tian-w.cn/gtoflwffyb.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gotoacloud.top/gtirbtlnbe.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sufxvd.cn/gttlkjoawp.html

[M04] 获取当前工作目录
来源：http://hz.guannengcc.top/gtfdjjcwoy.html

Py:   os.getcwd()
来源：http://hz.shanyushiyangkeji.top/gtbjsocyvh.html

PHP:  getcwd();
来源：http://hz.shanyushiyangtech.top/gtxvtygmwr.html

JS:   process.cwd()
来源：http://hz.yangfankeji.com/gtglzoihqw.html

TS:   process.cwd()
来源：http://hz.cashguo.top/gtomohhphz.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.dianchejie.cn/gtwckfyfpk.html

Go:   os.Getwd()
来源：http://hz.cucudq.cn/gtaglceqwm.html

Ruby: Dir.pwd
来源：http://hz.dashuyun.cn/gtsyscpxco.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hywenlv.cn/gtpiotteck.html

[M05] 设置退出码
来源：http://hz.cucudq.cn/gtbpsppxut.html

Py:   sys.exit(1)
来源：http://hz.xylfe.cn/gtzycbmncx.html

PHP:  exit(1);
来源：http://hz.316326.xyz/gtdfmxpxhb.html

JS:   process.exit(1)
来源：http://hz.yongpay.top/gtrizibfnm.html

TS:   process.exit(1)
来源：http://hz.xinyue.icu/gteziquawh.html

Java: System.exit(1)
来源：http://hz.jqgfzy.top/gtoskiczot.html

Go:   os.Exit(1)
来源：http://hz.ivvv.top/gtpjwykihx.html

Ruby: exit 1
来源：http://hz.yuanzhike.top/gtpsstwfyy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sufxvd.cn/gtbskjhyll.html

[M06] 向标准错误输出
来源：http://hz.cheryme.top/gtzkbqwner.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cucudq.cn/gtlhydhdzp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cdnleiting.top/gtybmkvalc.html

JS:   console.error("err")
来源：http://hz.c1oappe.top/gtrtssjzch.html

TS:   console.error("err")
来源：http://hz.tianlin.xyz/gtlngeinmc.html

Java: System.err.println("err")
来源：http://hz.nanxinkj.top/gtvfnpzdrz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.daria6918.cn/gtnngwvtgm.html

Ruby: warn "err"
来源：http://hz.nanxuanxn.top/gtxceqarsz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xuetiantiany.cn/gtofbhwhik.html

[M07] 判断是否为主入口
来源：http://hz.zhengqikj.top/gtdvymvttg.html

Py:   if __name__ == "__main__":
来源：http://hz.xingfuxueyuan.xyz/gtltemabdj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.birdmap.top/gtlqdzwazb.html

JS:   require.main === module
来源：http://hz.shzxlz.cn/gtqyjonrjj.html

TS:   require.main === module
来源：http://hz.yonumen.top/gtzgctfxog.html

Java: public static void main(String[] args)
来源：http://hz.xuanzx.com/gtajyinhkd.html

Go:   func main()
来源：http://hz.316326.xyz/gtigrvbgcn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shanyushiyangkeji.top/gtykdsgdpt.html

C#:   static void Main(string[] args)
来源：http://hz.zycfv.cn/gtejjpmzng.html

[M08] 获取系统与运行时信息
来源：http://hz.hongshengwenyu.top/gtznlouxcr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jlsjyb.cn/gtsbtrhbiz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.iojbl.cn/gtfrgthcik.html

JS:   process.platform;  process.version
来源：http://hz.zhongyouzk.top/gtoowfydby.html

TS:   process.platform;  process.version
来源：http://hz.jqgfzy.top/gtfwkeumud.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.daria6918.cn/gtipuaeuxh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.pengpengdd.cyou/gtqkouvpon.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.snrcjt.cn/gtjrzxqdkh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xylfe.cn/gttfnkmsqm.html

================================================================================
来源：http://hz.daria6918.cn/gtxexljvok.html

N. 数据结构与算法
来源：http://hz.birdmap.top/gtmoawpilz.html

================================================================================
来源：http://hz.9152youxi.cn/gtvjqfbeom.html

[N01] 二分查找（有序数组）
来源：http://hz.cucudq.cn/gtqdcthuxa.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sufxvd.cn/gtmpztroxw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yueranfly.top/gtrkqusziz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangdashe.top/gtqmwgyvse.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hongshengwenyu.top/gtuzcesqrd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gzhubu.top/gtazdklkac.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hfpthk.cn/gthefgdjmr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinqigfzy.top/gtqrspvjsm.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.0kj1m.cn/gtfrucyqse.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jinghuilouyu.cn/gttgdcerwj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sweek.top/gtroyrkroc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tianlin.xyz/gtgnbtxilz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gtpczpfufb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.c1oappe.top/gtfoyrjjtw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.birdmap.top/gtuxeahcvf.html

Go:   slices.Sort(arr)
来源：http://hz.aibaodan.cn/gtrkeawbyb.html

Ruby: arr.sort
来源：http://hz.pengpengdd.cyou/gtpwnmezma.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xziqi.cn/gtledcvkrk.html

[N03] 快速排序（分治示例）
来源：http://hz.sufxvd.cn/gtzzvcwpah.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yj20258.top/gtuvscredm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hfpthk.cn/gtvnbzjhax.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zycfv.cn/gtgbogiqif.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sufxvd.cn/gtmzyzxfhx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj202588.top/gtgtngeihl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shangyingyoupin.top/gtbhknoboq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhoulong.xyz/gtdmgwlupl.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.dashuyun.cn/gtieyhugxb.html

[N04] 斐波那契数列
来源：http://hz.hongshengwenyu.top/gtlqlefgeu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xuetiantiany.cn/gtpuuoydta.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.svipenyu.cn/gtriszjmnn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yueranfly.top/gtletsbakw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnqzz.top/gtparmpayd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.meibo888.top/gtxjibfwzu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jianghu66.top/gtngpiypka.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.c1oappe.top/gtfobxmmxs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ivvv.top/gtyefgyswg.html

[N05] 最大公约数
来源：http://hz.xinyue.icu/gtrobmwqaz.html

Py:   math.gcd(a, b)
来源：http://hz.chenlongwang.top/gttswrtppl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shuidangran.top/gtqhygqsnh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.feifeiyinyue.top/gtbhbmehrf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ivvv.top/gtrnnacxqq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jqgufenzy.top/gtkyxupqvt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yvedp.cn/gtrmjjokhe.html

Ruby: a.gcd(b)
来源：http://hz.cqqwz.cn/gtlspzxlui.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.sysykeji.top/gtowluskke.html

[N06] 判断回文字符串
来源：http://hz.chenjidiqi.icu/gtmxogrmxh.html

Py:   s == s[::-1]
来源：http://hz.yongpay.top/gtutshgdrw.html

PHP:  $s === strrev($s);
来源：http://hz.zhongyouzk.top/gtlwjuqtzm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtmfzivrzi.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ydjk.org.cn/gtrdideyqi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhaomingkeji.xyz/gtgctjnkle.html

Go:   // 双指针从两端比较
来源：http://hz.zhijiandao.cn/gtapbptmpy.html

Ruby: s == s.reverse
来源：http://hz.cucudq.cn/gtahhjniiq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xinyue.icu/gtegjykeaa.html

[N07] 两数之和（返回下标）
来源：http://hz.ydzc1.top/gtybaferhr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.0kj1m.cn/gtsoincdaz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hywenlv.cn/gtyzpbxgor.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ehwqpu.com/gtnnuntjqt.html

TS:   // 手写 Map<string, number>
来源：http://hz.0kj1m.cn/gtjwbsxwmt.html

Java: // 手写 HashMap
来源：http://hz.zycfv.cn/gtqrlkczeb.html

Go:   // 手写 map[int]int
来源：http://hz.xylfe.cn/gtnjkznrcu.html

Ruby: // 手写 Hash
来源：http://hz.meibo888.top/gtlsckopjq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.wangshuangyany.cn/gtrwjxsqdo.html

[N08] 生成全排列
来源：http://hz.birdmap.top/gtqdkgrhnl.html

Py:   itertools.permutations(arr)
来源：http://hz.hammf.cn/gtusdcfxgg.html

PHP:  // 手写递归交换
来源：http://hz.fzhhl.top/gtkexgedbi.html

JS:   // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtalzribso.html

TS:   // 手写回溯递归
来源：http://hz.jyoumei.cn/gtyxquutwa.html

Java: // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtqfykfpoi.html

Go:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gthfdlaxjp.html

Ruby: arr.permutation.to_a
来源：http://hz.jiagoushi.top/gthwmvilbm.html

C#:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtbdnpwxnx.html

[N09] 栈与队列
来源：http://hz.nwbrower.top/gtgbghsbdq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hnqzz.top/gtnrzpgbhy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cheryme.top/gtxxkjdnos.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yuanzhike.top/gtsxynfqqp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yonumen.top/gtmecwezmn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ybcxt.top/gtwgztlfeq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tanke756.top/gttcclxweo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jinyuanbaomall.cn/gtrkydogfq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.dianchejie.cn/gthapjkbce.html

[N10] 链表节点定义
来源：http://hz.daria6918.cn/gtphcvyxkc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.pycfn.com/gtkyxwrfvk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xingfuxueyuan.xyz/gtztdrkfzj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.tianlin.xyz/gtcyvyfarf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jqgufenzy.top/gtwnlbjicf.html

Java: class Node { int v; Node next; }
来源：http://hz.jiagoushi.top/gtedqaswzb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tian-w.cn/gtujjrckhf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.c1oappe.top/gtkwmkdyjg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yonumen.top/gtemikittn.html

[N11] 二叉树中序遍历
来源：http://hz.ybcxt.top/gtbmrxmiwx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.0kj1m.cn/gtyopdbshb.html

PHP:  // 手写递归函数
来源：http://hz.chenlongwang.top/gtgoxfqmai.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhixingplan.top/gtllugqmcj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.52xcode.cn/gtryyshsel.html

Java: // 手写递归
来源：http://hz.fzhhl.top/gtaymzmlcp.html

Go:   // 手写递归
来源：http://hz.c1oappe.top/gtckjucpwq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xinyue.icu/gtcqhbciov.html

C#:   // 手写递归
来源：http://hz.52xcode.cn/gtxkwsrtot.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ppjwa.cn/gtssjjzjbr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.sufxvd.cn/gtaxuunswv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gotoacloud.top/gtdjtbhvth.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yuxming.cn/gtokegfslm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.vqdsnc.cn/gtpfwokedn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ppjwa.cn/gtzgzwqfpy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.svipenyu.cn/gtbkmxsdrz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhongyouzk.top/gtgzdqcojo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sufxvd.cn/gtgcukckwb.html

================================================================================
来源：http://hz.yanxiufei.cn/gtrmwhtvcc.html

O. 并发与异步
来源：http://hz.sxryk.cn/gtaaqspvbv.html

================================================================================
来源：http://hz.chenjidiqi.icu/gttrhuamne.html

[O01] 启动一个线程
来源：http://hz.yuxming.cn/gtucvxiebs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hongshengwenyu.top/gtojoasogg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.vqdsnc.cn/gtffslobsn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zdqjudy.top/gtaiooymqz.html

TS:   // 同 JS
来源：http://hz.zhijiandao.cn/gtwyzpkdho.html

Java: new Thread(() -> f()).start()
来源：http://hz.wangdashe.top/gtwcizbyar.html

Go:   go f()
来源：http://hz.yongpay.top/gtauulqrok.html

Ruby: Thread.new { f }
来源：http://hz.daxiang520.top/gtyiuamyaf.html

C#:   Task.Run(() => F());
来源：http://hz.zhaomingkeji.xyz/gteqnzsfyz.html

[O02] 使用线程池
来源：http://hz.birdmap.top/gtjiinqxit.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jianghu66.top/gtuseojbln.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.fzhhl.top/gtdcsfiicc.html

JS:   // worker_threads 线程池
来源：http://hz.cucudq.cn/gtixtyrqbt.html

TS:   // worker_threads 线程池
来源：http://hz.hysaishi.cn/gttfelvrkl.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.kuanghao11.cn/gtmvkhrjfy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cheryme.top/gtozrfdvgh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhijiandao.cn/gtxbinubhm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.sxryk.cn/gtloyehopd.html

[O03] 加锁保护共享数据
来源：http://hz.snrcjt.cn/gtggplxxhc.html

Py:   with lock: shared += 1
来源：http://hz.kuanghao11.cn/gtgbzhspqu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jqgfzy.top/gtvzrlxkzi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jiagoushi.top/gtbkfhfmop.html

TS:   // 同 JS
来源：http://hz.c1oappe.top/gtmrstcyyo.html

Java: synchronized (this) { shared++; }
来源：http://hz.chenzaomai.com/gtpdnlrdpe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jlsjyb.cn/gtluywruab.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.sufxvd.cn/gtxeletpfo.html

C#:   lock (gate) { shared++; }
来源：http://hz.cucudq.cn/gthvyphjxs.html

[O04] 定义异步函数并等待
来源：http://hz.nwbrower.top/gtbcprugrg.html

Py:   async def f():⏎    await g()
来源：http://hz.zhongyouzk.top/gtaefgpthy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sysykeji.top/gtccerahyt.html

JS:   async function f() { await g(); }
来源：http://hz.ppjwa.cn/gtfpcutrir.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shangyingyoupin.top/gttqyjrema.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ybcxt.top/gtldghffiu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.chenjidiqi.icu/gtjcszacfh.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xingfuxueyuan.xyz/gtybclkkkj.html

C#:   async Task F() { await G(); }
来源：http://hz.yj20258.top/gtdnfytwwa.html

[O05] 并发执行并等待全部完成
来源：http://hz.ppjwa.cn/gtcwkkxfuf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yonumen.top/gtlovpxzbx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jqgfzy.top/gtynjjutlv.html

JS:   await Promise.all(tasks)
来源：http://hz.yangfankeji.com/gticxlwkjk.html

TS:   await Promise.all(tasks)
来源：http://hz.cqqwz.cn/gtvzshdtdy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.tian-w.cn/gtrkpxbpal.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhongyouzk.top/gtkodrybfm.html

Ruby: threads.map(&:join)
来源：http://hz.hongshengwenyu.top/gtniadkeve.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ydjk.org.cn/gtcngwfpya.html

[O06] 使用进程池
来源：http://hz.svipenyu.cn/gtvwwiyuap.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yj202588.top/gtdgefuqdj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.vqdsnc.cn/gtveoukoag.html

JS:   // child_process / cluster 模块
来源：http://hz.gzhubu.top/gtqfzmgtye.html

TS:   // child_process / cluster 模块
来源：http://hz.sxryk.cn/gtuzfndyay.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.vqdsnc.cn/gtunqrgssm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.haohaochexian.top/gtqyfovxqy.html

Ruby: // fork 块
来源：http://hz.daxiang520.top/gtcrdbkfru.html

C#:   Parallel.For
来源：http://hz.haohaochexian.top/gtvcxppwbn.html

================================================================================
来源：http://hz.cheryme.top/gtazytqklp.html

P. 常用工具函数
来源：http://hz.cheryme.top/gthhemlwum.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtarjyvekl.html

[P01] 生成 UUID
来源：http://hz.hywenlv.cn/gtfwzgffsv.html

Py:   str(uuid.uuid4())
来源：http://hz.jqgufenzy.top/gtgwaibtol.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.guannengcc.top/gtzivghgpb.html

JS:   crypto.randomUUID()
来源：http://hz.jqgufenzy.top/gtqhdyprun.html

TS:   crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtulqldsjy.html

Java: UUID.randomUUID().toString()
来源：http://hz.redwolf501.top/gtvwjcxtfs.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yongpay.top/gtvaepvcvv.html

Ruby: SecureRandom.uuid
来源：http://hz.jinghuilouyu.cn/gtqyjuinpf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.wangdashe.top/gtxzvbpxtv.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ybcxt.top/gtildvndzg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenlongwang.top/gtcuyeqsjg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gogol.net.cn/gtyejaxrgf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ybcxt.top/gtdqhrmzbu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.meibo888.top/gttsqmmewy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.pengpengdd.cyou/gtywavcehe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hammf.cn/gtbvxuaciz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.tanke756.top/gtyngglyok.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yj20258.top/gtqryvhjmi.html

[P03] 生成短随机字符串
来源：http://hz.mhx1999.top/gtwmshicbj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sufxvd.cn/gtsmfelann.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.redwolf501.top/gtzlnmhlyl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhixingplan.top/gtbnfmgobc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ywan-chungtsiang.top/gtdvvfagfw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hnqzz.top/gtxugtzaze.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yuxming.cn/gtxmywsxfw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yuanzhike.top/gtvckflodw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gzhubu.top/gttpflgbmd.html

[P04] 求长度
来源：http://hz.ydjk.org.cn/gtkaccpzwg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.redwolf501.top/gtmfmaponb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cqqwz.cn/gthlpsfmdt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jlsjyb.cn/gttvelshyd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.kuanghao11.cn/gtwyfpntpz.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yongpay.top/gtvyimphll.html

Go:   len(arr);  len(m)
来源：http://hz.jqgfzy.top/gtjthbvdii.html

Ruby: x.length;  x.size
来源：http://hz.xuanzx.com/gtbpmmcbni.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhixingplan.top/gtqbsitxja.html

[P05] 判断两个对象内容是否相等
来源：http://hz.redwolf501.top/gtjzueruzh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sysykeji.top/gtjoilywso.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.feifeiyinyue.top/gtddobzepm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ywan-chungtsiang.top/gtieqiyzne.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xziqi.cn/gtbcoxbcdk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.iojbl.cn/gtfrrixiek.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.pengpengdd.cyou/gtdnahkxer.html

Ruby: a == b
来源：http://hz.pycfn.com/gtlefxsfmd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gaohongyu789.top/gtjzgqpkkq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yuxming.cn/gtpjkbcqow.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhengqikj.top/gtmmblxrhb.html

PHP:  if (empty($x)) {}
来源：http://hz.xziqi.cn/gttcumpjaa.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ydzc1.top/gtphweszhi.html

TS:   if (x == null) {}
来源：http://hz.zhengqikj.top/gttpqririi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.kuanghao11.cn/gtjlkxqebs.html

Go:   if x == nil {}
来源：http://hz.shanyushiyangkeji.top/gtkveghslc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.iojbl.cn/gtvpyhdmad.html

C#:   if (x is null) {}
来源：http://hz.jqgfzy.top/gttvqmjaol.html

[P07] 防抖与节流
来源：http://hz.ybcxt.top/gtcmllkizz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jlsjyb.cn/gtdwuqawks.html


<!-- 参考信息 -->