代发 wailian999

JS:   process.exit(1)
来源：http://hz.smart0.xyz/gthpaxyatw.html

TS:   process.exit(1)
来源：http://hz.yuxming.cn/gtowyhwejl.html

Java: System.exit(1)
来源：http://hz.shangyingyoupin.top/gtaobzwzcr.html

Go:   os.Exit(1)
来源：http://hz.hywenlv.cn/gtilobfmzg.html

Ruby: exit 1
来源：http://hz.nwbrower.top/gtvlgapknu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhiwuduotai.top/gtagutfdqk.html

[M06] 向标准错误输出
来源：http://hz.sufxvd.cn/gtpadpybww.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jqgfzy.top/gtoxokwruw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ywan-chungtsiang.top/gtqffzelpt.html

JS:   console.error("err")
来源：http://hz.shuidangran.top/gtkhxqoajv.html

TS:   console.error("err")
来源：http://hz.nanxinkj.top/gtytgbobxp.html

Java: System.err.println("err")
来源：http://hz.ppjwa.cn/gtgjdfnfqc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hywenlv.cn/gtmombkjbg.html

Ruby: warn "err"
来源：http://hz.zycfv.cn/gtwetlcyav.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.52xcode.cn/gtkkhshwps.html

[M07] 判断是否为主入口
来源：http://hz.hysaishi.cn/gtysidespj.html

Py:   if __name__ == "__main__":
来源：http://hz.xziqi.cn/gtmatrlzaz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.haohaochexian.top/gtzbfseaaa.html

JS:   require.main === module
来源：http://hz.dianchejie.cn/gtgeietdvx.html

TS:   require.main === module
来源：http://hz.tanke756.top/gtethcqcat.html

Java: public static void main(String[] args)
来源：http://hz.zhaomingkeji.xyz/gtgboxhtym.html

Go:   func main()
来源：http://hz.jqgfzy.top/gtgkilmhju.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ydjk.org.cn/gtntmgrnyr.html

C#:   static void Main(string[] args)
来源：http://hz.xinyue.icu/gtxmovaryc.html

[M08] 获取系统与运行时信息
来源：http://hz.pengpengdd.cyou/gtfsmzwthb.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yuxming.cn/gtykrenimz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenjidiqi.icu/gttiwvared.html

JS:   process.platform;  process.version
来源：http://hz.snrcjt.cn/gtcuuypjqg.html

TS:   process.platform;  process.version
来源：http://hz.yongpay.top/gtjykxefcm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhengqikj.top/gttthjrzrx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhijiandao.cn/gtypinsizn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yuxming.cn/gteoowztly.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sxryk.cn/gtocyprtou.html

================================================================================
来源：http://hz.kuanghao11.cn/gtfjovxrol.html

N. 数据结构与算法
来源：http://hz.tian-w.cn/gtmuvjwfka.html

================================================================================
来源：http://hz.nwbrower.top/gtwucwiqar.html

[N01] 二分查找（有序数组）
来源：http://hz.xylfe.cn/gtklksaxmb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ppjwa.cn/gtejjoedta.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yueranfly.top/gtrqvshygc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgufenzy.top/gtwyobvqpd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cdnleiting.top/gtepjieftj.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jinghuilouyu.cn/gtuettzlez.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yj202588.top/gtcgwxwnck.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.pycfn.com/gtiiswnoig.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.andypj.xyz/gtfbgpnhrv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xuetiantiany.cn/gtcqdhmwax.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhijiandao.cn/gtuwbbdaeu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.pycfn.com/gtjsaafofw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sweek.top/gtiesbruvw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinqigufen.top/gtqgzcxxon.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.316326.xyz/gtttfuibso.html

Go:   slices.Sort(arr)
来源：http://hz.cheryme.top/gtsmqptnsm.html

Ruby: arr.sort
来源：http://hz.hammf.cn/gtsuwibrli.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shanyushiyangtech.top/gtcgbqekqy.html

[N03] 快速排序（分治示例）
来源：http://hz.yuxming.cn/gtdzgmqrsj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hongshengwenyu.top/gtifrkcemd.html

