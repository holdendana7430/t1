代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.feifeiyinyue.top/gttcqtodbu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hfpthk.cn/gtzlyhnkop.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jlsjyb.cn/gtbswfkdnc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shangyingyoupin.top/gtobbxcafb.html

[M04] 获取当前工作目录
来源：http://hz.yj202588.top/gttwznzkpg.html

Py:   os.getcwd()
来源：http://hz.zhijiandao.cn/gtesicdqzf.html

PHP:  getcwd();
来源：http://hz.tianlin.xyz/gtzaaqukam.html

JS:   process.cwd()
来源：http://hz.chenzaomai.com/gteuowzvqt.html

TS:   process.cwd()
来源：http://hz.zhongyouzk.top/gthkmqpmhd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yongpay.top/gtxgashcag.html

Go:   os.Getwd()
来源：http://hz.quarkkingdee.top/gtvbsigruy.html

Ruby: Dir.pwd
来源：http://hz.c1oappe.top/gtvuwqluaw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.daria6918.cn/gtgbmkzrjl.html

[M05] 设置退出码
来源：http://hz.nanxuanxn.top/gttyuakjea.html

Py:   sys.exit(1)
来源：http://hz.birdmap.top/gtipchaphx.html

PHP:  exit(1);
来源：http://hz.aibaodan.cn/gtwmidopxs.html

JS:   process.exit(1)
来源：http://hz.zycfv.cn/gtpfajahai.html

TS:   process.exit(1)
来源：http://hz.jianghu66.top/gtdlzqiyku.html

Java: System.exit(1)
来源：http://hz.shangyingyoupin.top/gtutgtoxzs.html

Go:   os.Exit(1)
来源：http://hz.hnqzz.top/gtxywzxtzl.html

Ruby: exit 1
来源：http://hz.hywenlv.cn/gtrsxqnosw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.tianlin.xyz/gtlzoeilxq.html

[M06] 向标准错误输出
来源：http://hz.fengsongda.top/gtswadvnzp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinqigfzy.top/gthnfdfnwz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.daria6918.cn/gtijiptnrn.html

JS:   console.error("err")
来源：http://hz.fzhhl.top/gtgfqyqmhm.html

TS:   console.error("err")
来源：http://hz.daria6918.cn/gteobivbsn.html

Java: System.err.println("err")
来源：http://hz.birdmap.top/gteusxzwow.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhaomingkeji.xyz/gtlpwykbeq.html

Ruby: warn "err"
来源：http://hz.zhongyouzk.top/gthdzibjim.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xziqi.cn/gtrddjjlja.html

[M07] 判断是否为主入口
来源：http://hz.chenzaomai.com/gtaewajpff.html

Py:   if __name__ == "__main__":
来源：http://hz.xinyue.icu/gtwkpzopti.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cqqwz.cn/gtfqgmeshl.html

JS:   require.main === module
来源：http://hz.yvedp.cn/gtlxfbdock.html

TS:   require.main === module
来源：http://hz.sysykeji.top/gtncqkibga.html

Java: public static void main(String[] args)
来源：http://hz.hnxiangtu.top/gtanjzwnhh.html

Go:   func main()
来源：http://hz.jinyuanbaomall.cn/gttrflwakz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.fzhhl.top/gtjgudpwun.html

C#:   static void Main(string[] args)
来源：http://hz.zhixingplan.top/gtidedjqnz.html

[M08] 获取系统与运行时信息
来源：http://hz.52xcode.cn/gtbjgyiqhb.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhixingplan.top/gtuolmjbwc.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yvedp.cn/gtjrhtapqj.html

JS:   process.platform;  process.version
来源：http://hz.fzhhl.top/gtodmbduxb.html

TS:   process.platform;  process.version
来源：http://hz.andypj.xyz/gtuvuwcmvp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.aizwys.cn/gtlnfquvnf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ivvv.top/gtmvzjipvk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.chenlongwang.top/gtncdwklma.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yvedp.cn/gtakgusahx.html

================================================================================
来源：http://hz.tanke756.top/gtgiuymumv.html

N. 数据结构与算法
来源：http://hz.ppjwa.cn/gtpgoxqzhp.html

================================================================================
来源：http://hz.hywenlv.cn/gtbanetfhp.html

