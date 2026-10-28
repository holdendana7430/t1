代发 wailian999

Ruby: exit 1
来源：http://hz.daxiang520.top/gtudlvbjxi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.chenjidiqi.icu/gtocvehyse.html

[M06] 向标准错误输出
来源：http://hz.wangdashe.top/gtddyuoppq.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yanxiufei.cn/gtcmorocat.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.guowangkeji.top/gtllzqtxzc.html

JS:   console.error("err")
来源：http://hz.yuxming.cn/gtcytioxzt.html

TS:   console.error("err")
来源：http://hz.hammf.cn/gtscznywtn.html

Java: System.err.println("err")
来源：http://hz.wangdashe.top/gtdseuokgb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yvedp.cn/gtfjhnisls.html

Ruby: warn "err"
来源：http://hz.jinqigufen.top/gtdndntmns.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jqgufenzy.top/gtsqrfkmxq.html

[M07] 判断是否为主入口
来源：http://hz.xuetiantiany.cn/gtleqhpvib.html

Py:   if __name__ == "__main__":
来源：http://hz.chenlongwang.top/gthawbkvan.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ppjwa.cn/gtelcqanpq.html

JS:   require.main === module
来源：http://hz.sysykeji.top/gtxudfbqpn.html

TS:   require.main === module
来源：http://hz.ydjk.org.cn/gteycjqsta.html

Java: public static void main(String[] args)
来源：http://hz.9152youxi.cn/gtcnrwnhwx.html

Go:   func main()
来源：http://hz.aibaodan.cn/gtsmossuha.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sweek.top/gtewohdyqq.html

C#:   static void Main(string[] args)
来源：http://hz.jlsjyb.cn/gtkzctajzq.html

[M08] 获取系统与运行时信息
来源：http://hz.9152youxi.cn/gtwwpbfkcp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shanyushiyangtech.top/gtuomayxau.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cashguo.top/gtlqwnqmof.html

JS:   process.platform;  process.version
来源：http://hz.feifeiyinyue.top/gtpdwhlxsb.html

TS:   process.platform;  process.version
来源：http://hz.yonumen.top/gtleylezti.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hnqzz.top/gtpraueqxd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.c1oappe.top/gtfuktdywf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hongshengwenyu.top/gtmvteotjr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.kuanghao11.cn/gtwiixejbh.html

================================================================================
来源：http://hz.jqgfzy.top/gtolhprvce.html

N. 数据结构与算法
来源：http://hz.chenzaomai.com/gtnyimwopb.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtkfxryoka.html

[N01] 二分查找（有序数组）
来源：http://hz.ydzc1.top/gtdhotepbh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.chenlongwang.top/gtxcgzbnhd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yangfankeji.com/gtgyzrlsbv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yongpay.top/gtvdhmjbou.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shuidangran.top/gtyyhwwaxk.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhiwuduotai.top/gtxieldtbj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenzaomai.com/gtgbjjhbyh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.cqqwz.cn/gtcyedrcbk.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shangyingyoupin.top/gtzbnapjoj.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.havefunace.top/gtjxhakvaq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hnqzz.top/gtwpyyadwk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xinyue.icu/gtsptiuric.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuetiantiany.cn/gtovnrmyfx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhaomingkeji.xyz/gttudhsxjc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.daxiang520.top/gtxqevxiit.html

Go:   slices.Sort(arr)
来源：http://hz.yueranfly.top/gtbokutbuq.html

Ruby: arr.sort
来源：http://hz.jlsjyb.cn/gtljfimgvm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.gotoacloud.top/gtaxxaalyg.html

[N03] 快速排序（分治示例）
来源：http://hz.sufxvd.cn/gtgoozhecm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.sweek.top/gtbcrwgjwg.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yvedp.cn/gtpaboohsx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tanke756.top/gtnxoveyne.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.daxiang520.top/gtxtrhfbwz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.316326.xyz/gthpmvwgqe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jiagoushi.top/gtkqqalcgm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cashguo.top/gtznvwhsyb.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.sysykeji.top/gtnozqjlqr.html

