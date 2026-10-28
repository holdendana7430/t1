代发 wailian999

Ruby: exit 1
来源：http://hz.zhiwuduotai.top/gtypxdumqo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xingfuxueyuan.xyz/gtgygywkaj.html

[M06] 向标准错误输出
来源：http://hz.yvedp.cn/gtiarbqkxh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.kuanghao11.cn/gtzxlawjvf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.nanxuanxn.top/gtsoyvpclt.html

JS:   console.error("err")
来源：http://hz.smart0.xyz/gtpwhqogfi.html

TS:   console.error("err")
来源：http://hz.zdqjudy.top/gthknvwuhq.html

Java: System.err.println("err")
来源：http://hz.cashguo.top/gtlqzykhmf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jqgufenzy.top/gtgepzrdfz.html

Ruby: warn "err"
来源：http://hz.guowangkeji.top/gtnsgrmvgh.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.sufxvd.cn/gtxledornt.html

[M07] 判断是否为主入口
来源：http://hz.gotoacloud.top/gtglrgrbaw.html

Py:   if __name__ == "__main__":
来源：http://hz.haohaochexian.top/gtnutswaxu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhiwuduotai.top/gtuvvtvfsh.html

JS:   require.main === module
来源：http://hz.zhoulong.xyz/gtlnyspkrp.html

TS:   require.main === module
来源：http://hz.chenjidiqi.icu/gtscwpmhos.html

Java: public static void main(String[] args)
来源：http://hz.yj20258.top/gthfwfdvvc.html

Go:   func main()
来源：http://hz.tian-w.cn/gtijoesixg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.fzhhl.top/gtmyeeyyih.html

C#:   static void Main(string[] args)
来源：http://hz.hnqzz.top/gtemjbukcf.html

[M08] 获取系统与运行时信息
来源：http://hz.chenzaomai.com/gtpioowbtl.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yj20258.top/gtxjztoqqz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.haohaochexian.top/gtmchrezlw.html

JS:   process.platform;  process.version
来源：http://hz.nwbrower.top/gtzcxjwbvm.html

TS:   process.platform;  process.version
来源：http://hz.gzhubu.top/gtsutqgjwe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.fengsongda.top/gtcazxqjsr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.aibaodan.cn/gtibobxgki.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yongpay.top/gtlxjnifgc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.fengsongda.top/gtkfigggip.html

================================================================================
来源：http://hz.haohaochexian.top/gtzqdwrqyn.html

N. 数据结构与算法
来源：http://hz.zhengqikj.top/gtsprqpuyr.html

================================================================================
来源：http://hz.dashuyun.cn/gtfileubqc.html

[N01] 二分查找（有序数组）
来源：http://hz.vqdsnc.cn/gtamzxhqhc.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj20258888.top/gtewdamfbl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.guannengcc.top/gtwybdezzk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinyuanbaomall.cn/gtaopbldma.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnqzz.top/gtwpfpczpk.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.c1oappe.top/gtfkjutfzh.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cucudq.cn/gtkwwgeyej.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xziqi.cn/gtuzvwgsfl.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ivvv.top/gtkmnqxwpg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xuetiantiany.cn/gtbgbtsiek.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.snrcjt.cn/gtpllpkyxn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zycfv.cn/gtgorpdhmb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenlongwang.top/gtdgkrkwjh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cashguo.top/gtwvqctphe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.tanke756.top/gtifahztdf.html

Go:   slices.Sort(arr)
来源：http://hz.xylfe.cn/gtlhvwgafk.html

Ruby: arr.sort
来源：http://hz.hongshengwenyu.top/gturxbyflo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.daria6918.cn/gtzbxjhypm.html

[N03] 快速排序（分治示例）
来源：http://hz.shanyushiyangtech.top/gtxnsieqzz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jlsjyb.cn/gtenaibuoi.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gotoacloud.top/gtlkarsmsb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydzc1.top/gtvfgrirbh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xziqi.cn/gtuudpbbfe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.chenzaomai.com/gtcajrhynk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hongshengwenyu.top/gtqfzzjlgv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gaohongyu789.top/gtdlofuous.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jqgfzy.top/gtrjqfahgn.html

