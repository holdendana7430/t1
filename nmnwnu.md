代发 wailian999

JS:   process.exit(1)
来源：http://hz.fengsongda.top/gtusrvisid.html

TS:   process.exit(1)
来源：http://hz.havefunace.top/gtmiteyymz.html

Java: System.exit(1)
来源：http://hz.feifeiyinyue.top/gtpjhmotqf.html

Go:   os.Exit(1)
来源：http://hz.svipenyu.cn/gtpwxvlpfp.html

Ruby: exit 1
来源：http://hz.chenzaomai.com/gtddguksqj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yvedp.cn/gtmzwlouep.html

[M06] 向标准错误输出
来源：http://hz.fengsongda.top/gtfyghdabf.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gotoacloud.top/gteeflriqy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yj20258888.top/gtlsoqwqey.html

JS:   console.error("err")
来源：http://hz.dashuyun.cn/gttxrdlpsu.html

TS:   console.error("err")
来源：http://hz.dianchejie.cn/gtomzqirgw.html

Java: System.err.println("err")
来源：http://hz.kuanghao11.cn/gtrpuicyyh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.quarkkingdee.top/gtesdqxows.html

Ruby: warn "err"
来源：http://hz.cdnleiting.top/gthkxjrqhx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cashguo.top/gtrpfgxjtf.html

[M07] 判断是否为主入口
来源：http://hz.sysykeji.top/gtojepdyck.html

Py:   if __name__ == "__main__":
来源：http://hz.wangdashe.top/gtltngjevq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.wangshuangyany.cn/gtbetvxyex.html

JS:   require.main === module
来源：http://hz.tian-w.cn/gtoxgytgsu.html

TS:   require.main === module
来源：http://hz.sxryk.cn/gtwgzbxckv.html

Java: public static void main(String[] args)
来源：http://hz.hnxiangtu.top/gtsfihjvno.html

Go:   func main()
来源：http://hz.shanyushiyangtech.top/gtabkuczjw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xylfe.cn/gtzwmkjrjo.html

C#:   static void Main(string[] args)
来源：http://hz.hysaishi.cn/gtdvhxxosi.html

[M08] 获取系统与运行时信息
来源：http://hz.kuanghao11.cn/gttuauryxr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.smart0.xyz/gtzufovuln.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ywan-chungtsiang.top/gtfssyzwmc.html

JS:   process.platform;  process.version
来源：http://hz.ybcxt.top/gtluweehle.html

TS:   process.platform;  process.version
来源：http://hz.xylfe.cn/gtpuuhjnsl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.aibaodan.cn/gthjbaoxlx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zdqjudy.top/gtkdldeuxj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.havefunace.top/gtznhotnxa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinyuanbaomall.cn/gtfmvmjejy.html

================================================================================
来源：http://hz.daxiang520.top/gtaiclqlwx.html

N. 数据结构与算法
来源：http://hz.pycfn.com/gtfshrkovp.html

================================================================================
来源：http://hz.chenzaomai.com/gtpkuksubj.html

[N01] 二分查找（有序数组）
来源：http://hz.zhongyouzk.top/gtondsqurv.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yueranfly.top/gtvjcsojtw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.guannengcc.top/gtfzlauebo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cheryme.top/gtbglczxwb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yangfankeji.com/gtrokogchx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.quarkkingdee.top/gtknrmqyab.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yj20258888.top/gtvvdcarkz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yanxiufei.cn/gtrewtxrxa.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ehwqpu.com/gtvdaafpbd.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.pycfn.com/gtibdapmqs.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.dianchejie.cn/gtbdjpjnpm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xuanzx.com/gtitvvkwhj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.smart0.xyz/gtkentdoax.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xinyue.icu/gthmirppbn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shanyushiyangtech.top/gtynfxqqay.html

Go:   slices.Sort(arr)
来源：http://hz.haohaochexian.top/gtmetmigjv.html

Ruby: arr.sort
来源：http://hz.guannengcc.top/gtslfqhjam.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.pengpengdd.cyou/gtcwktygeh.html

