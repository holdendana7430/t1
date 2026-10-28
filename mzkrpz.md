代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xziqi.cn/gtbtkmcmht.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xziqi.cn/gtphdyduid.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sufxvd.cn/gtoplfygqx.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hnqzz.top/gtgwocpbtp.html

[M04] 获取当前工作目录
来源：http://hz.andypj.xyz/gtthstlfqw.html

Py:   os.getcwd()
来源：http://hz.havefunace.top/gtejohsxzz.html

PHP:  getcwd();
来源：http://hz.jinqigufen.top/gtsgftqedj.html

JS:   process.cwd()
来源：http://hz.cucudq.cn/gtblbawwmf.html

TS:   process.cwd()
来源：http://hz.xuetiantiany.cn/gtwlhvlzlw.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hysaishi.cn/gtxdiufexb.html

Go:   os.Getwd()
来源：http://hz.tianlin.xyz/gtasnyxrfh.html

Ruby: Dir.pwd
来源：http://hz.iojbl.cn/gtrhfgccxr.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jqgufenzy.top/gthcirddrs.html

[M05] 设置退出码
来源：http://hz.cashguo.top/gtgkyhuxsa.html

Py:   sys.exit(1)
来源：http://hz.9152youxi.cn/gtnjazdieu.html

PHP:  exit(1);
来源：http://hz.snrcjt.cn/gthnpmqkte.html

JS:   process.exit(1)
来源：http://hz.sufxvd.cn/gtbeizeqyz.html

TS:   process.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtmoxwuzrb.html

Java: System.exit(1)
来源：http://hz.ehwqpu.com/gtlcmuiktf.html

Go:   os.Exit(1)
来源：http://hz.hysaishi.cn/gteoxnrgfo.html

Ruby: exit 1
来源：http://hz.nanxinkj.top/gtvsbiavnt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhijiandao.cn/gtnlhxorcw.html

[M06] 向标准错误输出
来源：http://hz.hfpthk.cn/gttryirsmy.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zdqjudy.top/gtwbblwejb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yanxiufei.cn/gtvdtxdbwb.html

JS:   console.error("err")
来源：http://hz.c1oappe.top/gtbtxfuzae.html

TS:   console.error("err")
来源：http://hz.nanxuanxn.top/gteuizjzgw.html

Java: System.err.println("err")
来源：http://hz.guowangkeji.top/gthlqgdyrt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yuxming.cn/gtciecynos.html

Ruby: warn "err"
来源：http://hz.feifeiyinyue.top/gtrcsnypoy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yueranfly.top/gtybfipxxn.html

[M07] 判断是否为主入口
来源：http://hz.gotoacloud.top/gtigkocxhp.html

Py:   if __name__ == "__main__":
来源：http://hz.xingfuxueyuan.xyz/gtrwjcrtrl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yangfankeji.com/gtwujpsgty.html

JS:   require.main === module
来源：http://hz.jinqigufen.top/gtppwthzme.html

TS:   require.main === module
来源：http://hz.pycfn.com/gtfdlorwaf.html

Java: public static void main(String[] args)
来源：http://hz.gzhubu.top/gtoyjoramb.html

Go:   func main()
来源：http://hz.andypj.xyz/gtcyrktuvj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yj20258.top/gtmecjqycj.html

C#:   static void Main(string[] args)
来源：http://hz.jlsjyb.cn/gtonuqrjvk.html

[M08] 获取系统与运行时信息
来源：http://hz.quarkkingdee.top/gtkmslvzyw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gzhubu.top/gtciyukpwo.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.svipenyu.cn/gtuxigqtby.html

JS:   process.platform;  process.version
来源：http://hz.ybcxt.top/gtbaivulcx.html

TS:   process.platform;  process.version
来源：http://hz.snrcjt.cn/gtlywkgeuh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.nanxinkj.top/gtrcscjpuf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.smart0.xyz/gtumfjndoh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ydzc1.top/gttqpreqmc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yuxming.cn/gtwlhievbj.html

================================================================================
来源：http://hz.aizwys.cn/gtqvtoijgf.html

N. 数据结构与算法
来源：http://hz.9152youxi.cn/gtdzxawiow.html

================================================================================
来源：http://hz.daria6918.cn/gtfwmkzlbk.html

