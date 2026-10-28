代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.dashuyun.cn/gtbipdkzjt.html

JS:   console.error("err")
来源：http://hz.fengsongda.top/gtnvfinilc.html

TS:   console.error("err")
来源：http://hz.redwolf501.top/gtedcyjuwl.html

Java: System.err.println("err")
来源：http://hz.yonumen.top/gtedoydzej.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.mhx1999.top/gtvbdhvjns.html

Ruby: warn "err"
来源：http://hz.guowangkeji.top/gtivmundoe.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shanyushiyangtech.top/gtmsjodjck.html

[M07] 判断是否为主入口
来源：http://hz.zycfv.cn/gtshxodfbb.html

Py:   if __name__ == "__main__":
来源：http://hz.quarkkingdee.top/gtcjpdaayj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gzhubu.top/gtvjqbhyvr.html

JS:   require.main === module
来源：http://hz.mhx1999.top/gthkdeggyo.html

TS:   require.main === module
来源：http://hz.yj202588.top/gtmhsuywxr.html

Java: public static void main(String[] args)
来源：http://hz.zhaomingkeji.xyz/gtcruzfhgg.html

Go:   func main()
来源：http://hz.xuetiantiany.cn/gtrszajibl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cdnleiting.top/gtsbjtyeqx.html

C#:   static void Main(string[] args)
来源：http://hz.chenjidiqi.icu/gtytkrihrt.html

[M08] 获取系统与运行时信息
来源：http://hz.yuanzhike.top/gtzvykoetc.html

Py:   platform.system();  platform.python_version()
来源：http://hz.feifeiyinyue.top/gtfzxsglzp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gaohongyu789.top/gtztcnwdoz.html

JS:   process.platform;  process.version
来源：http://hz.nanxinkj.top/gthqfrnslt.html

TS:   process.platform;  process.version
来源：http://hz.0kj1m.cn/gtmzomawtm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.snrcjt.cn/gthfzpbgex.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.52xcode.cn/gtopgvnzdj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shuidangran.top/gtfmuxqkwg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.quarkkingdee.top/gtrilrxxgo.html

================================================================================
来源：http://hz.jinqigufen.top/gtetfvfwqe.html

N. 数据结构与算法
来源：http://hz.nwbrower.top/gtgybdtxvv.html

================================================================================
来源：http://hz.yueranfly.top/gtqgqfnvdq.html

[N01] 二分查找（有序数组）
来源：http://hz.shzxlz.cn/gtiyplnlde.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yueranfly.top/gtxibwjecz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.chenzaomai.com/gtsiypagwp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangdashe.top/gtwurfyqwk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigufen.top/gtgxqnlnor.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhongyouzk.top/gtyzpcdxbs.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.sweek.top/gtfcetpsck.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sweek.top/gtiyyidlaw.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shuidangran.top/gtkvbhubvt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jinghuilouyu.cn/gtcidsmixg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.dashuyun.cn/gtwgkkymlq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.52xcode.cn/gtbcgryelm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258.top/gtntmjisbz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cdnleiting.top/gthedgwghj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.meibo888.top/gtksawtpio.html

Go:   slices.Sort(arr)
来源：http://hz.yj202588.top/gtirgicxnt.html

Ruby: arr.sort
来源：http://hz.haohaochexian.top/gthanbbqdk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yangfankeji.com/gtjfepgpud.html

[N03] 快速排序（分治示例）
来源：http://hz.birdmap.top/gtiiqvjfvf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yj20258.top/gtybskiolu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.fzhhl.top/gtychrdnkt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xingfuxueyuan.xyz/gtivjtwwho.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hysaishi.cn/gthfyvtowl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj202588.top/gtuhevwqwt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yangfankeji.com/gtqmymerap.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gogol.net.cn/gterptmoen.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cdnleiting.top/gtibtchgyq.html

[N04] 斐波那契数列
来源：http://hz.xuetiantiany.cn/gtdavwhihl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhixingplan.top/gtyydzoocn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhiwuduotai.top/gtfomuvigu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhijiandao.cn/gtfdrfbuxw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nwbrower.top/gtizwdnvwi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jqgfzy.top/gtbjxgszqq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.tian-w.cn/gtwbkuhlnz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.316326.xyz/gtvdccakkp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ybcxt.top/gtcqedruzx.html