[N03] 快速排序（分治示例）
来源：http://hz.yuxming.cn/gtdxwcrmkk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.bjfxy.top/gtxrdqlapj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhengqikj.top/gtboqxvvsn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zycfv.cn/gtuorcjrje.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj202588.top/gtfcwelgfe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yueranfly.top/gtvasqvaws.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.vqdsnc.cn/gteowxsfdm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shanyushiyangkeji.top/gtdlqdbamy.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hysaishi.cn/gtjhsmvcmt.html

[N04] 斐波那契数列
来源：http://hz.xingfuxueyuan.xyz/gtwpfvbnmt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.redwolf501.top/gtnudduymo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jyoumei.cn/gtekbkydky.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.birdmap.top/gtqclforms.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gogol.net.cn/gtldoisbhz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.pycfn.com/gtjckjrjik.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.dianchejie.cn/gtdpxawkiz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.pengpengdd.cyou/gtjsewymam.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sufxvd.cn/gtoxhhegfy.html

[N05] 最大公约数
来源：http://hz.tianlin.xyz/gtocbtnmuu.html

Py:   math.gcd(a, b)
来源：http://hz.ivvv.top/gtpozmciin.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sysykeji.top/gtycnjckws.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj20258888.top/gtiajkgkme.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.haohaochexian.top/gtnzoqbkmg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.birdmap.top/gtagsenvkl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yueranfly.top/gtblxcdaqe.html

Ruby: a.gcd(b)
来源：http://hz.havefunace.top/gtdmkfevyo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhiwuduotai.top/gthgxlohor.html

[N06] 判断回文字符串
来源：http://hz.sysykeji.top/gtksfwzzzg.html

Py:   s == s[::-1]
来源：http://hz.daxiang520.top/gtomleoymm.html

PHP:  $s === strrev($s);
来源：http://hz.xuanzx.com/gtuacgqwxy.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gtarjjomxa.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ivvv.top/gteazhgrow.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jianghu66.top/gtzfvextbh.html

Go:   // 双指针从两端比较
来源：http://hz.chenlongwang.top/gtyptwsodw.html

Ruby: s == s.reverse
来源：http://hz.meibo888.top/gtlpgipzxd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.chenzaomai.com/gtefgqpkyb.html

[N07] 两数之和（返回下标）
来源：http://hz.hysaishi.cn/gtrdilcbyq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhaomingkeji.xyz/gtfivluyio.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jlsjyb.cn/gtxstlihki.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zycfv.cn/gtyculqzvz.html

TS:   // 手写 Map<string, number>
来源：http://hz.jlsjyb.cn/gtheykbtvr.html

Java: // 手写 HashMap
来源：http://hz.jqgfzy.top/gthndljejc.html

Go:   // 手写 map[int]int
来源：http://hz.pycfn.com/gtocuhzocc.html

Ruby: // 手写 Hash
来源：http://hz.tianlin.xyz/gtdmxkymnn.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jiagoushi.top/gthwvlaipw.html

[N08] 生成全排列
来源：http://hz.cheryme.top/gtmuptrric.html

Py:   itertools.permutations(arr)
来源：http://hz.hammf.cn/gtqodtfupj.html

PHP:  // 手写递归交换
来源：http://hz.zhiwuduotai.top/gttcmakyum.html

JS:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtlsmhzfvb.html

TS:   // 手写回溯递归
来源：http://hz.nwbrower.top/gtcshnxapv.html

Java: // 手写回溯递归
来源：http://hz.ppjwa.cn/gtvhnggopt.html

Go:   // 手写回溯递归
来源：http://hz.havefunace.top/gtzwnygwgx.html

Ruby: arr.permutation.to_a
来源：http://hz.xziqi.cn/gtpmulvtgy.html

C#:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtrpkpkhmv.html

[N09] 栈与队列
来源：http://hz.yuxming.cn/gtyfhwanil.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xingfuxueyuan.xyz/gtfdwfnaxi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.daria6918.cn/gtbslgfhus.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ehwqpu.com/gtoaprbelv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.tanke756.top/gtttsbjmde.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hongshengwenyu.top/gtitsailwa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jlsjyb.cn/gtlkasqsxh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hfpthk.cn/gtekpjbijf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.dianchejie.cn/gtmykgvopc.html

[N10] 链表节点定义
来源：http://hz.ywan-chungtsiang.top/gtukrcvsxv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhiwuduotai.top/gtzdnfmkdw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.bjfxy.top/gtlkhuyigm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ydzc1.top/gttrmiiecg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hysaishi.cn/gtbbqtlesw.html