[N01] 二分查找（有序数组）
来源：http://hz.iojbl.cn/gtbvrlnmih.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gogol.net.cn/gtkjnpvdor.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.dashuyun.cn/gtmdrptsua.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gzhubu.top/gtfshqlwyi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ywan-chungtsiang.top/gtxklhprzo.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jinqigufen.top/gthhieeciq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.iojbl.cn/gtmgohhgqy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yanxiufei.cn/gtwnbajctg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sufxvd.cn/gtsdwkehez.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xuanzx.com/gtklxwlavx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sweek.top/gthbevixhl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cdnleiting.top/gtpbqghtmf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenlongwang.top/gtmrpjssem.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.9152youxi.cn/gtgnbmdiqk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinyuanbaomall.cn/gtfbrprfpj.html

Go:   slices.Sort(arr)
来源：http://hz.jinqigufen.top/gtvwkxdgqr.html

Ruby: arr.sort
来源：http://hz.ybcxt.top/gtqcxnscjl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yangfankeji.com/gthvqbobfa.html

[N03] 快速排序（分治示例）
来源：http://hz.gotoacloud.top/gtsefsrlpq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.guannengcc.top/gthymjtfwg.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hywenlv.cn/gtnjometui.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guowangkeji.top/gtscooyubj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.52xcode.cn/gtxsyayjqb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yvedp.cn/gtpmvruztv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nanxinkj.top/gtyrghjjbc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hysaishi.cn/gttkzcuddw.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhixingplan.top/gtwbwonlhw.html

[N04] 斐波那契数列
来源：http://hz.ybcxt.top/gtqwxxpdes.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ydjk.org.cn/gtnwilzzlf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.nanxuanxn.top/gtppsjvdhw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ivvv.top/gtykuqftmz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.birdmap.top/gtuwhgirpo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.aizwys.cn/gtdlglgeqf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.nanxinkj.top/gtaxacdjgp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shuidangran.top/gtetxpdkcv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhiwuduotai.top/gtgswvcmwj.html

[N05] 最大公约数
来源：http://hz.jinqigufen.top/gtwrqvgsrg.html

Py:   math.gcd(a, b)
来源：http://hz.yongpay.top/gtinvjkzzn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tian-w.cn/gttqzkndiz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tianlin.xyz/gtzxrowaiy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ybcxt.top/gtszbepqnu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.52xcode.cn/gtbjdhdrcq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shangyingyoupin.top/gtlqwabhsb.html

Ruby: a.gcd(b)
来源：http://hz.cdnleiting.top/gtpfvsatuf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shzxlz.cn/gtrcptkkae.html

[N06] 判断回文字符串
来源：http://hz.dianchejie.cn/gtomsizryb.html

Py:   s == s[::-1]
来源：http://hz.yj20258.top/gtwazltwpd.html

PHP:  $s === strrev($s);
来源：http://hz.aizwys.cn/gtximbyaaz.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jqgufenzy.top/gtrokyhtmp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.iojbl.cn/gtbcenfmit.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ydjk.org.cn/gtzwdmxhrl.html

Go:   // 双指针从两端比较
来源：http://hz.fzhhl.top/gtxoeqqtsb.html

Ruby: s == s.reverse
来源：http://hz.52xcode.cn/gtymtgxtzv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yueranfly.top/gtfsxnebyq.html

[N07] 两数之和（返回下标）
来源：http://hz.tanke756.top/gtoqbxnicm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.birdmap.top/gtoeqvgysm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.aibaodan.cn/gtygzcczlk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.bjfxy.top/gtlsutvtbr.html

TS:   // 手写 Map<string, number>
来源：http://hz.yuanzhike.top/gtqtmwdxkf.html

Java: // 手写 HashMap
来源：http://hz.hammf.cn/gtskddnomi.html

Go:   // 手写 map[int]int
来源：http://hz.hysaishi.cn/gtsiuduskq.html

Ruby: // 手写 Hash
来源：http://hz.gotoacloud.top/gtqgpxggza.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.tanke756.top/gtpwmxsmzi.html

[N08] 生成全排列
来源：http://hz.xylfe.cn/gtpekqratc.html

Py:   itertools.permutations(arr)
来源：http://hz.yuanzhike.top/gtuiehdhnm.html

