代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.bjfxy.top/gtjthnzbei.html

Ruby: warn "err"
来源：http://hz.cashguo.top/gtkvzpwqfa.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yanxiufei.cn/gthxnvmeps.html

[M07] 判断是否为主入口
来源：http://hz.daxiang520.top/gtprugdohz.html

Py:   if __name__ == "__main__":
来源：http://hz.pengpengdd.cyou/gtodbecvyz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ydzc1.top/gtmjuembqc.html

JS:   require.main === module
来源：http://hz.birdmap.top/gtquwmounk.html

TS:   require.main === module
来源：http://hz.shuidangran.top/gtulfwsswy.html

Java: public static void main(String[] args)
来源：http://hz.zhaomingkeji.xyz/gtyfroinuq.html

Go:   func main()
来源：http://hz.snrcjt.cn/gthmgwfoig.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.c1oappe.top/gtvxmbccpt.html

C#:   static void Main(string[] args)
来源：http://hz.cheryme.top/gtkklkheim.html

[M08] 获取系统与运行时信息
来源：http://hz.daxiang520.top/gtfsyzjfpn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ydzc1.top/gtpifcggai.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.kuanghao11.cn/gthljqrqaz.html

JS:   process.platform;  process.version
来源：http://hz.birdmap.top/gtxwxhhlqc.html

TS:   process.platform;  process.version
来源：http://hz.hammf.cn/gtfnqoezbf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sysykeji.top/gtcrdisdyn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zycfv.cn/gtcpxnqtyc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhoulong.xyz/gtixjbylaz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.redwolf501.top/gtttqftvak.html

================================================================================
来源：http://hz.fzhhl.top/gtntwjhigl.html

N. 数据结构与算法
来源：http://hz.ehwqpu.com/gtzvhbykec.html

================================================================================
来源：http://hz.chenlongwang.top/gtfzugbqyy.html

[N01] 二分查找（有序数组）
来源：http://hz.ywan-chungtsiang.top/gtfnxoaiol.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sysykeji.top/gtpuahoubr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhiwuduotai.top/gtrdcoxdpq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yangfankeji.com/gtmsfmmufn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.0kj1m.cn/gtlznmtjce.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jinghuilouyu.cn/gtezokyqls.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ydjk.org.cn/gtfxalxdkt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jlsjyb.cn/gtwfaxtncm.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtfdnxhdbp.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.sweek.top/gtjxbfzpra.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ivvv.top/gtgmneafvs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cucudq.cn/gtsocvmpfo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hysaishi.cn/gtltylkrrw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xylfe.cn/gtdpsylimg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.daxiang520.top/gtjzqwrvmo.html

Go:   slices.Sort(arr)
来源：http://hz.yangfankeji.com/gtsmjsicsh.html

Ruby: arr.sort
来源：http://hz.havefunace.top/gtyhiyoleo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinqigfzy.top/gthbhwycur.html

[N03] 快速排序（分治示例）
来源：http://hz.xuanzx.com/gthuojkhrj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.pengpengdd.cyou/gtkipsnnjt.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ywan-chungtsiang.top/gtncbxtlih.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sxryk.cn/gtycdzdvqy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhengqikj.top/gtslrouxic.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cqqwz.cn/gtqqytkwyi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.andypj.xyz/gtjbhfpuhj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.aizwys.cn/gtdzowemtl.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xziqi.cn/gtnsarsyzv.html

[N04] 斐波那契数列
来源：http://hz.ppjwa.cn/gtqvrkboae.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yvedp.cn/gtjwyulinh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.guannengcc.top/gtduzdnheb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tianlin.xyz/gthtfhinuo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ywan-chungtsiang.top/gtdtptdxgi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sysykeji.top/gtyzkobcnx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.9152youxi.cn/gtqmyhdrbj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.wangdashe.top/gtrzuejnfk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.haohaochexian.top/gtjwnrboaf.html

[N05] 最大公约数
来源：http://hz.zycfv.cn/gtjbkyejbp.html

Py:   math.gcd(a, b)
来源：http://hz.yj202588.top/gtnuhonoez.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shanyushiyangtech.top/gtfkjyzzgm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aizwys.cn/gtmcxcdrjj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yuxming.cn/gtdojmyemx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shangyingyoupin.top/gtqvgxieyh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.guannengcc.top/gteneuazxa.html