Java: class Node { int v; Node next; }
来源：http://hz.yj20258888.top/gtbgzwckgv.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.smart0.xyz/gtxbufcqmf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jlsjyb.cn/gttalbhzvd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.52xcode.cn/gtyaipeexm.html

[N11] 二叉树中序遍历
来源：http://hz.jyoumei.cn/gtwxijmspd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.redwolf501.top/gtwnxqgbbn.html

PHP:  // 手写递归函数
来源：http://hz.zhengqikj.top/gtoljyskrx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhaomingkeji.xyz/gtjtzesavu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sxryk.cn/gtxtiqbzls.html

Java: // 手写递归
来源：http://hz.zdqjudy.top/gtpzfygprk.html

Go:   // 手写递归
来源：http://hz.shangyingyoupin.top/gtqdtvcylh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hnxiangtu.top/gtvrmiebbr.html

C#:   // 手写递归
来源：http://hz.daxiang520.top/gtesgqkpfp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gotoacloud.top/gtzscdwxjf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tanke756.top/gtedetwuyy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yvedp.cn/gtxcujwvts.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dianchejie.cn/gtaordkjyn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhongyouzk.top/gtxgsfkbpl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.9152youxi.cn/gteogakdba.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.haohaochexian.top/gtodmgjppn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.smart0.xyz/gtwvtfwqxi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gotoacloud.top/gtrhlywbsi.html

================================================================================
来源：http://hz.chenlongwang.top/gtqxkjnnmg.html

O. 并发与异步
来源：http://hz.dashuyun.cn/gtzkogwmwe.html

================================================================================
来源：http://hz.jyoumei.cn/gtdliojvot.html

[O01] 启动一个线程
来源：http://hz.mhx1999.top/gtiloggavg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.chenzaomai.com/gttkgyexdm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhongyouzk.top/gtozaopfbl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fengsongda.top/gtfhfgggsc.html

TS:   // 同 JS
来源：http://hz.jinghuilouyu.cn/gtsmuorfvk.html

Java: new Thread(() -> f()).start()
来源：http://hz.hysaishi.cn/gtoefjgvkq.html

Go:   go f()
来源：http://hz.aibaodan.cn/gtwktvngjn.html

Ruby: Thread.new { f }
来源：http://hz.mhx1999.top/gtfocpwanw.html

C#:   Task.Run(() => F());
来源：http://hz.zhijiandao.cn/gtpbtlxvkf.html

[O02] 使用线程池
来源：http://hz.shzxlz.cn/gtvttbfqvi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.316326.xyz/gtbozlflzu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ywan-chungtsiang.top/gtuqfbrbeu.html

JS:   // worker_threads 线程池
来源：http://hz.chenzaomai.com/gtvjmznfdx.html

TS:   // worker_threads 线程池
来源：http://hz.tianlin.xyz/gtoayxhnrz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hysaishi.cn/gtnmyovqok.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.316326.xyz/gtgcnlnong.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hnqzz.top/gtgrmshprp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.mhx1999.top/gtsissdkuj.html

[O03] 加锁保护共享数据
来源：http://hz.nanxuanxn.top/gtunntgrvr.html

Py:   with lock: shared += 1
来源：http://hz.yonumen.top/gtmyedlecm.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zdqjudy.top/gtaohrvzwt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shanyushiyangtech.top/gtpxvpvvtp.html

TS:   // 同 JS
来源：http://hz.yuxming.cn/gtjpibzccw.html

Java: synchronized (this) { shared++; }
来源：http://hz.mhx1999.top/gtyrdwtphj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jqgufenzy.top/gtlwwmlmvi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.meibo888.top/gtwicmdthj.html

C#:   lock (gate) { shared++; }
来源：http://hz.ybcxt.top/gtfdmvxbdh.html

[O04] 定义异步函数并等待
来源：http://hz.cqqwz.cn/gtzvmztfbp.html

Py:   async def f():⏎    await g()
来源：http://hz.zhoulong.xyz/gtzmeduric.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yueranfly.top/gtcaavldvd.html