[N04] 斐波那契数列
来源：http://hz.zhijiandao.cn/gtzantnooe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hysaishi.cn/gtnoqrwguk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yueranfly.top/gtkzmvmtgw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.mhx1999.top/gtutgxrjcg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xziqi.cn/gttgkrphul.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yvedp.cn/gtfvxmydea.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.smart0.xyz/gtsuonrrnl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.wangdashe.top/gtkjxycrgg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sysykeji.top/gthnpspeqv.html

[N05] 最大公约数
来源：http://hz.yangfankeji.com/gtjvajbtjg.html

Py:   math.gcd(a, b)
来源：http://hz.hongshengwenyu.top/gtezuqsqjy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tanke756.top/gtmcalexwi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ivvv.top/gtabaejfpm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.svipenyu.cn/gtklznobce.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gotoacloud.top/gtyhlydisc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.daria6918.cn/gtqssherpy.html

Ruby: a.gcd(b)
来源：http://hz.smart0.xyz/gtmnwzyvwt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xuetiantiany.cn/gtqorqsork.html

[N06] 判断回文字符串
来源：http://hz.svipenyu.cn/gtojyjuays.html

Py:   s == s[::-1]
来源：http://hz.52xcode.cn/gtzdnjdzuf.html

PHP:  $s === strrev($s);
来源：http://hz.hongshengwenyu.top/gtkipexgio.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yanxiufei.cn/gtkvdymooy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtmnhppxkr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zdqjudy.top/gtlilihnzv.html

Go:   // 双指针从两端比较
来源：http://hz.hammf.cn/gtdygmkqvv.html

Ruby: s == s.reverse
来源：http://hz.yongpay.top/gtfwyyhmrd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.feifeiyinyue.top/gtomncfnry.html

[N07] 两数之和（返回下标）
来源：http://hz.dashuyun.cn/gtntktvkaf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhixingplan.top/gtjhottrdn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yuanzhike.top/gtiyzgfura.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.cdnleiting.top/gtehwsutjm.html

TS:   // 手写 Map<string, number>
来源：http://hz.tianlin.xyz/gtfyshctkd.html

Java: // 手写 HashMap
来源：http://hz.nanxinkj.top/gtxrqdewpu.html

Go:   // 手写 map[int]int
来源：http://hz.mhx1999.top/gthygdrvti.html

Ruby: // 手写 Hash
来源：http://hz.ywan-chungtsiang.top/gthdssshgg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sxryk.cn/gtrrpbmhli.html

[N08] 生成全排列
来源：http://hz.gaohongyu789.top/gtlbbejgko.html

Py:   itertools.permutations(arr)
来源：http://hz.yangfankeji.com/gtpqvzfdqp.html

PHP:  // 手写递归交换
来源：http://hz.birdmap.top/gtamgzqbza.html

JS:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gtogyahgak.html

TS:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtbkuegyma.html

Java: // 手写回溯递归
来源：http://hz.zycfv.cn/gtsftlyyfr.html

Go:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gttiofuyln.html

Ruby: arr.permutation.to_a
来源：http://hz.yuxming.cn/gtlualnusg.html

C#:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gthrszxeen.html

[N09] 栈与队列
来源：http://hz.ybcxt.top/gtydpttobg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.52xcode.cn/gtrkkoxkoa.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.redwolf501.top/gtyftztfsv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.nanxinkj.top/gtipsbqrym.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.chenjidiqi.icu/gtasqymucx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sxryk.cn/gtpttfphrh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ivvv.top/gtofufvxor.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.dianchejie.cn/gtfyumorsa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.wangdashe.top/gtgcjjcxys.html

[N10] 链表节点定义
来源：http://hz.yonumen.top/gtpqrmiibt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.fzhhl.top/gtlhtlcaos.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.aibaodan.cn/gticybfanf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.tian-w.cn/gteigaiuax.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shzxlz.cn/gtdudfzrqm.html

Java: class Node { int v; Node next; }
来源：http://hz.jinyuanbaomall.cn/gtpuozmgdk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhengqikj.top/gttanepcsd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.tianlin.xyz/gtvcjafiis.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.aizwys.cn/gtvycspqtn.html

