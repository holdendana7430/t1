代发 wailian999

Ruby: exit 1
来源：http://hz.xuanzx.com/gtpdeckdkh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.0kj1m.cn/gtdqyakuae.html

[M06] 向标准错误输出
来源：http://hz.c1oappe.top/gtxqfndyqs.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ywan-chungtsiang.top/gtlzwjiege.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.tian-w.cn/gtnltobsti.html

JS:   console.error("err")
来源：http://hz.cqqwz.cn/gtlhggwpzt.html

TS:   console.error("err")
来源：http://hz.316326.xyz/gtrptopkbo.html

Java: System.err.println("err")
来源：http://hz.nwbrower.top/gtanwixvnc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hnxiangtu.top/gtwpizlsvn.html

Ruby: warn "err"
来源：http://hz.nanxinkj.top/gtwxghnnpt.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.guowangkeji.top/gtpligebfm.html

[M07] 判断是否为主入口
来源：http://hz.fengsongda.top/gtgykmjigg.html

Py:   if __name__ == "__main__":
来源：http://hz.yj202588.top/gtqnewdfqx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.sysykeji.top/gtskrhvemp.html

JS:   require.main === module
来源：http://hz.sweek.top/gtarobulsl.html

TS:   require.main === module
来源：http://hz.9152youxi.cn/gtqvlmfeuh.html

Java: public static void main(String[] args)
来源：http://hz.birdmap.top/gtwurpgkfu.html

Go:   func main()
来源：http://hz.hfpthk.cn/gtgkbskrse.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.redwolf501.top/gtrzkogflp.html

C#:   static void Main(string[] args)
来源：http://hz.guannengcc.top/gtxjenfhlb.html

[M08] 获取系统与运行时信息
来源：http://hz.zhijiandao.cn/gtvjyscfpo.html

Py:   platform.system();  platform.python_version()
来源：http://hz.nanxuanxn.top/gtztwiyxkf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhixingplan.top/gtqggoejcn.html

JS:   process.platform;  process.version
来源：http://hz.feifeiyinyue.top/gtypdfsbkd.html

TS:   process.platform;  process.version
来源：http://hz.gzhubu.top/gtplviiezj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sysykeji.top/gtvijuckrm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.guowangkeji.top/gtifdurpnc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.iojbl.cn/gtmgypqpnu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.pycfn.com/gtyrymzkex.html

================================================================================
来源：http://hz.yj202588.top/gtdrlywoow.html

N. 数据结构与算法
来源：http://hz.ydjk.org.cn/gtelfvnmmi.html

================================================================================
来源：http://hz.aibaodan.cn/gttarhdxbu.html

[N01] 二分查找（有序数组）
来源：http://hz.tianlin.xyz/gtxseuvtmy.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.pycfn.com/gtkmdhfwve.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shangyingyoupin.top/gtflskmpmh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.smart0.xyz/gtrpyuqkut.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sufxvd.cn/gtapgwdpom.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hammf.cn/gtlkylhkns.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.svipenyu.cn/gtnohbrkqj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.fzhhl.top/gtqkgnawtm.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sufxvd.cn/gtuwlanfqv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shanyushiyangkeji.top/gtibgsdesf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhaomingkeji.xyz/gtasgbeqdp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj20258.top/gtdzcsvbox.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guannengcc.top/gtltlasvsk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shuidangran.top/gtkwksvlyh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.guowangkeji.top/gtfbqpials.html

Go:   slices.Sort(arr)
来源：http://hz.jqgfzy.top/gttmrdrlpr.html

Ruby: arr.sort
来源：http://hz.xziqi.cn/gtacnbierg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.iojbl.cn/gtlejusnsk.html

[N03] 快速排序（分治示例）
来源：http://hz.sysykeji.top/gtbzptveaf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhixingplan.top/gtftprtlry.html

PHP:  // 递归实现，或用 usort
来源：http://hz.fzhhl.top/gtawwspjwv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.iojbl.cn/gtnmefdrwl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigfzy.top/gttyazgwaw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tian-w.cn/gtbhztzzva.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhoulong.xyz/gtlvpwozvh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yvedp.cn/gtijikykao.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cashguo.top/gtigifanro.html

