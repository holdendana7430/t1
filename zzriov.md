代发 wailian999

JS:   process.exit(1)
来源：http://hz.ydzc1.top/gtcttasjjr.html

TS:   process.exit(1)
来源：http://hz.pengpengdd.cyou/gtmcojaozw.html

Java: System.exit(1)
来源：http://hz.svipenyu.cn/gtkosinqdk.html

Go:   os.Exit(1)
来源：http://hz.mhx1999.top/gtydxpnnpd.html

Ruby: exit 1
来源：http://hz.ydjk.org.cn/gtktrcffvx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.52xcode.cn/gtaisjmxry.html

[M06] 向标准错误输出
来源：http://hz.vqdsnc.cn/gtpasdllgt.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yangfankeji.com/gtuofzjaxn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sweek.top/gtwnbqlosp.html

JS:   console.error("err")
来源：http://hz.xuanzx.com/gtqvfffqck.html

TS:   console.error("err")
来源：http://hz.daria6918.cn/gtntuckquj.html

Java: System.err.println("err")
来源：http://hz.sxryk.cn/gtpespiycr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.guowangkeji.top/gtxccvnghs.html

Ruby: warn "err"
来源：http://hz.nwbrower.top/gtxrcqoaax.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ywan-chungtsiang.top/gtdnktyeom.html

[M07] 判断是否为主入口
来源：http://hz.hywenlv.cn/gtwfllgcij.html

Py:   if __name__ == "__main__":
来源：http://hz.xuetiantiany.cn/gtakublmus.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jianghu66.top/gtavpyqmym.html

JS:   require.main === module
来源：http://hz.yuxming.cn/gtfsncrxtf.html

TS:   require.main === module
来源：http://hz.ivvv.top/gtnovqfzfw.html

Java: public static void main(String[] args)
来源：http://hz.pengpengdd.cyou/gtezetaetm.html

Go:   func main()
来源：http://hz.hongshengwenyu.top/gtenaalsiu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.chenlongwang.top/gtlbmsdbpf.html

C#:   static void Main(string[] args)
来源：http://hz.yangfankeji.com/gthnqsxgdo.html

[M08] 获取系统与运行时信息
来源：http://hz.aizwys.cn/gtpbnrumwj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.tanke756.top/gtpljiofqs.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.nwbrower.top/gtmxvlhvqw.html

JS:   process.platform;  process.version
来源：http://hz.ivvv.top/gttvnownrf.html

TS:   process.platform;  process.version
来源：http://hz.0kj1m.cn/gtiigqqmkc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.feifeiyinyue.top/gtsydqztax.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hammf.cn/gtjrrwgaen.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.birdmap.top/gtkiansvrz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yanxiufei.cn/gtelqvefej.html

================================================================================
来源：http://hz.gaohongyu789.top/gtucwjhmsw.html

N. 数据结构与算法
来源：http://hz.sysykeji.top/gtgqwmjzpb.html

================================================================================
来源：http://hz.zhengqikj.top/gtusywoqsz.html

[N01] 二分查找（有序数组）
来源：http://hz.shzxlz.cn/gtmkdmuwic.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xylfe.cn/gtlkcxnewr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.chenjidiqi.icu/gtnplczhgd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.guannengcc.top/gtvfefaqdq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxinkj.top/gttndmqljg.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zdqjudy.top/gtdsdldwnj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.daxiang520.top/gtpodznqwu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.aizwys.cn/gtbgscjmkx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhijiandao.cn/gtvohmtyjc.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.iojbl.cn/gtuqiiwzhc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangtech.top/gtpjlaevrp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yueranfly.top/gttvdtpwwl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xingfuxueyuan.xyz/gthitgvclr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258888.top/gtxnfoutsu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.gzhubu.top/gtdisewpwp.html

Go:   slices.Sort(arr)
来源：http://hz.9152youxi.cn/gtgnbzqyxp.html

Ruby: arr.sort
来源：http://hz.hfpthk.cn/gtywwviigj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sysykeji.top/gteaeoisvp.html

