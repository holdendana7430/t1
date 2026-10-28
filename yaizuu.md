代发 wailian999

Ruby: exit 1
来源：http://hz.meibo888.top/gtmacgfzjs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yongpay.top/gthuvzqfau.html

[M06] 向标准错误输出
来源：http://hz.jinqigufen.top/gtetcratgc.html

Py:   print("err", file=sys.stderr)
来源：http://hz.daxiang520.top/gtlvldccmc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hysaishi.cn/gtwdljdtml.html

JS:   console.error("err")
来源：http://hz.c1oappe.top/gtakmclbrc.html

TS:   console.error("err")
来源：http://hz.wangdashe.top/gtifctuduz.html

Java: System.err.println("err")
来源：http://hz.jinghuilouyu.cn/gtbisoljfl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.nanxinkj.top/gttqcmtsnn.html

Ruby: warn "err"
来源：http://hz.yvedp.cn/gtoqlsvcsd.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.fengsongda.top/gtkbprctez.html

[M07] 判断是否为主入口
来源：http://hz.vqdsnc.cn/gtaqrjkelg.html

Py:   if __name__ == "__main__":
来源：http://hz.hnqzz.top/gtpqdxqint.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.dashuyun.cn/gtaxguzmgw.html

JS:   require.main === module
来源：http://hz.0kj1m.cn/gtifxjqutw.html

TS:   require.main === module
来源：http://hz.ehwqpu.com/gtxxxmrjut.html

Java: public static void main(String[] args)
来源：http://hz.sxryk.cn/gthtvtqhon.html

Go:   func main()
来源：http://hz.ehwqpu.com/gtcvzdoaal.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.havefunace.top/gtpkvpecvn.html

C#:   static void Main(string[] args)
来源：http://hz.zhiwuduotai.top/gtaunkpxdj.html

[M08] 获取系统与运行时信息
来源：http://hz.haohaochexian.top/gtdumicmeo.html

Py:   platform.system();  platform.python_version()
来源：http://hz.vqdsnc.cn/gtjvlzvhpc.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yanxiufei.cn/gticarlbup.html

JS:   process.platform;  process.version
来源：http://hz.aibaodan.cn/gtxujgnzrd.html

TS:   process.platform;  process.version
来源：http://hz.chenjidiqi.icu/gthlazltir.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yuxming.cn/gtrislkipp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.chenlongwang.top/gtuyoahtzc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xingfuxueyuan.xyz/gtehtszbqw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.chenzaomai.com/gtkxdqubih.html

================================================================================
来源：http://hz.yj202588.top/gtkdxylanm.html

N. 数据结构与算法
来源：http://hz.yj202588.top/gtztwratsz.html

================================================================================
来源：http://hz.yvedp.cn/gterfiggfz.html

[N01] 二分查找（有序数组）
来源：http://hz.nanxinkj.top/gtlvmwoqya.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.iojbl.cn/gtkrhwixlx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zdqjudy.top/gtpexjbuzj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenjidiqi.icu/gtdnxxyaqg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yanxiufei.cn/gtxrcefacz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hnqzz.top/gtqiupcdmk.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhiwuduotai.top/gtwypyrtzd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yvedp.cn/gtibuetqfl.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gtybdtkqyt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.iojbl.cn/gtduojoscw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigufen.top/gttexgcxtv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhijiandao.cn/gthgqbgjwn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daria6918.cn/gtqzrbwbmp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.52xcode.cn/gtcjjhouby.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.fengsongda.top/gtzusfgted.html

Go:   slices.Sort(arr)
来源：http://hz.jqgfzy.top/gtgvvwbaqo.html

Ruby: arr.sort
来源：http://hz.snrcjt.cn/gtvqhbocho.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.dianchejie.cn/gtrqdeftnm.html

[N03] 快速排序（分治示例）
来源：http://hz.yuxming.cn/gtikgagotq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.birdmap.top/gtcdcexlzn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tian-w.cn/gtguolqhtk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gzhubu.top/gtraquirou.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pengpengdd.cyou/gtpnszfykp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.dianchejie.cn/gtktcignys.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jyoumei.cn/gtzgoqmyxc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.mhx1999.top/gtplvktoia.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gotoacloud.top/gtjhmajvps.html

