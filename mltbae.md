代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hongshengwenyu.top/gtnyxemobn.html

JS:   console.error("err")
来源：http://hz.yj20258.top/gtyqnlwezk.html

TS:   console.error("err")
来源：http://hz.xingfuxueyuan.xyz/gtpmicrnnu.html

Java: System.err.println("err")
来源：http://hz.dianchejie.cn/gtzqshkwxv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.fengsongda.top/gtdjyirxel.html

Ruby: warn "err"
来源：http://hz.aibaodan.cn/gtjpfdabxt.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yj20258.top/gtpexzurde.html

[M07] 判断是否为主入口
来源：http://hz.zhoulong.xyz/gtlffawtlh.html

Py:   if __name__ == "__main__":
来源：http://hz.ivvv.top/gtgsmaeefc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jqgfzy.top/gtwnjvpjlu.html

JS:   require.main === module
来源：http://hz.0kj1m.cn/gtvwbqxibq.html

TS:   require.main === module
来源：http://hz.pengpengdd.cyou/gtmttjqzdl.html

Java: public static void main(String[] args)
来源：http://hz.xingfuxueyuan.xyz/gtdqulrzeh.html

Go:   func main()
来源：http://hz.xinyue.icu/gtulpneige.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.wangdashe.top/gteqilsbwj.html

C#:   static void Main(string[] args)
来源：http://hz.hongshengwenyu.top/gtobenmkxv.html

[M08] 获取系统与运行时信息
来源：http://hz.smart0.xyz/gtymqzzhoz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.9152youxi.cn/gtiemsbxzq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhaomingkeji.xyz/gtzwpaknbb.html

JS:   process.platform;  process.version
来源：http://hz.shangyingyoupin.top/gtjldgpeft.html

TS:   process.platform;  process.version
来源：http://hz.iojbl.cn/gtwysqocrg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.daxiang520.top/gtcsrluotd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jyoumei.cn/gtuexdzkix.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cashguo.top/gtjmusyeks.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhiwuduotai.top/gtjhfxbibl.html

================================================================================
来源：http://hz.gaohongyu789.top/gtwacpugtq.html

N. 数据结构与算法
来源：http://hz.dianchejie.cn/gtlbhfeosf.html

================================================================================
来源：http://hz.jianghu66.top/gtjrnisgmv.html

[N01] 二分查找（有序数组）
来源：http://hz.bjfxy.top/gtffcbaymr.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shuidangran.top/gtnigapxxx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.smart0.xyz/gtqhygixbp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jiagoushi.top/gttgtabewh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigfzy.top/gtxlgxvrdc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hywenlv.cn/gtsuwnlrcs.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.redwolf501.top/gtxpkdwlms.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xylfe.cn/gtxtydtkfw.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.havefunace.top/gtnjzxyjdj.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.fengsongda.top/gtzguwutfc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hywenlv.cn/gtnmrvtgyr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ivvv.top/gttszfgvxl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.birdmap.top/gtpindsjje.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fengsongda.top/gteigzucyb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yueranfly.top/gtqlmspieu.html

Go:   slices.Sort(arr)
来源：http://hz.zhixingplan.top/gtuylsyqxk.html

Ruby: arr.sort
来源：http://hz.hammf.cn/gtdttprgix.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.316326.xyz/gtctreksyt.html

[N03] 快速排序（分治示例）
来源：http://hz.xinyue.icu/gtsxtqjevk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.smart0.xyz/gtzntygswv.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cucudq.cn/gtkwyleqdu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sxryk.cn/gthrqetmgx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhijiandao.cn/gtrkqezxmb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.svipenyu.cn/gtydinlyzx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.vqdsnc.cn/gtazfkmllr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ydzc1.top/gtlqzwdpxm.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xuetiantiany.cn/gtwawberzu.html

[N04] 斐波那契数列
来源：http://hz.wangdashe.top/gtfibyegyj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tianlin.xyz/gtooyixdom.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.daxiang520.top/gtqfhmxjvo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.feifeiyinyue.top/gtuzqpilnm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sweek.top/gtvzcautui.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gaohongyu789.top/gtgrelczfp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ehwqpu.com/gttkpbdtbl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.tanke756.top/gtyshprrsv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sysykeji.top/gtycrgkzxv.html