[N04] 斐波那契数列
来源：http://hz.ydzc1.top/gtoypsilbu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.iojbl.cn/gtyjkuxcdf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhiwuduotai.top/gtgipihtsn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daxiang520.top/gtkobochcp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.snrcjt.cn/gtdxlzqdjd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.fengsongda.top/gtogbjvnsf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cashguo.top/gthlsfwiwh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.52xcode.cn/gtujsbmhal.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.nwbrower.top/gtrpvvkggl.html

[N05] 最大公约数
来源：http://hz.fengsongda.top/gtsfgyjsnm.html

Py:   math.gcd(a, b)
来源：http://hz.hysaishi.cn/gtfoanlgyb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yongpay.top/gtokmvdxru.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.andypj.xyz/gtywmbkpqn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jiagoushi.top/gtvknborhn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xinyue.icu/gtjwjxgliz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shangyingyoupin.top/gtijjujqcw.html

Ruby: a.gcd(b)
来源：http://hz.fengsongda.top/gtocbmtqrt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.wangdashe.top/gtkcwijkcb.html

[N06] 判断回文字符串
来源：http://hz.ivvv.top/gtqxxakmny.html

Py:   s == s[::-1]
来源：http://hz.iojbl.cn/gtqodkjpmr.html

PHP:  $s === strrev($s);
来源：http://hz.yangfankeji.com/gtbbfhhaiu.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtedcdryov.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tian-w.cn/gtuineyzdk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zdqjudy.top/gtybjmpsgn.html

Go:   // 双指针从两端比较
来源：http://hz.feifeiyinyue.top/gtbtotdhem.html

Ruby: s == s.reverse
来源：http://hz.hfpthk.cn/gthiubyfhv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinyuanbaomall.cn/gtgvlwjsfa.html

[N07] 两数之和（返回下标）
来源：http://hz.fengsongda.top/gtczmthllq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cqqwz.cn/gttycnsmfp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.chenzaomai.com/gtltabwkbf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhoulong.xyz/gtihhjzpyf.html

TS:   // 手写 Map<string, number>
来源：http://hz.havefunace.top/gtfeajzpmx.html

Java: // 手写 HashMap
来源：http://hz.guannengcc.top/gtyhqlxfyo.html

Go:   // 手写 map[int]int
来源：http://hz.nwbrower.top/gtluqcayhq.html

Ruby: // 手写 Hash
来源：http://hz.hnqzz.top/gtgkiqxncf.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.mhx1999.top/gtcqdgmfcu.html

[N08] 生成全排列
来源：http://hz.ehwqpu.com/gtqahurrjb.html

Py:   itertools.permutations(arr)
来源：http://hz.cqqwz.cn/gttsymzlfx.html

PHP:  // 手写递归交换
来源：http://hz.wangdashe.top/gtixmdyppj.html

JS:   // 手写回溯递归
来源：http://hz.yvedp.cn/gtekpdblcx.html

TS:   // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtennaldus.html

Java: // 手写回溯递归
来源：http://hz.gzhubu.top/gtvbgezfxr.html

Go:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtzahfefan.html

Ruby: arr.permutation.to_a
来源：http://hz.hammf.cn/gtvtegurpu.html

C#:   // 手写回溯递归
来源：http://hz.fengsongda.top/gtkskxykjo.html

[N09] 栈与队列
来源：http://hz.hfpthk.cn/gtvowvfpwk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shangyingyoupin.top/gteivniwnr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhijiandao.cn/gttmhicajf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.gaohongyu789.top/gtnrfyoggd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yvedp.cn/gtjkhfgfay.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yj202588.top/gtrzrznewd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.snrcjt.cn/gtwgwsoleh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ybcxt.top/gthdgqneue.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jiagoushi.top/gthppnubtz.html

[N10] 链表节点定义
来源：http://hz.nanxuanxn.top/gtsqdjltkc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.nanxinkj.top/gtwxebnuyb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ydjk.org.cn/gtasfshgvf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.svipenyu.cn/gtaiahqnof.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shangyingyoupin.top/gtnvkjbqmg.html

Java: class Node { int v; Node next; }
来源：http://hz.cqqwz.cn/gtxqgsvihb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ehwqpu.com/gtjytlijjp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shzxlz.cn/gtastwhogd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.sweek.top/gtdtcqxhij.html