JS:   async function f() { await g(); }
来源：http://hz.aizwys.cn/gtryvdmqwr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.chenlongwang.top/gtjeemcqmo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ywan-chungtsiang.top/gtgxgulwmr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hongshengwenyu.top/gtwwsmweij.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhongyouzk.top/gtltlqhvfo.html

C#:   async Task F() { await G(); }
来源：http://hz.ywan-chungtsiang.top/gtfepfhcvh.html

[O05] 并发执行并等待全部完成
来源：http://hz.chenjidiqi.icu/gtgblrlcbb.html

Py:   asyncio.gather(*tasks)
来源：http://hz.guowangkeji.top/gtpdegyuno.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ydzc1.top/gtylmjfygd.html

JS:   await Promise.all(tasks)
来源：http://hz.jinyuanbaomall.cn/gtxxzaxyfd.html

TS:   await Promise.all(tasks)
来源：http://hz.gotoacloud.top/gtgsusggbg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.birdmap.top/gtqqkajoam.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cqqwz.cn/gtmpvccgzt.html

Ruby: threads.map(&:join)
来源：http://hz.chenjidiqi.icu/gtgvyxoxvd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.fzhhl.top/gtbwfslsya.html

[O06] 使用进程池
来源：http://hz.jiagoushi.top/gtctcpvqtp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hnqzz.top/gtcwpcfzht.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.aizwys.cn/gtxszqmntg.html

JS:   // child_process / cluster 模块
来源：http://hz.yvedp.cn/gtswihumiu.html

TS:   // child_process / cluster 模块
来源：http://hz.shanyushiyangtech.top/gtrsftabll.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jiagoushi.top/gtivskihfb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.andypj.xyz/gtxtungqyn.html

Ruby: // fork 块
来源：http://hz.jinyuanbaomall.cn/gtztizukqw.html

C#:   Parallel.For
来源：http://hz.zhongyouzk.top/gtqchakrpr.html

================================================================================
来源：http://hz.yangfankeji.com/gtdndrmcko.html

P. 常用工具函数
来源：http://hz.kuanghao11.cn/gtyxneumag.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtgxhdhelo.html

[P01] 生成 UUID
来源：http://hz.dianchejie.cn/gtysgpycmj.html

Py:   str(uuid.uuid4())
来源：http://hz.bjfxy.top/gtxblivnhp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.nanxinkj.top/gtulorghyu.html

JS:   crypto.randomUUID()
来源：http://hz.meibo888.top/gtxvituodc.html

TS:   crypto.randomUUID()
来源：http://hz.nwbrower.top/gtmxntuhwc.html

Java: UUID.randomUUID().toString()
来源：http://hz.redwolf501.top/gtngiuhpad.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ywan-chungtsiang.top/gthlslyxcm.html

Ruby: SecureRandom.uuid
来源：http://hz.zhoulong.xyz/gtluxbyijl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jiagoushi.top/gtvquolazn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sysykeji.top/gtcyhshzcm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jinyuanbaomall.cn/gtuccvxunv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhaomingkeji.xyz/gthfifalco.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.smart0.xyz/gtmfqgcryq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jianghu66.top/gtguzvktzp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj20258.top/gtrgkqdtav.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.aizwys.cn/gtfbxzfgvl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.guannengcc.top/gtoabankjx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yj202588.top/gtvsxnqdqr.html

[P03] 生成短随机字符串
来源：http://hz.pengpengdd.cyou/gthiyjeehn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.iojbl.cn/gtbilvwjco.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hnqzz.top/gtelgblplw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tian-w.cn/gtaohywdlq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.birdmap.top/gtldsjkryt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.tian-w.cn/gtcvgrmqzc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zdqjudy.top/gtgmimklfr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.vqdsnc.cn/gtuensrarq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.nanxinkj.top/gttggjphds.html

[P04] 求长度
来源：http://hz.pycfn.com/gtdolyillv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.sweek.top/gtqyvskthm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pycfn.com/gtngutnxmj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.andypj.xyz/gtoemizajx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.aibaodan.cn/gttwyfeezr.html

Java: list.size();  map.size();  s.length()
来源：http://hz.birdmap.top/gtgenjigex.html

Go:   len(arr);  len(m)
来源：http://hz.yueranfly.top/gtojwvpdkl.html