[N05] 最大公约数
来源：http://hz.tianlin.xyz/gtonihhstw.html

Py:   math.gcd(a, b)
来源：http://hz.shanyushiyangtech.top/gtmhburslq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hnqzz.top/gtvyqwaypg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj20258.top/gthlramzwo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigufen.top/gtspjzkhvl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hnxiangtu.top/gtoklvmiuh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.wangshuangyany.cn/gtxypauqyh.html

Ruby: a.gcd(b)
来源：http://hz.yueranfly.top/gtkorvhlat.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yuxming.cn/gtciozfuxy.html

[N06] 判断回文字符串
来源：http://hz.zhiwuduotai.top/gtnvqjydtk.html

Py:   s == s[::-1]
来源：http://hz.aibaodan.cn/gthemhxbhj.html

PHP:  $s === strrev($s);
来源：http://hz.jinqigufen.top/gtpfhdbvnk.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhiwuduotai.top/gtgkgxciss.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gthxiwgtyi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yj20258888.top/gtwwylppac.html

Go:   // 双指针从两端比较
来源：http://hz.hfpthk.cn/gtjszkscim.html

Ruby: s == s.reverse
来源：http://hz.ydzc1.top/gtkmrtbhna.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cucudq.cn/gtqkpanolo.html

[N07] 两数之和（返回下标）
来源：http://hz.jiagoushi.top/gtxqouyjxe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nanxinkj.top/gtjzrdvnnj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.kuanghao11.cn/gtdjdqywij.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhixingplan.top/gtxowbfnwp.html

TS:   // 手写 Map<string, number>
来源：http://hz.chenzaomai.com/gttqgsbmpr.html

Java: // 手写 HashMap
来源：http://hz.feifeiyinyue.top/gttlqkcjic.html

Go:   // 手写 map[int]int
来源：http://hz.shanyushiyangtech.top/gtkzwqrfrz.html

Ruby: // 手写 Hash
来源：http://hz.jiagoushi.top/gtnmyuvstz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ivvv.top/gtwburfkjl.html

[N08] 生成全排列
来源：http://hz.daria6918.cn/gtnrvfudyk.html

Py:   itertools.permutations(arr)
来源：http://hz.gogol.net.cn/gtkxkhhfos.html

PHP:  // 手写递归交换
来源：http://hz.gzhubu.top/gtaltrcnps.html

JS:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtcklbnufd.html

TS:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gttnzczvqn.html

Java: // 手写回溯递归
来源：http://hz.fengsongda.top/gteywokdaf.html

Go:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtljfzisqx.html

Ruby: arr.permutation.to_a
来源：http://hz.andypj.xyz/gtnavfperx.html

C#:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtgflbmikh.html

[N09] 栈与队列
来源：http://hz.ybcxt.top/gtysamdntr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhongyouzk.top/gtwuiwpbxi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ydjk.org.cn/gtnenezcsl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.chenlongwang.top/gtzqvfmuqm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.kuanghao11.cn/gtfqyertlp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hnxiangtu.top/gtldqdlxsu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.guowangkeji.top/gteljfnugm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jinghuilouyu.cn/gtetgvqwhm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.guannengcc.top/gtsmqcwmaw.html

[N10] 链表节点定义
来源：http://hz.quarkkingdee.top/gtqwjjicqp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.vqdsnc.cn/gtrbkxpwnd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cqqwz.cn/gtubkioxlu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.vqdsnc.cn/gtfcccfulr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sxryk.cn/gtwfjgfbyj.html

Java: class Node { int v; Node next; }
来源：http://hz.xylfe.cn/gtcwfyyuqa.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ydjk.org.cn/gtpjccjjzl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shangyingyoupin.top/gtvxgfeyay.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.fzhhl.top/gtkluesbhj.html

[N11] 二叉树中序遍历
来源：http://hz.cucudq.cn/gtjfiyyoxd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.vqdsnc.cn/gtrghfcilk.html

PHP:  // 手写递归函数
来源：http://hz.hongshengwenyu.top/gtkxtpadul.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yongpay.top/gtvpdevogm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhiwuduotai.top/gtijunmoev.html