[N11] 二叉树中序遍历
来源：http://hz.birdmap.top/gttwggqvea.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.bjfxy.top/gtaeupurtz.html

PHP:  // 手写递归函数
来源：http://hz.nanxuanxn.top/gtpyycxknt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenlongwang.top/gtcrfduczi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sweek.top/gtryoqfmjy.html

Java: // 手写递归
来源：http://hz.yj20258.top/gtrncbjhfl.html

Go:   // 手写递归
来源：http://hz.mhx1999.top/gtraaqdlom.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.chenjidiqi.icu/gtvbusialo.html

C#:   // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtuknwtecm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.svipenyu.cn/gtfkyiovdw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tian-w.cn/gtagklbexb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.guannengcc.top/gtvejmutry.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.fzhhl.top/gtsecgjxeb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hywenlv.cn/gtjfzsbihp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shuidangran.top/gtwyrvqrvz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenlongwang.top/gtylgahgbf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.chenjidiqi.icu/gthvwawlcd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sweek.top/gtaxspkofo.html

================================================================================
来源：http://hz.quarkkingdee.top/gtvddphomn.html

O. 并发与异步
来源：http://hz.pengpengdd.cyou/gtlrjdxgpy.html

================================================================================
来源：http://hz.gaohongyu789.top/gtbtogreuu.html

[O01] 启动一个线程
来源：http://hz.jiagoushi.top/gtheyyjblj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.bjfxy.top/gtmljmluue.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hysaishi.cn/gtgfxommcx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xylfe.cn/gtgymazzvl.html

TS:   // 同 JS
来源：http://hz.xuetiantiany.cn/gtebandvlo.html

Java: new Thread(() -> f()).start()
来源：http://hz.hywenlv.cn/gtxfronpry.html

Go:   go f()
来源：http://hz.yangfankeji.com/gtekqbsomm.html

Ruby: Thread.new { f }
来源：http://hz.hysaishi.cn/gtacewbuwq.html

C#:   Task.Run(() => F());
来源：http://hz.chenjidiqi.icu/gtbjtfepov.html

[O02] 使用线程池
来源：http://hz.zhoulong.xyz/gtrqffrrka.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinqigufen.top/gtqjinxqjx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yj20258888.top/gttbstxuee.html

JS:   // worker_threads 线程池
来源：http://hz.hywenlv.cn/gtxexajjyc.html

TS:   // worker_threads 线程池
来源：http://hz.yj202588.top/gtxohjbkcr.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.chenlongwang.top/gtsregjfoj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jqgfzy.top/gtzaqopxie.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.andypj.xyz/gtpzdzbyxd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yueranfly.top/gtlnmtkhmi.html

[O03] 加锁保护共享数据
来源：http://hz.zdqjudy.top/gtqulorcjy.html

Py:   with lock: shared += 1
来源：http://hz.daria6918.cn/gtzsqefoxm.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.guannengcc.top/gtlvjsfxnn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.sweek.top/gtqnnzkxxd.html

TS:   // 同 JS
来源：http://hz.ywan-chungtsiang.top/gtmwsybyio.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhixingplan.top/gtpjezfhcs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yuanzhike.top/gtniexjgbw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zycfv.cn/gthvkzhwwb.html

C#:   lock (gate) { shared++; }
来源：http://hz.jqgufenzy.top/gtqhlwqxml.html

[O04] 定义异步函数并等待
来源：http://hz.zhengqikj.top/gtoehopdht.html

Py:   async def f():⏎    await g()
来源：http://hz.hnqzz.top/gtetrikghe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sxryk.cn/gtjeodkihq.html

JS:   async function f() { await g(); }
来源：http://hz.xuetiantiany.cn/gtdlsdfkpf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.gogol.net.cn/gteljwkwid.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.daxiang520.top/gtcpmwnaue.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hnqzz.top/gtuzlsrlzg.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.pycfn.com/gtskvestxt.html

C#:   async Task F() { await G(); }
来源：http://hz.zhongyouzk.top/gtxjiepsdz.html

[O05] 并发执行并等待全部完成
来源：http://hz.sweek.top/gtffconjth.html