[N04] 斐波那契数列
来源：http://hz.hnqzz.top/gtyzfnybfk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhengqikj.top/gtarmafhna.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.chenlongwang.top/gtoikqtkpz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dashuyun.cn/gtxjxblwzv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sweek.top/gtsevtecmq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.feifeiyinyue.top/gtxcvhdpth.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.guowangkeji.top/gthmmgrpek.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.smart0.xyz/gtykwbtilf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinyuanbaomall.cn/gtbosbtllz.html

[N05] 最大公约数
来源：http://hz.cheryme.top/gtgcochlmn.html

Py:   math.gcd(a, b)
来源：http://hz.pengpengdd.cyou/gtrcvkkixi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yongpay.top/gtccvcwlwl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnxiangtu.top/gtlhrqqvtv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yuanzhike.top/gthvjqhsei.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yj20258888.top/gtyknrpyac.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xingfuxueyuan.xyz/gtbvsevgrp.html

Ruby: a.gcd(b)
来源：http://hz.hysaishi.cn/gtnkzzpeqh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shuidangran.top/gtxqdfrwkl.html

[N06] 判断回文字符串
来源：http://hz.hnxiangtu.top/gtblitlvjs.html

Py:   s == s[::-1]
来源：http://hz.tianlin.xyz/gtxzcxfgzp.html

PHP:  $s === strrev($s);
来源：http://hz.pengpengdd.cyou/gtkexwnbkk.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtgjtnwxub.html

TS:   s === [...s].reverse().join("")
来源：http://hz.birdmap.top/gtrfjfxwok.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.aizwys.cn/gtvkyvetcq.html

Go:   // 双指针从两端比较
来源：http://hz.yvedp.cn/gtwwenqvhu.html

Ruby: s == s.reverse
来源：http://hz.ivvv.top/gtnzsdeshf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xinyue.icu/gtzvnxfblu.html

[N07] 两数之和（返回下标）
来源：http://hz.hfpthk.cn/gtujoubyun.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ppjwa.cn/gtpgebrxpn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ivvv.top/gtushczklk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.cqqwz.cn/gtqsdazjlw.html

TS:   // 手写 Map<string, number>
来源：http://hz.xinyue.icu/gtmrqbhush.html

Java: // 手写 HashMap
来源：http://hz.ybcxt.top/gtsouwnztk.html

Go:   // 手写 map[int]int
来源：http://hz.andypj.xyz/gtyytrafru.html

Ruby: // 手写 Hash
来源：http://hz.zhongyouzk.top/gtfozxaawh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.snrcjt.cn/gtryrcmvja.html

[N08] 生成全排列
来源：http://hz.shzxlz.cn/gtireomihm.html

Py:   itertools.permutations(arr)
来源：http://hz.cashguo.top/gtydlihlhi.html

PHP:  // 手写递归交换
来源：http://hz.sweek.top/gtvfwvimhk.html

JS:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtskamrjcq.html

TS:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtjfpnekkp.html

Java: // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtwwnlzpra.html

Go:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtwbgadasl.html

Ruby: arr.permutation.to_a
来源：http://hz.xingfuxueyuan.xyz/gtdmqlfugp.html

C#:   // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtnvhozwnd.html

[N09] 栈与队列
来源：http://hz.chenlongwang.top/gttexpkmls.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.mhx1999.top/gtrkcvpnmo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.mhx1999.top/gtcceahoyw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jqgfzy.top/gtrpzygwoh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zdqjudy.top/gtuviehsxy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hnxiangtu.top/gttawmzvys.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.daxiang520.top/gtxxwcvbpq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xuetiantiany.cn/gttakybnmh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hysaishi.cn/gtqopvzvoz.html

[N10] 链表节点定义
来源：http://hz.hywenlv.cn/gtibxugxrm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhiwuduotai.top/gtjfthtfzh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhongyouzk.top/gtyuxfopjp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yonumen.top/gthterupyn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.guannengcc.top/gtpiajisaf.html

Java: class Node { int v; Node next; }
来源：http://hz.hnxiangtu.top/gtfcqntxle.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yj202588.top/gtycwtsxin.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.redwolf501.top/gtxbztgucs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jianghu66.top/gtjepdkhpy.html