Ruby: a.gcd(b)
来源：http://hz.ppjwa.cn/gtprfrbwbr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.0kj1m.cn/gtbozdlels.html

[N06] 判断回文字符串
来源：http://hz.zhongyouzk.top/gtqewoxyvu.html

Py:   s == s[::-1]
来源：http://hz.ywan-chungtsiang.top/gtcovzekjj.html

PHP:  $s === strrev($s);
来源：http://hz.ydjk.org.cn/gtbejzdydx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtplocrhyw.html

TS:   s === [...s].reverse().join("")
来源：http://hz.daxiang520.top/gtevgmddgy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.52xcode.cn/gtmhlguebu.html

Go:   // 双指针从两端比较
来源：http://hz.dianchejie.cn/gtdmnuntos.html

Ruby: s == s.reverse
来源：http://hz.jlsjyb.cn/gtgkdwsikf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gogol.net.cn/gtkcjyutsx.html

[N07] 两数之和（返回下标）
来源：http://hz.ywan-chungtsiang.top/gtonpbweod.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.wangdashe.top/gtjqssnobz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.redwolf501.top/gtzcljwsbi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jqgufenzy.top/gtpjlvvipk.html

TS:   // 手写 Map<string, number>
来源：http://hz.snrcjt.cn/gtmjnwaxfl.html

Java: // 手写 HashMap
来源：http://hz.birdmap.top/gtkvaoikgt.html

Go:   // 手写 map[int]int
来源：http://hz.ehwqpu.com/gtrwtryoqs.html

Ruby: // 手写 Hash
来源：http://hz.zycfv.cn/gtotazfifz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhengqikj.top/gtdtqfsnop.html

[N08] 生成全排列
来源：http://hz.yvedp.cn/gthglqarex.html

Py:   itertools.permutations(arr)
来源：http://hz.gzhubu.top/gtfosmojwy.html

PHP:  // 手写递归交换
来源：http://hz.jqgfzy.top/gtjtemosjx.html

JS:   // 手写回溯递归
来源：http://hz.pycfn.com/gtimzmmsku.html

TS:   // 手写回溯递归
来源：http://hz.kuanghao11.cn/gtmldkfdkd.html

Java: // 手写回溯递归
来源：http://hz.yj202588.top/gtkpkrwljn.html

Go:   // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtuevsscpo.html

Ruby: arr.permutation.to_a
来源：http://hz.yj20258888.top/gtvkodjsca.html

C#:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtromlupno.html

[N09] 栈与队列
来源：http://hz.ywan-chungtsiang.top/gtvvwdfqji.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.316326.xyz/gtelxflapg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cheryme.top/gtolikbtbb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinqigfzy.top/gtqgdsmahu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.chenzaomai.com/gtnwjjizcu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.dianchejie.cn/gtwxijdqsr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.wangshuangyany.cn/gtdkwmehbx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.svipenyu.cn/gtjvtcymwk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yvedp.cn/gtbckexunf.html

[N10] 链表节点定义
来源：http://hz.gogol.net.cn/gtgridglwd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yj202588.top/gtyxfgudwx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xinyue.icu/gtkorwxyxa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hfpthk.cn/gtreydlvon.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cqqwz.cn/gtmgrbdnpf.html

Java: class Node { int v; Node next; }
来源：http://hz.ydzc1.top/gtipuomehb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.316326.xyz/gtpunatokg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yuxming.cn/gtotodfrdo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.pycfn.com/gtpszcaidy.html

[N11] 二叉树中序遍历
来源：http://hz.sysykeji.top/gtrmjjvlze.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.nanxuanxn.top/gtknzujcqp.html

PHP:  // 手写递归函数
来源：http://hz.wangshuangyany.cn/gteboqkcrw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.feifeiyinyue.top/gtevsenbby.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.52xcode.cn/gtwhjooaup.html

Java: // 手写递归
来源：http://hz.tianlin.xyz/gtvyurzixa.html

Go:   // 手写递归
来源：http://hz.yj20258888.top/gtyfxvxdsp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jlsjyb.cn/gtzakrulbd.html