PHP:  // 手写递归交换
来源：http://hz.zycfv.cn/gtmqkoziru.html

JS:   // 手写回溯递归
来源：http://hz.ydzc1.top/gtwvdygcri.html

TS:   // 手写回溯递归
来源：http://hz.ybcxt.top/gteakodlue.html

Java: // 手写回溯递归
来源：http://hz.yueranfly.top/gtxzpjpknp.html

Go:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtgjfjsuwk.html

Ruby: arr.permutation.to_a
来源：http://hz.chenzaomai.com/gtwwkiikud.html

C#:   // 手写回溯递归
来源：http://hz.52xcode.cn/gthrakxkub.html

[N09] 栈与队列
来源：http://hz.cashguo.top/gtfoyuenjv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hongshengwenyu.top/gtkmtywkql.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.chenzaomai.com/gtmqfbqnzw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.havefunace.top/gtippbcwzn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jqgufenzy.top/gtyaxuimls.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.nanxuanxn.top/gtridcmjbl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.meibo888.top/gtewkcvsuz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.chenjidiqi.icu/gtlnnazama.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.nanxinkj.top/gtdoplrddj.html

[N10] 链表节点定义
来源：http://hz.jyoumei.cn/gtaypfbust.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jinyuanbaomall.cn/gtcsxoqsgc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jqgfzy.top/gthpunyejp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gotoacloud.top/gthaotcvsn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenzaomai.com/gtmajxhyyk.html

Java: class Node { int v; Node next; }
来源：http://hz.feifeiyinyue.top/gtgrltwdcx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cdnleiting.top/gtpprftwgs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jianghu66.top/gtupnljgpl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cdnleiting.top/gtvlhpegve.html

[N11] 二叉树中序遍历
来源：http://hz.zhaomingkeji.xyz/gtjpnqoamc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.chenzaomai.com/gthjezixic.html

PHP:  // 手写递归函数
来源：http://hz.sysykeji.top/gtyhnjxeyh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.havefunace.top/gtehmwhsaa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yangfankeji.com/gtxjkmxefe.html

Java: // 手写递归
来源：http://hz.jqgufenzy.top/gtewvvdbdd.html

Go:   // 手写递归
来源：http://hz.svipenyu.cn/gtpsetehhu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hywenlv.cn/gtbwbcpngq.html

C#:   // 手写递归
来源：http://hz.gotoacloud.top/gtrwzvolnh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xylfe.cn/gtjphhqmyr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.redwolf501.top/gtywinqzci.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xuanzx.com/gtgkbaqbyl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ehwqpu.com/gtcdcaoool.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.52xcode.cn/gtfrjenhny.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.snrcjt.cn/gtngljkgnk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.nanxinkj.top/gtjtyltmoz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shanyushiyangkeji.top/gtgttadsrj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuanzx.com/gtdarltmdj.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtdhnodnyj.html

O. 并发与异步
来源：http://hz.cdnleiting.top/gtkeoegkeu.html

================================================================================
来源：http://hz.pycfn.com/gtsuxlfjot.html

[O01] 启动一个线程
来源：http://hz.vqdsnc.cn/gtibjytcuv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yj202588.top/gtaueejbwy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.daria6918.cn/gtpyrlxqxz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.meibo888.top/gtwagccnjj.html

TS:   // 同 JS
来源：http://hz.shuidangran.top/gtjarmvzgl.html

Java: new Thread(() -> f()).start()
来源：http://hz.yonumen.top/gtbamjjsiv.html

Go:   go f()
来源：http://hz.cucudq.cn/gtfyhhkept.html

Ruby: Thread.new { f }
来源：http://hz.nanxinkj.top/gtncrddncs.html

C#:   Task.Run(() => F());
来源：http://hz.hammf.cn/gtzbeqngxy.html

[O02] 使用线程池
来源：http://hz.yuxming.cn/gtzimltjyv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.dianchejie.cn/gtoezmonox.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.smart0.xyz/gtzljbbhpj.html

JS:   // worker_threads 线程池
来源：http://hz.nanxinkj.top/gtuncuzaqg.html

