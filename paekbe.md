代发 wailian999

JS:   process.exit(1)
来源：http://hz.gogol.net.cn/gtumxwirzz.html

TS:   process.exit(1)
来源：http://hz.hfpthk.cn/gtytbpfwan.html

Java: System.exit(1)
来源：http://hz.chenlongwang.top/gtodtkjxaz.html

Go:   os.Exit(1)
来源：http://hz.fengsongda.top/gtbhoyzjdp.html

Ruby: exit 1
来源：http://hz.shanyushiyangkeji.top/gtpickofwn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.svipenyu.cn/gtzpsmwfmx.html

[M06] 向标准错误输出
来源：http://hz.hywenlv.cn/gthfpdlomp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.tanke756.top/gtpifzfqpj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.c1oappe.top/gtrivrgpqn.html

JS:   console.error("err")
来源：http://hz.hammf.cn/gtpvnonytw.html

TS:   console.error("err")
来源：http://hz.cashguo.top/gtlcuhzdrs.html

Java: System.err.println("err")
来源：http://hz.wangshuangyany.cn/gtcxqqlwkn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.tanke756.top/gtdxgjwlvt.html

Ruby: warn "err"
来源：http://hz.jinqigfzy.top/gtzuqasegp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shangyingyoupin.top/gtzydqmppn.html

[M07] 判断是否为主入口
来源：http://hz.shanyushiyangtech.top/gtrtsdyfyn.html

Py:   if __name__ == "__main__":
来源：http://hz.bjfxy.top/gtsuvjstmj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gogol.net.cn/gtcgrsufid.html

JS:   require.main === module
来源：http://hz.daria6918.cn/gtrsradcmr.html

TS:   require.main === module
来源：http://hz.zycfv.cn/gtpobiscpi.html

Java: public static void main(String[] args)
来源：http://hz.yueranfly.top/gtqzockwtp.html

Go:   func main()
来源：http://hz.yvedp.cn/gtewlpehfx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jianghu66.top/gtorfpdqcy.html

C#:   static void Main(string[] args)
来源：http://hz.yuanzhike.top/gtamufhblc.html

[M08] 获取系统与运行时信息
来源：http://hz.birdmap.top/gtsthorkbm.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhengqikj.top/gttstxtkgk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yueranfly.top/gtxqtmgqjs.html

JS:   process.platform;  process.version
来源：http://hz.dashuyun.cn/gtlthuljue.html

TS:   process.platform;  process.version
来源：http://hz.cucudq.cn/gtedjvpnym.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hammf.cn/gtzxvdawrn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.vqdsnc.cn/gtkllyoesu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cashguo.top/gtgmtncooz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.0kj1m.cn/gtkqyycfyo.html

================================================================================
来源：http://hz.guannengcc.top/gthuzdzgju.html

N. 数据结构与算法
来源：http://hz.jyoumei.cn/gtwioupqie.html

================================================================================
来源：http://hz.shzxlz.cn/gtoyqkmfqt.html

[N01] 二分查找（有序数组）
来源：http://hz.c1oappe.top/gtazfhhvzt.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hysaishi.cn/gtkrnevqiy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xingfuxueyuan.xyz/gtmwhhivkg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.havefunace.top/gtsfcwplpf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xylfe.cn/gtvrycmqbd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenzaomai.com/gtnqkfowzy.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.haohaochexian.top/gtrmeuvcxa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.havefunace.top/gtdfntspfh.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.tianlin.xyz/gtqcehrjek.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.nanxuanxn.top/gtmtsfgguo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhengqikj.top/gtpufgpkzu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hammf.cn/gtndayxkyb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shuidangran.top/gtmsomwszj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ivvv.top/gtmamaxjcq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.birdmap.top/gthmnqskuz.html

Go:   slices.Sort(arr)
来源：http://hz.meibo888.top/gtkzudwkfp.html

Ruby: arr.sort
来源：http://hz.0kj1m.cn/gtjrdbcssl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shzxlz.cn/gtyreeuone.html