C#:   // 手写递归
来源：http://hz.smart0.xyz/gtpmpnpigi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shangyingyoupin.top/gtejgjiqag.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhijiandao.cn/gtpuotxtnj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jqgufenzy.top/gtuxxsvzgm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shuidangran.top/gtovutijfh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinqigfzy.top/gtmpxarfpg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hywenlv.cn/gtteomqmre.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.316326.xyz/gtulyocrto.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.gzhubu.top/gtbnvqaemg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cdnleiting.top/gtvftuouna.html

================================================================================
来源：http://hz.gotoacloud.top/gtjnqeexjx.html

O. 并发与异步
来源：http://hz.sxryk.cn/gtlolnjhyy.html

================================================================================
来源：http://hz.birdmap.top/gtzmbxcugm.html

[O01] 启动一个线程
来源：http://hz.shangyingyoupin.top/gtslqcuttt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jiagoushi.top/gtnirtqwdn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hnxiangtu.top/gtyjbkkell.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yanxiufei.cn/gtbgyjujoj.html

TS:   // 同 JS
来源：http://hz.cqqwz.cn/gtgmvycvut.html

Java: new Thread(() -> f()).start()
来源：http://hz.cheryme.top/gtiwsbhnzh.html

Go:   go f()
来源：http://hz.chenzaomai.com/gtqqvesuor.html

Ruby: Thread.new { f }
来源：http://hz.wangdashe.top/gtlkcumazk.html

C#:   Task.Run(() => F());
来源：http://hz.xuetiantiany.cn/gtnpjubrqm.html

[O02] 使用线程池
来源：http://hz.shanyushiyangkeji.top/gtvgtdsmaq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ywan-chungtsiang.top/gtnxosidhq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hfpthk.cn/gttoyyvcrq.html

JS:   // worker_threads 线程池
来源：http://hz.hnqzz.top/gtaqjrdqyf.html

TS:   // worker_threads 线程池
来源：http://hz.aizwys.cn/gtcdugywac.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yuanzhike.top/gtievfuwbp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.dianchejie.cn/gttgyqtbab.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yvedp.cn/gtyhdketnh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.dashuyun.cn/gtropjbbdf.html

[O03] 加锁保护共享数据
来源：http://hz.jiagoushi.top/gtwfrtwtyd.html

Py:   with lock: shared += 1
来源：http://hz.xuetiantiany.cn/gtdzbfqygl.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hnxiangtu.top/gtuekshrat.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.iojbl.cn/gteeineqnh.html

TS:   // 同 JS
来源：http://hz.quarkkingdee.top/gtuchkalbm.html

Java: synchronized (this) { shared++; }
来源：http://hz.52xcode.cn/gtgpoxqmoy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zycfv.cn/gtiqjsgwaf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jlsjyb.cn/gtwxtahibt.html

C#:   lock (gate) { shared++; }
来源：http://hz.yanxiufei.cn/gtgfldkzpr.html

[O04] 定义异步函数并等待
来源：http://hz.gzhubu.top/gtqpubopuq.html

Py:   async def f():⏎    await g()
来源：http://hz.jinghuilouyu.cn/gtvvyvpjvb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sxryk.cn/gtkpquzafz.html

JS:   async function f() { await g(); }
来源：http://hz.shzxlz.cn/gtljvhndmv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zdqjudy.top/gtkoggckcq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xinyue.icu/gtauzfttoj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.tianlin.xyz/gtqrihecwi.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ydzc1.top/gtjkeqklae.html

C#:   async Task F() { await G(); }
来源：http://hz.cucudq.cn/gtjsivhjir.html

[O05] 并发执行并等待全部完成
来源：http://hz.svipenyu.cn/gtkoxhvemb.html

Py:   asyncio.gather(*tasks)
来源：http://hz.pengpengdd.cyou/gtxufaixha.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.fengsongda.top/gtzfgtvafk.html

JS:   await Promise.all(tasks)
来源：http://hz.9152youxi.cn/gtbjvfsybl.html

TS:   await Promise.all(tasks)
来源：http://hz.jinqigfzy.top/gthcarqoye.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hnqzz.top/gtmdpnpoup.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.tian-w.cn/gtscxwtwvx.html

Ruby: threads.map(&:join)
来源：http://hz.xuetiantiany.cn/gtzzvcshvz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.daxiang520.top/gtmdouwgsb.html