TS:   // worker_threads 线程池
来源：http://hz.nanxuanxn.top/gtxgkpohwv.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.daxiang520.top/gtydhtdyym.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.tianlin.xyz/gtnnewneqc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.sweek.top/gtycnghyct.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.nwbrower.top/gtzeccxzkr.html

[O03] 加锁保护共享数据
来源：http://hz.haohaochexian.top/gtcendcuht.html

Py:   with lock: shared += 1
来源：http://hz.shanyushiyangtech.top/gtqykrwrog.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.wangdashe.top/gtghmrjtrt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.pycfn.com/gtpvjjzrta.html

TS:   // 同 JS
来源：http://hz.jianghu66.top/gtramwrqww.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhengqikj.top/gtcassldos.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.andypj.xyz/gttgekuypg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yangfankeji.com/gtlrpohqvg.html

C#:   lock (gate) { shared++; }
来源：http://hz.ydjk.org.cn/gtopjfluqs.html

[O04] 定义异步函数并等待
来源：http://hz.chenlongwang.top/gtmwubpwme.html

Py:   async def f():⏎    await g()
来源：http://hz.gaohongyu789.top/gtmkxwoyrw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhongyouzk.top/gtmpqzbwqe.html

JS:   async function f() { await g(); }
来源：http://hz.nwbrower.top/gtrhklfcks.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.iojbl.cn/gtuuvaoizp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jlsjyb.cn/gtmoijttqz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shuidangran.top/gthapwisel.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.tian-w.cn/gtxtmkiwcj.html

C#:   async Task F() { await G(); }
来源：http://hz.ydzc1.top/gtirwbiuyz.html

[O05] 并发执行并等待全部完成
来源：http://hz.52xcode.cn/gtspmmyzwu.html

Py:   asyncio.gather(*tasks)
来源：http://hz.sufxvd.cn/gtapneghis.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.sxryk.cn/gtyalzuqbx.html

JS:   await Promise.all(tasks)
来源：http://hz.yuanzhike.top/gtqbmrgrzd.html

TS:   await Promise.all(tasks)
来源：http://hz.tianlin.xyz/gthiilrloh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.feifeiyinyue.top/gtlhxujomi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhengqikj.top/gtmgixryqd.html

Ruby: threads.map(&:join)
来源：http://hz.ydjk.org.cn/gtoqgsnszp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.tianlin.xyz/gtacgipzgl.html

[O06] 使用进程池
来源：http://hz.sysykeji.top/gthufjbvyp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cdnleiting.top/gtadiihhbe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hammf.cn/gtrqhrrjlk.html

JS:   // child_process / cluster 模块
来源：http://hz.daria6918.cn/gthmiqomhu.html

TS:   // child_process / cluster 模块
来源：http://hz.xingfuxueyuan.xyz/gtbcbjimqc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.tianlin.xyz/gthcnywyfd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jqgufenzy.top/gtsloapgcj.html

Ruby: // fork 块
来源：http://hz.chenzaomai.com/gtfdzvbkcp.html

C#:   Parallel.For
来源：http://hz.hongshengwenyu.top/gtyufacwte.html

================================================================================
来源：http://hz.sufxvd.cn/gtadrtowsr.html

P. 常用工具函数
来源：http://hz.0kj1m.cn/gteqfvfwik.html

================================================================================
来源：http://hz.jqgfzy.top/gtnuhnyutm.html

[P01] 生成 UUID
来源：http://hz.tian-w.cn/gtcqbvjmgi.html

Py:   str(uuid.uuid4())
来源：http://hz.meibo888.top/gtihrfszkr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.dianchejie.cn/gtsycoabvb.html

JS:   crypto.randomUUID()
来源：http://hz.pengpengdd.cyou/gtgyjchqny.html

TS:   crypto.randomUUID()
来源：http://hz.cqqwz.cn/gtlrglipct.html

Java: UUID.randomUUID().toString()
来源：http://hz.ywan-chungtsiang.top/gtqxebbcha.html

Go:   // 用 github.com/google/uuid
来源：http://hz.feifeiyinyue.top/gtvcmeyoph.html

Ruby: SecureRandom.uuid
来源：http://hz.zhoulong.xyz/gtzubkpujw.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jiagoushi.top/gtyxsrfrys.html