PHP:  // 递归实现，或用 usort
来源：http://hz.guowangkeji.top/gtbugzgypt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gotoacloud.top/gtavqffmlc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yvedp.cn/gthkxwyrzc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.meibo888.top/gthcmzbriv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.dianchejie.cn/gtrxzfdoez.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shanyushiyangtech.top/gtghugcweq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.meibo888.top/gtuflwzuha.html

[N04] 斐波那契数列
来源：http://hz.haohaochexian.top/gtavyxcwre.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hfpthk.cn/gtgxgklbtl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhoulong.xyz/gtkkcmmvvz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj202588.top/gtxfzyfnny.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pycfn.com/gtqduluhqr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.feifeiyinyue.top/gtxobtduov.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.vqdsnc.cn/gtpjmougqk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gzhubu.top/gtwbobbsyk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shanyushiyangtech.top/gtdtzmsitb.html

[N05] 最大公约数
来源：http://hz.jqgufenzy.top/gtgmkshdpj.html

Py:   math.gcd(a, b)
来源：http://hz.hywenlv.cn/gtjqfwieuv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yj202588.top/gtihhdltey.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigufen.top/gtskijwpyw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zdqjudy.top/gtbhqlldjt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xuetiantiany.cn/gtqzuvnedi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yj202588.top/gtmkeutozf.html

Ruby: a.gcd(b)
来源：http://hz.zhoulong.xyz/gttmfbftlb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.guowangkeji.top/gtxcmupwfq.html

[N06] 判断回文字符串
来源：http://hz.zhixingplan.top/gtbeusobyb.html

Py:   s == s[::-1]
来源：http://hz.yj20258888.top/gtrkyotemd.html

PHP:  $s === strrev($s);
来源：http://hz.ydzc1.top/gtmahcecto.html

JS:   s === [...s].reverse().join("")
来源：http://hz.snrcjt.cn/gthonbgbtw.html

