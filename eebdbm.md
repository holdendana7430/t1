代发 wailian999

JS:   process.exit(1)
来源：http://hz.cucudq.cn/gtsbjkjdtl.html

TS:   process.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtbasyxffy.html

Java: System.exit(1)
来源：http://hz.ybcxt.top/gtgzvihwfq.html

Go:   os.Exit(1)
来源：http://hz.zhixingplan.top/gtooyblpzq.html

Ruby: exit 1
来源：http://hz.ppjwa.cn/gtwmeohzbm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhengqikj.top/gtuidwxowh.html

[M06] 向标准错误输出
来源：http://hz.tian-w.cn/gtvnyxiokd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yueranfly.top/gtjaedbpon.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yuxming.cn/gtuirbfipc.html

JS:   console.error("err")
来源：http://hz.bjfxy.top/gtwbvduyrj.html

TS:   console.error("err")
来源：http://hz.hfpthk.cn/gtzvrgrsou.html

Java: System.err.println("err")
来源：http://hz.pengpengdd.cyou/gtjzumxchp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shzxlz.cn/gtpaclyyqy.html

Ruby: warn "err"
来源：http://hz.jqgufenzy.top/gtqfhvmhwa.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ppjwa.cn/gtnjyoxzvu.html

[M07] 判断是否为主入口
来源：http://hz.xziqi.cn/gtbabxijwk.html

Py:   if __name__ == "__main__":
来源：http://hz.quarkkingdee.top/gtgzdjqlji.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shangyingyoupin.top/gtysxxcevd.html

JS:   require.main === module
来源：http://hz.aibaodan.cn/gtyosaeork.html

TS:   require.main === module
来源：http://hz.daria6918.cn/gtfulnkfyn.html

Java: public static void main(String[] args)
来源：http://hz.zhijiandao.cn/gtljhonoap.html

Go:   func main()
来源：http://hz.sufxvd.cn/gtcldpoycg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cqqwz.cn/gtyqaohlph.html

C#:   static void Main(string[] args)
来源：http://hz.hnxiangtu.top/gttdhtfpyj.html

[M08] 获取系统与运行时信息
来源：http://hz.sysykeji.top/gtkcxapior.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ehwqpu.com/gtlwydiowy.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhongyouzk.top/gtvievwjhl.html

JS:   process.platform;  process.version
来源：http://hz.zdqjudy.top/gtpjhkxpwk.html

TS:   process.platform;  process.version
来源：http://hz.shzxlz.cn/gtsahzlhmz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jqgfzy.top/gtcduwwgtd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.c1oappe.top/gtncnkrtat.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shuidangran.top/gtbfubhklq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shanyushiyangtech.top/gtskigikgr.html

================================================================================
来源：http://hz.ydjk.org.cn/gtxelqulfr.html

N. 数据结构与算法
来源：http://hz.hnqzz.top/gtfffmyjoq.html

================================================================================
来源：http://hz.dianchejie.cn/gtnpabgguv.html

[N01] 二分查找（有序数组）
来源：http://hz.9152youxi.cn/gtawkapwcg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xinyue.icu/gtxkwdnbfj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.52xcode.cn/gtijgsbzhk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xingfuxueyuan.xyz/gthdcqquze.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jyoumei.cn/gtfxnfidpz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yj20258888.top/gthbmjbfgh.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhiwuduotai.top/gtnzrffnln.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.andypj.xyz/gtwlypwndv.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gaohongyu789.top/gtvwuhjejq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.nwbrower.top/gtrpdvfbvb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hywenlv.cn/gtubuxkyop.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yangfankeji.com/gttiimfmnh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.mhx1999.top/gtsmoiuqkl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guannengcc.top/gticpvkoex.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hywenlv.cn/gtupngezcm.html

Go:   slices.Sort(arr)
来源：http://hz.hongshengwenyu.top/gtqjibtfkh.html

Ruby: arr.sort
来源：http://hz.jinqigufen.top/gtmcslfslr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yueranfly.top/gtpeqwdnfj.html

[N03] 快速排序（分治示例）
来源：http://hz.pycfn.com/gttdyhvbxc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jlsjyb.cn/gtqaszwinl.html

