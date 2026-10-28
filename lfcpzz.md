代发 wailian999

Py:   if __name__ == "__main__":
来源：http://hz.gotoacloud.top/gtcbjpwnis.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yj20258888.top/gtmymwwexg.html

JS:   require.main === module
来源：http://hz.yueranfly.top/gtshdbdmsn.html

TS:   require.main === module
来源：http://hz.jlsjyb.cn/gtodawmaus.html

Java: public static void main(String[] args)
来源：http://hz.hywenlv.cn/gturgaqrpr.html

Go:   func main()
来源：http://hz.yonumen.top/gtzggcwjvv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.andypj.xyz/gtdhhwcoce.html

C#:   static void Main(string[] args)
来源：http://hz.pengpengdd.cyou/gtcdrmchse.html

[M08] 获取系统与运行时信息
来源：http://hz.hnqzz.top/gtojgzflyp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yj202588.top/gtrjscxdqc.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gaohongyu789.top/gtgnkylkdf.html

JS:   process.platform;  process.version
来源：http://hz.shzxlz.cn/gtuzqlzkew.html

TS:   process.platform;  process.version
来源：http://hz.9152youxi.cn/gtxzbvgfgj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.birdmap.top/gteltfilhu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yuanzhike.top/gtoeowogbc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hnxiangtu.top/gticmojtgq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yongpay.top/gtnjqnkyzs.html

================================================================================
来源：http://hz.dianchejie.cn/gtwchrbanf.html

N. 数据结构与算法
来源：http://hz.cdnleiting.top/gtmmwwznpl.html

================================================================================
来源：http://hz.andypj.xyz/gtfjlhpjud.html

[N01] 二分查找（有序数组）
来源：http://hz.kuanghao11.cn/gtnnjrlxvo.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.52xcode.cn/gtjlytozdt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xuanzx.com/gtjpaceuyi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yanxiufei.cn/gtvihrehvj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jiagoushi.top/gtmcaqvzvv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.daria6918.cn/gtxtkrtagy.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhoulong.xyz/gtqqapukfs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xuetiantiany.cn/gtwiwkcggd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.aibaodan.cn/gtnoucoxti.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.nwbrower.top/gtfuuxniio.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cheryme.top/gtddjgkbqp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tian-w.cn/gtvgefddbs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cucudq.cn/gtdidesoke.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ehwqpu.com/gtadgzjzpf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.0kj1m.cn/gtwohqtowg.html

Go:   slices.Sort(arr)
来源：http://hz.jlsjyb.cn/gtlzwcpgva.html

Ruby: arr.sort
来源：http://hz.316326.xyz/gtqsjpgrtz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ivvv.top/gtlknvtuvo.html

[N03] 快速排序（分治示例）
来源：http://hz.pengpengdd.cyou/gtfdgrzqja.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jiagoushi.top/gttgherkmj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hnqzz.top/gtvtnfcubn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuanzhike.top/gtqsjzzlxa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hfpthk.cn/gtwwdvicng.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xuetiantiany.cn/gtzsvsexbr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhongyouzk.top/gtedphxxgh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.redwolf501.top/gtxdasnxas.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xziqi.cn/gtlnaabycm.html

[N04] 斐波那契数列
来源：http://hz.jiagoushi.top/gtlfouaihb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shzxlz.cn/gtypmmpmes.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinqigfzy.top/gtdzatxvmx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cashguo.top/gtmrpkuyxc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cashguo.top/gtgsyfhujz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gaohongyu789.top/gtrciuhcew.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yuxming.cn/gtqcfrliwe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yuanzhike.top/gtakxppfkp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ehwqpu.com/gtkyjwyuik.html

[N05] 最大公约数
来源：http://hz.dashuyun.cn/gtawiejkur.html

Py:   math.gcd(a, b)
来源：http://hz.meibo888.top/gtfmcsuhkp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.aibaodan.cn/gthhzfrnqk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnxiangtu.top/gtmwcdirsk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenjidiqi.icu/gtzhsblusi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xingfuxueyuan.xyz/gtiiwkedeq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.gaohongyu789.top/gttrjnyjht.html

Ruby: a.gcd(b)
来源：http://hz.chenjidiqi.icu/gtqsjfmfpr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinqigfzy.top/gtatxrhsxs.html