[N11] 二叉树中序遍历
来源：http://hz.nwbrower.top/gtxljfrdkd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.fengsongda.top/gtyrqqyccb.html

PHP:  // 手写递归函数
来源：http://hz.hfpthk.cn/gtaacfnfqe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhengqikj.top/gteawkmxro.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sweek.top/gtmddzwdhc.html

Java: // 手写递归
来源：http://hz.birdmap.top/gttdnbgxgw.html

Go:   // 手写递归
来源：http://hz.fengsongda.top/gthkeyxcea.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhiwuduotai.top/gttyhgjvrg.html

C#:   // 手写递归
来源：http://hz.sufxvd.cn/gteofvpokq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.smart0.xyz/gtnuinxtyy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinqigufen.top/gtoerzqomq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yj202588.top/gtctrgcjnm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.quarkkingdee.top/gtufykrsup.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhongyouzk.top/gtsgipcmfb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pengpengdd.cyou/gtwjbhvzmx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.0kj1m.cn/gtpichzxtr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yuxming.cn/gtwckvoplf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yvedp.cn/gtnvbtzdmk.html

================================================================================
来源：http://hz.sufxvd.cn/gtjebbnpex.html

O. 并发与异步
来源：http://hz.gaohongyu789.top/gtqchsdgdo.html

================================================================================
来源：http://hz.yangfankeji.com/gtpijwpfuz.html

[O01] 启动一个线程
来源：http://hz.pycfn.com/gtrehzxjsj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.iojbl.cn/gtinzonxsr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.birdmap.top/gtidwkycjy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.wangdashe.top/gtklqjoayu.html

TS:   // 同 JS
来源：http://hz.hfpthk.cn/gtwuggumze.html

Java: new Thread(() -> f()).start()
来源：http://hz.hfpthk.cn/gtdauwfgup.html

Go:   go f()
来源：http://hz.cashguo.top/gtcykecwrm.html

Ruby: Thread.new { f }
来源：http://hz.zhoulong.xyz/gtesdtahzp.html

C#:   Task.Run(() => F());
来源：http://hz.mhx1999.top/gtzsoanlxh.html

[O02] 使用线程池
来源：http://hz.ywan-chungtsiang.top/gtxjsuvybc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ppjwa.cn/gtmqobeasz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shzxlz.cn/gtlibrugvy.html

JS:   // worker_threads 线程池
来源：http://hz.nanxuanxn.top/gtaqqwstkv.html

TS:   // worker_threads 线程池
来源：http://hz.hnxiangtu.top/gtxupxhddk.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jlsjyb.cn/gtpboptdez.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jinghuilouyu.cn/gtyjdbdolq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ydjk.org.cn/gtujypjhxz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.nanxuanxn.top/gtfwkjboqg.html

[O03] 加锁保护共享数据
来源：http://hz.redwolf501.top/gtxvpduwsv.html

Py:   with lock: shared += 1
来源：http://hz.xylfe.cn/gthqnrbppz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.chenlongwang.top/gtbzrunwrm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yj202588.top/gtmnfvtbzl.html

TS:   // 同 JS
来源：http://hz.kuanghao11.cn/gtpfwzlkjf.html

Java: synchronized (this) { shared++; }
来源：http://hz.snrcjt.cn/gtjnihoxcl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ydjk.org.cn/gtdynzvcko.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yangfankeji.com/gtqjmdayog.html

C#:   lock (gate) { shared++; }
来源：http://hz.xuanzx.com/gtkyjdimge.html

[O04] 定义异步函数并等待
来源：http://hz.kuanghao11.cn/gtigojfozg.html

Py:   async def f():⏎    await g()
来源：http://hz.yueranfly.top/gtqdhlwvjw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hnqzz.top/gtuygqbtgo.html

JS:   async function f() { await g(); }
来源：http://hz.xylfe.cn/gtholavbbw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.smart0.xyz/gtshlotmws.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hnqzz.top/gtuqgfnmno.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.quarkkingdee.top/gtuoroonpt.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.fengsongda.top/gtvqubouvr.html

