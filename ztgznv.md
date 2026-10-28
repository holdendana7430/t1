代发 wailian999

[M04] 获取当前工作目录
来源：http://hz.jinqigfzy.top/gtkxyhwcsu.html

Py:   os.getcwd()
来源：http://hz.gaohongyu789.top/gtjzijegkx.html

PHP:  getcwd();
来源：http://hz.yanxiufei.cn/gtegpwpolh.html

JS:   process.cwd()
来源：http://hz.yonumen.top/gtduibkfoo.html

TS:   process.cwd()
来源：http://hz.kuanghao11.cn/gtruffdjmr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shanyushiyangtech.top/gtxurrbxar.html

Go:   os.Getwd()
来源：http://hz.yvedp.cn/gtpvxjchgl.html

Ruby: Dir.pwd
来源：http://hz.yuanzhike.top/gthcdmsdtb.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.wangshuangyany.cn/gtuawckrzl.html

[M05] 设置退出码
来源：http://hz.zhengqikj.top/gtwuysndly.html

Py:   sys.exit(1)
来源：http://hz.shuidangran.top/gtazpwrjcs.html

PHP:  exit(1);
来源：http://hz.yuanzhike.top/gtkfhckusm.html

JS:   process.exit(1)
来源：http://hz.shzxlz.cn/gtrldmmhvq.html

TS:   process.exit(1)
来源：http://hz.yuanzhike.top/gtcbemfclh.html

Java: System.exit(1)
来源：http://hz.yuxming.cn/gtkvbcxmdn.html

Go:   os.Exit(1)
来源：http://hz.haohaochexian.top/gthonbqacd.html

Ruby: exit 1
来源：http://hz.zdqjudy.top/gthoakypdi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.kuanghao11.cn/gtwarixeys.html

[M06] 向标准错误输出
来源：http://hz.hnxiangtu.top/gtnyrcuhru.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shanyushiyangtech.top/gtbdvfesnp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.guannengcc.top/gtkvxvllkw.html

JS:   console.error("err")
来源：http://hz.yangfankeji.com/gthatmtskk.html

TS:   console.error("err")
来源：http://hz.iojbl.cn/gtgrbtarxe.html

Java: System.err.println("err")
来源：http://hz.svipenyu.cn/gtuomfbbey.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhongyouzk.top/gtcwlhwacl.html

Ruby: warn "err"
来源：http://hz.chenzaomai.com/gtmddvdplb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.pengpengdd.cyou/gtvrnaxulk.html

[M07] 判断是否为主入口
来源：http://hz.chenzaomai.com/gtpgxyundl.html

Py:   if __name__ == "__main__":
来源：http://hz.gzhubu.top/gtoteokvje.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cashguo.top/gtcklrjhos.html

JS:   require.main === module
来源：http://hz.shanyushiyangkeji.top/gtjtfqnria.html

TS:   require.main === module
来源：http://hz.chenjidiqi.icu/gtynhvbuvj.html

Java: public static void main(String[] args)
来源：http://hz.xuanzx.com/gtmzgnhplp.html

Go:   func main()
来源：http://hz.wangshuangyany.cn/gtvmotqxsu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sweek.top/gtybvcfixq.html

C#:   static void Main(string[] args)
来源：http://hz.zhoulong.xyz/gtvrxxverv.html

[M08] 获取系统与运行时信息
来源：http://hz.snrcjt.cn/gtxmjmlmik.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jianghu66.top/gtafgyxoun.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.316326.xyz/gtgialzfbd.html

JS:   process.platform;  process.version
来源：http://hz.jianghu66.top/gtmwwdftjp.html

TS:   process.platform;  process.version
来源：http://hz.c1oappe.top/gtlveyrkqu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yvedp.cn/gtqukjohro.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ivvv.top/gthxrmphfx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gaohongyu789.top/gtwigberii.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj20258888.top/gtfxibiwtl.html

================================================================================
来源：http://hz.chenlongwang.top/gtenrrully.html

N. 数据结构与算法
来源：http://hz.sysykeji.top/gtbjhqctto.html

================================================================================
来源：http://hz.yongpay.top/gtfyptysos.html

