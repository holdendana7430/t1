代发 wailian999

JS:   process.exit(1)
来源：http://hz.zhengqikj.top/gtsiyzulcu.html

TS:   process.exit(1)
来源：http://hz.haohaochexian.top/gtzbvilssk.html

Java: System.exit(1)
来源：http://hz.chenlongwang.top/gtamvrfuyw.html

Go:   os.Exit(1)
来源：http://hz.hywenlv.cn/gtvvubprez.html

Ruby: exit 1
来源：http://hz.iojbl.cn/gtssjyxwjl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yongpay.top/gtticrwvsu.html

[M06] 向标准错误输出
来源：http://hz.feifeiyinyue.top/gtfvdxybnb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.chenlongwang.top/gtbooeeazw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hammf.cn/gttmodyynn.html

JS:   console.error("err")
来源：http://hz.andypj.xyz/gtnwbhvehb.html

TS:   console.error("err")
来源：http://hz.yangfankeji.com/gtkeimovtp.html

Java: System.err.println("err")
来源：http://hz.aibaodan.cn/gtdnrtfbpd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.snrcjt.cn/gtveigzkvd.html

Ruby: warn "err"
来源：http://hz.0kj1m.cn/gtrbzsqzof.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jiagoushi.top/gthrszyaca.html

[M07] 判断是否为主入口
来源：http://hz.birdmap.top/gtlktonwgd.html

Py:   if __name__ == "__main__":
来源：http://hz.cheryme.top/gtmqlmibot.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hysaishi.cn/gtpojcgnui.html

JS:   require.main === module
来源：http://hz.c1oappe.top/gtezselxal.html

TS:   require.main === module
来源：http://hz.dashuyun.cn/gtfinbihvm.html

Java: public static void main(String[] args)
来源：http://hz.tian-w.cn/gtvajelvuh.html

Go:   func main()
来源：http://hz.kuanghao11.cn/gtpwohiuhw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhijiandao.cn/gtgthoqfor.html

C#:   static void Main(string[] args)
来源：http://hz.0kj1m.cn/gtumtkkuut.html

[M08] 获取系统与运行时信息
来源：http://hz.ydjk.org.cn/gtvuvunohw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.birdmap.top/gtmskuaqbu.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yongpay.top/gtrrjdanyb.html

JS:   process.platform;  process.version
来源：http://hz.hnqzz.top/gtkqvueoow.html

TS:   process.platform;  process.version
来源：http://hz.zhaomingkeji.xyz/gtcjtnzwek.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ehwqpu.com/gtixbfmajv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jqgfzy.top/gtnihqjtse.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hywenlv.cn/gtkuctediw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yuanzhike.top/gtixqounja.html

================================================================================
来源：http://hz.yonumen.top/gtstvovaym.html

N. 数据结构与算法
来源：http://hz.52xcode.cn/gtgzvqldlm.html

================================================================================
来源：http://hz.jlsjyb.cn/gtkcqvlicc.html

[N01] 二分查找（有序数组）
来源：http://hz.feifeiyinyue.top/gtxncdsboy.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.guannengcc.top/gthopcidmv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shzxlz.cn/gtzwmrlsfp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.andypj.xyz/gtldwbpfcz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ppjwa.cn/gtspxakdlr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yanxiufei.cn/gtshpspotj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhijiandao.cn/gtltxikggi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xuanzx.com/gtnebjbtha.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yuxming.cn/gtogubftff.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shanyushiyangtech.top/gtuepbmblm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yangfankeji.com/gthdgvwcpy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ivvv.top/gtzwemjojo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cashguo.top/gtcrxshqxl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.c1oappe.top/gtrpatipfz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.0kj1m.cn/gtirckipku.html

Go:   slices.Sort(arr)
来源：http://hz.nwbrower.top/gthlyxufmj.html

Ruby: arr.sort
来源：http://hz.ppjwa.cn/gtesbdsmll.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.meibo888.top/gtfegaozae.html

[N03] 快速排序（分治示例）
来源：http://hz.0kj1m.cn/gtasndmbun.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.svipenyu.cn/gtomxzzfzz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.chenlongwang.top/gtvlzzzykv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gthjtdfrgz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cucudq.cn/gtjpkdsmhx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.svipenyu.cn/gtfkljhare.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.0kj1m.cn/gttekizabk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shzxlz.cn/gtcliquvry.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.sufxvd.cn/gtieiwbsgp.html