Py:   asyncio.gather(*tasks)
来源：http://hz.sweek.top/gtflzidwik.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jinqigfzy.top/gtmqthteyc.html

JS:   await Promise.all(tasks)
来源：http://hz.nanxuanxn.top/gtwnpbcaxb.html

TS:   await Promise.all(tasks)
来源：http://hz.shuidangran.top/gtazkhxiec.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xinyue.icu/gtkbufpjih.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.pengpengdd.cyou/gtzxujxizz.html

Ruby: threads.map(&:join)
来源：http://hz.nanxinkj.top/gtyrfdgypv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yonumen.top/gtsyahsafk.html

[O06] 使用进程池
来源：http://hz.tianlin.xyz/gttegwiczx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yj20258888.top/gtqmmawvbo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ehwqpu.com/gtdelvomfo.html

JS:   // child_process / cluster 模块
来源：http://hz.gogol.net.cn/gtzvebinru.html

TS:   // child_process / cluster 模块
来源：http://hz.sufxvd.cn/gteumcbhmf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.birdmap.top/gtmhaxuflg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.quarkkingdee.top/gtqyhgfwjm.html

Ruby: // fork 块
来源：http://hz.52xcode.cn/gtjmduldzk.html

C#:   Parallel.For
来源：http://hz.hongshengwenyu.top/gtwxkcfbhx.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtfvefczwg.html

P. 常用工具函数
来源：http://hz.hysaishi.cn/gtulcsysdp.html

================================================================================
来源：http://hz.yangfankeji.com/gtjwxafoee.html

[P01] 生成 UUID
来源：http://hz.gogol.net.cn/gtuuwgnogh.html

Py:   str(uuid.uuid4())
来源：http://hz.shzxlz.cn/gthoxzqeee.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sxryk.cn/gtyjaahjze.html

JS:   crypto.randomUUID()
来源：http://hz.feifeiyinyue.top/gthfeqbfzq.html

TS:   crypto.randomUUID()
来源：http://hz.cheryme.top/gtvpyelhgf.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhaomingkeji.xyz/gtnimtvmul.html

Go:   // 用 github.com/google/uuid
来源：http://hz.meibo888.top/gtnubzlcwb.html

Ruby: SecureRandom.uuid
来源：http://hz.pengpengdd.cyou/gtnnydfpfb.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xinyue.icu/gtkywzzvwe.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ydjk.org.cn/gtazblbvnl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gotoacloud.top/gtwbmpjzeg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.redwolf501.top/gtzmufhkuv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.chenlongwang.top/gtwwkemxoh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xuanzx.com/gtykhewgll.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj202588.top/gtrcbzwltt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yonumen.top/gtzqdmzorv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.gaohongyu789.top/gtghgzidrr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hnqzz.top/gthqeajpqk.html

[P03] 生成短随机字符串
来源：http://hz.wangshuangyany.cn/gttidkorwo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gogol.net.cn/gtjimxtras.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.guannengcc.top/gtxhcptmyt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnqzz.top/gtdwzsjcbv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hammf.cn/gtzgjoowlg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.fzhhl.top/gtfourdvfx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jinqigfzy.top/gturyplfph.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhaomingkeji.xyz/gtrzfboozj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xingfuxueyuan.xyz/gtsdllupri.html

[P04] 求长度
来源：http://hz.yongpay.top/gtyrytkktk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.svipenyu.cn/gtwkllmseh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sxryk.cn/gtngptyomw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fengsongda.top/gtgoemnrgn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhaomingkeji.xyz/gtupuzwhpb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ppjwa.cn/gtdoijcuxq.html

Go:   len(arr);  len(m)
来源：http://hz.c1oappe.top/gtoztsjojh.html

Ruby: x.length;  x.size
来源：http://hz.feifeiyinyue.top/gtylaqctpx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.dianchejie.cn/gtepuolesq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.daria6918.cn/gtxjtkupde.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.iojbl.cn/gtyqauirvz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinyuanbaomall.cn/gtgyxkigho.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jinqigfzy.top/gtnzpzpyvc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gogol.net.cn/gtttlursof.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cqqwz.cn/gtuhqqfqec.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.daria6918.cn/gtswtpyshf.html