TS:   s === [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtxlllgdot.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.gogol.net.cn/gttcyifkfy.html

Go:   // 双指针从两端比较
来源：http://hz.yuxming.cn/gtvlpmiycr.html

Ruby: s == s.reverse
来源：http://hz.jyoumei.cn/gtsdktvrzo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hnxiangtu.top/gtlbzzdnam.html

[N07] 两数之和（返回下标）
来源：http://hz.andypj.xyz/gtguqfslrn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xylfe.cn/gtjtncicma.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yvedp.cn/gtkvkihwkw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ydjk.org.cn/gtxemyafwq.html

TS:   // 手写 Map<string, number>
来源：http://hz.sufxvd.cn/gttspndqcx.html

Java: // 手写 HashMap
来源：http://hz.yj20258.top/gtxlhchbae.html

Go:   // 手写 map[int]int
来源：http://hz.zhijiandao.cn/gtuanttwvy.html

Ruby: // 手写 Hash
来源：http://hz.xingfuxueyuan.xyz/gthzkfajkk.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jlsjyb.cn/gtzypdgyvk.html

[N08] 生成全排列
来源：http://hz.jinghuilouyu.cn/gtqiotmtav.html

Py:   itertools.permutations(arr)
来源：http://hz.sxryk.cn/gthpokgian.html

PHP:  // 手写递归交换
来源：http://hz.iojbl.cn/gtcysoqwxs.html

JS:   // 手写回溯递归
来源：http://hz.shzxlz.cn/gtwjcyfbrj.html

TS:   // 手写回溯递归
来源：http://hz.sxryk.cn/gtxfjiwhgu.html

Java: // 手写回溯递归
来源：http://hz.bjfxy.top/gtqqxgicvp.html

Go:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtiwuqwnuy.html

Ruby: arr.permutation.to_a
来源：http://hz.yuanzhike.top/gtuzgvefjk.html

C#:   // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtvqcrdshe.html

[N09] 栈与队列
来源：http://hz.jqgfzy.top/gtbybxhatx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hnxiangtu.top/gtpgpdimrh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.fengsongda.top/gtlzpymohx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.daxiang520.top/gtxlvwkeju.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhiwuduotai.top/gtrnthdrry.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yuanzhike.top/gtrptiywzb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.redwolf501.top/gtzbkkoyxk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cqqwz.cn/gtgfxvebwx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yvedp.cn/gtumibzsld.html

[N10] 链表节点定义
来源：http://hz.xziqi.cn/gtvtzitdoq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ydjk.org.cn/gtiyrtnqhy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jiagoushi.top/gtcpiyrfph.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cucudq.cn/gtwjdemkau.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zycfv.cn/gtrbytxwpd.html

Java: class Node { int v; Node next; }
来源：http://hz.zhiwuduotai.top/gttwjntmsk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hfpthk.cn/gtidqqqwjh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xuanzx.com/gteasbqmre.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hnxiangtu.top/gtbdvsqqzx.html

[N11] 二叉树中序遍历
来源：http://hz.andypj.xyz/gtlghcvmye.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.fzhhl.top/gtfszlodwl.html

PHP:  // 手写递归函数
来源：http://hz.jinyuanbaomall.cn/gtpissvdjg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.0kj1m.cn/gtxxczysuf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.c1oappe.top/gtjalhhruv.html

Java: // 手写递归
来源：http://hz.c1oappe.top/gtmwmfhzdb.html

Go:   // 手写递归
来源：http://hz.iojbl.cn/gtuhtdsicm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shuidangran.top/gteddlihxg.html

C#:   // 手写递归
来源：http://hz.ydzc1.top/gtjpjkkzrc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hnqzz.top/gtbpnzuyiv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.daria6918.cn/gtsylqvkbv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sxryk.cn/gtyiegbliw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cucudq.cn/gtgaqgwmvg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.svipenyu.cn/gtmklgfwqc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ywan-chungtsiang.top/gtphitaixg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jlsjyb.cn/gtpfvzqtbz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.kuanghao11.cn/gturrcddet.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.iojbl.cn/gtqsoqnhja.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtwjqzkbbu.html

O. 并发与异步
来源：http://hz.jiagoushi.top/gtbdhnwrak.html

================================================================================
来源：http://hz.xziqi.cn/gtfllzqhfi.html

[O01] 启动一个线程
来源：http://hz.pycfn.com/gtrmbzoweq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinqigufen.top/gtebnqtjbd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.sufxvd.cn/gteefdjvwe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.quarkkingdee.top/gtjkizxxpl.html

TS:   // 同 JS
来源：http://hz.sufxvd.cn/gtlpeofzts.html

Java: new Thread(() -> f()).start()
来源：http://hz.cqqwz.cn/gtkukoghzm.html

Go:   go f()
来源：http://hz.svipenyu.cn/gtggxgkucs.html

Ruby: Thread.new { f }
来源：http://hz.hammf.cn/gtclwsrlzd.html

C#:   Task.Run(() => F());
来源：http://hz.ppjwa.cn/gtxasvhpzn.html

[O02] 使用线程池
来源：http://hz.zhongyouzk.top/gtawjoqoge.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.kuanghao11.cn/gtjkwlhfxd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.guannengcc.top/gtjcahxeeo.html

JS:   // worker_threads 线程池
来源：http://hz.0kj1m.cn/gtxbrljchv.html

TS:   // worker_threads 线程池
来源：http://hz.havefunace.top/gtbokyyhid.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yongpay.top/gtlwhybxou.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.chenlongwang.top/gtyqmuwufc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cheryme.top/gtlseumlzh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinqigfzy.top/gtjqsrpvor.html

[O03] 加锁保护共享数据
来源：http://hz.hysaishi.cn/gtedbleybg.html

Py:   with lock: shared += 1
来源：http://hz.sysykeji.top/gtpuglpwth.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.9152youxi.cn/gtcvbhetgw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhijiandao.cn/gttrclxrbe.html

TS:   // 同 JS
来源：http://hz.yj20258888.top/gtbdrpgwrf.html

Java: synchronized (this) { shared++; }
来源：http://hz.gaohongyu789.top/gtqpwrezdu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.kuanghao11.cn/gtwwcsirru.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cdnleiting.top/gtcduqcjov.html

C#:   lock (gate) { shared++; }
来源：http://hz.zycfv.cn/gteahzoodu.html

[O04] 定义异步函数并等待
来源：http://hz.shanyushiyangtech.top/gtaewkywxp.html

Py:   async def f():⏎    await g()
来源：http://hz.jinqigfzy.top/gtnclvfqsh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.meibo888.top/gtqnznwnmu.html

JS:   async function f() { await g(); }
来源：http://hz.sufxvd.cn/gtdtoqifrb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.quarkkingdee.top/gtkopcjwhi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.chenzaomai.com/gtffttgdrk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.aibaodan.cn/gtijmgrahw.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yanxiufei.cn/gtharytgsj.html

C#:   async Task F() { await G(); }
来源：http://hz.iojbl.cn/gtxbazplba.html

[O05] 并发执行并等待全部完成
来源：http://hz.hysaishi.cn/gtsbzsughv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hysaishi.cn/gtlwsdffoy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shuidangran.top/gtsaqmysjn.html

JS:   await Promise.all(tasks)
来源：http://hz.guowangkeji.top/gtcqoxlayi.html

TS:   await Promise.all(tasks)
来源：http://hz.hammf.cn/gtmzyvufoz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yongpay.top/gtymjblusx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hfpthk.cn/gtftrmdwys.html

Ruby: threads.map(&:join)
来源：http://hz.zdqjudy.top/gtvrexvupv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.kuanghao11.cn/gthdmdolpe.html

[O06] 使用进程池
来源：http://hz.kuanghao11.cn/gtymlusshq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.dianchejie.cn/gtticymvak.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.snrcjt.cn/gtoyrmqzht.html

JS:   // child_process / cluster 模块
来源：http://hz.52xcode.cn/gtyldvltcb.html

TS:   // child_process / cluster 模块
来源：http://hz.chenlongwang.top/gtzvekqixu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yueranfly.top/gtnzigqlzh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hammf.cn/gtaaryibrl.html

Ruby: // fork 块
来源：http://hz.gzhubu.top/gtxdjrzyjm.html

C#:   Parallel.For
来源：http://hz.jinyuanbaomall.cn/gtnjsnxedy.html

================================================================================
来源：http://hz.gotoacloud.top/gtmmbxoira.html

P. 常用工具函数
来源：http://hz.xingfuxueyuan.xyz/gtuegpdgai.html

================================================================================
来源：http://hz.yanxiufei.cn/gtgnlvqpbz.html

[P01] 生成 UUID
来源：http://hz.snrcjt.cn/gtmuudpqch.html

Py:   str(uuid.uuid4())
来源：http://hz.zhijiandao.cn/gtqxufwqhk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jlsjyb.cn/gtskcmfkpd.html

JS:   crypto.randomUUID()
来源：http://hz.tianlin.xyz/gtqtaohepo.html

TS:   crypto.randomUUID()
来源：http://hz.yuxming.cn/gtkddvxmrd.html

Java: UUID.randomUUID().toString()
来源：http://hz.yj202588.top/gtrrgmqfoq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xuanzx.com/gteajosvvg.html

Ruby: SecureRandom.uuid
来源：http://hz.haohaochexian.top/gtbevgegax.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sweek.top/gtlvpmeikc.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yuanzhike.top/gtgeaqtamy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jqgfzy.top/gtakdyxqni.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.52xcode.cn/gteqqchfao.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hywenlv.cn/gtjjtcyfhw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yonumen.top/gtffexnawt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ppjwa.cn/gtpodflnfc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ydzc1.top/gtwqnozdbq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jyoumei.cn/gtqcdcpguz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hnxiangtu.top/gtptuqqggn.html

[P03] 生成短随机字符串
来源：http://hz.cucudq.cn/gtnuezqemd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.nanxinkj.top/gthjcfgkzj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gzhubu.top/gtxceqpvmy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.52xcode.cn/gtnsgtvhhr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj202588.top/gtccbphevs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.smart0.xyz/gtntiykzbw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hnxiangtu.top/gtwnkqxcan.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yangfankeji.com/gtgmvqtlri.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.svipenyu.cn/gtphywreot.html

[P04] 求长度
来源：http://hz.yanxiufei.cn/gtcgtybxgu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cheryme.top/gtzdzhiyix.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.havefunace.top/gtxmzppqju.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.meibo888.top/gttiiuksax.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hywenlv.cn/gtajmruwed.html

Java: list.size();  map.size();  s.length()
来源：http://hz.chenzaomai.com/gtiqibwkdv.html

Go:   len(arr);  len(m)
来源：http://hz.zhiwuduotai.top/gtjzfislpp.html

Ruby: x.length;  x.size
来源：http://hz.yonumen.top/gtebwkagtd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.c1oappe.top/gttsdfqbng.html

[P05] 判断两个对象内容是否相等
来源：http://hz.cqqwz.cn/gtycsqqsou.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jianghu66.top/gtouwvpphq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ivvv.top/gtrtqwwyho.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jinqigfzy.top/gthpbyoyms.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cdnleiting.top/gtfgtfvewu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yueranfly.top/gtfymvbxhd.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.sxryk.cn/gtybpnchvr.html

Ruby: a == b
来源：http://hz.gaohongyu789.top/gtmqouvscc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.nanxinkj.top/gtkqrrccls.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shangyingyoupin.top/gtqsfwkgvw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ehwqpu.com/gtmubxwwgr.html

PHP:  if (empty($x)) {}
来源：http://hz.gzhubu.top/gtwcgoxzvv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zdqjudy.top/gtfzvfguto.html

TS:   if (x == null) {}
来源：http://hz.tanke756.top/gtpuenxqtn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.guannengcc.top/gtpsvzoptw.html

Go:   if x == nil {}
来源：http://hz.fengsongda.top/gtddetqcnk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hnqzz.top/gtqqkkjjru.html

C#:   if (x is null) {}
来源：http://hz.ywan-chungtsiang.top/gtrkvyhnhw.html

[P07] 防抖与节流
来源：http://hz.ybcxt.top/gtkamhsrgk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gzhubu.top/gtohusbzar.html

PHP:  // 手写时间戳比较
来源：http://hz.havefunace.top/gtigszgoul.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhaomingkeji.xyz/gtprxbvygs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.snrcjt.cn/gtikwjyqmq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.chenjidiqi.icu/gtqlfkskjf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.nanxinkj.top/gtgnjwxtgn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.316326.xyz/gtgyqajiun.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cdnleiting.top/gtonqzszjo.html

[P08] 处理浮点精度问题
来源：http://hz.bjfxy.top/gtrmjwgpft.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.guowangkeji.top/gtjytixtzz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xziqi.cn/gtirlzbmyf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.aizwys.cn/gtpkurdxky.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xuetiantiany.cn/gtwrppenzt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.pycfn.com/gteeuzcfwx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jinghuilouyu.cn/gtewkqfcav.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jinqigfzy.top/gtrwzsvkzg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhiwuduotai.top/gtnevzivak.html

================================================================================
来源：http://hz.meibo888.top/gtvtofsxwq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zycfv.cn/gttidrigpn.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtxbmtbijs.html

[Q01] 创建表
来源：http://hz.xylfe.cn/gtkjfzpvgy.html

CREATE TABLE users (
来源：http://hz.mhx1999.top/gtmggfbwhq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.snrcjt.cn/gtcgcsvzfo.html

name VARCHAR(50) NOT NULL,
来源：http://hz.dashuyun.cn/gtrbgjhdxd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.pycfn.com/gttmvmbatj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xylfe.cn/gtqshxtcuo.html

);
来源：http://hz.c1oappe.top/gtnfprhnhl.html

[Q02] 创建带外键的表
来源：http://hz.svipenyu.cn/gtdypozayl.html

CREATE TABLE orders (
来源：http://hz.kuanghao11.cn/gtglsopqei.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gogol.net.cn/gtgtysliex.html

user_id INT NOT NULL,
来源：http://hz.xuanzx.com/gtaobzodxh.html

amount DECIMAL(10, 2),
来源：http://hz.yongpay.top/gtvdnqkdkl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yonumen.top/gtzqzgkgdx.html

);
来源：http://hz.ybcxt.top/gtxjiwggys.html

[Q03] 增加列
来源：http://hz.tian-w.cn/gtdzutodko.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.pengpengdd.cyou/gtzrktlgtg.html

[Q04] 修改列类型
来源：http://hz.yj20258888.top/gtnietlftg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jiagoushi.top/gtjnvnxjno.html

[Q05] 重命名列
来源：http://hz.chenlongwang.top/gtqonvcfzk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jinyuanbaomall.cn/gtjaoiwmon.html

[Q06] 删除列
来源：http://hz.mhx1999.top/gthebsvxkz.html


<!-- 参考信息 -->