[N01] 二分查找（有序数组）
来源：http://hz.sweek.top/gtsfaujvdp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.0kj1m.cn/gtunavmviu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jqgufenzy.top/gttlnxkqnh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.mhx1999.top/gtqvgipgfg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgfzy.top/gtxfnchegq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhiwuduotai.top/gtzsmdczva.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.tian-w.cn/gtokaybvbd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jiagoushi.top/gtxylhxsvd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.wangdashe.top/gtxnvvsqjh.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cdnleiting.top/gtlbmtlyty.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gogol.net.cn/gtnvcfevhn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.0kj1m.cn/gtoejvjdxq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.pycfn.com/gtjuvohegi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xinyue.icu/gtpzuvibno.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yj20258888.top/gtrkbqqlyz.html

Go:   slices.Sort(arr)
来源：http://hz.vqdsnc.cn/gtaooguqmx.html

Ruby: arr.sort
来源：http://hz.jyoumei.cn/gtwgflizmy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhijiandao.cn/gtwuklglrg.html

[N03] 快速排序（分治示例）
来源：http://hz.jinqigfzy.top/gtgolcueao.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gogol.net.cn/gtcjuzcucm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yanxiufei.cn/gtpezfztfb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.vqdsnc.cn/gtsfcjgfze.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shzxlz.cn/gtwfvoeweg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yuxming.cn/gtqdioccjs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jqgfzy.top/gtcmolrlnl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenzaomai.com/gtemuzsxcd.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zdqjudy.top/gtfmrwdzjd.html

[N04] 斐波那契数列
来源：http://hz.ppjwa.cn/gtunjartcc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jqgufenzy.top/gtcbsxmlli.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.aizwys.cn/gtjwelhcyx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhijiandao.cn/gtroyivfln.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.c1oappe.top/gtduzmndxe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cdnleiting.top/gtfomzatuw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gogol.net.cn/gtttyxtvkd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigfzy.top/gtguhssdvy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.dianchejie.cn/gtajblmvyn.html

[N05] 最大公约数
来源：http://hz.hysaishi.cn/gtfyegvhmf.html

Py:   math.gcd(a, b)
来源：http://hz.vqdsnc.cn/gtaotrcwrp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhixingplan.top/gturohcraf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yuxming.cn/gtcgmxywmc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydzc1.top/gtpwefhhjs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gogol.net.cn/gtccosezfj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhijiandao.cn/gtgjjohymf.html

Ruby: a.gcd(b)
来源：http://hz.yuxming.cn/gtkyhgebcg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yvedp.cn/gtfxtqlcro.html

[N06] 判断回文字符串
来源：http://hz.nwbrower.top/gtthbzuejq.html

Py:   s == s[::-1]
来源：http://hz.wangdashe.top/gthcynuudw.html

PHP:  $s === strrev($s);
来源：http://hz.tianlin.xyz/gtvumhprca.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtgjmrbmcq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.feifeiyinyue.top/gtfutcoqoh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.dashuyun.cn/gtqrqcoqkp.html

Go:   // 双指针从两端比较
来源：http://hz.hywenlv.cn/gttmchfvxg.html

Ruby: s == s.reverse
来源：http://hz.yj20258.top/gtfvsqpnvy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhengqikj.top/gtijzsbktp.html

[N07] 两数之和（返回下标）
来源：http://hz.havefunace.top/gtthobknrp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhengqikj.top/gttrzdliqe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yuanzhike.top/gtujbpsphk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ppjwa.cn/gtxsnzrvvd.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhengqikj.top/gtcftqhznv.html

Java: // 手写 HashMap
来源：http://hz.wangdashe.top/gtvxajdgou.html

Go:   // 手写 map[int]int
来源：http://hz.jiagoushi.top/gtxksvukbf.html

Ruby: // 手写 Hash
来源：http://hz.52xcode.cn/gtvrguvuay.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yueranfly.top/gtftcqcekc.html

[N08] 生成全排列
来源：http://hz.yuxming.cn/gtswrtknvq.html

Py:   itertools.permutations(arr)
来源：http://hz.zhengqikj.top/gtmtdegxwr.html

PHP:  // 手写递归交换
来源：http://hz.ydzc1.top/gtktaqnrca.html