PHP:  // 递归实现，或用 usort
来源：http://hz.daxiang520.top/gttawflaot.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.birdmap.top/gtuecblrdr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.fzhhl.top/gthsgeadqt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.fzhhl.top/gthgqhlkxj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.chenlongwang.top/gtqejgoosu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.nanxinkj.top/gtlwkbxtnz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.meibo888.top/gtmaihtiqh.html

[N04] 斐波那契数列
来源：http://hz.guannengcc.top/gtpqzubxgp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sufxvd.cn/gtmhyfshuw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yj202588.top/gtaomodctv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.iojbl.cn/gtwzacjgot.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ybcxt.top/gthqgmkvcs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sxryk.cn/gtsosokizi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.wangshuangyany.cn/gtcfqtafnr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yueranfly.top/gtegihniuu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yongpay.top/gtqqrtbdji.html

[N05] 最大公约数
来源：http://hz.pengpengdd.cyou/gtcepvxkfi.html

Py:   math.gcd(a, b)
来源：http://hz.gotoacloud.top/gtdihvgubt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinghuilouyu.cn/gtwyvzbdpy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.quarkkingdee.top/gtdmdzpfwu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cheryme.top/gtkawnxbnw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.feifeiyinyue.top/gthjbtzyru.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jlsjyb.cn/gtvoayfhos.html

Ruby: a.gcd(b)
来源：http://hz.guowangkeji.top/gtmqajjpck.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yanxiufei.cn/gtpfuzwjvd.html

[N06] 判断回文字符串
来源：http://hz.shuidangran.top/gtusbivglw.html

Py:   s == s[::-1]
来源：http://hz.hfpthk.cn/gtdlbioczm.html

PHP:  $s === strrev($s);
来源：http://hz.birdmap.top/gtulpeitvl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtrdrjiixo.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtdrelqpks.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hnxiangtu.top/gtdxuohilx.html

Go:   // 双指针从两端比较
来源：http://hz.chenzaomai.com/gtyynvagdv.html

Ruby: s == s.reverse
来源：http://hz.zycfv.cn/gtzciuxubw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ydzc1.top/gtcsankhnc.html

[N07] 两数之和（返回下标）
来源：http://hz.havefunace.top/gtxpfntpsx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yuanzhike.top/gtjplqullz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hnxiangtu.top/gtdqsfjqvy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.cqqwz.cn/gtmwahzpii.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinyuanbaomall.cn/gtssceuutd.html

Java: // 手写 HashMap
来源：http://hz.zycfv.cn/gtrudmfzbt.html

Go:   // 手写 map[int]int
来源：http://hz.jinyuanbaomall.cn/gtyyutozjg.html

Ruby: // 手写 Hash
来源：http://hz.zycfv.cn/gtsrxeiima.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sufxvd.cn/gtumnlbjcs.html

[N08] 生成全排列
来源：http://hz.yvedp.cn/gtgnedavak.html

Py:   itertools.permutations(arr)
来源：http://hz.dianchejie.cn/gtxgwhiqex.html

PHP:  // 手写递归交换
来源：http://hz.xuanzx.com/gtfjghuiyu.html

JS:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtbmglmppr.html

TS:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtoirtwxpw.html

Java: // 手写回溯递归
来源：http://hz.yueranfly.top/gtylqynmwn.html

Go:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtxaoqtodh.html

Ruby: arr.permutation.to_a
来源：http://hz.andypj.xyz/gtfauxpija.html

C#:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtuctyutoq.html

[N09] 栈与队列
来源：http://hz.andypj.xyz/gtqcqgsqbz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sysykeji.top/gtpudxbrvd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhiwuduotai.top/gtwxrupqpp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.daxiang520.top/gtpsolstxi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.gogol.net.cn/gtwtxkowar.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ydzc1.top/gttcdfzitq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.aizwys.cn/gtismocygl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xziqi.cn/gtqodgycvm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.aibaodan.cn/gtfmjyluqc.html

[N10] 链表节点定义
来源：http://hz.xingfuxueyuan.xyz/gttvstwmqz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jqgfzy.top/gthvdfesbl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xziqi.cn/gtfbimnrcj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ivvv.top/gtukgnehpa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.bjfxy.top/gtxmlpqfbj.html