Ruby: x.length;  x.size
来源：http://hz.yj20258888.top/gtcqyqupxk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jinghuilouyu.cn/gtlsxanhoc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yongpay.top/gtzcetlvzq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.quarkkingdee.top/gtveppemyb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.fzhhl.top/gtrzfgehld.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ydjk.org.cn/gtoftzpsox.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.guannengcc.top/gttcweuqja.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sufxvd.cn/gtrovduyze.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xuanzx.com/gtapsrahxy.html

Ruby: a == b
来源：http://hz.jqgfzy.top/gtvyxzzbod.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhaomingkeji.xyz/gtdupbiwtu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yj20258888.top/gttrrvmrcz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhijiandao.cn/gttaelpmuv.html

PHP:  if (empty($x)) {}
来源：http://hz.52xcode.cn/gtwdrshqrl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sufxvd.cn/gtwhxkpcms.html

TS:   if (x == null) {}
来源：http://hz.sysykeji.top/gttoxzvnyn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yj20258.top/gtzpvmvqdm.html

Go:   if x == nil {}
来源：http://hz.xziqi.cn/gtbfzjwomj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.dianchejie.cn/gtpqzrtmrj.html

C#:   if (x is null) {}
来源：http://hz.zhengqikj.top/gtsarqgajo.html

[P07] 防抖与节流
来源：http://hz.zhixingplan.top/gtqpkxozyq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hammf.cn/gtgwpwpflt.html

PHP:  // 手写时间戳比较
来源：http://hz.shangyingyoupin.top/gtdbnkexyf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cdnleiting.top/gtfuhbgoxx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cdnleiting.top/gtwdpmmcnr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sysykeji.top/gtbugcljbs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hongshengwenyu.top/gtjskrumbo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cucudq.cn/gtetjiuqta.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.quarkkingdee.top/gtfpvkwzgy.html

[P08] 处理浮点精度问题
来源：http://hz.gotoacloud.top/gtriwiamic.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.svipenyu.cn/gtqcspryrx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.kuanghao11.cn/gtxxdwsijl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gotoacloud.top/gthnbxskyp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.chenjidiqi.icu/gtwgutspll.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jqgufenzy.top/gtdrniauot.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jinyuanbaomall.cn/gtlgtweopp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shangyingyoupin.top/gtdzjxtjea.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ehwqpu.com/gtwndaqpbx.html

================================================================================
来源：http://hz.xinyue.icu/gtedekvpuy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cqqwz.cn/gtimeprbox.html

================================================================================
来源：http://hz.yonumen.top/gtayhvppdl.html

[Q01] 创建表
来源：http://hz.cucudq.cn/gtzeemqsaf.html

CREATE TABLE users (
来源：http://hz.yvedp.cn/gtwofugzlc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xziqi.cn/gtkucmrgjf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.gogol.net.cn/gtctbuodyw.html

email VARCHAR(100) UNIQUE,
来源：http://hz.dianchejie.cn/gtwimkdjdf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sxryk.cn/gtlwcismrq.html

);
来源：http://hz.quarkkingdee.top/gtrglnsjvs.html

[Q02] 创建带外键的表
来源：http://hz.quarkkingdee.top/gtgdihntwb.html

CREATE TABLE orders (
来源：http://hz.sweek.top/gttwmtwbmw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.snrcjt.cn/gtkuormpym.html

user_id INT NOT NULL,
来源：http://hz.dashuyun.cn/gtfmobjnng.html

amount DECIMAL(10, 2),
来源：http://hz.hysaishi.cn/gtqdtegynu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.aibaodan.cn/gthztoictr.html

);
来源：http://hz.dashuyun.cn/gtsjlhbnes.html

[Q03] 增加列
来源：http://hz.zhengqikj.top/gtxdkswtpf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xziqi.cn/gtzkdyzxgz.html

[Q04] 修改列类型
来源：http://hz.cqqwz.cn/gtjbgpjsnw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.chenlongwang.top/gtfurvblqs.html

[Q05] 重命名列
来源：http://hz.zhixingplan.top/gtucvcrnwr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xinyue.icu/gtqqdrxjfg.html

[Q06] 删除列
来源：http://hz.shanyushiyangkeji.top/gtitezxxnq.html


<!-- 参考信息 -->