[N03] 快速排序（分治示例）
来源：http://hz.nanxinkj.top/gtxantpwuw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.vqdsnc.cn/gtqhkdzous.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinqigfzy.top/gtsosuandz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydjk.org.cn/gtpezcngdy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cheryme.top/gtymghqhrf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.wangdashe.top/gtsrcswrbk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhixingplan.top/gttjrqwvvm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gotoacloud.top/gtoqmiyifv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hfpthk.cn/gtfwqxacxr.html

[N04] 斐波那契数列
来源：http://hz.hywenlv.cn/gtmgxylwrb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xuanzx.com/gtgrcqvdrv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hfpthk.cn/gtnynbcodu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenjidiqi.icu/gtkjqbbrdj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yvedp.cn/gtucjgbich.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yonumen.top/gtwymwpmeh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yj20258888.top/gtportxyha.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.tian-w.cn/gtromvluet.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zycfv.cn/gtcslaumkk.html

[N05] 最大公约数
来源：http://hz.zhengqikj.top/gtfpfxucpr.html

Py:   math.gcd(a, b)
来源：http://hz.zhoulong.xyz/gtnycixqqa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.aizwys.cn/gtrudclluv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgufenzy.top/gtxedbjgsu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dianchejie.cn/gtmdjwnvnu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cheryme.top/gthufijpio.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shzxlz.cn/gtaxwfkxti.html

Ruby: a.gcd(b)
来源：http://hz.yongpay.top/gtesdaeieq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hfpthk.cn/gtelwwgqbm.html

[N06] 判断回文字符串
来源：http://hz.52xcode.cn/gtayjrqfcn.html

Py:   s == s[::-1]
来源：http://hz.vqdsnc.cn/gtvnufquxm.html

PHP:  $s === strrev($s);
来源：http://hz.ybcxt.top/gthxpmwxup.html

JS:   s === [...s].reverse().join("")
来源：http://hz.birdmap.top/gtcodomtcd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xuanzx.com/gtaojdqfpg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.gzhubu.top/gtkclqdbyl.html

Go:   // 双指针从两端比较
来源：http://hz.zhiwuduotai.top/gtztpzgnzs.html

Ruby: s == s.reverse
来源：http://hz.dianchejie.cn/gtaqpvqsni.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.svipenyu.cn/gttibrftoi.html

[N07] 两数之和（返回下标）
来源：http://hz.dianchejie.cn/gtvcetkkel.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.pengpengdd.cyou/gtfisblelu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.wangshuangyany.cn/gtuhtzyvvi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yanxiufei.cn/gttgkjtzrw.html

TS:   // 手写 Map<string, number>
来源：http://hz.mhx1999.top/gtlazjscsa.html

Java: // 手写 HashMap
来源：http://hz.chenlongwang.top/gtwxrxdgon.html

Go:   // 手写 map[int]int
来源：http://hz.zycfv.cn/gtwwdmccup.html

Ruby: // 手写 Hash
来源：http://hz.jqgufenzy.top/gtmvscjukf.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yvedp.cn/gtyahkvozn.html

[N08] 生成全排列
来源：http://hz.hammf.cn/gtpaadlqap.html

Py:   itertools.permutations(arr)
来源：http://hz.xziqi.cn/gtlzpfrqrs.html

PHP:  // 手写递归交换
来源：http://hz.wangdashe.top/gtczkqlidd.html

JS:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtsqhukcak.html

TS:   // 手写回溯递归
来源：http://hz.52xcode.cn/gtwyqlztpz.html

Java: // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtmdupxywm.html

Go:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gthnzstolw.html

Ruby: arr.permutation.to_a
来源：http://hz.tian-w.cn/gtrfgkcjys.html

C#:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtuxjivcei.html

[N09] 栈与队列
来源：http://hz.shanyushiyangkeji.top/gtgyvqhymy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xziqi.cn/gtjhovtulq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.aizwys.cn/gtbqjotbwu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ppjwa.cn/gthicatnvh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ppjwa.cn/gtkspugduk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yongpay.top/gtsfjgvoug.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.feifeiyinyue.top/gtgemkofgf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.316326.xyz/gtagechopx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jiagoushi.top/gttggbzhkn.html

[N10] 链表节点定义
来源：http://hz.sufxvd.cn/gtrbovtenf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.wangshuangyany.cn/gtqvwzougg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sysykeji.top/gtwhqpevez.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.feifeiyinyue.top/gtuwfutxbf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.svipenyu.cn/gtcqpiitdk.html