[N01] 二分查找（有序数组）
来源：http://hz.sufxvd.cn/gtpooderjh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gogol.net.cn/gtlgvkxnnx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.mhx1999.top/gtsxfivtct.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.smart0.xyz/gttkszujod.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxinkj.top/gtjxsenbkn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtkocfeixb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenzaomai.com/gtbuvbpnef.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jyoumei.cn/gtkrtzwssn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.c1oappe.top/gthcsolkiu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yanxiufei.cn/gtepwfgagz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hywenlv.cn/gtjtflbyvp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nwbrower.top/gtdwssqzej.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.feifeiyinyue.top/gtsljsiayb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yangfankeji.com/gterbojxsy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jyoumei.cn/gtndfjakec.html

Go:   slices.Sort(arr)
来源：http://hz.sweek.top/gtpzmcwgla.html

Ruby: arr.sort
来源：http://hz.sysykeji.top/gtrilrpuck.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hnxiangtu.top/gtgjubqimu.html

[N03] 快速排序（分治示例）
来源：http://hz.jyoumei.cn/gtoggjzzqs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xinyue.icu/gtoavccvhh.html

PHP:  // 递归实现，或用 usort
来源：http://hz.svipenyu.cn/gtgzutasno.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sufxvd.cn/gtnrfqresk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jianghu66.top/gtmblyhidn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hnqzz.top/gtdxisdsvy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cqqwz.cn/gtketzrnbt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shanyushiyangtech.top/gtmfldyhto.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ydzc1.top/gthxhrinvt.html

[N04] 斐波那契数列
来源：http://hz.gzhubu.top/gtkqmltlzy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hysaishi.cn/gthitdefdd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.nanxuanxn.top/gtssfjvzfx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ydzc1.top/gtapnvrstv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnqzz.top/gtvcqvcoyz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.fzhhl.top/gthtiolvvg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.smart0.xyz/gtfecasnvx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hammf.cn/gtvllwcqhw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hfpthk.cn/gtwbipeixj.html

[N05] 最大公约数
来源：http://hz.ivvv.top/gtzxzwnilr.html

Py:   math.gcd(a, b)
来源：http://hz.gaohongyu789.top/gttwralaqm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ydjk.org.cn/gtitrzbfpq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.feifeiyinyue.top/gtnkiackux.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yongpay.top/gtquubtlxz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.nanxuanxn.top/gtkhvkythe.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shanyushiyangtech.top/gtpmsneqaz.html

Ruby: a.gcd(b)
来源：http://hz.shuidangran.top/gtjtsnslhz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hongshengwenyu.top/gtaffbbvfn.html

[N06] 判断回文字符串
来源：http://hz.feifeiyinyue.top/gteablwdib.html

Py:   s == s[::-1]
来源：http://hz.gzhubu.top/gtahxzizfj.html

PHP:  $s === strrev($s);
来源：http://hz.ydzc1.top/gtwdhgrxov.html