[N05] 最大公约数
来源：http://hz.chenjidiqi.icu/gtqeqpnkqi.html

Py:   math.gcd(a, b)
来源：http://hz.smart0.xyz/gtoxqgpfbs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jlsjyb.cn/gtzjbjaomv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhijiandao.cn/gtkkfzliow.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangdashe.top/gtclqyhtuw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xuanzx.com/gtrqsqyfsr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.tanke756.top/gtafdjignf.html

Ruby: a.gcd(b)
来源：http://hz.cashguo.top/gtxdytjjle.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.316326.xyz/gtbngobzpn.html

[N06] 判断回文字符串
来源：http://hz.hywenlv.cn/gtldojuawr.html

Py:   s == s[::-1]
来源：http://hz.xinyue.icu/gtuinrmxsv.html

PHP:  $s === strrev($s);
来源：http://hz.yj20258888.top/gtciwrtzxv.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtrqsfcqrz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jinghuilouyu.cn/gthqtasndx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ehwqpu.com/gtrvrmlpsf.html

Go:   // 双指针从两端比较
来源：http://hz.zhengqikj.top/gtbbyhjrhu.html

Ruby: s == s.reverse
来源：http://hz.jinqigufen.top/gthelamjil.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ybcxt.top/gtqhgrurat.html

[N07] 两数之和（返回下标）
来源：http://hz.hywenlv.cn/gthzbpktww.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinqigufen.top/gtwdatsqpg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.smart0.xyz/gthsxlganb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shangyingyoupin.top/gtnhriwkoc.html

TS:   // 手写 Map<string, number>
来源：http://hz.shuidangran.top/gtuifovryx.html

Java: // 手写 HashMap
来源：http://hz.zhengqikj.top/gtgyalnvao.html

Go:   // 手写 map[int]int
来源：http://hz.c1oappe.top/gtszeulddz.html

Ruby: // 手写 Hash
来源：http://hz.shzxlz.cn/gtrutjnrys.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinghuilouyu.cn/gtwcbuaoqn.html

[N08] 生成全排列
来源：http://hz.pengpengdd.cyou/gtycqxrkxl.html

Py:   itertools.permutations(arr)
来源：http://hz.hnxiangtu.top/gtjmhfhfto.html

PHP:  // 手写递归交换
来源：http://hz.yj202588.top/gtfcghesoc.html

JS:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtdnrcmiaf.html

TS:   // 手写回溯递归
来源：http://hz.shzxlz.cn/gthmrcqtfm.html

Java: // 手写回溯递归
来源：http://hz.hfpthk.cn/gtkqwssbmi.html

Go:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtiopqckso.html

Ruby: arr.permutation.to_a
来源：http://hz.52xcode.cn/gtlfslowee.html

C#:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtxovimszb.html

[N09] 栈与队列
来源：http://hz.andypj.xyz/gtmugcmjnu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jqgfzy.top/gtxpbcewna.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhiwuduotai.top/gtxkagadwt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hywenlv.cn/gtjnfavxsw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhijiandao.cn/gtpdtvdcby.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xylfe.cn/gtosyypvii.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.guowangkeji.top/gtvgqddoxl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yj20258.top/gtfwhawwcb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gzhubu.top/gtmcvofcho.html

[N10] 链表节点定义
来源：http://hz.hywenlv.cn/gtvbwevynd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hnxiangtu.top/gtyoutjzno.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhixingplan.top/gtglzdutkn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.feifeiyinyue.top/gtfbgfuuln.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.haohaochexian.top/gtoydimczm.html

Java: class Node { int v; Node next; }
来源：http://hz.guannengcc.top/gtfwkkekgf.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cdnleiting.top/gtiwdglerh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhaomingkeji.xyz/gtoosublsi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ydzc1.top/gttxgzxijg.html

[N11] 二叉树中序遍历
来源：http://hz.aibaodan.cn/gthmjwfuin.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yongpay.top/gtaeqytcvn.html

PHP:  // 手写递归函数
来源：http://hz.jinqigfzy.top/gtifcafdas.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.feifeiyinyue.top/gtbbjuyveu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.9152youxi.cn/gttfjickvt.html