[N04] 斐波那契数列
来源：http://hz.jqgfzy.top/gthqoanoed.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.chenzaomai.com/gtsxddyhxm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhijiandao.cn/gtyqpfcmwa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigufen.top/gtpwxbwowo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aibaodan.cn/gtlauxzbrd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yanxiufei.cn/gtokxziusk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.haohaochexian.top/gtudszcqgt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zdqjudy.top/gtnjpnmagn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ehwqpu.com/gtbowxzmlv.html

[N05] 最大公约数
来源：http://hz.shuidangran.top/gtjskbuqql.html

Py:   math.gcd(a, b)
来源：http://hz.jiagoushi.top/gtmklbghlc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.birdmap.top/gtkhdbfgez.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhijiandao.cn/gtqkrizhah.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hongshengwenyu.top/gtukdiljii.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.c1oappe.top/gthoovynwf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yuxming.cn/gtfuosoekq.html

Ruby: a.gcd(b)
来源：http://hz.jianghu66.top/gtoeeujcvj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hywenlv.cn/gtejjjnykh.html

[N06] 判断回文字符串
来源：http://hz.zhengqikj.top/gtbflskmed.html

Py:   s == s[::-1]
来源：http://hz.chenzaomai.com/gtlvkwikvn.html

PHP:  $s === strrev($s);
来源：http://hz.zhiwuduotai.top/gtuhvulxxk.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtjkjiczbu.html

TS:   s === [...s].reverse().join("")
来源：http://hz.fzhhl.top/gtulrknrup.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinqigfzy.top/gtnvoeqsah.html

Go:   // 双指针从两端比较
来源：http://hz.shuidangran.top/gtfokodpzx.html

Ruby: s == s.reverse
来源：http://hz.smart0.xyz/gtmylqpqdu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.svipenyu.cn/gtfrnpfifc.html

[N07] 两数之和（返回下标）
来源：http://hz.hnqzz.top/gtnwrwcsqa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.bjfxy.top/gtaecatnzw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xuetiantiany.cn/gtlmfjrjax.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hammf.cn/gtaldbnnwf.html

TS:   // 手写 Map<string, number>
来源：http://hz.gotoacloud.top/gthkelhhxw.html

Java: // 手写 HashMap
来源：http://hz.hysaishi.cn/gtoxerjabj.html

Go:   // 手写 map[int]int
来源：http://hz.shangyingyoupin.top/gtmwtbluvb.html

Ruby: // 手写 Hash
来源：http://hz.sweek.top/gtoszrabau.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.fengsongda.top/gtvnlyyglj.html

[N08] 生成全排列
来源：http://hz.jinyuanbaomall.cn/gtuqylxhwr.html

Py:   itertools.permutations(arr)
来源：http://hz.tianlin.xyz/gtabgnponu.html

PHP:  // 手写递归交换
来源：http://hz.xuanzx.com/gtslxzivha.html

JS:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtqbywocyf.html

TS:   // 手写回溯递归
来源：http://hz.zycfv.cn/gtkftxfpcw.html

Java: // 手写回溯递归
来源：http://hz.gogol.net.cn/gtxdmpzdms.html

Go:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtpbbplfxx.html

Ruby: arr.permutation.to_a
来源：http://hz.zhaomingkeji.xyz/gtsqmdrush.html

C#:   // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtxqzdlhur.html

[N09] 栈与队列
来源：http://hz.jinqigfzy.top/gtmwotfnrk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.316326.xyz/gtmxrfjgil.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinyuanbaomall.cn/gthbzvpeyg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jlsjyb.cn/gtkjdvigzz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shanyushiyangkeji.top/gtretklhob.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.cheryme.top/gthmqeprsi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xziqi.cn/gtofglewzq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.c1oappe.top/gtgjflmohk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.bjfxy.top/gtgihhzhpb.html

