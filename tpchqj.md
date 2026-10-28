代发 wailian999

JS:   process.exit(1)
来源：http://hz.hfpthk.cn/gtaqxdmaui.html

TS:   process.exit(1)
来源：http://hz.yueranfly.top/gtdbignxsx.html

Java: System.exit(1)
来源：http://hz.chenjidiqi.icu/gtilqdffza.html

Go:   os.Exit(1)
来源：http://hz.316326.xyz/gtyqjmvajp.html

Ruby: exit 1
来源：http://hz.nwbrower.top/gtdrhzotuw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hammf.cn/gtvgqcepnr.html

[M06] 向标准错误输出
来源：http://hz.hongshengwenyu.top/gtlyjivhmf.html

Py:   print("err", file=sys.stderr)
来源：http://hz.wangdashe.top/gtwmpbgigh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zdqjudy.top/gttmjqdwuu.html

JS:   console.error("err")
来源：http://hz.aibaodan.cn/gtolsuuipm.html

TS:   console.error("err")
来源：http://hz.zhaomingkeji.xyz/gtptmgbtos.html

Java: System.err.println("err")
来源：http://hz.nwbrower.top/gttbpombwg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.dashuyun.cn/gtuaeivxtf.html

Ruby: warn "err"
来源：http://hz.pycfn.com/gtmpcvkrlk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hywenlv.cn/gtdhrnfbpp.html

[M07] 判断是否为主入口
来源：http://hz.0kj1m.cn/gtbkiefhvr.html

Py:   if __name__ == "__main__":
来源：http://hz.hfpthk.cn/gtlolxglkt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.aibaodan.cn/gtufamhdsx.html

JS:   require.main === module
来源：http://hz.jinqigfzy.top/gtmdhczmfv.html

TS:   require.main === module
来源：http://hz.meibo888.top/gtbkpwuygr.html

Java: public static void main(String[] args)
来源：http://hz.jinghuilouyu.cn/gtfjdmztos.html

Go:   func main()
来源：http://hz.hnxiangtu.top/gtnriqvfcc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.havefunace.top/gthywdywui.html

C#:   static void Main(string[] args)
来源：http://hz.zhaomingkeji.xyz/gtqcepqppz.html

[M08] 获取系统与运行时信息
来源：http://hz.zhengqikj.top/gtbscflrlc.html

Py:   platform.system();  platform.python_version()
来源：http://hz.316326.xyz/gtwtedxkfu.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.smart0.xyz/gtjbfntxla.html

JS:   process.platform;  process.version
来源：http://hz.ywan-chungtsiang.top/gtauincnpg.html

TS:   process.platform;  process.version
来源：http://hz.yuanzhike.top/gthavwevda.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yj20258.top/gtyvxfxeis.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.dianchejie.cn/gtptzdljvz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhixingplan.top/gtokopvuyu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.daria6918.cn/gtvmsyudyw.html

================================================================================
来源：http://hz.yj20258888.top/gtznjodujq.html

N. 数据结构与算法
来源：http://hz.snrcjt.cn/gtqdzshrxn.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtmqikcxxa.html

[N01] 二分查找（有序数组）
来源：http://hz.kuanghao11.cn/gtvncicbvm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sweek.top/gtfudhnzak.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.chenjidiqi.icu/gtgeslqqnr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jlsjyb.cn/gtbovwpxda.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fzhhl.top/gthlznmmho.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zdqjudy.top/gtzxdghpme.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cashguo.top/gtifflbvkh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.wangshuangyany.cn/gtyseqgawp.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.dianchejie.cn/gthrsuczty.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.0kj1m.cn/gtezizfaow.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangshuangyany.cn/gtuqdbcaxw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shanyushiyangkeji.top/gtvxsnamqk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aibaodan.cn/gtycnrkpok.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cdnleiting.top/gtbqqtheac.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.gotoacloud.top/gthbjzaitp.html

Go:   slices.Sort(arr)
来源：http://hz.cdnleiting.top/gtmhnrqcor.html

Ruby: arr.sort
来源：http://hz.ydjk.org.cn/gtjtfnhnvl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.chenlongwang.top/gtorepfqao.html