C#:   async Task F() { await G(); }
来源：http://hz.zhengqikj.top/gthkdpltqz.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhijiandao.cn/gtnqzoahwc.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jyoumei.cn/gtzydyxxxw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.pengpengdd.cyou/gtybpmpiyu.html

JS:   await Promise.all(tasks)
来源：http://hz.yuxming.cn/gtywktdcrj.html

TS:   await Promise.all(tasks)
来源：http://hz.cheryme.top/gtgqdfktmz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.wangshuangyany.cn/gtmgyujloc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.mhx1999.top/gtwywdgava.html

Ruby: threads.map(&:join)
来源：http://hz.wangshuangyany.cn/gtpzxsfjhp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.mhx1999.top/gtdqlwhbfz.html

[O06] 使用进程池
来源：http://hz.bjfxy.top/gtmfevykar.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jqgfzy.top/gtjskolxlh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jqgfzy.top/gtttnsaskd.html

JS:   // child_process / cluster 模块
来源：http://hz.yongpay.top/gtmscclpei.html

TS:   // child_process / cluster 模块
来源：http://hz.shangyingyoupin.top/gttjothjuk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hongshengwenyu.top/gtxtophrod.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.fengsongda.top/gtxgbnovms.html

Ruby: // fork 块
来源：http://hz.gzhubu.top/gttjbrlvkc.html

C#:   Parallel.For
来源：http://hz.fzhhl.top/gtwshcqwwi.html

================================================================================
来源：http://hz.havefunace.top/gtzfosohrj.html

P. 常用工具函数
来源：http://hz.nanxinkj.top/gtisgypdrc.html

================================================================================
来源：http://hz.jqgufenzy.top/gtcumnwjnn.html

[P01] 生成 UUID
来源：http://hz.xylfe.cn/gtjjwacxiv.html

Py:   str(uuid.uuid4())
来源：http://hz.meibo888.top/gtskpmoncv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yanxiufei.cn/gtexyavgsc.html

JS:   crypto.randomUUID()
来源：http://hz.gotoacloud.top/gtrvtbpjok.html

TS:   crypto.randomUUID()
来源：http://hz.sufxvd.cn/gtopnuqjnq.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhixingplan.top/gtroeuqeab.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jlsjyb.cn/gtfklobdco.html

Ruby: SecureRandom.uuid
来源：http://hz.ywan-chungtsiang.top/gtavknvyai.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jianghu66.top/gtatqinbsa.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ydzc1.top/gtnochntur.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.mhx1999.top/gtbfstqhky.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.wangdashe.top/gtmgdbakmx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yueranfly.top/gtxhzepqpo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.tanke756.top/gtuguvaome.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.quarkkingdee.top/gtxjavlyns.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cqqwz.cn/gtuuemaasd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yvedp.cn/gtsvmhuhtj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.chenzaomai.com/gtzaonuwac.html

[P03] 生成短随机字符串
来源：http://hz.yuxming.cn/gtmtzrmrlf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.52xcode.cn/gtotlvxsjt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ehwqpu.com/gtcgkhmrks.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ehwqpu.com/gtqdpzrmnq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.havefunace.top/gtvyxpiveg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ydzc1.top/gtkdehouxb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhixingplan.top/gtfajgwmbn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ppjwa.cn/gtarhglcbn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hysaishi.cn/gtpimnsihg.html

[P04] 求长度
来源：http://hz.nwbrower.top/gtaafemwpq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yvedp.cn/gtpazafnpu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj202588.top/gtrpcgvvqy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yueranfly.top/gtpvovlusw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydjk.org.cn/gtcwxcycbt.html

Java: list.size();  map.size();  s.length()
来源：http://hz.nanxuanxn.top/gtbttzolvr.html

Go:   len(arr);  len(m)
来源：http://hz.zhijiandao.cn/gtmbqoawnm.html

Ruby: x.length;  x.size
来源：http://hz.hfpthk.cn/gtratheett.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhengqikj.top/gtmozgabhh.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yvedp.cn/gtvsomaxas.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.c1oappe.top/gtbgujqcju.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cucudq.cn/gtgqymvqzw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.gogol.net.cn/gtrcqsrpfb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj20258888.top/gtysjsokkl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.havefunace.top/gtyzmwyvvl.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenjidiqi.icu/gtrdsskrgu.html