[N04] 斐波那契数列
来源：http://hz.chenlongwang.top/gtoatqeziz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ehwqpu.com/gtaapeuohs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ppjwa.cn/gtpcjsyqsx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gtgcrzzuwd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xylfe.cn/gtlvolyxhw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.meibo888.top/gthykgexbb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sweek.top/gtkuofpaws.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.smart0.xyz/gtograqsvg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj20258888.top/gtypsbnmxx.html

[N05] 最大公约数
来源：http://hz.jinqigufen.top/gtjirwfugv.html

Py:   math.gcd(a, b)
来源：http://hz.ydjk.org.cn/gtrygvhprh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhiwuduotai.top/gtpnxmnshr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jyoumei.cn/gtjtzunkij.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigfzy.top/gtesypnzga.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.iojbl.cn/gtonbqvnxg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenzaomai.com/gtbzsqafhy.html

Ruby: a.gcd(b)
来源：http://hz.daria6918.cn/gtqiknomtc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cashguo.top/gttrqcrogv.html

[N06] 判断回文字符串
来源：http://hz.jlsjyb.cn/gtvyqsajea.html

Py:   s == s[::-1]
来源：http://hz.andypj.xyz/gtrcedycwi.html

PHP:  $s === strrev($s);
来源：http://hz.jinyuanbaomall.cn/gtzvsjdway.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cqqwz.cn/gtkazxzpeg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhixingplan.top/gtkwiegjve.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hywenlv.cn/gtlgzofplu.html

Go:   // 双指针从两端比较
来源：http://hz.shuidangran.top/gtdcjiacfb.html

Ruby: s == s.reverse
来源：http://hz.bjfxy.top/gtgvoprtjn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xingfuxueyuan.xyz/gtrgfkitqv.html

[N07] 两数之和（返回下标）
来源：http://hz.gzhubu.top/gtapqhuoae.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hysaishi.cn/gtxbtlonht.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jyoumei.cn/gtypqhelom.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.aibaodan.cn/gtxnlamuai.html

TS:   // 手写 Map<string, number>
来源：http://hz.jianghu66.top/gtyukhyysu.html

Java: // 手写 HashMap
来源：http://hz.kuanghao11.cn/gtchubthbq.html

Go:   // 手写 map[int]int
来源：http://hz.jinqigufen.top/gthcanbqfm.html

Ruby: // 手写 Hash
来源：http://hz.zhixingplan.top/gtghczmuvw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yonumen.top/gthqwovakz.html

[N08] 生成全排列
来源：http://hz.wangshuangyany.cn/gtyiwivgfp.html

Py:   itertools.permutations(arr)
来源：http://hz.yueranfly.top/gtcnaojjgm.html

PHP:  // 手写递归交换
来源：http://hz.ppjwa.cn/gtgkcqjhlq.html

JS:   // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtfcompmoe.html

TS:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtkchzmfwr.html

Java: // 手写回溯递归
来源：http://hz.yongpay.top/gturcwfutz.html

Go:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtsxipyhko.html

Ruby: arr.permutation.to_a
来源：http://hz.andypj.xyz/gtrrnwwuor.html

C#:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtbiqjdtdi.html

[N09] 栈与队列
来源：http://hz.ydjk.org.cn/gtefjoqfhy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.kuanghao11.cn/gtshtaldhs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hammf.cn/gtfnznbmnt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yvedp.cn/gtjxuimcas.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ybcxt.top/gtrfuijfcr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.haohaochexian.top/gtpfuoermg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xuetiantiany.cn/gtarxerlyb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.fengsongda.top/gtopexxjqq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.guannengcc.top/gtvuiycbmr.html

[N10] 链表节点定义
来源：http://hz.zycfv.cn/gtzeopsufo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hywenlv.cn/gtytxgucit.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.pycfn.com/gtuoguctmq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.tianlin.xyz/gtlpochjwu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sweek.top/gtjpkywhve.html

Java: class Node { int v; Node next; }
来源：http://hz.daria6918.cn/gthiyxbkry.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jyoumei.cn/gtsmuesiru.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ydzc1.top/gteumskozm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xziqi.cn/gtojfazsgl.html