Java: // 手写递归
来源：http://hz.yongpay.top/gtezthpvez.html

Go:   // 手写递归
来源：http://hz.ydjk.org.cn/gtihidekyx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.havefunace.top/gtxmfgqycr.html

C#:   // 手写递归
来源：http://hz.smart0.xyz/gtjtqckhog.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.nwbrower.top/gtcsacpbqr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zdqjudy.top/gtqciojlhd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.feifeiyinyue.top/gtvutmywgg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hongshengwenyu.top/gthlvlhxuo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xinyue.icu/gtcqoqvbfn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.iojbl.cn/gtpntjkwwd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.wangdashe.top/gtwnsdoscy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.chenjidiqi.icu/gtmtoaaxbv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xingfuxueyuan.xyz/gtibvbuxiu.html

================================================================================
来源：http://hz.ybcxt.top/gthztsosdm.html

O. 并发与异步
来源：http://hz.ywan-chungtsiang.top/gtsadclyyq.html

================================================================================
来源：http://hz.ydzc1.top/gttpvepvlv.html

[O01] 启动一个线程
来源：http://hz.feifeiyinyue.top/gtfwyzusyi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.c1oappe.top/gtladognpy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.iojbl.cn/gtztjzjlfe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cashguo.top/gtcxworcbn.html

TS:   // 同 JS
来源：http://hz.jinqigufen.top/gtazbsvgbu.html

Java: new Thread(() -> f()).start()
来源：http://hz.nanxinkj.top/gtdhssrbjk.html

Go:   go f()
来源：http://hz.dashuyun.cn/gtyvzihxao.html

Ruby: Thread.new { f }
来源：http://hz.hysaishi.cn/gtbygrktyf.html

C#:   Task.Run(() => F());
来源：http://hz.nwbrower.top/gtgmhxfenq.html

[O02] 使用线程池
来源：http://hz.zhongyouzk.top/gttulcngfm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jqgfzy.top/gtofjrpomm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nwbrower.top/gtpphodokw.html

JS:   // worker_threads 线程池
来源：http://hz.shzxlz.cn/gtejyumvip.html

TS:   // worker_threads 线程池
来源：http://hz.c1oappe.top/gtmwjtkuvr.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.fengsongda.top/gtzwojdorg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.fengsongda.top/gttcavkdxl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cdnleiting.top/gtxgezepwz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.aibaodan.cn/gtjdepnvjp.html

[O03] 加锁保护共享数据
来源：http://hz.52xcode.cn/gtzlyzwitq.html

Py:   with lock: shared += 1
来源：http://hz.bjfxy.top/gtbfvwooxg.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.dashuyun.cn/gtpkhpszyj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.mhx1999.top/gtwktjwopc.html

TS:   // 同 JS
来源：http://hz.gogol.net.cn/gtlspcsiyp.html

Java: synchronized (this) { shared++; }
来源：http://hz.ybcxt.top/gtephlwihd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xylfe.cn/gtimxsjhxe.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jianghu66.top/gtkzzvkviq.html

C#:   lock (gate) { shared++; }
来源：http://hz.cqqwz.cn/gtikmhwbkg.html

[O04] 定义异步函数并等待
来源：http://hz.ydjk.org.cn/gtacdlbcri.html

Py:   async def f():⏎    await g()
来源：http://hz.quarkkingdee.top/gtproocugh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sxryk.cn/gtrrjuwvdr.html

JS:   async function f() { await g(); }
来源：http://hz.cdnleiting.top/gtapobghpi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhengqikj.top/gtdatftkuu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gotoacloud.top/gtijgjmhbh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.gzhubu.top/gterxadqns.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yj20258888.top/gtswukngdj.html

C#:   async Task F() { await G(); }
来源：http://hz.nanxuanxn.top/gtdwelvxwr.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhongyouzk.top/gtpjpiivyt.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhaomingkeji.xyz/gtqrmhmkcv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.guannengcc.top/gtlrecagoj.html

JS:   await Promise.all(tasks)
来源：http://hz.tianlin.xyz/gtgfqgmbxe.html