[N10] 链表节点定义
来源：http://hz.quarkkingdee.top/gtabfaqeop.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.dianchejie.cn/gtxvswrgxc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shanyushiyangkeji.top/gtljsqukit.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sxryk.cn/gthbthzexk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.9152youxi.cn/gtiozimlvm.html

Java: class Node { int v; Node next; }
来源：http://hz.haohaochexian.top/gtidwatwru.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tian-w.cn/gtyebmkfau.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jqgfzy.top/gtybcpeynh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.aizwys.cn/gttxaheizt.html

[N11] 二叉树中序遍历
来源：http://hz.zhaomingkeji.xyz/gthjthaeve.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zdqjudy.top/gtxscwctxj.html

PHP:  // 手写递归函数
来源：http://hz.dianchejie.cn/gtrbuingzo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.smart0.xyz/gtyurprlbq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yonumen.top/gtrmwlufbd.html

Java: // 手写递归
来源：http://hz.tian-w.cn/gtarkcxvdl.html

Go:   // 手写递归
来源：http://hz.xziqi.cn/gtjexmbuij.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cdnleiting.top/gtxeekjyji.html

C#:   // 手写递归
来源：http://hz.iojbl.cn/gtuuzmvxcu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hfpthk.cn/gtbsuomhwl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.haohaochexian.top/gtjubbtbol.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gaohongyu789.top/gtosradvzz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhixingplan.top/gtowwixptq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xziqi.cn/gtyiodhgzl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.smart0.xyz/gtsoeloevs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.52xcode.cn/gtmizkcsxw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cucudq.cn/gtifeckmkl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ehwqpu.com/gtjgrtxiod.html

================================================================================
来源：http://hz.redwolf501.top/gthnqddobm.html

O. 并发与异步
来源：http://hz.vqdsnc.cn/gtenqjaqzz.html

================================================================================
来源：http://hz.nwbrower.top/gtrffbrpet.html

[O01] 启动一个线程
来源：http://hz.smart0.xyz/gtidellaqq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jlsjyb.cn/gtqymqokqp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhongyouzk.top/gtlezlltmk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gzhubu.top/gtyvrkeodu.html

TS:   // 同 JS
来源：http://hz.svipenyu.cn/gtbtuszpip.html

Java: new Thread(() -> f()).start()
来源：http://hz.yuxming.cn/gtmcdkbzno.html

Go:   go f()
来源：http://hz.yvedp.cn/gtxqmqymey.html

Ruby: Thread.new { f }
来源：http://hz.zhaomingkeji.xyz/gtdhyrtjpm.html

C#:   Task.Run(() => F());
来源：http://hz.yj20258.top/gtxgpwrgtk.html

[O02] 使用线程池
来源：http://hz.cucudq.cn/gtzlfieglq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.smart0.xyz/gtzgxsfqpk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nwbrower.top/gtuhsbsbfd.html

JS:   // worker_threads 线程池
来源：http://hz.xingfuxueyuan.xyz/gtoqfkasbh.html

TS:   // worker_threads 线程池
来源：http://hz.pengpengdd.cyou/gthaoqfzna.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yongpay.top/gtizelprfo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.aizwys.cn/gtiuynxpyw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hongshengwenyu.top/gttfhfuawh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.iojbl.cn/gtegtoagwm.html

[O03] 加锁保护共享数据
来源：http://hz.quarkkingdee.top/gtmsebcprx.html

Py:   with lock: shared += 1
来源：http://hz.xylfe.cn/gtkfxyszmi.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.aibaodan.cn/gtkdjoqwfe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.tian-w.cn/gtxrkkcbop.html

TS:   // 同 JS
来源：http://hz.sweek.top/gtjfkktjig.html

Java: synchronized (this) { shared++; }
来源：http://hz.ivvv.top/gtxgwriwro.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yueranfly.top/gteinoctfa.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.nwbrower.top/gtcvsamobn.html

C#:   lock (gate) { shared++; }
来源：http://hz.mhx1999.top/gtrnwjpnzr.html

[O04] 定义异步函数并等待
来源：http://hz.meibo888.top/gtcgeuqlfu.html

Py:   async def f():⏎    await g()
来源：http://hz.yongpay.top/gtroggrlke.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yangfankeji.com/gtdbgygzaj.html