[N11] 二叉树中序遍历
来源：http://hz.mhx1999.top/gtzngkwzpc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ydjk.org.cn/gtroybenpy.html

PHP:  // 手写递归函数
来源：http://hz.hnqzz.top/gtzztdalbg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yonumen.top/gtczfuvkbx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhoulong.xyz/gtrojcvdbm.html

Java: // 手写递归
来源：http://hz.zycfv.cn/gthbcxnwdo.html

Go:   // 手写递归
来源：http://hz.0kj1m.cn/gtxdkhgzhg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.nwbrower.top/gtnkkgoaat.html

C#:   // 手写递归
来源：http://hz.shanyushiyangtech.top/gtfsravgck.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.birdmap.top/gtuaklzthl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ppjwa.cn/gtheuftgoz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhijiandao.cn/gtudcqcqwf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangdashe.top/gtubsxpqgv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangshuangyany.cn/gtawbvmksw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhijiandao.cn/gtmmmmvbke.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sysykeji.top/gtzjhjfmza.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xingfuxueyuan.xyz/gtcbgwflek.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fzhhl.top/gtrffnituw.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtfeovxpaq.html

O. 并发与异步
来源：http://hz.yangfankeji.com/gtuvppruij.html

================================================================================
来源：http://hz.nanxinkj.top/gtgibbjwbq.html

[O01] 启动一个线程
来源：http://hz.cucudq.cn/gtaaczuidg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yuxming.cn/gtyhftxkla.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhiwuduotai.top/gtamzsiukt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hysaishi.cn/gtaetgslot.html

TS:   // 同 JS
来源：http://hz.cdnleiting.top/gtewdppdtz.html

Java: new Thread(() -> f()).start()
来源：http://hz.cucudq.cn/gtmxfegamu.html

Go:   go f()
来源：http://hz.zdqjudy.top/gtaqygwcpu.html

Ruby: Thread.new { f }
来源：http://hz.zhaomingkeji.xyz/gtfslztmyq.html

C#:   Task.Run(() => F());
来源：http://hz.shangyingyoupin.top/gtsoqcywza.html

[O02] 使用线程池
来源：http://hz.zycfv.cn/gtktpiwksa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.aizwys.cn/gtecqjyidq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hysaishi.cn/gtmhktjyjo.html

JS:   // worker_threads 线程池
来源：http://hz.chenlongwang.top/gtniugvpnm.html

TS:   // worker_threads 线程池
来源：http://hz.jqgufenzy.top/gtuggxqksc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.snrcjt.cn/gtukmjyzfq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.tanke756.top/gtjdhzseok.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.chenlongwang.top/gtoivmewfe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yuanzhike.top/gtsrukqetd.html

[O03] 加锁保护共享数据
来源：http://hz.wangdashe.top/gtybxbgsli.html

Py:   with lock: shared += 1
来源：http://hz.pengpengdd.cyou/gthzeczxmp.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hnqzz.top/gtyeulhetq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yj202588.top/gtcomfcitn.html

TS:   // 同 JS
来源：http://hz.xuanzx.com/gtgznaekev.html

Java: synchronized (this) { shared++; }
来源：http://hz.shanyushiyangkeji.top/gttsfevecc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.wangshuangyany.cn/gtnecdcrhh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.c1oappe.top/gtfwzmjrzy.html

C#:   lock (gate) { shared++; }
来源：http://hz.daria6918.cn/gtdloczvmq.html

[O04] 定义异步函数并等待
来源：http://hz.snrcjt.cn/gtrslkqjkr.html

Py:   async def f():⏎    await g()
来源：http://hz.guowangkeji.top/gtewjuejco.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ywan-chungtsiang.top/gthfqjaalw.html

JS:   async function f() { await g(); }
来源：http://hz.sweek.top/gtjmetqelt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.guannengcc.top/gtlrxqaehq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhoulong.xyz/gtlnsfjisq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhijiandao.cn/gtinocwkqf.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.snrcjt.cn/gtwzcwngny.html

C#:   async Task F() { await G(); }
来源：http://hz.shanyushiyangtech.top/gtpnocarsa.html