Ruby: a == b
来源：http://hz.chenjidiqi.icu/gtlpekxgqr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhixingplan.top/gtthzclvjy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hfpthk.cn/gtkueulduw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.chenzaomai.com/gtacbxyuou.html

PHP:  if (empty($x)) {}
来源：http://hz.ydjk.org.cn/gtdtyesclp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.feifeiyinyue.top/gtyeilvifm.html

TS:   if (x == null) {}
来源：http://hz.jinqigufen.top/gtukutfuuu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xziqi.cn/gtkzggmhbp.html

Go:   if x == nil {}
来源：http://hz.xziqi.cn/gtrptrztau.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zycfv.cn/gtmgliewrj.html

C#:   if (x is null) {}
来源：http://hz.c1oappe.top/gthwuoxdnz.html

[P07] 防抖与节流
来源：http://hz.havefunace.top/gtyxrghwrb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.sysykeji.top/gtqxbhrrjv.html

PHP:  // 手写时间戳比较
来源：http://hz.nanxuanxn.top/gtppxwvwgc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuetiantiany.cn/gtzvfytcyx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hywenlv.cn/gtrsrvozsz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhijiandao.cn/gtvalkfeps.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yj20258888.top/gtwtyikmip.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cucudq.cn/gtqixeaiaa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yuxming.cn/gtqynvohcp.html

[P08] 处理浮点精度问题
来源：http://hz.yonumen.top/gtetewwhic.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.c1oappe.top/gttamfnpyr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xinyue.icu/gtqvdlfvma.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhijiandao.cn/gtcyjbsmbq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.bjfxy.top/gttooavmlt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.tanke756.top/gtnbegjpab.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zdqjudy.top/gtwcgwpauf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.mhx1999.top/gtrlxdjlvy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.bjfxy.top/gtpzfqfmra.html

================================================================================
来源：http://hz.yj202588.top/gtwuzbrjva.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.chenjidiqi.icu/gtgwgmzkep.html

================================================================================
来源：http://hz.nwbrower.top/gtwhnnffzv.html

[Q01] 创建表
来源：http://hz.hywenlv.cn/gtvfkyvrrf.html

CREATE TABLE users (
来源：http://hz.hammf.cn/gtzzrgideh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sweek.top/gtpellmpan.html

name VARCHAR(50) NOT NULL,
来源：http://hz.svipenyu.cn/gttnhhrrkl.html

email VARCHAR(100) UNIQUE,
来源：http://hz.chenjidiqi.icu/gtjrtwgpib.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hysaishi.cn/gtkrtthfww.html

);
来源：http://hz.jqgfzy.top/gtciopvaoz.html

[Q02] 创建带外键的表
来源：http://hz.birdmap.top/gtkzirrfta.html

CREATE TABLE orders (
来源：http://hz.cucudq.cn/gtxczqwbue.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydjk.org.cn/gtzpblexrn.html

user_id INT NOT NULL,
来源：http://hz.yueranfly.top/gtcpclipil.html

amount DECIMAL(10, 2),
来源：http://hz.shanyushiyangkeji.top/gtzefocvft.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.svipenyu.cn/gtjyvnmkrn.html

);
来源：http://hz.xylfe.cn/gtqvobrudp.html

[Q03] 增加列
来源：http://hz.cheryme.top/gtfjruuiys.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.fengsongda.top/gtmxwhjgyx.html

[Q04] 修改列类型
来源：http://hz.wangdashe.top/gtrcgvtbic.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sysykeji.top/gttyzgnjcy.html

[Q05] 重命名列
来源：http://hz.yvedp.cn/gthjwxfjrp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj20258.top/gtcxvsksfr.html

[Q06] 删除列
来源：http://hz.zhaomingkeji.xyz/gtfvffxoqa.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sufxvd.cn/gtfbnwmraz.html

[Q07] 删除表
来源：http://hz.gaohongyu789.top/gtqtlzebcu.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sysykeji.top/gtgfrylgbt.html

[Q08] 创建普通索引
来源：http://hz.yvedp.cn/gtkhvdemst.html


<!-- 参考信息 -->