[N11] 二叉树中序遍历
来源：http://hz.sysykeji.top/gtjmcwbxio.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yangfankeji.com/gtuagxygti.html

PHP:  // 手写递归函数
来源：http://hz.xingfuxueyuan.xyz/gteruecegd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhijiandao.cn/gtwnjdcqpd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenzaomai.com/gtwhnesgil.html

Java: // 手写递归
来源：http://hz.tianlin.xyz/gtkhuoppob.html

Go:   // 手写递归
来源：http://hz.yonumen.top/gttwzarbas.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yangfankeji.com/gtmcaosvfl.html

C#:   // 手写递归
来源：http://hz.xuetiantiany.cn/gthilfsyph.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.fzhhl.top/gtiftwzrla.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.fzhhl.top/gtzqytdarl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.tianlin.xyz/gtvbffhbul.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.fzhhl.top/gtnfqckufy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aibaodan.cn/gtdfrbkjug.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guowangkeji.top/gtddzgljdc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jianghu66.top/gtmqaaztll.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.0kj1m.cn/gtdmurtyjd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yongpay.top/gtzbsxegjz.html

================================================================================
来源：http://hz.hnxiangtu.top/gteytzssui.html

O. 并发与异步
来源：http://hz.dashuyun.cn/gtmavugmrz.html

================================================================================
来源：http://hz.nanxuanxn.top/gtqcipyjkc.html

[O01] 启动一个线程
来源：http://hz.xuanzx.com/gtvuqanion.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ydzc1.top/gtxkbtzniy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.kuanghao11.cn/gtacmvdsil.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.shanyushiyangtech.top/gtpojxqaom.html

TS:   // 同 JS
来源：http://hz.52xcode.cn/gtmxnvctve.html

Java: new Thread(() -> f()).start()
来源：http://hz.guowangkeji.top/gtdtkiycho.html

Go:   go f()
来源：http://hz.xinyue.icu/gtkcvjqqfo.html

Ruby: Thread.new { f }
来源：http://hz.316326.xyz/gtilkpbvtt.html

C#:   Task.Run(() => F());
来源：http://hz.jinghuilouyu.cn/gtupuepeqg.html

[O02] 使用线程池
来源：http://hz.havefunace.top/gtcanxecik.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yuxming.cn/gtckwttyyx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.wangdashe.top/gtmxnagjag.html

JS:   // worker_threads 线程池
来源：http://hz.0kj1m.cn/gtvpwmwejz.html

TS:   // worker_threads 线程池
来源：http://hz.smart0.xyz/gttnjquoim.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shanyushiyangtech.top/gtznjbczpy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jqgufenzy.top/gtilazqpxj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.haohaochexian.top/gtrlwbzefo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ivvv.top/gtlfkkdmiv.html

[O03] 加锁保护共享数据
来源：http://hz.tianlin.xyz/gtuvujerxb.html

Py:   with lock: shared += 1
来源：http://hz.svipenyu.cn/gtxyxfmzvk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.0kj1m.cn/gtpaneqyhe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.aizwys.cn/gtsanyotpq.html

TS:   // 同 JS
来源：http://hz.9152youxi.cn/gtmtacnfmq.html

Java: synchronized (this) { shared++; }
来源：http://hz.yonumen.top/gtjtxpilji.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.svipenyu.cn/gtniqgaqoi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinqigfzy.top/gtthpumxnu.html

C#:   lock (gate) { shared++; }
来源：http://hz.chenzaomai.com/gteiggmivp.html

[O04] 定义异步函数并等待
来源：http://hz.tianlin.xyz/gthhywbjkg.html

Py:   async def f():⏎    await g()
来源：http://hz.yj20258888.top/gtcrfympvw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.316326.xyz/gtmmguuiwp.html

JS:   async function f() { await g(); }
来源：http://hz.hywenlv.cn/gtuxgcomni.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.nanxuanxn.top/gtwxlyhpna.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.guannengcc.top/gtngktzrjl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ywan-chungtsiang.top/gtfkluwhps.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xuetiantiany.cn/gtcktfpexi.html