[N03] 快速排序（分治示例）
来源：http://hz.zhaomingkeji.xyz/gtfdbnxtxn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jqgfzy.top/gtcrciwjuw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.52xcode.cn/gtclxmhnja.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xinyue.icu/gtkylykwiz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.svipenyu.cn/gtgdrmlgvx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tanke756.top/gthdrpfkhf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.guannengcc.top/gthvxfxtuj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ywan-chungtsiang.top/gtgobmfzqw.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.316326.xyz/gtkleiumtx.html

[N04] 斐波那契数列
来源：http://hz.hywenlv.cn/gtpejjzifq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhiwuduotai.top/gtrldfmjxe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.birdmap.top/gtxgvrfvng.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dashuyun.cn/gthoiosvir.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cheryme.top/gtqebxouak.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sweek.top/gthfzfszsd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.haohaochexian.top/gtwonyegva.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhoulong.xyz/gtmmikxysj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yuanzhike.top/gtdysevowk.html

[N05] 最大公约数
来源：http://hz.zhoulong.xyz/gtlvprzcpy.html

Py:   math.gcd(a, b)
来源：http://hz.andypj.xyz/gtyjxvmsjd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinghuilouyu.cn/gtbdtemrir.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gotoacloud.top/gtelpgbaya.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dashuyun.cn/gtaejxsyii.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.vqdsnc.cn/gtnejqaaqw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.wangdashe.top/gtovqotcuc.html

Ruby: a.gcd(b)
来源：http://hz.havefunace.top/gtvfzmqkns.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhaomingkeji.xyz/gthtlyobyz.html

[N06] 判断回文字符串
来源：http://hz.bjfxy.top/gtfjjbnwcx.html

Py:   s == s[::-1]
来源：http://hz.yuxming.cn/gtvkkxpxwl.html

PHP:  $s === strrev($s);
来源：http://hz.zycfv.cn/gtjojgmntt.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtnoeumvjt.html