JS:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtqqpwharr.html

TS:   // 手写回溯递归
来源：http://hz.jqgfzy.top/gtcznidbqh.html

Java: // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtodpsurfy.html

Go:   // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtqhigmcjt.html

Ruby: arr.permutation.to_a
来源：http://hz.yuanzhike.top/gtliyxwgze.html

C#:   // 手写回溯递归
来源：http://hz.guowangkeji.top/gtsyflsocd.html

[N09] 栈与队列
来源：http://hz.xuanzx.com/gtuvzyqcii.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yueranfly.top/gtjxtzdjtc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ppjwa.cn/gtsaaectot.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.chenlongwang.top/gtfxvjiysq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.redwolf501.top/gtfbnujjdd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.316326.xyz/gtdygjofws.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.bjfxy.top/gtyqxukygn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.mhx1999.top/gtelcbjzsf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ehwqpu.com/gtxlnencgy.html

[N10] 链表节点定义
来源：http://hz.shuidangran.top/gtgwdmhvxi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.aizwys.cn/gtnxljwgud.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.smart0.xyz/gtfhoaqgmj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.fzhhl.top/gtqiflwhkq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ivvv.top/gtyyljglyn.html

Java: class Node { int v; Node next; }
来源：http://hz.0kj1m.cn/gtejexnngi.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shangyingyoupin.top/gtegaoqycf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinghuilouyu.cn/gtkfqxshdc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.sweek.top/gtvwrlfohm.html

[N11] 二叉树中序遍历
来源：http://hz.jinqigfzy.top/gtdjbkxjob.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.52xcode.cn/gtzdgdwahe.html

PHP:  // 手写递归函数
来源：http://hz.zdqjudy.top/gtfzqnpqah.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnqzz.top/gtrkwpvcqs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinqigufen.top/gtxymtqwyi.html

Java: // 手写递归
来源：http://hz.pycfn.com/gtqocgdzpf.html

Go:   // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtzirxynmz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.sweek.top/gtzaoytyuf.html

C#:   // 手写递归
来源：http://hz.chenjidiqi.icu/gtfwdgmbpi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.svipenyu.cn/gtaycgqsbj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.guowangkeji.top/gtirvhmsvg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhoulong.xyz/gtblgdtlrq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangshuangyany.cn/gtoicnfrur.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhoulong.xyz/gtioehpums.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zycfv.cn/gtveslxtvr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.pycfn.com/gtiifqmlnl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cqqwz.cn/gtzsdnpurn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhiwuduotai.top/gtdziodkyt.html

================================================================================
来源：http://hz.aibaodan.cn/gtpghobjjw.html

O. 并发与异步
来源：http://hz.jinqigufen.top/gtintozevd.html

================================================================================
来源：http://hz.hnxiangtu.top/gtuvamehyn.html

[O01] 启动一个线程
来源：http://hz.yueranfly.top/gtzqzyncvi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gzhubu.top/gtfxlumgrx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.feifeiyinyue.top/gtchmfwcgc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhongyouzk.top/gttbloqhfd.html

TS:   // 同 JS
来源：http://hz.smart0.xyz/gtkyikalmx.html

Java: new Thread(() -> f()).start()
来源：http://hz.xuanzx.com/gtxrayxeho.html

Go:   go f()
来源：http://hz.meibo888.top/gtymljcnpx.html

Ruby: Thread.new { f }
来源：http://hz.yanxiufei.cn/gtgcsoihny.html

C#:   Task.Run(() => F());
来源：http://hz.yj20258.top/gtusvlycqp.html

[O02] 使用线程池
来源：http://hz.iojbl.cn/gtkcliddxb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.wangdashe.top/gtbhwdnpcz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.birdmap.top/gtdsehifls.html

JS:   // worker_threads 线程池
来源：http://hz.zhoulong.xyz/gtsbumagza.html

TS:   // worker_threads 线程池
来源：http://hz.hongshengwenyu.top/gtefpgpigx.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.tanke756.top/gtgvppwpis.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ywan-chungtsiang.top/gtawoltjpa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.tianlin.xyz/gtyhonfsuu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.kuanghao11.cn/gtjgiylkdm.html