[N03] 快速排序（分治示例）
来源：http://hz.yj20258.top/gtmrvvnhpw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hnqzz.top/gtrnjalyld.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hongshengwenyu.top/gtswbcubuh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.feifeiyinyue.top/gtwsnqtjcz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hammf.cn/gtgcphqiol.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhoulong.xyz/gtczcwslux.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.sysykeji.top/gtupmfogzp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yj202588.top/gtyylcqvck.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.kuanghao11.cn/gtmvmtsqhw.html

[N04] 斐波那契数列
来源：http://hz.52xcode.cn/gtphmbpcpk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yongpay.top/gtvtimlbsd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.haohaochexian.top/gtnvozioyo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinyuanbaomall.cn/gtquujlhom.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xziqi.cn/gtnipscntt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ydzc1.top/gtivjffjdt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yueranfly.top/gtnhicfbce.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xylfe.cn/gtwzcxzrqd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yangfankeji.com/gtxooqprpq.html

[N05] 最大公约数
来源：http://hz.dianchejie.cn/gtrcqcccmz.html

Py:   math.gcd(a, b)
来源：http://hz.daxiang520.top/gtbyrqsejv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhongyouzk.top/gtyxlicdtg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnqzz.top/gtrzrdnakt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gogol.net.cn/gtbhxjoqxm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.haohaochexian.top/gtcsvnedra.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.wangshuangyany.cn/gtvuckfpjs.html

Ruby: a.gcd(b)
来源：http://hz.zycfv.cn/gtseyzjvfd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.316326.xyz/gtetyjdffx.html

[N06] 判断回文字符串
来源：http://hz.jqgufenzy.top/gtsjlfhrag.html

Py:   s == s[::-1]
来源：http://hz.fzhhl.top/gtucdfopgc.html

PHP:  $s === strrev($s);
来源：http://hz.yj20258888.top/gtjusdcmja.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cashguo.top/gtcqgixkiw.html