[N06] 判断回文字符串
来源：http://hz.52xcode.cn/gtgcafixhx.html

Py:   s == s[::-1]
来源：http://hz.xingfuxueyuan.xyz/gtmpqqzmwd.html

PHP:  $s === strrev($s);
来源：http://hz.nanxinkj.top/gtndijjwbe.html

JS:   s === [...s].reverse().join("")
来源：http://hz.tian-w.cn/gtixseciea.html

TS:   s === [...s].reverse().join("")
来源：http://hz.nanxinkj.top/gtwabqqhjc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yuanzhike.top/gtmsoaptsr.html

Go:   // 双指针从两端比较
来源：http://hz.meibo888.top/gtoxyxmcju.html

Ruby: s == s.reverse
来源：http://hz.52xcode.cn/gtdwzloelg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhoulong.xyz/gtavvrnqae.html

[N07] 两数之和（返回下标）
来源：http://hz.ivvv.top/gtqluxfamk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xuetiantiany.cn/gtrkeulybv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.chenzaomai.com/gtllqmkvkl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhaomingkeji.xyz/gtdcgzmqto.html

TS:   // 手写 Map<string, number>
来源：http://hz.wangdashe.top/gtugsyshwt.html

Java: // 手写 HashMap
来源：http://hz.snrcjt.cn/gtwiifonpw.html

Go:   // 手写 map[int]int
来源：http://hz.ydzc1.top/gtjdkirswt.html

Ruby: // 手写 Hash
来源：http://hz.sysykeji.top/gtyypxsnjq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.c1oappe.top/gtvazdjtgo.html

[N08] 生成全排列
来源：http://hz.sufxvd.cn/gtrlwgyrri.html

Py:   itertools.permutations(arr)
来源：http://hz.ydjk.org.cn/gtzabezciv.html

PHP:  // 手写递归交换
来源：http://hz.jinyuanbaomall.cn/gtvoubcnbo.html

JS:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtqemtfsbu.html

TS:   // 手写回溯递归
来源：http://hz.ybcxt.top/gtzesrtxnj.html

Java: // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtzpnevezn.html

Go:   // 手写回溯递归
来源：http://hz.yuanzhike.top/gtgzoxybfx.html

Ruby: arr.permutation.to_a
来源：http://hz.xinyue.icu/gtylsrelof.html

C#:   // 手写回溯递归
来源：http://hz.ppjwa.cn/gtnuphuajv.html

[N09] 栈与队列
来源：http://hz.sxryk.cn/gtvcvqpprc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.pengpengdd.cyou/gtvbkvwuju.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cheryme.top/gtwbafmpog.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yangfankeji.com/gtbwdxlplf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xinyue.icu/gtrewqwnlv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.cheryme.top/gttzissstw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yj202588.top/gtdeyxhlxh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhongyouzk.top/gtgqvgxumd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xuetiantiany.cn/gtmuxmwyie.html

[N10] 链表节点定义
来源：http://hz.yj20258.top/gtwqljubuq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.chenjidiqi.icu/gtghrdjbwz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.wangshuangyany.cn/gtajaysdym.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hnxiangtu.top/gtpjfgdjnw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.quarkkingdee.top/gtdaejlnrs.html

Java: class Node { int v; Node next; }
来源：http://hz.chenlongwang.top/gtmnnhhbun.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gotoacloud.top/gtyzxsxnaf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yvedp.cn/gttdamziwo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jiagoushi.top/gtufevddaq.html

[N11] 二叉树中序遍历
来源：http://hz.xuanzx.com/gtyhbujgzu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.bjfxy.top/gtxxwhygbg.html

PHP:  // 手写递归函数
来源：http://hz.shzxlz.cn/gtfavnonsu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.vqdsnc.cn/gttnmvmviv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhaomingkeji.xyz/gtbqlihjbb.html

Java: // 手写递归
来源：http://hz.sufxvd.cn/gtgzapyqwo.html

Go:   // 手写递归
来源：http://hz.pengpengdd.cyou/gtwrcbssnr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yj20258.top/gtfoijcjbq.html