Java: class Node { int v; Node next; }
来源：http://hz.cheryme.top/gtgjppbwjz.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.sysykeji.top/gtgktromaq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhengqikj.top/gtmhpvazfk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xingfuxueyuan.xyz/gtvwiflfgt.html

[N11] 二叉树中序遍历
来源：http://hz.xuetiantiany.cn/gtgchdqrmo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ybcxt.top/gtxtwjgfbg.html

PHP:  // 手写递归函数
来源：http://hz.ivvv.top/gtdglpfyqh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ivvv.top/gtmmwuvgwa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zycfv.cn/gtczzutokr.html

Java: // 手写递归
来源：http://hz.0kj1m.cn/gthisigcsl.html

Go:   // 手写递归
来源：http://hz.smart0.xyz/gtemmhkzxj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.vqdsnc.cn/gtajgdmtla.html

C#:   // 手写递归
来源：http://hz.zhongyouzk.top/gtenjjqyqf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gzhubu.top/gtlymcdcox.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shzxlz.cn/gtwijvswqn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.bjfxy.top/gtouhvppmz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yueranfly.top/gtjvvxdbgy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sxryk.cn/gtidpwtpgm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hfpthk.cn/gtvlhmahkj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jianghu66.top/gtofjfowpw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.tian-w.cn/gthrwipwco.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hysaishi.cn/gtswkwjpqw.html

================================================================================
来源：http://hz.sysykeji.top/gtjjsoccik.html

O. 并发与异步
来源：http://hz.yj20258888.top/gtaodatwsa.html

================================================================================
来源：http://hz.birdmap.top/gtnfuvpmze.html

[O01] 启动一个线程
来源：http://hz.nanxinkj.top/gtfdourahn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.tianlin.xyz/gtboyluemh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shzxlz.cn/gtqodtkttx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yj20258888.top/gtnzxqftvd.html

TS:   // 同 JS
来源：http://hz.yuanzhike.top/gtmezhtpvx.html

Java: new Thread(() -> f()).start()
来源：http://hz.quarkkingdee.top/gtkpgdpxvy.html

Go:   go f()
来源：http://hz.yj202588.top/gtddhrmpof.html

Ruby: Thread.new { f }
来源：http://hz.jyoumei.cn/gtweeurprz.html

C#:   Task.Run(() => F());
来源：http://hz.0kj1m.cn/gtfpnwczsn.html

[O02] 使用线程池
来源：http://hz.xuetiantiany.cn/gtnqooegbu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sweek.top/gtjrbusvpl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yuanzhike.top/gtehtupngw.html

JS:   // worker_threads 线程池
来源：http://hz.pengpengdd.cyou/gtiqffzrsm.html

TS:   // worker_threads 线程池
来源：http://hz.xuetiantiany.cn/gtpknvybuf.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.havefunace.top/gtsgxvyazn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yueranfly.top/gthmplilzf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.sufxvd.cn/gtxhzeysmy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gogol.net.cn/gtskydcvkm.html

[O03] 加锁保护共享数据
来源：http://hz.yueranfly.top/gtwzfxqmgj.html

Py:   with lock: shared += 1
来源：http://hz.xuetiantiany.cn/gtjlpvsdxt.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jianghu66.top/gtrryqdcoj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.dianchejie.cn/gtiewytbuk.html

TS:   // 同 JS
来源：http://hz.gotoacloud.top/gthfschlva.html

Java: synchronized (this) { shared++; }
来源：http://hz.yongpay.top/gthghoxuhr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.snrcjt.cn/gtuxmvztzs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.bjfxy.top/gtergsdbcm.html

C#:   lock (gate) { shared++; }
来源：http://hz.xuetiantiany.cn/gtnnlqvcus.html

[O04] 定义异步函数并等待
来源：http://hz.c1oappe.top/gtfhjpxihm.html

Py:   async def f():⏎    await g()
来源：http://hz.dashuyun.cn/gtrvbmpbdd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinqigufen.top/gtryvwmsbm.html

JS:   async function f() { await g(); }
来源：http://hz.haohaochexian.top/gtopdsdbnz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhiwuduotai.top/gtmjrdodir.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ybcxt.top/gtuqopotsw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jianghu66.top/gtkmiaheiy.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.nwbrower.top/gtxfsshrzg.html