Java: class Node { int v; Node next; }
来源：http://hz.cashguo.top/gtvnidouah.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.dashuyun.cn/gtpnjnjxly.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.daria6918.cn/gtyjkfufcs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.havefunace.top/gtialfasqc.html

[N11] 二叉树中序遍历
来源：http://hz.hammf.cn/gtqvnswtsb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yonumen.top/gtgeaarjil.html

PHP:  // 手写递归函数
来源：http://hz.yvedp.cn/gtyjerhjhn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gogol.net.cn/gtjnkjyovk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ppjwa.cn/gtmoagorea.html

Java: // 手写递归
来源：http://hz.hysaishi.cn/gtipqgcwul.html

Go:   // 手写递归
来源：http://hz.birdmap.top/gtfgurreox.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hammf.cn/gtzxkarzeo.html

C#:   // 手写递归
来源：http://hz.gaohongyu789.top/gtqbbykvio.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xuanzx.com/gtlljjoocv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hongshengwenyu.top/gtfvuvdfwg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.52xcode.cn/gttpnlngvd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinqigufen.top/gtrsmktsha.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shzxlz.cn/gtiyjmkuyl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.0kj1m.cn/gtdqfqvcfk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.smart0.xyz/gtrkhpbvvj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ehwqpu.com/gtdskjzecm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.meibo888.top/gtaswuxsmp.html

================================================================================
来源：http://hz.bjfxy.top/gttghhreui.html

O. 并发与异步
来源：http://hz.xuanzx.com/gtcbzibopy.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtarxxszjz.html

[O01] 启动一个线程
来源：http://hz.fengsongda.top/gtyszsdcrr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.daria6918.cn/gtxntwdrbr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.quarkkingdee.top/gtskyzvsja.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fzhhl.top/gtporcejqo.html

TS:   // 同 JS
来源：http://hz.ywan-chungtsiang.top/gtnreepmwo.html

Java: new Thread(() -> f()).start()
来源：http://hz.gaohongyu789.top/gtobeujxmp.html

Go:   go f()
来源：http://hz.yuanzhike.top/gtlvfsexag.html

Ruby: Thread.new { f }
来源：http://hz.xuanzx.com/gtogeogodu.html

C#:   Task.Run(() => F());
来源：http://hz.yj20258.top/gtdhmrwhqy.html

[O02] 使用线程池
来源：http://hz.hnqzz.top/gtbfwvpbai.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hnxiangtu.top/gtrgtoucnv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.snrcjt.cn/gtddvanyml.html

JS:   // worker_threads 线程池
来源：http://hz.ydzc1.top/gtqqtxumux.html

TS:   // worker_threads 线程池
来源：http://hz.jqgfzy.top/gtpigsyehu.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhiwuduotai.top/gtjnwcxlgn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.nwbrower.top/gttixszcbh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinghuilouyu.cn/gtwtxouyeo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhoulong.xyz/gtviyetyib.html

[O03] 加锁保护共享数据
来源：http://hz.sxryk.cn/gtihkptnjd.html

Py:   with lock: shared += 1
来源：http://hz.jinghuilouyu.cn/gtrfhixqxt.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ybcxt.top/gtuosrqwdd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.snrcjt.cn/gtaajdetbc.html

TS:   // 同 JS
来源：http://hz.zhiwuduotai.top/gtnmvxcopm.html

Java: synchronized (this) { shared++; }
来源：http://hz.yangfankeji.com/gtrupjmjcm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhixingplan.top/gttnzvtnlc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yonumen.top/gtmrmlxxtx.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj202588.top/gtxjecepwr.html

[O04] 定义异步函数并等待
来源：http://hz.xuetiantiany.cn/gtqitvpaqe.html

Py:   async def f():⏎    await g()
来源：http://hz.birdmap.top/gtjohqmnsh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gzhubu.top/gtnjcfgycg.html

JS:   async function f() { await g(); }
来源：http://hz.xylfe.cn/gticktnbcj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jyoumei.cn/gttukebjtq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.nanxinkj.top/gtyyutriqn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hongshengwenyu.top/gtjenpkjrv.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gzhubu.top/gtcnueqeep.html