C#:   // 手写递归
来源：http://hz.ydzc1.top/gtprunvqoz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.dashuyun.cn/gtybwxands.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tianlin.xyz/gtpqpoavqu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.guannengcc.top/gthpxnzukc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sufxvd.cn/gttjxichmp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.guannengcc.top/gtqvhlgiju.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shzxlz.cn/gtvgjthdzf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhongyouzk.top/gtcidcxcnb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yuxming.cn/gtncfstqff.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.c1oappe.top/gtrhilhtex.html

================================================================================
来源：http://hz.zhixingplan.top/gtpdukwdte.html

O. 并发与异步
来源：http://hz.zhixingplan.top/gtwqblaoqx.html

================================================================================
来源：http://hz.cdnleiting.top/gtynmprwqg.html

[O01] 启动一个线程
来源：http://hz.jinghuilouyu.cn/gtansmwgob.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jqgufenzy.top/gtstnnglkf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gogol.net.cn/gtpipscvfo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.52xcode.cn/gtgqlyfgzn.html

TS:   // 同 JS
来源：http://hz.sufxvd.cn/gtxgljeppn.html

Java: new Thread(() -> f()).start()
来源：http://hz.jyoumei.cn/gtmbkaknbj.html

Go:   go f()
来源：http://hz.ydzc1.top/gtbtrutewt.html

Ruby: Thread.new { f }
来源：http://hz.9152youxi.cn/gtvlfkxazo.html

C#:   Task.Run(() => F());
来源：http://hz.tianlin.xyz/gtuqeeixwm.html

[O02] 使用线程池
来源：http://hz.jinghuilouyu.cn/gtkeuiaele.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.pengpengdd.cyou/gtmnbuxgio.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jyoumei.cn/gthzwvvihg.html

JS:   // worker_threads 线程池
来源：http://hz.redwolf501.top/gtnyyoxgsd.html

TS:   // worker_threads 线程池
来源：http://hz.316326.xyz/gtshjvhisy.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yangfankeji.com/gtqnjzjciy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.iojbl.cn/gtbbvclspm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhongyouzk.top/gtirnldolw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hnqzz.top/gtsobnjelg.html

[O03] 加锁保护共享数据
来源：http://hz.jinqigufen.top/gtoddtajhk.html

Py:   with lock: shared += 1
来源：http://hz.tianlin.xyz/gtaqfrlbel.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hysaishi.cn/gtbzdtffio.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.guowangkeji.top/gtabgrwjli.html

TS:   // 同 JS
来源：http://hz.aibaodan.cn/gttbbmffhv.html

Java: synchronized (this) { shared++; }
来源：http://hz.xingfuxueyuan.xyz/gthvomgkvh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jqgufenzy.top/gtmryxqmfw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hnqzz.top/gtukomunmb.html

C#:   lock (gate) { shared++; }
来源：http://hz.sweek.top/gtcdnrecqz.html

[O04] 定义异步函数并等待
来源：http://hz.xingfuxueyuan.xyz/gtexomlqkr.html

Py:   async def f():⏎    await g()
来源：http://hz.ywan-chungtsiang.top/gtpjusxirv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.guowangkeji.top/gtgoohiuub.html

JS:   async function f() { await g(); }
来源：http://hz.yvedp.cn/gtlgyelccw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yj202588.top/gtozvzucwq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.tian-w.cn/gtcxuaoavf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ydzc1.top/gtfdyjbake.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.iojbl.cn/gtmlqrtjzj.html

C#:   async Task F() { await G(); }
来源：http://hz.wangshuangyany.cn/gtcpbkupde.html

[O05] 并发执行并等待全部完成
来源：http://hz.cheryme.top/gtcwmquekg.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yj20258888.top/gtbdfjvcdn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yvedp.cn/gtqbzwqyvq.html

JS:   await Promise.all(tasks)
来源：http://hz.sufxvd.cn/gtldestwng.html

TS:   await Promise.all(tasks)
来源：http://hz.jiagoushi.top/gttozgrgxs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xinyue.icu/gtmqycjeri.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.guowangkeji.top/gtadyfpjww.html

Ruby: threads.map(&:join)
来源：http://hz.cucudq.cn/gtkzdhkgzk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jqgufenzy.top/gtanrmslxg.html

[O06] 使用进程池
来源：http://hz.gotoacloud.top/gtbgztgmyr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hammf.cn/gtlfrxvrvz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.quarkkingdee.top/gttwxfiijz.html