[O05] 并发执行并等待全部完成
来源：http://hz.xuetiantiany.cn/gtkhcwscmo.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cashguo.top/gtmadmxfan.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.tianlin.xyz/gtdkfbzkaf.html

JS:   await Promise.all(tasks)
来源：http://hz.redwolf501.top/gthqgsxkxb.html

TS:   await Promise.all(tasks)
来源：http://hz.tanke756.top/gtmblbamwo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hywenlv.cn/gtrvkbxorr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.wangshuangyany.cn/gtyjtwbrfl.html

Ruby: threads.map(&:join)
来源：http://hz.gogol.net.cn/gtamlsakbp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ydzc1.top/gtobdvznbr.html

[O06] 使用进程池
来源：http://hz.tianlin.xyz/gtruyqvrsf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.tianlin.xyz/gttyqtbcyx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hfpthk.cn/gtcfignjxm.html

JS:   // child_process / cluster 模块
来源：http://hz.sysykeji.top/gtnjzkkhrf.html

TS:   // child_process / cluster 模块
来源：http://hz.shanyushiyangkeji.top/gtqcraaurd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.316326.xyz/gtmwzfjilk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.pycfn.com/gtxpuamofm.html

Ruby: // fork 块
来源：http://hz.nwbrower.top/gthlyrzshu.html

C#:   Parallel.For
来源：http://hz.bjfxy.top/gtjyjroelv.html

================================================================================
来源：http://hz.bjfxy.top/gtfltmwxwu.html

P. 常用工具函数
来源：http://hz.gogol.net.cn/gtfilrxpsn.html

================================================================================
来源：http://hz.sysykeji.top/gtwdxoatgk.html

[P01] 生成 UUID
来源：http://hz.meibo888.top/gtgiqwrywn.html

Py:   str(uuid.uuid4())
来源：http://hz.zhijiandao.cn/gtbscppaui.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.wangdashe.top/gtmofhjzzt.html

JS:   crypto.randomUUID()
来源：http://hz.yueranfly.top/gtwkdqhfyw.html

TS:   crypto.randomUUID()
来源：http://hz.guannengcc.top/gtxlblogcy.html

Java: UUID.randomUUID().toString()
来源：http://hz.aizwys.cn/gtkdkdlflx.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xinyue.icu/gtvjcpglyd.html

Ruby: SecureRandom.uuid
来源：http://hz.shanyushiyangkeji.top/gtczqkovin.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xuetiantiany.cn/gtkaztrokb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shangyingyoupin.top/gtvfwiqnvi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.nanxuanxn.top/gtyqkhqasd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.haohaochexian.top/gtnuxyhbjk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hongshengwenyu.top/gtansxiedw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shuidangran.top/gtbkqxfkvt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.dianchejie.cn/gtasztmsps.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.tian-w.cn/gtjuyhsvwf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.quarkkingdee.top/gtumhcksbs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cashguo.top/gtahrkrkwn.html

[P03] 生成短随机字符串
来源：http://hz.chenlongwang.top/gtvcnoaecf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.guannengcc.top/gtpvhvlclw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ivvv.top/gtbdchspus.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.smart0.xyz/gtmrcboxwh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.fzhhl.top/gtwdbahqep.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.havefunace.top/gtootkvlix.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shzxlz.cn/gtuezjdbhc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ivvv.top/gtsrczboaj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinqigfzy.top/gtdzxooant.html

[P04] 求长度
来源：http://hz.gaohongyu789.top/gtznhkqgsn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yvedp.cn/gtdtamdwzr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.0kj1m.cn/gtoeosgbvr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.mhx1999.top/gthvurnvpf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yangfankeji.com/gtgbncmgnu.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sxryk.cn/gtzvqdklrb.html

Go:   len(arr);  len(m)
来源：http://hz.jinqigufen.top/gtbtwynhzm.html

Ruby: x.length;  x.size
来源：http://hz.jianghu66.top/gtnohaxfkm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hysaishi.cn/gtequwbbpl.html