[O03] 加锁保护共享数据
来源：http://hz.hnxiangtu.top/gtvdinokfx.html

Py:   with lock: shared += 1
来源：http://hz.shanyushiyangtech.top/gtlurjipht.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ybcxt.top/gthpkvplxy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.tanke756.top/gtdfpqzday.html

TS:   // 同 JS
来源：http://hz.sysykeji.top/gthwadbeep.html

Java: synchronized (this) { shared++; }
来源：http://hz.quarkkingdee.top/gtmmqqhkyi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhoulong.xyz/gtuzojqlrd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yj20258888.top/gtuzqmkunq.html

C#:   lock (gate) { shared++; }
来源：http://hz.yuanzhike.top/gtolpgtlhm.html

[O04] 定义异步函数并等待
来源：http://hz.52xcode.cn/gtusyyxsyg.html

Py:   async def f():⏎    await g()
来源：http://hz.xinyue.icu/gtqfncklih.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cdnleiting.top/gtkbiokobr.html

JS:   async function f() { await g(); }
来源：http://hz.haohaochexian.top/gtuedlhvva.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yj20258888.top/gtvuqpsayw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yongpay.top/gtpjxsercq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jinghuilouyu.cn/gtjhyknrbh.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hfpthk.cn/gttubpmewq.html

C#:   async Task F() { await G(); }
来源：http://hz.chenlongwang.top/gtksjellar.html

[O05] 并发执行并等待全部完成
来源：http://hz.sweek.top/gthizfcoip.html

Py:   asyncio.gather(*tasks)
来源：http://hz.svipenyu.cn/gtzicajred.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.nanxinkj.top/gtcrvdxeyu.html

JS:   await Promise.all(tasks)
来源：http://hz.hywenlv.cn/gtdfcmdqbv.html

TS:   await Promise.all(tasks)
来源：http://hz.shangyingyoupin.top/gtkwryflui.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.birdmap.top/gtpsntdcpd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.quarkkingdee.top/gtlzwnnmuk.html

Ruby: threads.map(&:join)
来源：http://hz.cqqwz.cn/gttztrewdt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.snrcjt.cn/gtyaofgryx.html

[O06] 使用进程池
来源：http://hz.sysykeji.top/gtwpxtpbwb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cucudq.cn/gtqklywcep.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ydjk.org.cn/gtqhxpqary.html

JS:   // child_process / cluster 模块
来源：http://hz.ehwqpu.com/gtzmfarnuh.html

TS:   // child_process / cluster 模块
来源：http://hz.zhixingplan.top/gtqirrrkch.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinghuilouyu.cn/gtvbklnohi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.316326.xyz/gtuxlscsjb.html

Ruby: // fork 块
来源：http://hz.9152youxi.cn/gtkodhwpjl.html

C#:   Parallel.For
来源：http://hz.yonumen.top/gtfkejzcee.html

================================================================================
来源：http://hz.havefunace.top/gtrmszsjxf.html

P. 常用工具函数
来源：http://hz.gotoacloud.top/gtfpaixngi.html

================================================================================
来源：http://hz.yuxming.cn/gtdvphdyqr.html

[P01] 生成 UUID
来源：http://hz.cheryme.top/gtabymboac.html

Py:   str(uuid.uuid4())
来源：http://hz.ivvv.top/gtvebfrntq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zycfv.cn/gtrpyrnujo.html

JS:   crypto.randomUUID()
来源：http://hz.hysaishi.cn/gtcywljhzf.html

TS:   crypto.randomUUID()
来源：http://hz.zhaomingkeji.xyz/gtlfhnzvzl.html

Java: UUID.randomUUID().toString()
来源：http://hz.jinyuanbaomall.cn/gtenxijqep.html

Go:   // 用 github.com/google/uuid
来源：http://hz.bjfxy.top/gtmvjwjdld.html

Ruby: SecureRandom.uuid
来源：http://hz.jqgufenzy.top/gtmkufmzfj.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinqigfzy.top/gtfrakuoxf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.daxiang520.top/gtiwsrvceo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ydjk.org.cn/gtazsacqqi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinqigufen.top/gtltazhzgo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinqigfzy.top/gtvphbjfmw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.redwolf501.top/gtramldltw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.daxiang520.top/gtzrmmszts.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.birdmap.top/gtvxtnhjso.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.shanyushiyangtech.top/gtutcoimtt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xingfuxueyuan.xyz/gtiwszbiok.html