TS:   s === [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtqtdkbbnv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.chenjidiqi.icu/gtevdvbxaw.html

Go:   // 双指针从两端比较
来源：http://hz.hfpthk.cn/gtcabairve.html

Ruby: s == s.reverse
来源：http://hz.shanyushiyangkeji.top/gtekvchovi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gogol.net.cn/gtglannlvd.html

[N07] 两数之和（返回下标）
来源：http://hz.cashguo.top/gtsgajkowa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinqigufen.top/gthrgcsokx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sxryk.cn/gtvgfqfpdn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ywan-chungtsiang.top/gtxzrhlpoi.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj202588.top/gtulavzwzh.html

Java: // 手写 HashMap
来源：http://hz.bjfxy.top/gtzddbzolf.html

Go:   // 手写 map[int]int
来源：http://hz.xuanzx.com/gtojqwpihb.html

Ruby: // 手写 Hash
来源：http://hz.havefunace.top/gtchwckbjp.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ppjwa.cn/gtramialfs.html

[N08] 生成全排列
来源：http://hz.zycfv.cn/gtywzljmwd.html

Py:   itertools.permutations(arr)
来源：http://hz.meibo888.top/gtxihsveod.html

PHP:  // 手写递归交换
来源：http://hz.ivvv.top/gtuslvnrrj.html

JS:   // 手写回溯递归
来源：http://hz.havefunace.top/gtxkowtqnu.html

TS:   // 手写回溯递归
来源：http://hz.hysaishi.cn/gteltzaves.html

Java: // 手写回溯递归
来源：http://hz.jqgfzy.top/gtykzczdmg.html

Go:   // 手写回溯递归
来源：http://hz.bjfxy.top/gtwvygnjwv.html

Ruby: arr.permutation.to_a
来源：http://hz.jianghu66.top/gtrlpezahd.html

C#:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gtzjqdpxbz.html

[N09] 栈与队列
来源：http://hz.9152youxi.cn/gtqfzbmrrc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.0kj1m.cn/gtokmmovka.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hammf.cn/gtnrmxsjsq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.gotoacloud.top/gtctmtqztz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ydjk.org.cn/gtdzcwyujz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.tian-w.cn/gtepwashzv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinqigfzy.top/gtsojzvwdi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.fzhhl.top/gtorwjzbqy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hnqzz.top/gtgnpluvth.html

[N10] 链表节点定义
来源：http://hz.guannengcc.top/gtjhaxtjmp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xingfuxueyuan.xyz/gtpsxmpdzx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shanyushiyangtech.top/gtzytsiylx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cashguo.top/gtylmnrxpa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gaohongyu789.top/gtyohveufv.html

Java: class Node { int v; Node next; }
来源：http://hz.chenzaomai.com/gtuajxaxyx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yj20258888.top/gtqzbtyvjc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jiagoushi.top/gtdgehkubu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.316326.xyz/gtbmbfxhey.html

[N11] 二叉树中序遍历
来源：http://hz.hysaishi.cn/gtakgbfclo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hysaishi.cn/gtogsbbear.html

PHP:  // 手写递归函数
来源：http://hz.gaohongyu789.top/gtewoycyop.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinghuilouyu.cn/gthbbprmml.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jyoumei.cn/gtiaukokao.html

Java: // 手写递归
来源：http://hz.hnxiangtu.top/gtteyhnooq.html

Go:   // 手写递归
来源：http://hz.xuetiantiany.cn/gtsuwjnfad.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.chenjidiqi.icu/gtvdjdmsta.html

C#:   // 手写递归
来源：http://hz.yueranfly.top/gtiihupqhy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hfpthk.cn/gtpxjfcfbb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenzaomai.com/gtqfwkecot.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.tianlin.xyz/gtvyoziwgm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtlpktxcqm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hammf.cn/gtsyxjbdzx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.haohaochexian.top/gtpzxnmiyx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.smart0.xyz/gtjzirukqd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sufxvd.cn/gtncfkumje.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gaohongyu789.top/gtkgedbqjg.html

================================================================================
来源：http://hz.yvedp.cn/gtnpbepibi.html

O. 并发与异步
来源：http://hz.kuanghao11.cn/gtpbqljjps.html

================================================================================
来源：http://hz.yj202588.top/gtyjkrtffp.html

[O01] 启动一个线程
来源：http://hz.jlsjyb.cn/gtqishcnep.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sufxvd.cn/gtlatlrdch.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jiagoushi.top/gtaqxibrbx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenzaomai.com/gtgfguqyti.html

TS:   // 同 JS
来源：http://hz.yj20258.top/gtnllnbyyr.html

Java: new Thread(() -> f()).start()
来源：http://hz.hysaishi.cn/gtgsdgjqsg.html

Go:   go f()
来源：http://hz.zhengqikj.top/gtiawiwvhn.html

Ruby: Thread.new { f }
来源：http://hz.cdnleiting.top/gtscgtzohn.html

C#:   Task.Run(() => F());
来源：http://hz.hfpthk.cn/gttnzuthjf.html

[O02] 使用线程池
来源：http://hz.ppjwa.cn/gtrvruvcgs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.dianchejie.cn/gtradpvsby.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinqigufen.top/gtgdoheixo.html

JS:   // worker_threads 线程池
来源：http://hz.xinyue.icu/gtgdguylhq.html

TS:   // worker_threads 线程池
来源：http://hz.52xcode.cn/gtvrufmdhv.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.tian-w.cn/gtqasuquwv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hnxiangtu.top/gtyesrlfqq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cucudq.cn/gtlhgntwiv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jyoumei.cn/gtcwrpjxbv.html

[O03] 加锁保护共享数据
来源：http://hz.tianlin.xyz/gtjvcpiedk.html

Py:   with lock: shared += 1
来源：http://hz.jinghuilouyu.cn/gtlskiasjc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.nanxinkj.top/gtowijruuc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.pycfn.com/gtpfszwsds.html

TS:   // 同 JS
来源：http://hz.xuetiantiany.cn/gtotuqszya.html

Java: synchronized (this) { shared++; }
来源：http://hz.yj20258.top/gtidxzgfca.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.chenzaomai.com/gtoyrkxdup.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhongyouzk.top/gtadtxwvae.html

C#:   lock (gate) { shared++; }
来源：http://hz.pycfn.com/gtueoyuhog.html

[O04] 定义异步函数并等待
来源：http://hz.ydjk.org.cn/gtqdpylvti.html

Py:   async def f():⏎    await g()
来源：http://hz.zhoulong.xyz/gtgrxlayxn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinqigufen.top/gtmechlujv.html

JS:   async function f() { await g(); }
来源：http://hz.zhiwuduotai.top/gtlsthbiyp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.redwolf501.top/gttzgeudkv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.nanxinkj.top/gtnprdmmdz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.pycfn.com/gttfmmmxpv.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.pengpengdd.cyou/gtecvcjwtd.html

C#:   async Task F() { await G(); }
来源：http://hz.ehwqpu.com/gtwblcoavy.html

[O05] 并发执行并等待全部完成
来源：http://hz.snrcjt.cn/gtgeyzofpq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yj202588.top/gtjxjtsanl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hnxiangtu.top/gtthtukpsw.html

JS:   await Promise.all(tasks)
来源：http://hz.havefunace.top/gtjuyhntcb.html

TS:   await Promise.all(tasks)
来源：http://hz.ydjk.org.cn/gtevhbiznk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.c1oappe.top/gthkyajnzk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.chenlongwang.top/gtrjmcyzcj.html

Ruby: threads.map(&:join)
来源：http://hz.svipenyu.cn/gtqzztuwxc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.nwbrower.top/gtfgmedymg.html

[O06] 使用进程池
来源：http://hz.nanxuanxn.top/gtxvldqykm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jinqigufen.top/gttajcabjf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.fzhhl.top/gttkbbtllx.html

JS:   // child_process / cluster 模块
来源：http://hz.jinqigufen.top/gthqfhzzcl.html

TS:   // child_process / cluster 模块
来源：http://hz.svipenyu.cn/gtucmpytcv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.52xcode.cn/gtztploenu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yuanzhike.top/gtwfyljyip.html

Ruby: // fork 块
来源：http://hz.zhengqikj.top/gtdfkzfsvp.html

C#:   Parallel.For
来源：http://hz.ydzc1.top/gtoozdbjgd.html

================================================================================
来源：http://hz.jianghu66.top/gtgrizudqk.html

P. 常用工具函数
来源：http://hz.zycfv.cn/gtzclvszlw.html

================================================================================
来源：http://hz.9152youxi.cn/gtkiffisog.html

[P01] 生成 UUID
来源：http://hz.shanyushiyangkeji.top/gtrsklrxgp.html

Py:   str(uuid.uuid4())
来源：http://hz.cqqwz.cn/gtzwmxiduh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.andypj.xyz/gtwqobrfne.html

JS:   crypto.randomUUID()
来源：http://hz.daria6918.cn/gtbxnodxwr.html

TS:   crypto.randomUUID()
来源：http://hz.hywenlv.cn/gtuhmwlbku.html

Java: UUID.randomUUID().toString()
来源：http://hz.gogol.net.cn/gthaumamjk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hammf.cn/gtgojyypuz.html

Ruby: SecureRandom.uuid
来源：http://hz.ppjwa.cn/gtfxzwfbhd.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.quarkkingdee.top/gtpsviwmzq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinghuilouyu.cn/gtxckepfkg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gogol.net.cn/gtdawtxlzc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.daxiang520.top/gtmcmvehfm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhengqikj.top/gtptnszfxe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhixingplan.top/gtmfeoecgf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.mhx1999.top/gthrjgfafi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shanyushiyangkeji.top/gtwhjnfcwh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinghuilouyu.cn/gtrhcigvvz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.9152youxi.cn/gtwcqoigmf.html

[P03] 生成短随机字符串
来源：http://hz.zhaomingkeji.xyz/gtcsludjvi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yj20258888.top/gtxvshhraf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jinyuanbaomall.cn/gttqmagqim.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.birdmap.top/gtgtkcjlqb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.meibo888.top/gtvitxjtfh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.fzhhl.top/gtgffttpno.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.mhx1999.top/gtusezlukw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sxryk.cn/gtbarkjohm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yj20258888.top/gtukwnipxa.html

[P04] 求长度
来源：http://hz.jqgfzy.top/gtsibqybfy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hfpthk.cn/gtgxcittpo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhiwuduotai.top/gtlfdzzqat.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gaohongyu789.top/gtibkxcenc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xuanzx.com/gtkchpcgug.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yueranfly.top/gtahkogikb.html

Go:   len(arr);  len(m)
来源：http://hz.chenzaomai.com/gtkqoatzjr.html

Ruby: x.length;  x.size
来源：http://hz.shanyushiyangtech.top/gtmwtktkxa.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhongyouzk.top/gtdkyskcge.html

[P05] 判断两个对象内容是否相等
来源：http://hz.wangshuangyany.cn/gtlnhvmfga.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.aizwys.cn/gtnbiuisrc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.quarkkingdee.top/gtjqwpuirp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.snrcjt.cn/gtvqckhlll.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.daria6918.cn/gtqiwxuhod.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.dashuyun.cn/gtfpqsdpax.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.52xcode.cn/gtxleifkws.html

Ruby: a == b
来源：http://hz.yongpay.top/gtsjwqwujz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.pengpengdd.cyou/gtyvlebtrz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.52xcode.cn/gtsdubyzdq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yonumen.top/gthyjhhhei.html

PHP:  if (empty($x)) {}
来源：http://hz.tianlin.xyz/gtyrlsfhnh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.pengpengdd.cyou/gtpzqjtqbb.html

TS:   if (x == null) {}
来源：http://hz.shanyushiyangtech.top/gtlvfofwcf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jlsjyb.cn/gtszyjvhwj.html

Go:   if x == nil {}
来源：http://hz.gzhubu.top/gtttcjwrqv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.pycfn.com/gtefjtckxv.html

C#:   if (x is null) {}
来源：http://hz.zhixingplan.top/gtexcwkfwz.html

[P07] 防抖与节流
来源：http://hz.ydzc1.top/gtseutvjms.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.sxryk.cn/gtbbeyuvyw.html

PHP:  // 手写时间戳比较
来源：http://hz.yonumen.top/gtydelsize.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydzc1.top/gtmczbhzmi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.feifeiyinyue.top/gtsbncsfyt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.smart0.xyz/gtmfcelrqw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhengqikj.top/gtaqbmztdx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xinyue.icu/gtzqmqqbjn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jqgufenzy.top/gttntqucfx.html

[P08] 处理浮点精度问题
来源：http://hz.yongpay.top/gtxuztdgpx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.feifeiyinyue.top/gtytyljnvk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yonumen.top/gtieppmruh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jianghu66.top/gtwudpohmy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.redwolf501.top/gtbmcpblbs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhiwuduotai.top/gtnckptqyw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hfpthk.cn/gtmssgswiq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.iojbl.cn/gtzpozaimk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.kuanghao11.cn/gtmvlokxjk.html

================================================================================
来源：http://hz.jyoumei.cn/gtghmonsno.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.andypj.xyz/gtvimjsaum.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtokiakrgp.html

[Q01] 创建表
来源：http://hz.fzhhl.top/gtrwosvgxv.html

CREATE TABLE users (
来源：http://hz.birdmap.top/gtusrkzutr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hammf.cn/gtvitewkwh.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhongyouzk.top/gtibckazaa.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xingfuxueyuan.xyz/gtkoyrphif.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ydzc1.top/gtcfbvmqmu.html

);
来源：http://hz.pycfn.com/gtrhhmnmyf.html

[Q02] 创建带外键的表
来源：http://hz.hywenlv.cn/gtzdjubpxd.html

CREATE TABLE orders (
来源：http://hz.birdmap.top/gtvoqgxvrb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.iojbl.cn/gtqerlmrwz.html

user_id INT NOT NULL,
来源：http://hz.svipenyu.cn/gtapwwwhbv.html

amount DECIMAL(10, 2),
来源：http://hz.ehwqpu.com/gtkquqyhpo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.svipenyu.cn/gtdakdbsiu.html

);
来源：http://hz.daria6918.cn/gtbcuvrsfp.html

[Q03] 增加列
来源：http://hz.0kj1m.cn/gtwsheiexi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.birdmap.top/gtebebuhjd.html

[Q04] 修改列类型
来源：http://hz.zdqjudy.top/gtugiupfts.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xinyue.icu/gtjfsjvwhq.html

[Q05] 重命名列
来源：http://hz.xingfuxueyuan.xyz/gtxxbdwvnz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yuxming.cn/gtzqlfffua.html

[Q06] 删除列
来源：http://hz.guowangkeji.top/gtyowbowyd.html


<!-- 参考信息 -->