Java: // 手写递归
来源：http://hz.yongpay.top/gtbfirktqb.html

Go:   // 手写递归
来源：http://hz.fengsongda.top/gtpuagxjjc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.quarkkingdee.top/gtecoesxhe.html

C#:   // 手写递归
来源：http://hz.cashguo.top/gtkxxjhung.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.guannengcc.top/gttmtbwuri.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xinyue.icu/gtcnjfdbix.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinyuanbaomall.cn/gtmwqhmbgk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhongyouzk.top/gttzbtpjrb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.smart0.xyz/gtycppvkki.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258.top/gtheeibqxh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ppjwa.cn/gtfcgzdkrc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.dashuyun.cn/gtthzonssa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.andypj.xyz/gtzuazmlwb.html

================================================================================
来源：http://hz.yuxming.cn/gtnxiaxmct.html

O. 并发与异步
来源：http://hz.jiagoushi.top/gtrltcxloq.html

================================================================================
来源：http://hz.andypj.xyz/gtswcykdix.html

[O01] 启动一个线程
来源：http://hz.wangshuangyany.cn/gtokrysrex.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.kuanghao11.cn/gtjoervbpy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shuidangran.top/gtqydawxmb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yueranfly.top/gtrdiuvvnr.html

TS:   // 同 JS
来源：http://hz.vqdsnc.cn/gtskysdurs.html

Java: new Thread(() -> f()).start()
来源：http://hz.iojbl.cn/gtetydkwxj.html

Go:   go f()
来源：http://hz.smart0.xyz/gtwkleujqd.html

Ruby: Thread.new { f }
来源：http://hz.316326.xyz/gtwqeljhvn.html

C#:   Task.Run(() => F());
来源：http://hz.nanxinkj.top/gtfvzdyavs.html

[O02] 使用线程池
来源：http://hz.9152youxi.cn/gtafmntuwk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.haohaochexian.top/gtrxzhbhbq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.wangdashe.top/gtlumizyiq.html

JS:   // worker_threads 线程池
来源：http://hz.hongshengwenyu.top/gtsxebmhsx.html

TS:   // worker_threads 线程池
来源：http://hz.jiagoushi.top/gtmaansbzb.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shanyushiyangkeji.top/gtoxcfdpwg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.haohaochexian.top/gtvlhceqyt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ydjk.org.cn/gtywepcmfp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yvedp.cn/gtcnxeqjwd.html

[O03] 加锁保护共享数据
来源：http://hz.xinyue.icu/gtzrqmkyvd.html

Py:   with lock: shared += 1
来源：http://hz.mhx1999.top/gthnrhehks.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.meibo888.top/gtnunyfcyk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ydzc1.top/gtjslgxkjp.html

TS:   // 同 JS
来源：http://hz.yj20258888.top/gtjdnpoomi.html

Java: synchronized (this) { shared++; }
来源：http://hz.jqgfzy.top/gtusqqatdt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cdnleiting.top/gteironjwn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.0kj1m.cn/gtntirmtzr.html

C#:   lock (gate) { shared++; }
来源：http://hz.vqdsnc.cn/gtvurqlclv.html

[O04] 定义异步函数并等待
来源：http://hz.cheryme.top/gteijarmlj.html

Py:   async def f():⏎    await g()
来源：http://hz.zycfv.cn/gtciowtjhc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.svipenyu.cn/gtufjdgbon.html

JS:   async function f() { await g(); }
来源：http://hz.zdqjudy.top/gtuzbrjhyi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hfpthk.cn/gtwlialgtd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.316326.xyz/gtlmarzqoe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hnxiangtu.top/gtxfqtylqo.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xinyue.icu/gtjixihdpx.html

C#:   async Task F() { await G(); }
来源：http://hz.yonumen.top/gtcifuzflh.html

[O05] 并发执行并等待全部完成
来源：http://hz.andypj.xyz/gtfedysuap.html

Py:   asyncio.gather(*tasks)
来源：http://hz.wangshuangyany.cn/gtlmkcuzhs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xingfuxueyuan.xyz/gtgnnbhsxb.html

JS:   await Promise.all(tasks)
来源：http://hz.shzxlz.cn/gtbceboncq.html