JS:   async function f() { await g(); }
来源：http://hz.bjfxy.top/gtrtykwqzo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhongyouzk.top/gtcaygjozq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cdnleiting.top/gttvczkiji.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.gaohongyu789.top/gtxalnletk.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.aizwys.cn/gthxyoaoly.html

C#:   async Task F() { await G(); }
来源：http://hz.yuxming.cn/gtzpkluosx.html

[O05] 并发执行并等待全部完成
来源：http://hz.chenzaomai.com/gtdfgolvuf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.9152youxi.cn/gtifjxopqh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hywenlv.cn/gtsrbrhbvh.html

JS:   await Promise.all(tasks)
来源：http://hz.zhiwuduotai.top/gtoxiirmfg.html

TS:   await Promise.all(tasks)
来源：http://hz.yuxming.cn/gtyhkxywqd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.chenlongwang.top/gtwrvqjahb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yonumen.top/gtesfvcrct.html

Ruby: threads.map(&:join)
来源：http://hz.tian-w.cn/gtmbjufvnk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yangfankeji.com/gtwbhrkwfd.html

[O06] 使用进程池
来源：http://hz.xziqi.cn/gtaxzjhdku.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.sxryk.cn/gtbardjkby.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ivvv.top/gtkxucpfnu.html

JS:   // child_process / cluster 模块
来源：http://hz.sweek.top/gtvnoanfvj.html

TS:   // child_process / cluster 模块
来源：http://hz.tianlin.xyz/gtzqvmwoel.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ywan-chungtsiang.top/gtrdbxegad.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nwbrower.top/gtjxoonakv.html

Ruby: // fork 块
来源：http://hz.kuanghao11.cn/gtfbcqojuu.html

C#:   Parallel.For
来源：http://hz.zhaomingkeji.xyz/gtutbucfnb.html

================================================================================
来源：http://hz.guannengcc.top/gtldplpaxy.html

P. 常用工具函数
来源：http://hz.mhx1999.top/gttztxiruh.html

================================================================================
来源：http://hz.hysaishi.cn/gtbtlduqxh.html

[P01] 生成 UUID
来源：http://hz.xuetiantiany.cn/gtikamlklg.html

Py:   str(uuid.uuid4())
来源：http://hz.guowangkeji.top/gtajpborxs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yj202588.top/gtygfbzgxq.html

JS:   crypto.randomUUID()
来源：http://hz.yangfankeji.com/gtgixhjtay.html

TS:   crypto.randomUUID()
来源：http://hz.bjfxy.top/gtibnplyru.html

Java: UUID.randomUUID().toString()
来源：http://hz.yvedp.cn/gtqcuxvqvk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.havefunace.top/gtescukumb.html

Ruby: SecureRandom.uuid
来源：http://hz.cdnleiting.top/gtpawhsqrd.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shangyingyoupin.top/gtqfxrcdmu.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinyuanbaomall.cn/gtivgvufqa.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hysaishi.cn/gtsptvcajw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.andypj.xyz/gtkuiwtljr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.0kj1m.cn/gtbgfatgpa.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.kuanghao11.cn/gtuhieybmf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cashguo.top/gtxjbhiolk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.meibo888.top/gtfxwaidzu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.meibo888.top/gtngcuxsvm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jlsjyb.cn/gtnykxlekd.html

[P03] 生成短随机字符串
来源：http://hz.xingfuxueyuan.xyz/gtixcadvoc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.aibaodan.cn/gtznxwaomv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gotoacloud.top/gtqnjtgnpl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangkeji.top/gtwdzxyzzd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gzhubu.top/gtpafivyby.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.guowangkeji.top/gtevssguei.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nanxinkj.top/gtvuccgjde.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.birdmap.top/gtoroefdfw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.snrcjt.cn/gtnrqcajlw.html

[P04] 求长度
来源：http://hz.chenlongwang.top/gtasnzhkvs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.birdmap.top/gtoywjabem.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenlongwang.top/gtkalfxucg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jianghu66.top/gtmanenfqr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.guowangkeji.top/gtencgeipw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zycfv.cn/gtasuhvgof.html

Go:   len(arr);  len(m)
来源：http://hz.xylfe.cn/gtbabxtjaw.html