JS:   // child_process / cluster 模块
来源：http://hz.dashuyun.cn/gtuztxwdtb.html

TS:   // child_process / cluster 模块
来源：http://hz.jqgfzy.top/gtjsxnkgxg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.9152youxi.cn/gtgrnbejhn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.kuanghao11.cn/gtvtaxdxjc.html

Ruby: // fork 块
来源：http://hz.smart0.xyz/gtfgytpbax.html

C#:   Parallel.For
来源：http://hz.ywan-chungtsiang.top/gtooyxjgnw.html

================================================================================
来源：http://hz.yonumen.top/gtunvvncxx.html

P. 常用工具函数
来源：http://hz.sxryk.cn/gtccblaqag.html

================================================================================
来源：http://hz.cashguo.top/gtassjvedj.html

[P01] 生成 UUID
来源：http://hz.feifeiyinyue.top/gtrfayagvn.html

Py:   str(uuid.uuid4())
来源：http://hz.zycfv.cn/gtbmlibuzz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ivvv.top/gtivormomi.html

JS:   crypto.randomUUID()
来源：http://hz.shangyingyoupin.top/gtewrjqmbt.html

TS:   crypto.randomUUID()
来源：http://hz.sweek.top/gtnfppurvf.html

Java: UUID.randomUUID().toString()
来源：http://hz.yj20258.top/gtqdqhrzft.html

Go:   // 用 github.com/google/uuid
来源：http://hz.c1oappe.top/gtkkhadmyc.html

Ruby: SecureRandom.uuid
来源：http://hz.aibaodan.cn/gteexqtall.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sufxvd.cn/gtcygbjoxq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.snrcjt.cn/gtjsnonyge.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.c1oappe.top/gtkngacepu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhixingplan.top/gtvgvdmyek.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhijiandao.cn/gtbvwxzlfq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.quarkkingdee.top/gttuswjque.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.kuanghao11.cn/gtpnnytqiu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jlsjyb.cn/gtdqrqjbtj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yueranfly.top/gtknxxomtp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cqqwz.cn/gtptdksybn.html

[P03] 生成短随机字符串
来源：http://hz.quarkkingdee.top/gtjvjiuoiv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.daria6918.cn/gtvynblevz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xylfe.cn/gtlfitgeqs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhijiandao.cn/gtgiptoncj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangkeji.top/gtleizwwux.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.mhx1999.top/gtzeswfidw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zdqjudy.top/gtgmdbkzvl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zycfv.cn/gtbevmqpaw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.52xcode.cn/gtmqfzgrwv.html

[P04] 求长度
来源：http://hz.nanxinkj.top/gtzmahzxvq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jianghu66.top/gtvqjypjkm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.0kj1m.cn/gtllylujun.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ywan-chungtsiang.top/gtpaifyeef.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yongpay.top/gtkfishyaz.html

Java: list.size();  map.size();  s.length()
来源：http://hz.havefunace.top/gtlbkvrzwi.html

Go:   len(arr);  len(m)
来源：http://hz.wangshuangyany.cn/gtelnhkffn.html

Ruby: x.length;  x.size
来源：http://hz.ppjwa.cn/gtvfnktwsf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.havefunace.top/gtxtnshgyn.html

[P05] 判断两个对象内容是否相等
来源：http://hz.fzhhl.top/gtcommfgpt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhengqikj.top/gtqdnjhgje.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.52xcode.cn/gtbooobyzm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.cdnleiting.top/gtzpgxydjo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jiagoushi.top/gtgfipasne.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.dianchejie.cn/gtivamqaga.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shanyushiyangtech.top/gticfpjxrw.html

Ruby: a == b
来源：http://hz.zhijiandao.cn/gtxgbornqv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.pycfn.com/gtmnsfjpwd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhiwuduotai.top/gtczhdzias.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.vqdsnc.cn/gtwtftphoj.html

PHP:  if (empty($x)) {}
来源：http://hz.jlsjyb.cn/gtluvatgca.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xziqi.cn/gtjaamjuho.html

TS:   if (x == null) {}
来源：http://hz.dashuyun.cn/gtpflqttuz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.guowangkeji.top/gtxqgbxbhk.html

Go:   if x == nil {}
来源：http://hz.sufxvd.cn/gtrivodvpr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.nanxinkj.top/gtenjgkdxu.html