C#:   async Task F() { await G(); }
来源：http://hz.hongshengwenyu.top/gtnesoqzwg.html

[O05] 并发执行并等待全部完成
来源：http://hz.xziqi.cn/gtomdgfnpj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gzhubu.top/gtkhfkfwns.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhiwuduotai.top/gtsitqmndm.html

JS:   await Promise.all(tasks)
来源：http://hz.nwbrower.top/gtbgojypdf.html

TS:   await Promise.all(tasks)
来源：http://hz.hnqzz.top/gtofneizkh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.redwolf501.top/gtohfazfzw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.redwolf501.top/gtidgcswmd.html

Ruby: threads.map(&:join)
来源：http://hz.zhongyouzk.top/gtkcyasshv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shanyushiyangtech.top/gtuhjdqbjv.html

[O06] 使用进程池
来源：http://hz.chenlongwang.top/gtpkojdstw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yuanzhike.top/gtwmaajdtt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.sweek.top/gtlpkjpnuh.html

JS:   // child_process / cluster 模块
来源：http://hz.ydjk.org.cn/gtrtxwwjxp.html

TS:   // child_process / cluster 模块
来源：http://hz.yanxiufei.cn/gtjcendnfu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yueranfly.top/gtovdsoqvq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.iojbl.cn/gtixnaddbm.html

Ruby: // fork 块
来源：http://hz.bjfxy.top/gtltvqkbvs.html

C#:   Parallel.For
来源：http://hz.hnxiangtu.top/gtphbdyxlv.html

================================================================================
来源：http://hz.hysaishi.cn/gtwbjnrolp.html

P. 常用工具函数
来源：http://hz.andypj.xyz/gtrloioamv.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtmtcmfdcw.html

[P01] 生成 UUID
来源：http://hz.havefunace.top/gtcrdsvnkm.html

Py:   str(uuid.uuid4())
来源：http://hz.cashguo.top/gtpdonegks.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shanyushiyangkeji.top/gtkhhclzns.html

JS:   crypto.randomUUID()
来源：http://hz.andypj.xyz/gtdiudaomr.html

TS:   crypto.randomUUID()
来源：http://hz.andypj.xyz/gtvvdbsjei.html

Java: UUID.randomUUID().toString()
来源：http://hz.gaohongyu789.top/gtsqckwtsd.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sysykeji.top/gtdpyaveou.html

Ruby: SecureRandom.uuid
来源：http://hz.jinyuanbaomall.cn/gtafaygxfw.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinyuanbaomall.cn/gthcochdcy.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yj20258.top/gtkoialkrq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhijiandao.cn/gtgmittjey.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yj202588.top/gtkupcnkxq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ydjk.org.cn/gtojwxjaim.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yanxiufei.cn/gtzfyrbspo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhaomingkeji.xyz/gtekuvxbaf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gzhubu.top/gtsjqcpwja.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jiagoushi.top/gtmyawtjnr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jlsjyb.cn/gtbvzbfedc.html

[P03] 生成短随机字符串
来源：http://hz.zhongyouzk.top/gtbtvkduot.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhixingplan.top/gtsyehbsgw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zdqjudy.top/gtshxmpoyk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuanzx.com/gtjgjrirds.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhoulong.xyz/gtxfhnxarz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.feifeiyinyue.top/gtffpzklbx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ppjwa.cn/gtrhkqaozd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.nwbrower.top/gtqnpikjur.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.mhx1999.top/gtwvxyuchd.html

[P04] 求长度
来源：http://hz.yj20258888.top/gtunpnsfwc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gaohongyu789.top/gtdivdeitg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aibaodan.cn/gtjnhsdobg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.guannengcc.top/gtpjsjqbev.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj20258888.top/gtvsqgubcd.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cheryme.top/gtzbnyfxrd.html

Go:   len(arr);  len(m)
来源：http://hz.daria6918.cn/gtmkdahkrw.html

Ruby: x.length;  x.size
来源：http://hz.zhaomingkeji.xyz/gtrfbmrhyb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gotoacloud.top/gtypwfzzzl.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yueranfly.top/gtpdbnaeql.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cheryme.top/gtukmtknku.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.redwolf501.top/gtxtoqnnjq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.dashuyun.cn/gtjetfnrtx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgufenzy.top/gteqavdhkf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.mhx1999.top/gtkyopomox.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hysaishi.cn/gtwndaubor.html