[O06] 使用进程池
来源：http://hz.pengpengdd.cyou/gtcyqgeaja.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jiagoushi.top/gtkjelqjbs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.guowangkeji.top/gtuvepnjsd.html

JS:   // child_process / cluster 模块
来源：http://hz.zhaomingkeji.xyz/gtswztegdc.html

TS:   // child_process / cluster 模块
来源：http://hz.smart0.xyz/gtfyhcssaq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.gaohongyu789.top/gtbflnoibt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.kuanghao11.cn/gtjvdohmuo.html

Ruby: // fork 块
来源：http://hz.jqgufenzy.top/gtjsptzqxq.html

C#:   Parallel.For
来源：http://hz.nanxinkj.top/gtgfrbpgrx.html

================================================================================
来源：http://hz.gotoacloud.top/gttfbvhhgf.html

P. 常用工具函数
来源：http://hz.gotoacloud.top/gtdwowwzdc.html

================================================================================
来源：http://hz.ivvv.top/gtkgpnowmt.html

[P01] 生成 UUID
来源：http://hz.yuxming.cn/gtijoztpkc.html

Py:   str(uuid.uuid4())
来源：http://hz.xziqi.cn/gtziggcuap.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.0kj1m.cn/gtsciokwex.html

JS:   crypto.randomUUID()
来源：http://hz.ppjwa.cn/gtirktzdgu.html

TS:   crypto.randomUUID()
来源：http://hz.zhoulong.xyz/gtegnajlqp.html

Java: UUID.randomUUID().toString()
来源：http://hz.jianghu66.top/gtezvnbndq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhoulong.xyz/gtstfrjklg.html

Ruby: SecureRandom.uuid
来源：http://hz.yuxming.cn/gtcbfvqtxh.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.tanke756.top/gtbkidmbfk.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ybcxt.top/gtfhdxizco.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jianghu66.top/gtoicrvrxy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.pengpengdd.cyou/gtlypdihcg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.nanxinkj.top/gtmnjxscqc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.52xcode.cn/gtkslaqnaf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.iojbl.cn/gttrlibzfg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shuidangran.top/gtcnummxlm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenlongwang.top/gtdjdaawlp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yj202588.top/gtbjyohhna.html

[P03] 生成短随机字符串
来源：http://hz.cashguo.top/gtcqjlunvn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yuanzhike.top/gtbttglhnk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.wangdashe.top/gtbefhzcsf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xingfuxueyuan.xyz/gtbueonvnk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.havefunace.top/gtdvpqdsjh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hywenlv.cn/gtmgxpwvyd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xingfuxueyuan.xyz/gtfwrnonbc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jlsjyb.cn/gthdywnrqa.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.haohaochexian.top/gttbdvnppd.html

[P04] 求长度
来源：http://hz.nanxinkj.top/gtyvtmiwua.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.guannengcc.top/gtiiruftjq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zycfv.cn/gtjlxdtima.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ywan-chungtsiang.top/gtlxzttslw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.andypj.xyz/gtslqxqgrv.html

Java: list.size();  map.size();  s.length()
来源：http://hz.andypj.xyz/gtkmrnvezi.html

Go:   len(arr);  len(m)
来源：http://hz.52xcode.cn/gtspmcsnka.html

Ruby: x.length;  x.size
来源：http://hz.52xcode.cn/gtzokeapus.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jqgfzy.top/gtbeyidchm.html

[P05] 判断两个对象内容是否相等
来源：http://hz.gogol.net.cn/gtspzwlqhf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.smart0.xyz/gtwvzvzsca.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sysykeji.top/gtdegmoetr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nanxinkj.top/gtnfsrskmw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.0kj1m.cn/gttnqrpspb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.nanxuanxn.top/gtfclmdgvt.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.haohaochexian.top/gtugvgjtiu.html

Ruby: a == b
来源：http://hz.jqgufenzy.top/gtepuwanwp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gotoacloud.top/gtovqamxeu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zdqjudy.top/gtmyiygsdz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.quarkkingdee.top/gtkldrowqc.html

PHP:  if (empty($x)) {}
来源：http://hz.jiagoushi.top/gthjbjoyqa.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yonumen.top/gtosgrjmwf.html