Ruby: a == b
来源：http://hz.sweek.top/gtefkspbwh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yvedp.cn/gtlzzptreq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gogol.net.cn/gtlkezzquj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.bjfxy.top/gtknrhkycg.html

PHP:  if (empty($x)) {}
来源：http://hz.jianghu66.top/gtjfiifdrq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.smart0.xyz/gttzckoeoa.html

TS:   if (x == null) {}
来源：http://hz.yonumen.top/gtnrwfestt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hfpthk.cn/gttfshtvjf.html

Go:   if x == nil {}
来源：http://hz.jlsjyb.cn/gtnavxhpwn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jqgfzy.top/gtmrawexeq.html

C#:   if (x is null) {}
来源：http://hz.zhongyouzk.top/gtzwkexkcg.html

[P07] 防抖与节流
来源：http://hz.wangshuangyany.cn/gtxcrfwejy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shanyushiyangtech.top/gtdqbmzzcl.html

PHP:  // 手写时间戳比较
来源：http://hz.0kj1m.cn/gtqsxwunef.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuanzx.com/gtlenggonc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhiwuduotai.top/gtumijnhna.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yuanzhike.top/gtoebmktmc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.dianchejie.cn/gtwklhutqp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yueranfly.top/gtnjzhuqku.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jqgufenzy.top/gtqsnpfshg.html

[P08] 处理浮点精度问题
来源：http://hz.xuanzx.com/gtmmlacbty.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.daria6918.cn/gtpraqoupx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.aibaodan.cn/gthcwfbqhl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.smart0.xyz/gtbdhblhui.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hysaishi.cn/gtmokmqvff.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yuxming.cn/gtpkyggtfh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.iojbl.cn/gtbttsnjwx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yueranfly.top/gtdasglwon.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.daria6918.cn/gtqrggsdsl.html

================================================================================
来源：http://hz.havefunace.top/gtiwfouepx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cucudq.cn/gtsxuuhfvz.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtzzkbwwba.html

[Q01] 创建表
来源：http://hz.ehwqpu.com/gtsharwkmq.html

CREATE TABLE users (
来源：http://hz.jqgufenzy.top/gttdchleqf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.redwolf501.top/gtenivcvmy.html

name VARCHAR(50) NOT NULL,
来源：http://hz.chenlongwang.top/gtzdhvqidt.html

email VARCHAR(100) UNIQUE,
来源：http://hz.svipenyu.cn/gthxbntwgf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shangyingyoupin.top/gticlelljl.html

);
来源：http://hz.zhengqikj.top/gtnaiuyfrk.html

[Q02] 创建带外键的表
来源：http://hz.zhengqikj.top/gtmfjsmter.html

CREATE TABLE orders (
来源：http://hz.meibo888.top/gtvqkhfynr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gzhubu.top/gtyowxjuxi.html

user_id INT NOT NULL,
来源：http://hz.shanyushiyangtech.top/gtvopwlwab.html

amount DECIMAL(10, 2),
来源：http://hz.zhongyouzk.top/gtagccevaj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ehwqpu.com/gtfcwsnjim.html

);
来源：http://hz.cashguo.top/gtjclgebnw.html

[Q03] 增加列
来源：http://hz.jlsjyb.cn/gthkpqhzmi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shanyushiyangtech.top/gtnqztjbsk.html

[Q04] 修改列类型
来源：http://hz.316326.xyz/gtgblylsjc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.guowangkeji.top/gtqjlapdvd.html

[Q05] 重命名列
来源：http://hz.zhiwuduotai.top/gtiawvfrhn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ppjwa.cn/gttsbepaoo.html

[Q06] 删除列
来源：http://hz.kuanghao11.cn/gtsfwsbwlh.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ivvv.top/gtpvsimxkw.html

[Q07] 删除表
来源：http://hz.jinyuanbaomall.cn/gtiutrxejp.html

DROP TABLE IF EXISTS orders;
来源：http://hz.aibaodan.cn/gtcupsgbpy.html

[Q08] 创建普通索引
来源：http://hz.xingfuxueyuan.xyz/gtrjcsqkmv.html


<!-- 参考信息 -->