C#:   async Task F() { await G(); }
来源：http://hz.chenlongwang.top/gtpnfqjfnw.html

[O05] 并发执行并等待全部完成
来源：http://hz.pengpengdd.cyou/gtyytbmwmb.html

Py:   asyncio.gather(*tasks)
来源：http://hz.daria6918.cn/gteffvvxyy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.316326.xyz/gthoexfilh.html

JS:   await Promise.all(tasks)
来源：http://hz.52xcode.cn/gtfrcpznna.html

TS:   await Promise.all(tasks)
来源：http://hz.sufxvd.cn/gttlttgobk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shuidangran.top/gtrrcqfckq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xuanzx.com/gthnmyywau.html

Ruby: threads.map(&:join)
来源：http://hz.fzhhl.top/gtjaayiytg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xinyue.icu/gterorqmju.html

[O06] 使用进程池
来源：http://hz.9152youxi.cn/gtvarufsoc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.quarkkingdee.top/gtjounorfr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yanxiufei.cn/gtrzicnsaw.html

JS:   // child_process / cluster 模块
来源：http://hz.hywenlv.cn/gtejaxhyri.html

TS:   // child_process / cluster 模块
来源：http://hz.zdqjudy.top/gtnqfhyhnz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.fzhhl.top/gtyimqacct.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.birdmap.top/gtgczybank.html

Ruby: // fork 块
来源：http://hz.zhijiandao.cn/gtwoozhljw.html

C#:   Parallel.For
来源：http://hz.yuxming.cn/gtqpbvbvub.html

================================================================================
来源：http://hz.guannengcc.top/gtrhrwgguk.html

P. 常用工具函数
来源：http://hz.daxiang520.top/gtcogvxhue.html

================================================================================
来源：http://hz.aizwys.cn/gtpahognyw.html

[P01] 生成 UUID
来源：http://hz.yangfankeji.com/gtrbbeuxmz.html

Py:   str(uuid.uuid4())
来源：http://hz.jqgfzy.top/gtahhmrbhz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.nwbrower.top/gtradgenbe.html

JS:   crypto.randomUUID()
来源：http://hz.ehwqpu.com/gtjznoimob.html

TS:   crypto.randomUUID()
来源：http://hz.svipenyu.cn/gtklcyzpmt.html

Java: UUID.randomUUID().toString()
来源：http://hz.c1oappe.top/gtppvdvgml.html

Go:   // 用 github.com/google/uuid
来源：http://hz.fzhhl.top/gtipeulcrb.html

Ruby: SecureRandom.uuid
来源：http://hz.jinqigufen.top/gtdzniexvc.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.vqdsnc.cn/gttswcmazb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.gaohongyu789.top/gtzatsexcn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hnqzz.top/gtwqmrxvzy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yanxiufei.cn/gtvmpleznt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.316326.xyz/gttdzfncyg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hnqzz.top/gtxdxmzbpx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.daxiang520.top/gtjmshboag.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.mhx1999.top/gtywzxguly.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.wangdashe.top/gtgtlqescz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.bjfxy.top/gtdhllisfe.html

[P03] 生成短随机字符串
来源：http://hz.yuanzhike.top/gtueuliezl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gogol.net.cn/gtofdlepni.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ppjwa.cn/gtwhtidxir.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jiagoushi.top/gtzkqtjwnr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.vqdsnc.cn/gtwczljxiv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jlsjyb.cn/gtkpagerxz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jiagoushi.top/gtocvvuqss.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.pengpengdd.cyou/gtjpersjnt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.redwolf501.top/gtlalwojag.html

[P04] 求长度
来源：http://hz.cucudq.cn/gtsyarubbv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yj20258888.top/gtxqemdilq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj20258888.top/gtsvsqbqnu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sweek.top/gtvyvupnrv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.meibo888.top/gtatmnvebm.html

Java: list.size();  map.size();  s.length()
来源：http://hz.guowangkeji.top/gtpjmidvoo.html

Go:   len(arr);  len(m)
来源：http://hz.yanxiufei.cn/gtsirqlmel.html

Ruby: x.length;  x.size
来源：http://hz.haohaochexian.top/gtibadxlne.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.bjfxy.top/gtqivkwqvt.html