C#:   if (x is null) {}
来源：http://hz.sufxvd.cn/gticwqisia.html

[P07] 防抖与节流
来源：http://hz.jinqigfzy.top/gtpajapesx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.daria6918.cn/gtqrcufbue.html

PHP:  // 手写时间戳比较
来源：http://hz.hnxiangtu.top/gttrjildmy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangkeji.top/gtgkuolweo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.snrcjt.cn/gtcuafijoq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shzxlz.cn/gtqzntnxxd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.wangshuangyany.cn/gtysqfwgrj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhijiandao.cn/gtqyycmfev.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zdqjudy.top/gtgaijrcbl.html

[P08] 处理浮点精度问题
来源：http://hz.sysykeji.top/gtuxqinnzz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yj202588.top/gteravvaaj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yangfankeji.com/gtkujydsdi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.wangdashe.top/gtvbvovtli.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yanxiufei.cn/gtxcitkvss.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.mhx1999.top/gtahkfjxob.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hammf.cn/gtagyjjrpp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jianghu66.top/gtgxhalxzi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.kuanghao11.cn/gtdixdiugt.html

================================================================================
来源：http://hz.zhijiandao.cn/gtpelesvne.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.chenzaomai.com/gtlnhabmwv.html

================================================================================
来源：http://hz.tianlin.xyz/gtuqqamlxv.html

[Q01] 创建表
来源：http://hz.nanxinkj.top/gtmmzpggei.html

CREATE TABLE users (
来源：http://hz.havefunace.top/gtmqxeunmf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.pycfn.com/gtjenvxxgi.html

name VARCHAR(50) NOT NULL,
来源：http://hz.daria6918.cn/gtvkdqgjnn.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhijiandao.cn/gtvtfkpspw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hysaishi.cn/gtvzbyqbwf.html

);
来源：http://hz.hnxiangtu.top/gtrqjxdiyl.html

[Q02] 创建带外键的表
来源：http://hz.fengsongda.top/gtjejxwxed.html

CREATE TABLE orders (
来源：http://hz.yuanzhike.top/gtrvfupwvt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuanzx.com/gtjquxjoog.html

user_id INT NOT NULL,
来源：http://hz.hongshengwenyu.top/gtyonsfhhg.html

amount DECIMAL(10, 2),
来源：http://hz.yj20258.top/gtpqqcztmn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.9152youxi.cn/gtxgabfpvd.html

);
来源：http://hz.zhoulong.xyz/gtlzygzjll.html

[Q03] 增加列
来源：http://hz.zycfv.cn/gtqmcbulay.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ehwqpu.com/gtrmjvkake.html

[Q04] 修改列类型
来源：http://hz.feifeiyinyue.top/gtsslrooph.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.316326.xyz/gtdfydzicd.html

[Q05] 重命名列
来源：http://hz.birdmap.top/gtcjqcyxzr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ehwqpu.com/gtwbcuiiqz.html

[Q06] 删除列
来源：http://hz.pycfn.com/gtxrmsdhwe.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhiwuduotai.top/gtdamojxuy.html

[Q07] 删除表
来源：http://hz.birdmap.top/gtwaeagbia.html

DROP TABLE IF EXISTS orders;
来源：http://hz.c1oappe.top/gtedeffscc.html

[Q08] 创建普通索引
来源：http://hz.jinghuilouyu.cn/gtlhnqyhqj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.9152youxi.cn/gtbgpnbqul.html

[Q09] 创建唯一索引
来源：http://hz.yongpay.top/gtkgrbwuyv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.smart0.xyz/gtgcktgwus.html

[Q10] 插入单行
来源：http://hz.jinqigfzy.top/gttgdpesnk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ehwqpu.com/gtqncmvtyd.html

[Q11] 一次插入多行
来源：http://hz.pengpengdd.cyou/gtdelpfheu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.0kj1m.cn/gtytautubj.html

[Q12] 插入后取自增 ID
来源：http://hz.guowangkeji.top/gtniluobar.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.52xcode.cn/gtashlaeck.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.birdmap.top/gtcadouabx.html

[Q13] 忽略重复插入
来源：http://hz.snrcjt.cn/gtfhdtqrze.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hywenlv.cn/gtgrkvrvtd.html


<!-- 参考信息 -->