Ruby: a == b
来源：http://hz.zdqjudy.top/gtbitzrule.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ydjk.org.cn/gttfqmqaxt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.meibo888.top/gtczzqtlcx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhixingplan.top/gtaivhyqjl.html

PHP:  if (empty($x)) {}
来源：http://hz.jqgfzy.top/gtlefucnbx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinqigfzy.top/gtkvzzzagp.html

TS:   if (x == null) {}
来源：http://hz.yj20258.top/gtlkdjcjxb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xylfe.cn/gtizqcmdai.html

Go:   if x == nil {}
来源：http://hz.cucudq.cn/gtgyxwbbbe.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zdqjudy.top/gtjielicdk.html

C#:   if (x is null) {}
来源：http://hz.zycfv.cn/gtgwrjymnd.html

[P07] 防抖与节流
来源：http://hz.hammf.cn/gtixaiurbm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhixingplan.top/gtbkatizyh.html

PHP:  // 手写时间戳比较
来源：http://hz.shanyushiyangkeji.top/gtbdcpllpb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuanzx.com/gttspnuduc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fzhhl.top/gttjbfeosn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.wangdashe.top/gtvhoeflwx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jiagoushi.top/gttwmztnio.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhengqikj.top/gtpthtdzgy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hnxiangtu.top/gtzwariksa.html

[P08] 处理浮点精度问题
来源：http://hz.xziqi.cn/gtuyhxoaua.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.dashuyun.cn/gtizloupmj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.gogol.net.cn/gtzeyeierz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cheryme.top/gthtrvqdaz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cashguo.top/gtdnlrjbyi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.smart0.xyz/gtaojzqzxh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xziqi.cn/gttoemdaoe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.pengpengdd.cyou/gtkunlcbqa.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenzaomai.com/gtrbsxgpcn.html

================================================================================
来源：http://hz.9152youxi.cn/gtehwibrsj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.guowangkeji.top/gtdkhqfhpd.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtdggpcjke.html

[Q01] 创建表
来源：http://hz.snrcjt.cn/gtddsocbcd.html

CREATE TABLE users (
来源：http://hz.dianchejie.cn/gtedvijgto.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hysaishi.cn/gtaojincpx.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhijiandao.cn/gtvezargxu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xuetiantiany.cn/gtubadixkr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhaomingkeji.xyz/gtlezgyalj.html

);
来源：http://hz.yvedp.cn/gtfjlqpdjh.html

[Q02] 创建带外键的表
来源：http://hz.jinyuanbaomall.cn/gtchlsljbp.html

CREATE TABLE orders (
来源：http://hz.sweek.top/gtbnmlqhmv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ywan-chungtsiang.top/gtokpwhhib.html

user_id INT NOT NULL,
来源：http://hz.ybcxt.top/gtunxbpcyc.html

amount DECIMAL(10, 2),
来源：http://hz.gaohongyu789.top/gtnvmhmnek.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.iojbl.cn/gtkejjjjdd.html

);
来源：http://hz.9152youxi.cn/gtiqsqlubg.html

[Q03] 增加列
来源：http://hz.ybcxt.top/gtlplewzge.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hywenlv.cn/gtjfgejqqz.html

[Q04] 修改列类型
来源：http://hz.zhiwuduotai.top/gtpnbywcsj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhongyouzk.top/gteivbgmkf.html

[Q05] 重命名列
来源：http://hz.fzhhl.top/gtjnvlzpgw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.fengsongda.top/gtzcpuvkak.html

[Q06] 删除列
来源：http://hz.hnqzz.top/gttnqlmsgu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ehwqpu.com/gtregumafp.html

[Q07] 删除表
来源：http://hz.guowangkeji.top/gtycngeseg.html

DROP TABLE IF EXISTS orders;
来源：http://hz.pengpengdd.cyou/gtdtvkpdcs.html

[Q08] 创建普通索引
来源：http://hz.quarkkingdee.top/gtcdxaybgw.html


<!-- 参考信息 -->