C#:   async Task F() { await G(); }
来源：http://hz.yanxiufei.cn/gthbyfxfrd.html

[O05] 并发执行并等待全部完成
来源：http://hz.jqgufenzy.top/gtlgnevhef.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shanyushiyangtech.top/gtmwjavjjr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhiwuduotai.top/gtebwqtoyi.html

JS:   await Promise.all(tasks)
来源：http://hz.9152youxi.cn/gtkksejwhh.html

TS:   await Promise.all(tasks)
来源：http://hz.nanxinkj.top/gtpopanymt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shuidangran.top/gtnxymwifz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ydzc1.top/gtjomwrzjb.html

Ruby: threads.map(&:join)
来源：http://hz.sweek.top/gtoqafpysk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.chenjidiqi.icu/gtrdyolfei.html

[O06] 使用进程池
来源：http://hz.zdqjudy.top/gtiedwtjyq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cheryme.top/gtvecruary.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zdqjudy.top/gttyxtyrjr.html

JS:   // child_process / cluster 模块
来源：http://hz.aibaodan.cn/gtxyyuobzk.html

TS:   // child_process / cluster 模块
来源：http://hz.ivvv.top/gtofiheebi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhiwuduotai.top/gtrzzelrus.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yuxming.cn/gteqpgmgcb.html

Ruby: // fork 块
来源：http://hz.chenjidiqi.icu/gtgfpsoood.html

C#:   Parallel.For
来源：http://hz.dashuyun.cn/gtfocehziz.html

================================================================================
来源：http://hz.zdqjudy.top/gtbczyfjyz.html

P. 常用工具函数
来源：http://hz.wangdashe.top/gtwnmqznne.html

================================================================================
来源：http://hz.guowangkeji.top/gtngvngqpu.html

[P01] 生成 UUID
来源：http://hz.cucudq.cn/gtyfbexmjg.html

Py:   str(uuid.uuid4())
来源：http://hz.sxryk.cn/gttbispkhx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ybcxt.top/gtbuuouiyu.html

JS:   crypto.randomUUID()
来源：http://hz.shuidangran.top/gtqojagkzr.html

TS:   crypto.randomUUID()
来源：http://hz.meibo888.top/gtcvtqpevf.html

Java: UUID.randomUUID().toString()
来源：http://hz.dashuyun.cn/gtbffiayjj.html

Go:   // 用 github.com/google/uuid
来源：http://hz.redwolf501.top/gtxaueajnu.html

Ruby: SecureRandom.uuid
来源：http://hz.daxiang520.top/gtlziwpiys.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.nanxinkj.top/gtyidiulbs.html

[P02] MD5 / SHA256 摘要
来源：http://hz.9152youxi.cn/gtzsgxcmnj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gogol.net.cn/gtdlcaxzxy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhengqikj.top/gtnatldpda.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhongyouzk.top/gtjqqtigop.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hammf.cn/gtnrerpfpr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.kuanghao11.cn/gtbvhguvlb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jinyuanbaomall.cn/gtgoinplkx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenzaomai.com/gtqiolyywg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.9152youxi.cn/gtolbsphxe.html

[P03] 生成短随机字符串
来源：http://hz.9152youxi.cn/gtzotcnlmx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cqqwz.cn/gtmrifhgun.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jiagoushi.top/gtoigyllku.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.c1oappe.top/gtxzzpzkyl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnxiangtu.top/gtlqmaaxkv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.iojbl.cn/gticqotktt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.fengsongda.top/gtrgdsolqt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.guannengcc.top/gtbzbpxvqf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ydzc1.top/gtrlnepqkh.html

[P04] 求长度
来源：http://hz.cashguo.top/gtpsscpzzs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.daria6918.cn/gtnzzrupry.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cashguo.top/gtrtnixaja.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jiagoushi.top/gtunzprrtc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.tian-w.cn/gtjomsxpog.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jinqigufen.top/gtxldxhkme.html

Go:   len(arr);  len(m)
来源：http://hz.chenlongwang.top/gttwwkymgh.html