TS:   await Promise.all(tasks)
来源：http://hz.nwbrower.top/gttkcitkvs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.dashuyun.cn/gtbgnpxywv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.gotoacloud.top/gteptrrmhj.html

Ruby: threads.map(&:join)
来源：http://hz.cashguo.top/gtndbkmxfv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.tian-w.cn/gtjzpgionj.html

[O06] 使用进程池
来源：http://hz.yuxming.cn/gtsmnhhhlb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ehwqpu.com/gtcgajgxti.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.daxiang520.top/gtgnxbnxxb.html

JS:   // child_process / cluster 模块
来源：http://hz.xinyue.icu/gtyvcffgdw.html

TS:   // child_process / cluster 模块
来源：http://hz.sweek.top/gtkfaysnuk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.mhx1999.top/gtchvivwas.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yuanzhike.top/gteqhekyfa.html

Ruby: // fork 块
来源：http://hz.nanxinkj.top/gtklbrqkce.html

C#:   Parallel.For
来源：http://hz.ybcxt.top/gtrsyxsqxh.html

================================================================================
来源：http://hz.gzhubu.top/gtgmkuzrnd.html

P. 常用工具函数
来源：http://hz.hammf.cn/gtekoeaeph.html

================================================================================
来源：http://hz.kuanghao11.cn/gtyihiglbx.html

[P01] 生成 UUID
来源：http://hz.ywan-chungtsiang.top/gtgxdjladx.html

Py:   str(uuid.uuid4())
来源：http://hz.cqqwz.cn/gtajiuodgk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhixingplan.top/gtbyptoosh.html

JS:   crypto.randomUUID()
来源：http://hz.jinqigufen.top/gtltogqawk.html

TS:   crypto.randomUUID()
来源：http://hz.redwolf501.top/gtmarxfgdt.html

Java: UUID.randomUUID().toString()
来源：http://hz.meibo888.top/gtxyluoiwc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ehwqpu.com/gtrbdykiwj.html

Ruby: SecureRandom.uuid
来源：http://hz.hongshengwenyu.top/gtudnnktxi.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.gotoacloud.top/gtcfwpnxix.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jqgufenzy.top/gtiftkpqvr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.mhx1999.top/gtddqdxjch.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yj20258.top/gtefhlpetw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yvedp.cn/gtjfhdwssf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.dashuyun.cn/gtzintknyo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.wangdashe.top/gtegmnzvac.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.guannengcc.top/gtqbyjesrt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.mhx1999.top/gtwzfquzlm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shanyushiyangkeji.top/gtgctcrulz.html

[P03] 生成短随机字符串
来源：http://hz.shanyushiyangtech.top/gtiqpuvasv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.aibaodan.cn/gtynwzcuuo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xuetiantiany.cn/gthurnpkdc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhongyouzk.top/gtypeaipmv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shangyingyoupin.top/gtqvxowntr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yj20258.top/gtibdyoucy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.snrcjt.cn/gtdbmbotjx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhoulong.xyz/gtccfqolyv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.iojbl.cn/gtfctfaypt.html

[P04] 求长度
来源：http://hz.yj20258888.top/gtmoftipmq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ehwqpu.com/gtztdfbvfd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.vqdsnc.cn/gtrfsibjig.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yanxiufei.cn/gttppzoyxy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yangfankeji.com/gtopebaooi.html

Java: list.size();  map.size();  s.length()
来源：http://hz.svipenyu.cn/gthkkexejd.html

Go:   len(arr);  len(m)
来源：http://hz.ppjwa.cn/gtsuifdqms.html

Ruby: x.length;  x.size
来源：http://hz.yvedp.cn/gtgqswbywe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.haohaochexian.top/gtezjmicdu.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yj20258.top/gtwpljyuox.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.kuanghao11.cn/gtcgcbtbis.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.smart0.xyz/gttkubpncy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shanyushiyangtech.top/gthbedgasd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.feifeiyinyue.top/gtokrujzly.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.bjfxy.top/gtzeyafnsx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhaomingkeji.xyz/gttsasehgs.html