TS:   await Promise.all(tasks)
来源：http://hz.redwolf501.top/gtzuwffzmy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.sufxvd.cn/gtuvnhtmhp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yj20258.top/gtannmpxee.html

Ruby: threads.map(&:join)
来源：http://hz.guowangkeji.top/gtsaivvmly.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hnxiangtu.top/gtdysplmrj.html

[O06] 使用进程池
来源：http://hz.shuidangran.top/gtrecrrapn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jinqigufen.top/gtukrlltpe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.vqdsnc.cn/gtrrvvizjf.html

JS:   // child_process / cluster 模块
来源：http://hz.yangfankeji.com/gtddapxswk.html

TS:   // child_process / cluster 模块
来源：http://hz.jianghu66.top/gtzfmcnmfp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhijiandao.cn/gtkvunkwmt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.9152youxi.cn/gtamaammaz.html

Ruby: // fork 块
来源：http://hz.dianchejie.cn/gtmteqkrlj.html

C#:   Parallel.For
来源：http://hz.hfpthk.cn/gtrmkkeyjj.html

================================================================================
来源：http://hz.meibo888.top/gtyoaeityt.html

P. 常用工具函数
来源：http://hz.vqdsnc.cn/gtuvkgpmae.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtzezwcvpp.html

[P01] 生成 UUID
来源：http://hz.gogol.net.cn/gthepzrivb.html

Py:   str(uuid.uuid4())
来源：http://hz.yj202588.top/gtihtrtdni.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cucudq.cn/gttvbvawmo.html

JS:   crypto.randomUUID()
来源：http://hz.nwbrower.top/gtgpyszphg.html

TS:   crypto.randomUUID()
来源：http://hz.guannengcc.top/gtjilunxpd.html

Java: UUID.randomUUID().toString()
来源：http://hz.hfpthk.cn/gtascbyznc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jlsjyb.cn/gthasasiqw.html

Ruby: SecureRandom.uuid
来源：http://hz.xingfuxueyuan.xyz/gtqesedfsl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhiwuduotai.top/gtfyhqnopi.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sufxvd.cn/gtmcqmoqej.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.bjfxy.top/gtzbjbxjor.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ywan-chungtsiang.top/gtlgapdhdo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shanyushiyangtech.top/gtbuuugywr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xuetiantiany.cn/gttojdvxvh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hysaishi.cn/gtyzhstine.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ydzc1.top/gtdhtxjbuf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinqigfzy.top/gtftbxswdi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yueranfly.top/gtfcolhbsm.html

[P03] 生成短随机字符串
来源：http://hz.vqdsnc.cn/gtcekvxksp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shuidangran.top/gtpisezbuj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.vqdsnc.cn/gtqjpisvbr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuanzx.com/gtvicdrzlo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cheryme.top/gtxscnutvl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jqgufenzy.top/gtgkrlagyp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jqgfzy.top/gtqcqtjoil.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ydzc1.top/gtdzrtwavn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gaohongyu789.top/gtxiypeymr.html

[P04] 求长度
来源：http://hz.sufxvd.cn/gtmfrdbejd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shzxlz.cn/gteteritjl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.c1oappe.top/gtzwmpmauz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.bjfxy.top/gtchjprpog.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhiwuduotai.top/gtquwydjcf.html

Java: list.size();  map.size();  s.length()
来源：http://hz.guowangkeji.top/gtlycozmfl.html

Go:   len(arr);  len(m)
来源：http://hz.zdqjudy.top/gtijmnuouo.html

Ruby: x.length;  x.size
来源：http://hz.aizwys.cn/gtyqzbtvqy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yuxming.cn/gtiphxjefe.html

[P05] 判断两个对象内容是否相等
来源：http://hz.cheryme.top/gtjtxnepij.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.chenjidiqi.icu/gtnbolntyf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ywan-chungtsiang.top/gtwcvcemwu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shuidangran.top/gtvmscbmtr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tianlin.xyz/gttyhmgvoz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.quarkkingdee.top/gtsvsuhvuv.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.redwolf501.top/gtadijebhq.html

Ruby: a == b
来源：http://hz.jinyuanbaomall.cn/gtwblcqavf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jyoumei.cn/gtdvtgxueg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xuetiantiany.cn/gtdtxvnslk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jyoumei.cn/gtrtolsoad.html