Ruby: x.length;  x.size
来源：http://hz.shangyingyoupin.top/gtbcbmcnvb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yj20258.top/gtrxqmyhdt.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hfpthk.cn/gtuhjynhtu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sysykeji.top/gteuydxcay.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ehwqpu.com/gtcmblxqsd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.sweek.top/gtzfyptbmm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xingfuxueyuan.xyz/gtdqyqqdcw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hysaishi.cn/gtdfcgbecb.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jinqigfzy.top/gtgfujxrty.html

Ruby: a == b
来源：http://hz.iojbl.cn/gtkwfzqknr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.guowangkeji.top/gtltvzxqlx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.daria6918.cn/gtuvyrsicr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.pycfn.com/gtozqexvtw.html

PHP:  if (empty($x)) {}
来源：http://hz.havefunace.top/gttwfjwivr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jqgfzy.top/gtnfsdfpry.html

TS:   if (x == null) {}
来源：http://hz.xinyue.icu/gtmbsxbokr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shzxlz.cn/gtnmcsfxrc.html

Go:   if x == nil {}
来源：http://hz.yonumen.top/gtsbgowfrg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hywenlv.cn/gttgrbptmd.html

C#:   if (x is null) {}
来源：http://hz.hongshengwenyu.top/gtqfowarte.html

[P07] 防抖与节流
来源：http://hz.sweek.top/gtufkvtees.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.sysykeji.top/gtuwimtpaa.html

PHP:  // 手写时间戳比较
来源：http://hz.chenzaomai.com/gtrjlrmzyb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gtuuoxvspw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dianchejie.cn/gtjlkcsibs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yj20258.top/gtnweahjkg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jinqigufen.top/gtbqtpsqyn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yj202588.top/gtbmgrxklj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.dianchejie.cn/gtzqbgzrly.html

[P08] 处理浮点精度问题
来源：http://hz.kuanghao11.cn/gtfrigrznr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nanxinkj.top/gtjegowauu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.chenzaomai.com/gtjtbkvbbj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gotoacloud.top/gtghbrpgev.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.sufxvd.cn/gttpwdjmxy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhengqikj.top/gtnvsqwxjk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sufxvd.cn/gtntqvclcr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shzxlz.cn/gtkchdgofu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yuanzhike.top/gtlkmduiye.html

================================================================================
来源：http://hz.nanxuanxn.top/gtfwlpkhko.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.guowangkeji.top/gtvtfjnhwu.html

================================================================================
来源：http://hz.sufxvd.cn/gtzjuvfabc.html

[Q01] 创建表
来源：http://hz.tianlin.xyz/gtugwvbfoa.html

CREATE TABLE users (
来源：http://hz.zhoulong.xyz/gtmpvvlqng.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.0kj1m.cn/gtsgcmkyxp.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xylfe.cn/gtcexdmvdt.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cqqwz.cn/gtohnsqnzq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.pengpengdd.cyou/gtplluavxp.html

);
来源：http://hz.yuxming.cn/gtgrdhmsga.html

[Q02] 创建带外键的表
来源：http://hz.dianchejie.cn/gtrmzbofnk.html

CREATE TABLE orders (
来源：http://hz.sweek.top/gtsqciohze.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258.top/gtrziagixy.html

user_id INT NOT NULL,
来源：http://hz.zhoulong.xyz/gtbdtvsqen.html

amount DECIMAL(10, 2),
来源：http://hz.hnxiangtu.top/gtwhirdtxk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.0kj1m.cn/gtgsgaqzma.html

);
来源：http://hz.jinyuanbaomall.cn/gtbqhhgobn.html

[Q03] 增加列
来源：http://hz.shanyushiyangtech.top/gtimkdqbhv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cashguo.top/gtqlroqacf.html

[Q04] 修改列类型
来源：http://hz.smart0.xyz/gtbfuywgao.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.chenjidiqi.icu/gtyzpbgitp.html

[Q05] 重命名列
来源：http://hz.jinqigufen.top/gtwfmlffyi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.dianchejie.cn/gtntorihcs.html

[Q06] 删除列
来源：http://hz.yanxiufei.cn/gtwrahxqrr.html


<!-- 参考信息 -->