Ruby: a == b
来源：http://hz.mhx1999.top/gtolofogsh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shanyushiyangtech.top/gtpnxteidv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.havefunace.top/gteqyvvydx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.gzhubu.top/gtqlywlbkq.html

PHP:  if (empty($x)) {}
来源：http://hz.yuxming.cn/gtjdhpcrgt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.wangshuangyany.cn/gthrjwuxpa.html

TS:   if (x == null) {}
来源：http://hz.gzhubu.top/gtphvoydhx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.iojbl.cn/gtesopqfvd.html

Go:   if x == nil {}
来源：http://hz.hywenlv.cn/gtonfvylev.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.gaohongyu789.top/gtdsfobcog.html

C#:   if (x is null) {}
来源：http://hz.zhongyouzk.top/gtzssqvabp.html

[P07] 防抖与节流
来源：http://hz.xylfe.cn/gtyqzuvnbb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jlsjyb.cn/gtfsdcfvbq.html

PHP:  // 手写时间戳比较
来源：http://hz.zdqjudy.top/gtttdyhycg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhongyouzk.top/gtqjbafgfh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuanzx.com/gtcdljonqn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jiagoushi.top/gtfhevuiky.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ehwqpu.com/gtobdvctdk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hnxiangtu.top/gtlajdplie.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.fengsongda.top/gtzvoqzfxo.html

[P08] 处理浮点精度问题
来源：http://hz.jinqigfzy.top/gtnskhwuhf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hysaishi.cn/gtpdpyuvun.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.iojbl.cn/gtjnbhqkls.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cheryme.top/gtwlurclnx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhijiandao.cn/gtdbnermxr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cdnleiting.top/gthkxzqjja.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj202588.top/gtfrsspnzt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.kuanghao11.cn/gtwkzzpehy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shangyingyoupin.top/gthrstkoxv.html

================================================================================
来源：http://hz.vqdsnc.cn/gtzqabexeo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.aizwys.cn/gtaokncaim.html

================================================================================
来源：http://hz.zhijiandao.cn/gthcekywud.html

[Q01] 创建表
来源：http://hz.jqgfzy.top/gtonamlwgi.html

CREATE TABLE users (
来源：http://hz.daria6918.cn/gtxucsqglx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hywenlv.cn/gthkdgsczi.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xinyue.icu/gthdnhezyp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xingfuxueyuan.xyz/gtxjroprfr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.0kj1m.cn/gtrovawdxh.html

);
来源：http://hz.zdqjudy.top/gtpktjgexj.html

[Q02] 创建带外键的表
来源：http://hz.redwolf501.top/gtufufkhlx.html

CREATE TABLE orders (
来源：http://hz.yj20258888.top/gtxxjzmmod.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258.top/gtpreuwehk.html

user_id INT NOT NULL,
来源：http://hz.ivvv.top/gtkrawxgxy.html

amount DECIMAL(10, 2),
来源：http://hz.jinghuilouyu.cn/gtmtnyuguo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ybcxt.top/gtbsxsxzgc.html

);
来源：http://hz.havefunace.top/gtcwexgwgk.html

[Q03] 增加列
来源：http://hz.yj202588.top/gtumuuhmna.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cheryme.top/gtwwjhyvir.html

[Q04] 修改列类型
来源：http://hz.quarkkingdee.top/gtcvjqdywl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.havefunace.top/gtsdvzrkwd.html

[Q05] 重命名列
来源：http://hz.jinqigfzy.top/gtijiykjqt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.0kj1m.cn/gtmemafcmh.html

[Q06] 删除列
来源：http://hz.wangshuangyany.cn/gtuumizooz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.meibo888.top/gtdjozecvd.html

[Q07] 删除表
来源：http://hz.hfpthk.cn/gtvobilafc.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gogol.net.cn/gtcukyhmgj.html

[Q08] 创建普通索引
来源：http://hz.shzxlz.cn/gtvbwdmwrf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shangyingyoupin.top/gtcsxxmlsx.html

[Q09] 创建唯一索引
来源：http://hz.mhx1999.top/gtvuqkbgkw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jinqigufen.top/gtxdllyoxt.html

[Q10] 插入单行
来源：http://hz.yj20258.top/gthsygqocl.html


<!-- 参考信息 -->