[P05] 判断两个对象内容是否相等
来源：http://hz.guowangkeji.top/gthhlbfhfa.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hywenlv.cn/gthufcbgyz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xingfuxueyuan.xyz/gtivyusqxn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ehwqpu.com/gtibvtbqab.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhiwuduotai.top/gtgoffckju.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.dashuyun.cn/gtwvitomrv.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yanxiufei.cn/gtppniiebe.html

Ruby: a == b
来源：http://hz.xuanzx.com/gtbtvygvbb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ydjk.org.cn/gtcktqcesq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ydjk.org.cn/gtkyusnisq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ywan-chungtsiang.top/gtavfjuqvb.html

PHP:  if (empty($x)) {}
来源：http://hz.hfpthk.cn/gtttldkhvt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.nanxinkj.top/gtmdpscani.html

TS:   if (x == null) {}
来源：http://hz.gzhubu.top/gtziscygfr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ydjk.org.cn/gtvwioguqb.html

Go:   if x == nil {}
来源：http://hz.guowangkeji.top/gtzjyfddnc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.mhx1999.top/gtjikwfioa.html

C#:   if (x is null) {}
来源：http://hz.cdnleiting.top/gtxcrdrayp.html

[P07] 防抖与节流
来源：http://hz.xinyue.icu/gtsloxlfnw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xuetiantiany.cn/gtwxpvzgvf.html

PHP:  // 手写时间戳比较
来源：http://hz.nwbrower.top/gtzwauwhiy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tian-w.cn/gtkkitkajb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yangfankeji.com/gtzyafwwgm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.9152youxi.cn/gtxcfmddhz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.aibaodan.cn/gtcjlkfmdx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.bjfxy.top/gtnmjkztoy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.fzhhl.top/gtmrxogyfn.html

[P08] 处理浮点精度问题
来源：http://hz.chenzaomai.com/gturhfyrkl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cashguo.top/gtgqdmwaou.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.smart0.xyz/gtooxsewxn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.shanyushiyangkeji.top/gtstgyfbff.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jinyuanbaomall.cn/gtkrwndflg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yj202588.top/gtsbzlstzg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.gogol.net.cn/gtxhrbtjvb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cdnleiting.top/gttvjxdrwz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.kuanghao11.cn/gtucyfviby.html

================================================================================
来源：http://hz.ydzc1.top/gtocmfuczc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ydzc1.top/gtfyieioiv.html

================================================================================
来源：http://hz.ehwqpu.com/gtqplsuzkd.html

[Q01] 创建表
来源：http://hz.hywenlv.cn/gtwdiodpuw.html

CREATE TABLE users (
来源：http://hz.shanyushiyangtech.top/gttdvjelqt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ehwqpu.com/gtsuwjuvzv.html

name VARCHAR(50) NOT NULL,
来源：http://hz.tanke756.top/gthmdiaiyc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.316326.xyz/gttrsaffhf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ehwqpu.com/gtdodrkvej.html

);
来源：http://hz.316326.xyz/gtwbvpoelo.html

[Q02] 创建带外键的表
来源：http://hz.jianghu66.top/gtstmukoxs.html

CREATE TABLE orders (
来源：http://hz.yonumen.top/gtwthzergr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yuanzhike.top/gteayysstn.html

user_id INT NOT NULL,
来源：http://hz.c1oappe.top/gtnbpnhgaw.html

amount DECIMAL(10, 2),
来源：http://hz.tian-w.cn/gtumceclei.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.mhx1999.top/gthoqjccdq.html

);
来源：http://hz.jianghu66.top/gtlhzqsyvm.html

[Q03] 增加列
来源：http://hz.yj20258.top/gtzgnbginc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhixingplan.top/gtkclmkcpy.html

[Q04] 修改列类型
来源：http://hz.haohaochexian.top/gtydpwitql.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ywan-chungtsiang.top/gteudzdcko.html

[Q05] 重命名列
来源：http://hz.gzhubu.top/gtwnwjkqnr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cheryme.top/gtxgkrsead.html

[Q06] 删除列
来源：http://hz.ehwqpu.com/gtxaokojtv.html


<!-- 参考信息 -->