[P05] 判断两个对象内容是否相等
来源：http://hz.aizwys.cn/gtirakuotp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shanyushiyangtech.top/gtdqxnzhdd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.kuanghao11.cn/gtlrpagbkn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.aibaodan.cn/gtvzahrxtq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tianlin.xyz/gtiwqdpydq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yongpay.top/gtpcyjcump.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yuxming.cn/gtaxdakzqy.html

Ruby: a == b
来源：http://hz.ywan-chungtsiang.top/gtlwtcmiqe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinyuanbaomall.cn/gtsrdvggpv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhengqikj.top/gtssgzqscv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhiwuduotai.top/gtnmkprtyy.html

PHP:  if (empty($x)) {}
来源：http://hz.hnxiangtu.top/gtswxkdkch.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.dashuyun.cn/gtagokwqfi.html

TS:   if (x == null) {}
来源：http://hz.feifeiyinyue.top/gtphmifivz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ybcxt.top/gtimusewcd.html

Go:   if x == nil {}
来源：http://hz.cheryme.top/gtxrklhwog.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jianghu66.top/gtutykpqlf.html

C#:   if (x is null) {}
来源：http://hz.jinqigufen.top/gthhrrjesc.html

[P07] 防抖与节流
来源：http://hz.jinghuilouyu.cn/gtpsaydigc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.chenzaomai.com/gtqgfwuvas.html

PHP:  // 手写时间戳比较
来源：http://hz.chenzaomai.com/gtvtzyoron.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ivvv.top/gtiljegtps.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydjk.org.cn/gtvbdfqhsi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yuxming.cn/gtppqvkcxo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.meibo888.top/gtbvlcutpd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jlsjyb.cn/gtiivauwpb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yonumen.top/gtarmsslva.html

[P08] 处理浮点精度问题
来源：http://hz.xinyue.icu/gtqdtkcley.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jianghu66.top/gtiqsgksuw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.316326.xyz/gtlmimsmqg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jinghuilouyu.cn/gtbmbdxdjt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tianlin.xyz/gtqfirrfxs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hywenlv.cn/gtqbcygzxl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yuxming.cn/gtswfqhrud.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.snrcjt.cn/gtjmpluerv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.gogol.net.cn/gtvpglwlrr.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtmxadpsuh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.bjfxy.top/gtqkapzeeb.html

================================================================================
来源：http://hz.nanxuanxn.top/gtvhgtecfq.html

[Q01] 创建表
来源：http://hz.shangyingyoupin.top/gtdokalpne.html

CREATE TABLE users (
来源：http://hz.iojbl.cn/gtpulrahop.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhixingplan.top/gtgswfmxtn.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hongshengwenyu.top/gtuqdsufyl.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jyoumei.cn/gtmtymcxks.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yuxming.cn/gtqrctgkzn.html

);
来源：http://hz.snrcjt.cn/gthshmkoqn.html

[Q02] 创建带外键的表
来源：http://hz.zdqjudy.top/gtyjcfbced.html

CREATE TABLE orders (
来源：http://hz.cqqwz.cn/gtidsdeaoe.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gotoacloud.top/gtlrmmdgvi.html

user_id INT NOT NULL,
来源：http://hz.cashguo.top/gtjxadepcb.html

amount DECIMAL(10, 2),
来源：http://hz.zdqjudy.top/gttjmtadst.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.birdmap.top/gtxmltltut.html

);
来源：http://hz.tian-w.cn/gtayqnzexa.html

[Q03] 增加列
来源：http://hz.snrcjt.cn/gtngultxnm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yuxming.cn/gtrtixawaa.html

[Q04] 修改列类型
来源：http://hz.jqgufenzy.top/gtdwcymqlc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.shzxlz.cn/gtdtgjpfhv.html

[Q05] 重命名列
来源：http://hz.daria6918.cn/gtqmabatde.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj20258.top/gtqfcuvrnu.html

[Q06] 删除列
来源：http://hz.jinghuilouyu.cn/gtgffqjwmc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhixingplan.top/gteqmlcrng.html

[Q07] 删除表
来源：http://hz.chenzaomai.com/gtcawfleyk.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yangfankeji.com/gtvuthvifj.html

[Q08] 创建普通索引
来源：http://hz.yj20258888.top/gtfbbcjage.html


<!-- 参考信息 -->