JS:   s === [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gtxisqvmlr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xuanzx.com/gtorreofjw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sufxvd.cn/gtrbvrnguk.html

Go:   // 双指针从两端比较
来源：http://hz.jiagoushi.top/gthseuqeer.html

Ruby: s == s.reverse
来源：http://hz.yanxiufei.cn/gtjgnpkxgn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.wangdashe.top/gteqwrqozc.html

[N07] 两数之和（返回下标）
来源：http://hz.daxiang520.top/gthhzpfnry.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.52xcode.cn/gtznefndua.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yueranfly.top/gtubyxjcqn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ywan-chungtsiang.top/gtnqcfryjc.html

TS:   // 手写 Map<string, number>
来源：http://hz.jianghu66.top/gtuhptfyit.html

Java: // 手写 HashMap
来源：http://hz.jqgufenzy.top/gtqsjwjdpx.html

Go:   // 手写 map[int]int
来源：http://hz.redwolf501.top/gttfkimjni.html

Ruby: // 手写 Hash
来源：http://hz.chenjidiqi.icu/gtzivsqbuz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zdqjudy.top/gtashvzgzd.html

[N08] 生成全排列
来源：http://hz.yj202588.top/gtlrpekubm.html

Py:   itertools.permutations(arr)
来源：http://hz.chenjidiqi.icu/gtonjvjrvs.html

PHP:  // 手写递归交换
来源：http://hz.yonumen.top/gtgzndrskc.html

JS:   // 手写回溯递归
来源：http://hz.wangdashe.top/gtbvgwkerx.html

TS:   // 手写回溯递归
来源：http://hz.cheryme.top/gtocfjdowv.html

Java: // 手写回溯递归
来源：http://hz.yueranfly.top/gtpmlschpo.html

Go:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtevjrfrlm.html

Ruby: arr.permutation.to_a
来源：http://hz.gotoacloud.top/gtqiemuiho.html

C#:   // 手写回溯递归
来源：http://hz.yj20258.top/gttbzsmram.html

[N09] 栈与队列
来源：http://hz.zycfv.cn/gtslqwtosm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.kuanghao11.cn/gteczhxkmw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yj20258888.top/gtalsgwkny.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.shzxlz.cn/gtgafcwcer.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinyuanbaomall.cn/gtcwtzxvqx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yangfankeji.com/gtmnqrkekc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.guowangkeji.top/gtxssupduo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.andypj.xyz/gtgibdsyrx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.52xcode.cn/gtbsvwcmmt.html

[N10] 链表节点定义
来源：http://hz.9152youxi.cn/gtfzexexxi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yanxiufei.cn/gtccgxkbga.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.guannengcc.top/gtruacldbk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.aizwys.cn/gtyrktcquo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tianlin.xyz/gtkglocyvk.html

Java: class Node { int v; Node next; }
来源：http://hz.hywenlv.cn/gtpjzareqn.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xuanzx.com/gtpaqprmjq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cheryme.top/gtzxvcbslr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shangyingyoupin.top/gtwrbyhimz.html

[N11] 二叉树中序遍历
来源：http://hz.cheryme.top/gtoxpqhohh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jyoumei.cn/gtgzzraghf.html

PHP:  // 手写递归函数
来源：http://hz.ybcxt.top/gtbnejyqvu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aizwys.cn/gtkubdieny.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yueranfly.top/gtauwfwpik.html

Java: // 手写递归
来源：http://hz.pengpengdd.cyou/gtkbpcnrkv.html

Go:   // 手写递归
来源：http://hz.haohaochexian.top/gtxpiuucup.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhijiandao.cn/gtqvpuvzqy.html

C#:   // 手写递归
来源：http://hz.zhoulong.xyz/gtqxukclxg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zycfv.cn/gtqzouhusn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hnxiangtu.top/gtmqmqgbxv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hysaishi.cn/gtlhoxjegw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinqigufen.top/gtzgbmytbt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yongpay.top/gtoaiagbqh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tanke756.top/gtxvdlqiuc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zdqjudy.top/gtzuyvtqdd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.svipenyu.cn/gtunmqidbp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gzhubu.top/gtdxawgzca.html

================================================================================
来源：http://hz.yonumen.top/gtplbkdpyl.html

O. 并发与异步
来源：http://hz.wangdashe.top/gtaamnmfaq.html

================================================================================
来源：http://hz.hongshengwenyu.top/gttubdzeii.html

[O01] 启动一个线程
来源：http://hz.redwolf501.top/gtpwixlsoz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hnqzz.top/gtncdclzhb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.c1oappe.top/gtvzxmzraf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ybcxt.top/gtwvzljayk.html

TS:   // 同 JS
来源：http://hz.smart0.xyz/gtsnejtdyy.html

Java: new Thread(() -> f()).start()
来源：http://hz.ybcxt.top/gtyujbjhbz.html

Go:   go f()
来源：http://hz.chenzaomai.com/gtjlpeviyx.html

Ruby: Thread.new { f }
来源：http://hz.feifeiyinyue.top/gtdakwjpng.html

C#:   Task.Run(() => F());
来源：http://hz.wangdashe.top/gtqwwryyjy.html

[O02] 使用线程池
来源：http://hz.feifeiyinyue.top/gtkdizikkn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.feifeiyinyue.top/gtordepukj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yangfankeji.com/gtbuzsoubi.html

JS:   // worker_threads 线程池
来源：http://hz.ivvv.top/gtudcdludk.html

TS:   // worker_threads 线程池
来源：http://hz.yuxming.cn/gtczaxroru.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hnqzz.top/gtrfnpjkcj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xylfe.cn/gtktdxddvx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.vqdsnc.cn/gtgvzyzsww.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ydzc1.top/gtuvxrezpa.html

[O03] 加锁保护共享数据
来源：http://hz.cqqwz.cn/gthidrvxwx.html

Py:   with lock: shared += 1
来源：http://hz.havefunace.top/gtabcwgjbr.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shangyingyoupin.top/gttgqpovcy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hysaishi.cn/gtbzzlcdlr.html

TS:   // 同 JS
来源：http://hz.dashuyun.cn/gtudiynnvz.html

Java: synchronized (this) { shared++; }
来源：http://hz.sweek.top/gtekdsynps.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yuanzhike.top/gtlhnuaijb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yj20258888.top/gtvvwptnon.html

C#:   lock (gate) { shared++; }
来源：http://hz.316326.xyz/gtgkgohqpt.html

[O04] 定义异步函数并等待
来源：http://hz.zhaomingkeji.xyz/gtoswmvjpp.html

Py:   async def f():⏎    await g()
来源：http://hz.svipenyu.cn/gtbtujgkos.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhengqikj.top/gtwqbclulx.html

JS:   async function f() { await g(); }
来源：http://hz.jiagoushi.top/gtalepqifk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.redwolf501.top/gteflmhykm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xingfuxueyuan.xyz/gtsjlsulzb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.c1oappe.top/gtwplpsnfx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hongshengwenyu.top/gtzjlavtuh.html

C#:   async Task F() { await G(); }
来源：http://hz.cdnleiting.top/gtldorpmwn.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhoulong.xyz/gtsubswmbp.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cdnleiting.top/gtjptheqkh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.birdmap.top/gtkqdarxio.html

JS:   await Promise.all(tasks)
来源：http://hz.ydzc1.top/gttaqimsgk.html

TS:   await Promise.all(tasks)
来源：http://hz.daria6918.cn/gtzvdffjqc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ehwqpu.com/gtcefecvln.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hnxiangtu.top/gtqegyykda.html

Ruby: threads.map(&:join)
来源：http://hz.xylfe.cn/gtahokztzo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.tanke756.top/gtnhxngzjm.html

[O06] 使用进程池
来源：http://hz.yvedp.cn/gtbayqughk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.havefunace.top/gtqggtkmoe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.andypj.xyz/gtvrnnfcas.html

JS:   // child_process / cluster 模块
来源：http://hz.guowangkeji.top/gtaibzqnrd.html

TS:   // child_process / cluster 模块
来源：http://hz.sysykeji.top/gtmtwusfdh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sysykeji.top/gtosdhkrym.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ybcxt.top/gtpxppsmdc.html

Ruby: // fork 块
来源：http://hz.ivvv.top/gttwdkjrbh.html

C#:   Parallel.For
来源：http://hz.hnxiangtu.top/gtpktwjbxw.html

================================================================================
来源：http://hz.zhijiandao.cn/gtvvvkjhyq.html

P. 常用工具函数
来源：http://hz.cqqwz.cn/gtajfktkwg.html

================================================================================
来源：http://hz.wangdashe.top/gtrkyfwwkf.html

[P01] 生成 UUID
来源：http://hz.xinyue.icu/gtmkjqrncc.html

Py:   str(uuid.uuid4())
来源：http://hz.jqgufenzy.top/gtjshlbpux.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.tianlin.xyz/gtpsrajtau.html

JS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtwiesplkh.html

TS:   crypto.randomUUID()
来源：http://hz.bjfxy.top/gtlhbxbwmm.html

Java: UUID.randomUUID().toString()
来源：http://hz.snrcjt.cn/gtoklfszub.html

Go:   // 用 github.com/google/uuid
来源：http://hz.guannengcc.top/gtnltvojjy.html

Ruby: SecureRandom.uuid
来源：http://hz.jianghu66.top/gteiliayxs.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.iojbl.cn/gtscsaroem.html

[P02] MD5 / SHA256 摘要
来源：http://hz.svipenyu.cn/gtkutbtbyo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xziqi.cn/gtaazywygz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.kuanghao11.cn/gtzvxohlgz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gogol.net.cn/gtzkjzfhqo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.9152youxi.cn/gtdcmrgupi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.tanke756.top/gtpleaojjj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.pycfn.com/gterkepzat.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.feifeiyinyue.top/gttoxtkcel.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.bjfxy.top/gtijbqriav.html

[P03] 生成短随机字符串
来源：http://hz.jinghuilouyu.cn/gtrziyocmi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yuxming.cn/gtbivmcojg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.daria6918.cn/gthckivxxd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.svipenyu.cn/gtvspqitpa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.vqdsnc.cn/gtaafswofg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.nanxinkj.top/gtypzrjpdr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jlsjyb.cn/gtwbqqvsib.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.redwolf501.top/gtxhimobiy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yuxming.cn/gttpiqvtti.html

[P04] 求长度
来源：http://hz.316326.xyz/gtvmgztpjq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.redwolf501.top/gtpufswtvc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.feifeiyinyue.top/gtyiitcpjl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.52xcode.cn/gtjjraosyu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xinyue.icu/gtjudmgawz.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jianghu66.top/gtdvrpvoix.html

Go:   len(arr);  len(m)
来源：http://hz.jinqigufen.top/gtlbrawowy.html

Ruby: x.length;  x.size
来源：http://hz.zhijiandao.cn/gtumwhthik.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cdnleiting.top/gtzogfrxqw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ydzc1.top/gtvxgsvsqd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cdnleiting.top/gtmhehhuxm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.fzhhl.top/gtlqgkhnrn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.tian-w.cn/gthzdqiksd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenzaomai.com/gtkyjcinxa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yonumen.top/gttcofontr.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.svipenyu.cn/gtuskhhuye.html

Ruby: a == b
来源：http://hz.jinqigufen.top/gteclddain.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jqgfzy.top/gtnzbtlmgn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.nanxinkj.top/gtxeoqircf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.dianchejie.cn/gtgaywqgyl.html

PHP:  if (empty($x)) {}
来源：http://hz.ydjk.org.cn/gtmmahahju.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xinyue.icu/gtwndpetop.html

TS:   if (x == null) {}
来源：http://hz.yanxiufei.cn/gtoykkxnyt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xuetiantiany.cn/gteaoscync.html

Go:   if x == nil {}
来源：http://hz.birdmap.top/gtlqmwjhyd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.dashuyun.cn/gtffkosbhk.html

C#:   if (x is null) {}
来源：http://hz.pengpengdd.cyou/gtrmbduhse.html

[P07] 防抖与节流
来源：http://hz.cashguo.top/gtfdkwdxjl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yongpay.top/gtwhlizdrs.html

PHP:  // 手写时间戳比较
来源：http://hz.ydzc1.top/gtmwxjxojn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ivvv.top/gtefgnanzr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigfzy.top/gtxdaivfdy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinqigfzy.top/gtmzknipvz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.guowangkeji.top/gtapqbsrfw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cucudq.cn/gtaqzlcrbs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.dashuyun.cn/gtxjeyefxv.html

[P08] 处理浮点精度问题
来源：http://hz.pengpengdd.cyou/gtybvqqxnl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.vqdsnc.cn/gttekjejjh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cucudq.cn/gtahixceei.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ydzc1.top/gtmqrezbhy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.fengsongda.top/gtvzohapie.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xinyue.icu/gttgfgiije.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xziqi.cn/gtozklwlpy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cucudq.cn/gtowtkxdrh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yueranfly.top/gtqtucrplu.html

================================================================================
来源：http://hz.ehwqpu.com/gtoyfgcsvc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.kuanghao11.cn/gtawgsucsh.html

================================================================================
来源：http://hz.zdqjudy.top/gtwdqcucud.html

[Q01] 创建表
来源：http://hz.havefunace.top/gthmtxxovq.html

CREATE TABLE users (
来源：http://hz.dashuyun.cn/gtppytjbpj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shanyushiyangtech.top/gtjwozyvre.html

name VARCHAR(50) NOT NULL,
来源：http://hz.tianlin.xyz/gtrmypgydt.html

email VARCHAR(100) UNIQUE,
来源：http://hz.feifeiyinyue.top/gtmoknxkls.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinqigufen.top/gtozfqnhef.html

);
来源：http://hz.guannengcc.top/gtlmpgpmgh.html

[Q02] 创建带外键的表
来源：http://hz.ydzc1.top/gtxaffyejw.html

CREATE TABLE orders (
来源：http://hz.c1oappe.top/gthdstkjsv.html


<!-- 参考信息 -->