TS:   s === [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtktqbnjep.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ehwqpu.com/gtxyddezcy.html

Go:   // 双指针从两端比较
来源：http://hz.hongshengwenyu.top/gthcxuzxta.html

Ruby: s == s.reverse
来源：http://hz.jianghu66.top/gtobdhrdpv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yangfankeji.com/gtuqgdzvgk.html

[N07] 两数之和（返回下标）
来源：http://hz.yongpay.top/gtjbswkeal.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yueranfly.top/gtrqpugygn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hammf.cn/gtusdgcrno.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sysykeji.top/gtkshmhtnc.html

TS:   // 手写 Map<string, number>
来源：http://hz.yonumen.top/gtfhdhhysa.html

Java: // 手写 HashMap
来源：http://hz.hnxiangtu.top/gtvepyqcqs.html

Go:   // 手写 map[int]int
来源：http://hz.guowangkeji.top/gtckeadvxw.html

Ruby: // 手写 Hash
来源：http://hz.meibo888.top/gtprkhbsls.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.andypj.xyz/gtfrzuqmna.html

[N08] 生成全排列
来源：http://hz.aizwys.cn/gtyrcpfses.html

Py:   itertools.permutations(arr)
来源：http://hz.iojbl.cn/gtmerfehig.html

PHP:  // 手写递归交换
来源：http://hz.tian-w.cn/gthxgqutbl.html

JS:   // 手写回溯递归
来源：http://hz.nwbrower.top/gtqfhaocpc.html

TS:   // 手写回溯递归
来源：http://hz.cqqwz.cn/gtpqhkjgsu.html

Java: // 手写回溯递归
来源：http://hz.xziqi.cn/gtahjxeowf.html

Go:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtlqqcmgcn.html

Ruby: arr.permutation.to_a
来源：http://hz.zhongyouzk.top/gtfqcwbndx.html

C#:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtnmkmtpaq.html

[N09] 栈与队列
来源：http://hz.yonumen.top/gtdgtqktbr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhiwuduotai.top/gtzmvmtpvq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.pycfn.com/gtguqsknjz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jianghu66.top/gtcvkgnngq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.fengsongda.top/gtkktiybht.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ydzc1.top/gtozuzzqrx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cheryme.top/gtbjiciumn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.9152youxi.cn/gtrwzfeyno.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.316326.xyz/gtbnqtbhty.html

[N10] 链表节点定义
来源：http://hz.c1oappe.top/gtjkqgfxsm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.guowangkeji.top/gtckaitzpa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.redwolf501.top/gtsdlrvjem.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj20258888.top/gtguenhvdr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.fengsongda.top/gtjymymrlv.html

Java: class Node { int v; Node next; }
来源：http://hz.iojbl.cn/gtuxiavgsi.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.sufxvd.cn/gtkxgqnecr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.chenzaomai.com/gtrjbnpsei.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhongyouzk.top/gtoyysgyxo.html

[N11] 二叉树中序遍历
来源：http://hz.yj20258888.top/gtjnhsvhfy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cheryme.top/gtldolyxfj.html

PHP:  // 手写递归函数
来源：http://hz.wangdashe.top/gtzvnhwvzp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.feifeiyinyue.top/gtbgbgwysb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.kuanghao11.cn/gtrgmxkhbk.html

Java: // 手写递归
来源：http://hz.quarkkingdee.top/gthjznguai.html

Go:   // 手写递归
来源：http://hz.hysaishi.cn/gtfrvvkirw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.havefunace.top/gthupghnvq.html

C#:   // 手写递归
来源：http://hz.zhixingplan.top/gtivmwgwmk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.aizwys.cn/gtxuryxpqi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ydjk.org.cn/gthxkfagbl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.nwbrower.top/gtpztcujus.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cqqwz.cn/gtmklblpal.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhaomingkeji.xyz/gtpkaewmgo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yanxiufei.cn/gtsyagtcic.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hnxiangtu.top/gtmtpgppie.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zycfv.cn/gtdtobschh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigufen.top/gtcbupakqz.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gttksgzmww.html

O. 并发与异步
来源：http://hz.snrcjt.cn/gtznaedxxf.html

================================================================================
来源：http://hz.0kj1m.cn/gtapkrwypq.html

[O01] 启动一个线程
来源：http://hz.pengpengdd.cyou/gtetnlajds.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.dianchejie.cn/gteawggfkm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.52xcode.cn/gtaumyrinw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.iojbl.cn/gtflinjeye.html

TS:   // 同 JS
来源：http://hz.pengpengdd.cyou/gttgvteakr.html

Java: new Thread(() -> f()).start()
来源：http://hz.yj20258888.top/gtzavxchxl.html

Go:   go f()
来源：http://hz.cashguo.top/gtltxectjv.html

Ruby: Thread.new { f }
来源：http://hz.yongpay.top/gtvrzmcqow.html

C#:   Task.Run(() => F());
来源：http://hz.cqqwz.cn/gtrzwlyovj.html

[O02] 使用线程池
来源：http://hz.yangfankeji.com/gttvclbpcq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.mhx1999.top/gtiqiihemo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hfpthk.cn/gtypwmzcdw.html

JS:   // worker_threads 线程池
来源：http://hz.zhixingplan.top/gtrqbrzgap.html

TS:   // worker_threads 线程池
来源：http://hz.jyoumei.cn/gtcsdltawy.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhengqikj.top/gtihrnctee.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.chenjidiqi.icu/gtjbzjrsug.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.aizwys.cn/gtntkkmgab.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.mhx1999.top/gtdewjkctn.html

[O03] 加锁保护共享数据
来源：http://hz.jianghu66.top/gtyyqiuzwe.html

Py:   with lock: shared += 1
来源：http://hz.tanke756.top/gtsyxrbyrd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.c1oappe.top/gtphzmwmdy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.vqdsnc.cn/gtjjrgplxg.html

TS:   // 同 JS
来源：http://hz.ydjk.org.cn/gtemqpyhhj.html

Java: synchronized (this) { shared++; }
来源：http://hz.bjfxy.top/gtdfbskjlr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.pengpengdd.cyou/gtvexhlyrj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hnxiangtu.top/gtlrmgojrv.html

C#:   lock (gate) { shared++; }
来源：http://hz.wangdashe.top/gtqfupypuk.html

[O04] 定义异步函数并等待
来源：http://hz.pengpengdd.cyou/gtxtywqwap.html

Py:   async def f():⏎    await g()
来源：http://hz.cashguo.top/gtmoebzyvu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.iojbl.cn/gtfgbwjsuw.html

JS:   async function f() { await g(); }
来源：http://hz.bjfxy.top/gtcjidikrx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.daxiang520.top/gtrkripdmq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.wangdashe.top/gtvjglacpz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yuxming.cn/gtknzqafac.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ydjk.org.cn/gtuediheap.html

C#:   async Task F() { await G(); }
来源：http://hz.svipenyu.cn/gtwjmfxpdd.html

[O05] 并发执行并等待全部完成
来源：http://hz.jiagoushi.top/gtxwltbgra.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jqgufenzy.top/gtteofuhej.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.tanke756.top/gtqsyxbjao.html

JS:   await Promise.all(tasks)
来源：http://hz.gotoacloud.top/gtyfkwzthl.html

TS:   await Promise.all(tasks)
来源：http://hz.jinqigfzy.top/gtjogfckge.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yangfankeji.com/gtmmlysujy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.gogol.net.cn/gtivdqobhg.html

Ruby: threads.map(&:join)
来源：http://hz.cashguo.top/gttkeaeejz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.fzhhl.top/gtmbwxfxnm.html

[O06] 使用进程池
来源：http://hz.iojbl.cn/gtusmhjcvy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.wangshuangyany.cn/gtpnoxgjgs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cdnleiting.top/gtryxtbptn.html

JS:   // child_process / cluster 模块
来源：http://hz.tanke756.top/gtdhnntanb.html

TS:   // child_process / cluster 模块
来源：http://hz.chenzaomai.com/gtnxugkfpa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ydjk.org.cn/gtwiqpxvgu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.fengsongda.top/gtlafhqofu.html

Ruby: // fork 块
来源：http://hz.xziqi.cn/gtqutlmmin.html

C#:   Parallel.For
来源：http://hz.hysaishi.cn/gtdbfevlyu.html

================================================================================
来源：http://hz.cdnleiting.top/gtunlwoyap.html

P. 常用工具函数
来源：http://hz.sweek.top/gtovgiceoc.html

================================================================================
来源：http://hz.sxryk.cn/gtbaavccio.html

[P01] 生成 UUID
来源：http://hz.gzhubu.top/gtxwgkzewd.html

Py:   str(uuid.uuid4())
来源：http://hz.tanke756.top/gtvkqgdxuc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.fzhhl.top/gtixayvptf.html

JS:   crypto.randomUUID()
来源：http://hz.guowangkeji.top/gtzbropcjg.html

TS:   crypto.randomUUID()
来源：http://hz.jinqigfzy.top/gtbuojnswh.html

Java: UUID.randomUUID().toString()
来源：http://hz.quarkkingdee.top/gtjvrnercj.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xylfe.cn/gtwksnjcio.html

Ruby: SecureRandom.uuid
来源：http://hz.shanyushiyangtech.top/gtthsfptgn.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhixingplan.top/gtxepqulzd.html

[P02] MD5 / SHA256 摘要
来源：http://hz.snrcjt.cn/gtrwanyzpy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.tianlin.xyz/gtycppfhoa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.guowangkeji.top/gtaidkdbib.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.fengsongda.top/gthhjqhtuc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhijiandao.cn/gttrqfaxot.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hnxiangtu.top/gtoejltiqq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.guannengcc.top/gtduokkvwe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.316326.xyz/gtbpniqidd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jinqigufen.top/gtohlakkpt.html

[P03] 生成短随机字符串
来源：http://hz.fzhhl.top/gtetrjwzui.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ybcxt.top/gttjgdffyw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.guannengcc.top/gttffmgout.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.bjfxy.top/gtevbkccsn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gotoacloud.top/gtkopafxlo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ywan-chungtsiang.top/gtsedxstgc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ybcxt.top/gtvnjwtimb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.bjfxy.top/gtkxytrwlf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.quarkkingdee.top/gtuneasgxl.html

[P04] 求长度
来源：http://hz.hysaishi.cn/gtlxdyzxui.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.nwbrower.top/gtnnnfthym.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenzaomai.com/gtdemllqgc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnxiangtu.top/gtfbpwymbk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jlsjyb.cn/gtxuxbcnuu.html

Java: list.size();  map.size();  s.length()
来源：http://hz.daxiang520.top/gtsladdhzy.html

Go:   len(arr);  len(m)
来源：http://hz.ppjwa.cn/gtvuwrvhrd.html

Ruby: x.length;  x.size
来源：http://hz.jiagoushi.top/gtnjwmmyrc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.andypj.xyz/gtkjegaxfi.html

[P05] 判断两个对象内容是否相等
来源：http://hz.daria6918.cn/gthmkivzoa.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hysaishi.cn/gtyjsiyzbr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ydzc1.top/gtnvdmwnma.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.cheryme.top/gtsrsmgzrl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.daria6918.cn/gtwevumqno.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.guannengcc.top/gtjoqnedjt.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hysaishi.cn/gtnistkyat.html

Ruby: a == b
来源：http://hz.ybcxt.top/gtjwtkrnvl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.tianlin.xyz/gtqirzzifp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cqqwz.cn/gtmaoeljif.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hysaishi.cn/gtezmldyhq.html

PHP:  if (empty($x)) {}
来源：http://hz.vqdsnc.cn/gtxabkhiwf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhiwuduotai.top/gtffgagiwx.html

TS:   if (x == null) {}
来源：http://hz.sufxvd.cn/gtzlfqwbgw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sweek.top/gtkaqebvfo.html

Go:   if x == nil {}
来源：http://hz.jinqigfzy.top/gtnzcujjaw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.pengpengdd.cyou/gtasdvxzrb.html

C#:   if (x is null) {}
来源：http://hz.yanxiufei.cn/gtzubukzai.html

[P07] 防抖与节流
来源：http://hz.jinqigufen.top/gtdqwxjket.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.pengpengdd.cyou/gtazzshvou.html

PHP:  // 手写时间戳比较
来源：http://hz.9152youxi.cn/gtsplonkmf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.52xcode.cn/gtwjugesor.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.0kj1m.cn/gtdchqcakg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.guannengcc.top/gtpcnwvcdx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.meibo888.top/gtigiccznm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jianghu66.top/gtswacsbxf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.aibaodan.cn/gtvbxtnwgj.html

[P08] 处理浮点精度问题
来源：http://hz.zhijiandao.cn/gtnucfzqjq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.sufxvd.cn/gtbwivqguh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ydzc1.top/gtzqcpnser.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.316326.xyz/gtjwsmocmb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.aibaodan.cn/gtblbbvpwh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cdnleiting.top/gtlijaftcv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shanyushiyangkeji.top/gteiuvsvkw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cucudq.cn/gtotphqejf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xylfe.cn/gteowdyhps.html

================================================================================
来源：http://hz.gogol.net.cn/gtmqmxvpdm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jianghu66.top/gtjeshyckj.html

================================================================================
来源：http://hz.yongpay.top/gtjtfiqono.html

[Q01] 创建表
来源：http://hz.nanxinkj.top/gtgxokgxei.html

CREATE TABLE users (
来源：http://hz.zhijiandao.cn/gtbnwxehpo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.svipenyu.cn/gthvjohrhe.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xinyue.icu/gtrsgucvlu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.guowangkeji.top/gtlbipzyuf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xinyue.icu/gtjevoqzrp.html

);
来源：http://hz.ywan-chungtsiang.top/gtbwjdgjbt.html

[Q02] 创建带外键的表
来源：http://hz.andypj.xyz/gthvgarmiv.html

CREATE TABLE orders (
来源：http://hz.zdqjudy.top/gtystopyui.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.fengsongda.top/gtivbeaeum.html

user_id INT NOT NULL,
来源：http://hz.jyoumei.cn/gtksdnchck.html

amount DECIMAL(10, 2),
来源：http://hz.jinqigufen.top/gtdaknivfn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hfpthk.cn/gtptbvaifa.html

);
来源：http://hz.ehwqpu.com/gtqylotlob.html

[Q03] 增加列
来源：http://hz.svipenyu.cn/gtsbnldmxx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jqgfzy.top/gtlenbzpdv.html

[Q04] 修改列类型
来源：http://hz.xingfuxueyuan.xyz/gtrrhzcxdn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xingfuxueyuan.xyz/gtwxukncuv.html

[Q05] 重命名列
来源：http://hz.wangdashe.top/gtpzijdoyx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhengqikj.top/gtpwoehuqd.html

[Q06] 删除列
来源：http://hz.chenlongwang.top/gttfejmzza.html


<!-- 参考信息 -->