TS:   if (x == null) {}
来源：http://hz.hongshengwenyu.top/gtvylhlwhi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yvedp.cn/gtgqlskhvw.html

Go:   if x == nil {}
来源：http://hz.yuxming.cn/gtyfqmibiy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.gogol.net.cn/gtlmcjlzhd.html

C#:   if (x is null) {}
来源：http://hz.yueranfly.top/gtqehoxaov.html

[P07] 防抖与节流
来源：http://hz.jqgufenzy.top/gtnwsaxttz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.9152youxi.cn/gtmyyfxnik.html

PHP:  // 手写时间戳比较
来源：http://hz.zhiwuduotai.top/gtmxwyowwn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.haohaochexian.top/gtqdcxwrnk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuxming.cn/gtmzbykmpk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.daxiang520.top/gttuqxabwp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jianghu66.top/gtksiuzyvn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sxryk.cn/gtgsjzwyxe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yongpay.top/gtnnjgzfok.html

[P08] 处理浮点精度问题
来源：http://hz.0kj1m.cn/gtrykaiwzd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.0kj1m.cn/gthevqmkoa.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.tian-w.cn/gtkfxhbxqs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yongpay.top/gtipmxghei.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ywan-chungtsiang.top/gtqscluckm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.chenlongwang.top/gtcnqiqrdb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.meibo888.top/gtbbndgtkb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.fzhhl.top/gthkfiaiyc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cucudq.cn/gtwakqvtky.html

================================================================================
来源：http://hz.yj20258.top/gtbazqjuyi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj202588.top/gtcqlyyupt.html

================================================================================
来源：http://hz.sweek.top/gtlkxketzq.html

[Q01] 创建表
来源：http://hz.zhixingplan.top/gtlbbkxzsp.html

CREATE TABLE users (
来源：http://hz.yueranfly.top/gtvwrqvspi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jlsjyb.cn/gtketyigyh.html

name VARCHAR(50) NOT NULL,
来源：http://hz.kuanghao11.cn/gtrdhvnilg.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sufxvd.cn/gtbhlhgcui.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yuanzhike.top/gtdxkshkol.html

);
来源：http://hz.chenjidiqi.icu/gtkphvavox.html

[Q02] 创建带外键的表
来源：http://hz.hammf.cn/gtlhxpqbzg.html

CREATE TABLE orders (
来源：http://hz.xingfuxueyuan.xyz/gtcsdwmacq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.andypj.xyz/gtigwrcykx.html

user_id INT NOT NULL,
来源：http://hz.c1oappe.top/gthbdpkgza.html

amount DECIMAL(10, 2),
来源：http://hz.zhixingplan.top/gtbyrgkhmj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinyuanbaomall.cn/gtqtaefsfw.html

);
来源：http://hz.tianlin.xyz/gtovpyswgy.html

[Q03] 增加列
来源：http://hz.hfpthk.cn/gtyvlwzqgw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.52xcode.cn/gtdkgbgylm.html

[Q04] 修改列类型
来源：http://hz.sysykeji.top/gtdkxrmues.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gotoacloud.top/gtekxotrym.html

[Q05] 重命名列
来源：http://hz.ybcxt.top/gthwqcmwcb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ywan-chungtsiang.top/gtkiyassnu.html

[Q06] 删除列
来源：http://hz.bjfxy.top/gtnqeqcoxx.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.fzhhl.top/gtcmciqhyu.html

[Q07] 删除表
来源：http://hz.shzxlz.cn/gtskaozclt.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinqigufen.top/gtvkbqxayd.html

[Q08] 创建普通索引
来源：http://hz.meibo888.top/gtizhjgrqa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.fengsongda.top/gtnrcowxhf.html

[Q09] 创建唯一索引
来源：http://hz.yvedp.cn/gteedfaetl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yj20258.top/gtjsylcpts.html

[Q10] 插入单行
来源：http://hz.wangdashe.top/gtquvenkvc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jlsjyb.cn/gtqipemgfp.html

[Q11] 一次插入多行
来源：http://hz.hongshengwenyu.top/gtosaeimbf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shuidangran.top/gtnldiheyj.html

[Q12] 插入后取自增 ID
来源：http://hz.gzhubu.top/gtddntquez.html


<!-- 参考信息 -->