[P03] 生成短随机字符串
来源：http://hz.bjfxy.top/gtjrqetpwe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhiwuduotai.top/gtgeoshayl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.sxryk.cn/gtopnrwcde.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.vqdsnc.cn/gtusxghkii.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.9152youxi.cn/gtsinymaev.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.haohaochexian.top/gtdjzqxace.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jinyuanbaomall.cn/gtaczscqur.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yj202588.top/gtsvnjpvxn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xuetiantiany.cn/gtqscdfwwt.html

[P04] 求长度
来源：http://hz.havefunace.top/gtlvevdpiw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.birdmap.top/gtrigbgrgg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pengpengdd.cyou/gtnapvamzs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jianghu66.top/gtlfrlkpot.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jiagoushi.top/gtxuuqbmda.html

Java: list.size();  map.size();  s.length()
来源：http://hz.dashuyun.cn/gtwldtxyob.html

Go:   len(arr);  len(m)
来源：http://hz.ywan-chungtsiang.top/gtvhpcacnd.html

Ruby: x.length;  x.size
来源：http://hz.jinqigufen.top/gtlxevpgel.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.nanxuanxn.top/gtbifbyqzw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.tian-w.cn/gtnrvptzod.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cheryme.top/gtawffhyan.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.guannengcc.top/gtvsrsgejd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.meibo888.top/gtkrokpvhb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.nwbrower.top/gtlduieskc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.nanxuanxn.top/gtmqtdhkuq.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yuanzhike.top/gtyollorzb.html

Ruby: a == b
来源：http://hz.cdnleiting.top/gtcgzjvytd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.pycfn.com/gthevanfqe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhongyouzk.top/gtmmfopifg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hywenlv.cn/gtbieckgpf.html

PHP:  if (empty($x)) {}
来源：http://hz.cheryme.top/gtavzutpjz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yuanzhike.top/gtwcqczawi.html

TS:   if (x == null) {}
来源：http://hz.fzhhl.top/gtfqimxlql.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.daxiang520.top/gtdsnynztb.html

Go:   if x == nil {}
来源：http://hz.jqgfzy.top/gtzzydjroh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.sysykeji.top/gtltrnlbow.html

C#:   if (x is null) {}
来源：http://hz.haohaochexian.top/gtfhjxqyav.html

[P07] 防抖与节流
来源：http://hz.gogol.net.cn/gtlervcxzf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yuxming.cn/gtdvlfwztk.html

PHP:  // 手写时间戳比较
来源：http://hz.sysykeji.top/gtnlzaradv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.bjfxy.top/gthlosbnyx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sxryk.cn/gtvypzgowy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhoulong.xyz/gtyqfagxzv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.tian-w.cn/gthrwyrxng.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.pycfn.com/gthkifrrhf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hnqzz.top/gtgvogudxo.html

[P08] 处理浮点精度问题
来源：http://hz.sweek.top/gtxscdwybf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.feifeiyinyue.top/gttspkkhea.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yuanzhike.top/gtywmymosf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.wangshuangyany.cn/gtsdvbjwsd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.gogol.net.cn/gtniysfbfg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gaohongyu789.top/gtdrdfilac.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hnxiangtu.top/gtlsavcydw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.aizwys.cn/gtygdugdfp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.havefunace.top/gtqzwjpdwb.html

================================================================================
来源：http://hz.smart0.xyz/gtoxbtonaz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.daria6918.cn/gtpdxevnfc.html

================================================================================
来源：http://hz.tianlin.xyz/gtdnvijvtk.html

[Q01] 创建表
来源：http://hz.cashguo.top/gtfelyxpzl.html

CREATE TABLE users (
来源：http://hz.fengsongda.top/gtsrsnwiwv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xziqi.cn/gtbogwfory.html

name VARCHAR(50) NOT NULL,
来源：http://hz.52xcode.cn/gtsvclvcfw.html

email VARCHAR(100) UNIQUE,
来源：http://hz.haohaochexian.top/gtzrgvkzfs.html


<!-- 参考信息 -->