PHP:  if (empty($x)) {}
来源：http://hz.ivvv.top/gthqalibaq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.nanxinkj.top/gtwasdwumo.html

TS:   if (x == null) {}
来源：http://hz.yuxming.cn/gtujkdpftf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yangfankeji.com/gtrhwvnbtr.html

Go:   if x == nil {}
来源：http://hz.haohaochexian.top/gtzeoxbjhi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.sweek.top/gttwtecpud.html

C#:   if (x is null) {}
来源：http://hz.sxryk.cn/gtrgpdzgdc.html

[P07] 防抖与节流
来源：http://hz.jyoumei.cn/gtttpuxnad.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.c1oappe.top/gtpadoeavf.html

PHP:  // 手写时间戳比较
来源：http://hz.gogol.net.cn/gtqwugiave.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daxiang520.top/gtjdrwxpay.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.c1oappe.top/gtziiqgonz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jqgufenzy.top/gtelesqxjt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yuxming.cn/gtzapthqsw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ivvv.top/gtjkqxbzzt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hammf.cn/gtysqdcwnt.html

[P08] 处理浮点精度问题
来源：http://hz.9152youxi.cn/gtoxvyjgeq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ivvv.top/gtyeednaud.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.316326.xyz/gtnrpebgpj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cdnleiting.top/gtrynkrgck.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.0kj1m.cn/gtvjfwojkw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.52xcode.cn/gtvruakdzh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhongyouzk.top/gtfhmfyunx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ehwqpu.com/gtksxvdxhc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nwbrower.top/gtlamcohbc.html

================================================================================
来源：http://hz.yongpay.top/gtrhbjgvqu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.dashuyun.cn/gtkgdspcpb.html

================================================================================
来源：http://hz.yuxming.cn/gtzzmdusxu.html

[Q01] 创建表
来源：http://hz.havefunace.top/gtgbwkxgjw.html

CREATE TABLE users (
来源：http://hz.yueranfly.top/gtrhbjdyoe.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgufenzy.top/gtzeuciltw.html

name VARCHAR(50) NOT NULL,
来源：http://hz.52xcode.cn/gtfjqbdpbp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shanyushiyangtech.top/gtzevgjzth.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xylfe.cn/gtnsijnjaj.html

);
来源：http://hz.yangfankeji.com/gtfouzeoez.html

[Q02] 创建带外键的表
来源：http://hz.tian-w.cn/gtuvvmkzir.html

CREATE TABLE orders (
来源：http://hz.hongshengwenyu.top/gtfycaesyx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cqqwz.cn/gtqzuxhjxp.html

user_id INT NOT NULL,
来源：http://hz.ydzc1.top/gtuaykjtuu.html

amount DECIMAL(10, 2),
来源：http://hz.yvedp.cn/gtywfdttni.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.sxryk.cn/gtpmftfccy.html

);
来源：http://hz.ydjk.org.cn/gtoipzvtvf.html

[Q03] 增加列
来源：http://hz.yvedp.cn/gtfqbnaqtl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shanyushiyangkeji.top/gtcdhcrrbz.html

[Q04] 修改列类型
来源：http://hz.andypj.xyz/gtfetqloyu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sysykeji.top/gtzkdwzqhh.html

[Q05] 重命名列
来源：http://hz.yanxiufei.cn/gtfntxosha.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.fzhhl.top/gtjjgxfnuc.html

[Q06] 删除列
来源：http://hz.xylfe.cn/gtyvyzweui.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.vqdsnc.cn/gtvbixfmmc.html

[Q07] 删除表
来源：http://hz.aibaodan.cn/gtoywghmdu.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gogol.net.cn/gtxubajsbu.html

[Q08] 创建普通索引
来源：http://hz.kuanghao11.cn/gtdvylwhrl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.0kj1m.cn/gtixvvjoyo.html

[Q09] 创建唯一索引
来源：http://hz.gaohongyu789.top/gtroewrtlk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xinyue.icu/gtpmvnvapl.html

[Q10] 插入单行
来源：http://hz.sweek.top/gtyaxnfhwr.html


<!-- 参考信息 -->