Ruby: x.length;  x.size
来源：http://hz.yj20258.top/gtpxuylsvs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.pycfn.com/gtulfwgaiz.html

[P05] 判断两个对象内容是否相等
来源：http://hz.c1oappe.top/gtojbrbxey.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ehwqpu.com/gtzfpwrekb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hnqzz.top/gtyacfodcy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nanxinkj.top/gtzalaljby.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenjidiqi.icu/gtdsaridkz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jyoumei.cn/gtotcddwvx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.tianlin.xyz/gtapkywqqt.html

Ruby: a == b
来源：http://hz.daxiang520.top/gtvknfqqse.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.tian-w.cn/gtacrtewsw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jinghuilouyu.cn/gtuolntxpx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.tianlin.xyz/gtnmxczytv.html

PHP:  if (empty($x)) {}
来源：http://hz.yvedp.cn/gtjwdckwkb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinqigfzy.top/gtlrwsiivi.html

TS:   if (x == null) {}
来源：http://hz.ppjwa.cn/gtwhaktpab.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xuanzx.com/gtmznfounc.html

Go:   if x == nil {}
来源：http://hz.yuxming.cn/gtlskzjnlk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ywan-chungtsiang.top/gtfnebqnqn.html

C#:   if (x is null) {}
来源：http://hz.jiagoushi.top/gtegsugmav.html

[P07] 防抖与节流
来源：http://hz.xylfe.cn/gtjcamxvwn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jlsjyb.cn/gtfhonofeq.html

PHP:  // 手写时间戳比较
来源：http://hz.hnxiangtu.top/gtcvekxcss.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guannengcc.top/gtrygqjonp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258888.top/gtdhfzxdmo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinyuanbaomall.cn/gtawvjxztx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.fzhhl.top/gtedcgtsun.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zycfv.cn/gtcndicdcw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jinqigufen.top/gtgbkljkwe.html

[P08] 处理浮点精度问题
来源：http://hz.zhaomingkeji.xyz/gtqtcbpiod.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xingfuxueyuan.xyz/gtxuwokvth.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinyuanbaomall.cn/gtbzsmksix.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xinyue.icu/gtfyjgxqbl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhengqikj.top/gtqpjrbokn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jqgufenzy.top/gtlriovpsq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cashguo.top/gtvmohglmv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yvedp.cn/gtgznobedz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cqqwz.cn/gtvvlawrie.html

================================================================================
来源：http://hz.yanxiufei.cn/gtycemryhj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj20258.top/gtgxtrhhqo.html

================================================================================
来源：http://hz.nanxuanxn.top/gtfesizyks.html

[Q01] 创建表
来源：http://hz.yuanzhike.top/gtsywmphxe.html

CREATE TABLE users (
来源：http://hz.nanxuanxn.top/gtibnwxvyg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guannengcc.top/gtdwfqwlij.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ivvv.top/gtyppfnqkm.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shanyushiyangtech.top/gtsmsvprbo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ehwqpu.com/gtcyropzsp.html

);
来源：http://hz.sxryk.cn/gtidurjbdb.html

[Q02] 创建带外键的表
来源：http://hz.fzhhl.top/gtroyzfkkp.html

CREATE TABLE orders (
来源：http://hz.shangyingyoupin.top/gtifbhhjaw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenjidiqi.icu/gtrzgfjdht.html

user_id INT NOT NULL,
来源：http://hz.yuanzhike.top/gtarswwdnu.html

amount DECIMAL(10, 2),
来源：http://hz.9152youxi.cn/gtjphlyzqk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ywan-chungtsiang.top/gtdlmxkqga.html

);
来源：http://hz.quarkkingdee.top/gtfktekzwg.html

[Q03] 增加列
来源：http://hz.shanyushiyangkeji.top/gtawwxrark.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.daxiang520.top/gtaiiulctu.html

[Q04] 修改列类型
来源：http://hz.cashguo.top/gtwqzpqxiw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jiagoushi.top/gtdcidhpsz.html

[Q05] 重命名列
来源：http://hz.meibo888.top/gtzxuxcxtn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhengqikj.top/gtlcjusrbh.html

[Q06] 删除列
来源：http://hz.chenzaomai.com/gthtlrjksd.html


<!-- 参考信息 -->