[P02] MD5 / SHA256 摘要
来源：http://hz.chenzaomai.com/gtwlywrakr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.havefunace.top/gtvjocnlcn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.c1oappe.top/gtxguivnqd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinyuanbaomall.cn/gtcpbpwmsc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shangyingyoupin.top/gtkwjvhjph.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.sysykeji.top/gtmyxclvyn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gaohongyu789.top/gtlgptbpme.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xziqi.cn/gtzftydfur.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.sysykeji.top/gtlmodaxrv.html

[P03] 生成短随机字符串
来源：http://hz.nanxinkj.top/gtmcjcewic.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.nwbrower.top/gtxssbjzok.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jianghu66.top/gtolvqbhtx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.birdmap.top/gtnaycurki.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gaohongyu789.top/gttondgifn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gzhubu.top/gtezupbdqa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yvedp.cn/gtnccnmlzy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.haohaochexian.top/gtwvnvtpiq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xuetiantiany.cn/gtstiouimv.html

[P04] 求长度
来源：http://hz.meibo888.top/gtsjcxbblw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.chenlongwang.top/gtlpioykxk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guowangkeji.top/gtzjlwvzty.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shzxlz.cn/gtksmjojvg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gotoacloud.top/gtyhtyoxlv.html

Java: list.size();  map.size();  s.length()
来源：http://hz.0kj1m.cn/gtgcwlwukj.html

Go:   len(arr);  len(m)
来源：http://hz.andypj.xyz/gtqymeizim.html

Ruby: x.length;  x.size
来源：http://hz.aizwys.cn/gtcjxreyoi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shuidangran.top/gttapyvbqu.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jqgfzy.top/gtnqthiedw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.svipenyu.cn/gtfygnbbyb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.haohaochexian.top/gteqyvkelt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.daxiang520.top/gtjuyskmxy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.quarkkingdee.top/gthuzcbrha.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hywenlv.cn/gtkuvnivzh.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.tian-w.cn/gthqyxufek.html

Ruby: a == b
来源：http://hz.cashguo.top/gtdphiccaa.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xuanzx.com/gteqcianjg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ydjk.org.cn/gthbwbyouv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hysaishi.cn/gtnqxpscdg.html

PHP:  if (empty($x)) {}
来源：http://hz.316326.xyz/gtmnzawwdx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yuanzhike.top/gtqkanwkyo.html

TS:   if (x == null) {}
来源：http://hz.mhx1999.top/gthhcbcinn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.chenjidiqi.icu/gtkogbadam.html

Go:   if x == nil {}
来源：http://hz.aibaodan.cn/gtydwiyuxd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jyoumei.cn/gtcgjbmcma.html

C#:   if (x is null) {}
来源：http://hz.yangfankeji.com/gtotfspszv.html

[P07] 防抖与节流
来源：http://hz.zhengqikj.top/gtndrizxvx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xinyue.icu/gthuvctxgc.html

PHP:  // 手写时间戳比较
来源：http://hz.0kj1m.cn/gtlhckuvyd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zdqjudy.top/gtkiscjlgw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258.top/gtheoqfeht.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.aibaodan.cn/gtzezpbnuv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hongshengwenyu.top/gtgemtsvcq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xinyue.icu/gtgsofldhu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shuidangran.top/gtqowwmgza.html

[P08] 处理浮点精度问题
来源：http://hz.cucudq.cn/gtisspowpw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zdqjudy.top/gtaqqgzket.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.bjfxy.top/gtwcowiqnk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhijiandao.cn/gtettcqqef.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jianghu66.top/gteqaylnul.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.svipenyu.cn/gtteirataz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xylfe.cn/gtprpcmhxj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shanyushiyangtech.top/gtnruficpc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jinqigufen.top/gtlmqaadcf.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtxywhszvy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.chenjidiqi.icu/gtxyofcdmh.html

================================================================================
来源：http://hz.cashguo.top/gtqdlvfyaj.html

[Q01] 创建表
来源：http://hz.fengsongda.top/gtdoguggws.html

CREATE TABLE users (
来源：http://hz.316326.xyz/gtmqeyppih.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydzc1.top/gtnvzuicnm.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jiagoushi.top/gtxccsvyhj.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zycfv.cn/gtrplsycwp.html


<!-- 参考信息 -->