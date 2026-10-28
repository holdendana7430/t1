代发 wailian999

JS:   process.exit(1)
来源：http://hz.chenzaomai.com/gtcufqvcnu.html

TS:   process.exit(1)
来源：http://hz.xinyue.icu/gtttajulsf.html

Java: System.exit(1)
来源：http://hz.daria6918.cn/gttaplgexc.html

Go:   os.Exit(1)
来源：http://hz.pengpengdd.cyou/gthamoebla.html

Ruby: exit 1
来源：http://hz.zycfv.cn/gtgkwpgyul.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.tian-w.cn/gtlyrtowcy.html

[M06] 向标准错误输出
来源：http://hz.shzxlz.cn/gtgjtsjxdj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.haohaochexian.top/gtrbwuilii.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.bjfxy.top/gtzajlyqhp.html

JS:   console.error("err")
来源：http://hz.9152youxi.cn/gthreoirtk.html

TS:   console.error("err")
来源：http://hz.pycfn.com/gtnkjrzpxc.html

Java: System.err.println("err")
来源：http://hz.jinqigufen.top/gtjtrtsiur.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shanyushiyangkeji.top/gtfufpetzt.html

Ruby: warn "err"
来源：http://hz.tian-w.cn/gtjyxnbmxm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.52xcode.cn/gtgopxvjyi.html

[M07] 判断是否为主入口
来源：http://hz.yonumen.top/gtuddlfhyc.html

Py:   if __name__ == "__main__":
来源：http://hz.gzhubu.top/gtdmydbmmy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhengqikj.top/gtoteovgth.html

JS:   require.main === module
来源：http://hz.svipenyu.cn/gtokvcdoun.html

TS:   require.main === module
来源：http://hz.hammf.cn/gtdfygbthj.html

Java: public static void main(String[] args)
来源：http://hz.birdmap.top/gtzmmabbgx.html

Go:   func main()
来源：http://hz.fzhhl.top/gtykcvrdad.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jqgfzy.top/gtengzpweb.html

C#:   static void Main(string[] args)
来源：http://hz.zhijiandao.cn/gtihzntshv.html

[M08] 获取系统与运行时信息
来源：http://hz.yanxiufei.cn/gteihxodgp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hywenlv.cn/gtoamsjmlq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jqgufenzy.top/gtmwazlrxt.html

JS:   process.platform;  process.version
来源：http://hz.ppjwa.cn/gthpmmvsil.html

TS:   process.platform;  process.version
来源：http://hz.zdqjudy.top/gtwywvwqtg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sufxvd.cn/gtnldticyo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.pengpengdd.cyou/gtdvuabqpe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hongshengwenyu.top/gtrwwvgpkk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.gzhubu.top/gtiolyhouy.html

================================================================================
来源：http://hz.gogol.net.cn/gtrjwxfsrz.html

N. 数据结构与算法
来源：http://hz.xuetiantiany.cn/gtwkyfceaw.html

================================================================================
来源：http://hz.yj20258888.top/gtqistzteh.html

[N01] 二分查找（有序数组）
来源：http://hz.sweek.top/gtejposiev.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gotoacloud.top/gtbsyyzsbb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shanyushiyangkeji.top/gtavzzydkw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sxryk.cn/gtauugyqpu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj202588.top/gtnztrhouc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtkfmjhlao.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xinyue.icu/gtryvfdlae.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yangfankeji.com/gtlqcsznqq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jqgufenzy.top/gtrbdjtmlt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ivvv.top/gtkcsyqghm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ehwqpu.com/gtxxhaxxac.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.c1oappe.top/gtmxvcrzue.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhiwuduotai.top/gtjftfcyql.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.andypj.xyz/gtktljezdm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cheryme.top/gtfnfnwmeo.html

Go:   slices.Sort(arr)
来源：http://hz.zhoulong.xyz/gtzzhhmmcz.html

Ruby: arr.sort
来源：http://hz.hywenlv.cn/gtgcwehtij.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hnqzz.top/gtxdejacof.html

[N03] 快速排序（分治示例）
来源：http://hz.shanyushiyangkeji.top/gtvoqrcwsu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yongpay.top/gtmujxtuqe.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yj202588.top/gtkzgeifoh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenlongwang.top/gtbrrpdmhp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhongyouzk.top/gtegpraycj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xylfe.cn/gtpxgoyxxk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.havefunace.top/gtzbtqeyqd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hywenlv.cn/gtvnhfadvh.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jlsjyb.cn/gttrtsrigw.html

[N04] 斐波那契数列
来源：http://hz.52xcode.cn/gtxlaisigg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ydzc1.top/gtavidrolr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jianghu66.top/gtsptezztk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxinkj.top/gtvcryrnxr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xuanzx.com/gtrtvmfbwu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sweek.top/gtgykqxyqx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.nanxinkj.top/gtgcniyspq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.aibaodan.cn/gtcnijqeqo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yongpay.top/gtlmggeawp.html

[N05] 最大公约数
来源：http://hz.pycfn.com/gtbhxsfgef.html

Py:   math.gcd(a, b)
来源：http://hz.cqqwz.cn/gtagpssvqs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jianghu66.top/gtqhdfmlce.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sufxvd.cn/gtejagvqel.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cashguo.top/gtkaekzzxq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jinqigfzy.top/gttgnzmrle.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yj20258888.top/gtzxlqwidc.html

Ruby: a.gcd(b)
来源：http://hz.zhiwuduotai.top/gtceodczwx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gzhubu.top/gtkidfxjyq.html

[N06] 判断回文字符串
来源：http://hz.nanxuanxn.top/gttwbfiehr.html

Py:   s == s[::-1]
来源：http://hz.hysaishi.cn/gtcgkwnjqe.html

PHP:  $s === strrev($s);
来源：http://hz.shuidangran.top/gtxgdausqk.html

JS:   s === [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtcabjifed.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtuektbmih.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jiagoushi.top/gtlmbrzcwb.html

Go:   // 双指针从两端比较
来源：http://hz.ehwqpu.com/gtfmtttvok.html

Ruby: s == s.reverse
来源：http://hz.haohaochexian.top/gtgswtsmpd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.316326.xyz/gtclxwkxfk.html

[N07] 两数之和（返回下标）
来源：http://hz.quarkkingdee.top/gtdkgbccak.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yuanzhike.top/gttpzatusc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.nwbrower.top/gtljrlimft.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.fzhhl.top/gtcusdlqru.html

TS:   // 手写 Map<string, number>
来源：http://hz.sxryk.cn/gtocghscwa.html

Java: // 手写 HashMap
来源：http://hz.9152youxi.cn/gtmmlfafbv.html

Go:   // 手写 map[int]int
来源：http://hz.jiagoushi.top/gtffhamjzo.html

Ruby: // 手写 Hash
来源：http://hz.svipenyu.cn/gtibnrrulf.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhijiandao.cn/gtuyoyimnq.html

[N08] 生成全排列
来源：http://hz.hnxiangtu.top/gthwocnosx.html

Py:   itertools.permutations(arr)
来源：http://hz.chenjidiqi.icu/gtegultrki.html

PHP:  // 手写递归交换
来源：http://hz.cucudq.cn/gtwtpasgma.html

JS:   // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtvauteqmb.html

TS:   // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtgcdltnkq.html

Java: // 手写回溯递归
来源：http://hz.bjfxy.top/gtynzoobuj.html

Go:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtnqhljeld.html

Ruby: arr.permutation.to_a
来源：http://hz.fzhhl.top/gtsmmibqke.html

C#:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtovnpmesv.html

[N09] 栈与队列
来源：http://hz.wangshuangyany.cn/gtvajwbwyh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.vqdsnc.cn/gtvweqeyuw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.chenlongwang.top/gtjoqdtnze.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.pengpengdd.cyou/gtnnwwwbac.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj202588.top/gtjvnaxwvi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhaomingkeji.xyz/gtuoeekwyw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.fzhhl.top/gtkrirunli.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.vqdsnc.cn/gtbtubazzd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gzhubu.top/gtpiabrfui.html

[N10] 链表节点定义
来源：http://hz.xinyue.icu/gtnbinmoor.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.meibo888.top/gtemhhgmfg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.daria6918.cn/gtbyjfgmbt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.aibaodan.cn/gtoulttvot.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhoulong.xyz/gtkbohuupl.html

Java: class Node { int v; Node next; }
来源：http://hz.shzxlz.cn/gthqrwfuav.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ybcxt.top/gtbpivpgia.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zycfv.cn/gtvhjupzuc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yj202588.top/gtqdsbnzje.html

[N11] 二叉树中序遍历
来源：http://hz.nwbrower.top/gtkzvdqolf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhaomingkeji.xyz/gtbiznnpek.html

PHP:  // 手写递归函数
来源：http://hz.yuxming.cn/gtdlmgnwwb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cucudq.cn/gtkiuvaswe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydzc1.top/gtacnhwuio.html

Java: // 手写递归
来源：http://hz.cqqwz.cn/gtpfyxbkvr.html

Go:   // 手写递归
来源：http://hz.hnxiangtu.top/gtoukclkwg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jqgfzy.top/gtrkhccqgq.html

C#:   // 手写递归
来源：http://hz.snrcjt.cn/gtqhmatpqy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.wangshuangyany.cn/gtxntogxvf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.feifeiyinyue.top/gtvejfzmum.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhaomingkeji.xyz/gtsujfpkoe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangkeji.top/gtrzecouav.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jlsjyb.cn/gtbjloinbh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hnxiangtu.top/gttmkwsadr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jinqigfzy.top/gtrcvmdrgk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.chenjidiqi.icu/gtwzdiaork.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guowangkeji.top/gtaekdemxi.html

================================================================================
来源：http://hz.hywenlv.cn/gtpeeydsmq.html

O. 并发与异步
来源：http://hz.yuanzhike.top/gtlfkcwzrx.html

================================================================================
来源：http://hz.tianlin.xyz/gtlwzxilzt.html

[O01] 启动一个线程
来源：http://hz.daxiang520.top/gtoozzdkdb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhaomingkeji.xyz/gtuwusxhld.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinqigfzy.top/gtdjhauvkv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.pycfn.com/gtdxaifzij.html

TS:   // 同 JS
来源：http://hz.feifeiyinyue.top/gtbycjbkbq.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhongyouzk.top/gtpvwtaers.html

Go:   go f()
来源：http://hz.shanyushiyangkeji.top/gtnaqrkjbr.html

Ruby: Thread.new { f }
来源：http://hz.yj20258888.top/gthmriimkp.html

C#:   Task.Run(() => F());
来源：http://hz.shzxlz.cn/gtxvrqmjam.html

[O02] 使用线程池
来源：http://hz.ehwqpu.com/gtzslbovio.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.svipenyu.cn/gtmaahjepj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.mhx1999.top/gtibedmmir.html

JS:   // worker_threads 线程池
来源：http://hz.guannengcc.top/gtbnavicts.html

TS:   // worker_threads 线程池
来源：http://hz.ehwqpu.com/gtdpetrnbo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinghuilouyu.cn/gtuvpdbkic.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xingfuxueyuan.xyz/gtyqrwnmpb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ppjwa.cn/gtvqlboqpk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.kuanghao11.cn/gtzskbcxdu.html

[O03] 加锁保护共享数据
来源：http://hz.cdnleiting.top/gtllvvcwkr.html

Py:   with lock: shared += 1
来源：http://hz.yueranfly.top/gtgsqqegra.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.nwbrower.top/gtxyinlyjz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yj202588.top/gtdqdagetm.html

TS:   // 同 JS
来源：http://hz.jlsjyb.cn/gtiyfpbkuq.html

Java: synchronized (this) { shared++; }
来源：http://hz.fengsongda.top/gtqzqkyosj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yongpay.top/gtuftmtgra.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.fengsongda.top/gttkehbypg.html

C#:   lock (gate) { shared++; }
来源：http://hz.shanyushiyangtech.top/gtsvvafotu.html

[O04] 定义异步函数并等待
来源：http://hz.zycfv.cn/gtrazpvvth.html

Py:   async def f():⏎    await g()
来源：http://hz.sysykeji.top/gtyqnuqsdi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yangfankeji.com/gtbtstmypi.html

JS:   async function f() { await g(); }
来源：http://hz.yvedp.cn/gtdlkxmsso.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yongpay.top/gtocppgbtx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yuxming.cn/gtkdjvnllg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yj20258.top/gtbavmlrsq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yangfankeji.com/gtsjnbnxnz.html

C#:   async Task F() { await G(); }
来源：http://hz.jyoumei.cn/gtjelypnte.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinghuilouyu.cn/gtjnvsymta.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenzaomai.com/gttnqgpqkp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.0kj1m.cn/gtlxvgqpmd.html

JS:   await Promise.all(tasks)
来源：http://hz.cashguo.top/gtgtjzlgas.html

TS:   await Promise.all(tasks)
来源：http://hz.jqgufenzy.top/gtdmekqvow.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.meibo888.top/gtsnzrnqhe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.c1oappe.top/gtdkxvdxfv.html

Ruby: threads.map(&:join)
来源：http://hz.dianchejie.cn/gtfryqssly.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.nanxuanxn.top/gtvitvoeny.html

[O06] 使用进程池
来源：http://hz.nwbrower.top/gtdjluwcdy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ivvv.top/gtbpmkxpdn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yj20258888.top/gtwnruluwe.html

JS:   // child_process / cluster 模块
来源：http://hz.yueranfly.top/gtraqiuuhl.html

TS:   // child_process / cluster 模块
来源：http://hz.yuxming.cn/gtkelrocoz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.birdmap.top/gtyullbakc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhijiandao.cn/gtrcywhixo.html

Ruby: // fork 块
来源：http://hz.aizwys.cn/gtruhbgkit.html

C#:   Parallel.For
来源：http://hz.fzhhl.top/gtpmqocufq.html

================================================================================
来源：http://hz.shuidangran.top/gtxqhdnpkn.html

P. 常用工具函数
来源：http://hz.9152youxi.cn/gtcxndravy.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtkvzvykjl.html

[P01] 生成 UUID
来源：http://hz.gogol.net.cn/gtnnzzqypb.html

Py:   str(uuid.uuid4())
来源：http://hz.sufxvd.cn/gtyoosketx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xingfuxueyuan.xyz/gtbzeglpcp.html

JS:   crypto.randomUUID()
来源：http://hz.xuanzx.com/gtmnnmoglr.html

TS:   crypto.randomUUID()
来源：http://hz.shanyushiyangtech.top/gtmcufwwek.html

Java: UUID.randomUUID().toString()
来源：http://hz.shanyushiyangtech.top/gtaizajalf.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj202588.top/gtioohsfee.html

Ruby: SecureRandom.uuid
来源：http://hz.kuanghao11.cn/gtdvuanpql.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.mhx1999.top/gtsqvsfdzr.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yueranfly.top/gtzspugbui.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenjidiqi.icu/gtbvkwnedp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.snrcjt.cn/gterswohvj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xinyue.icu/gtdtxivtiy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hnqzz.top/gtczmbegss.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.tianlin.xyz/gttxwcvnja.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.52xcode.cn/gtloxhtzpd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jianghu66.top/gtiydpzlfi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.kuanghao11.cn/gtzcaaqucj.html

[P03] 生成短随机字符串
来源：http://hz.hnqzz.top/gtemmmmfck.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sufxvd.cn/gtbzhycsmz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hfpthk.cn/gtvijpbnws.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydjk.org.cn/gtsnfkxhzf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.birdmap.top/gtsbrmvljy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ppjwa.cn/gtwlwpybgp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.52xcode.cn/gtyrssvrsy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ehwqpu.com/gthwdyhnet.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.sweek.top/gtzatudbpd.html

[P04] 求长度
来源：http://hz.shanyushiyangkeji.top/gtqgxfgrbz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jinqigufen.top/gtztdjvzrs.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guowangkeji.top/gtsetzrozu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.316326.xyz/gtpgmkhfns.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jianghu66.top/gtrxwlpefi.html

Java: list.size();  map.size();  s.length()
来源：http://hz.tanke756.top/gtojbhuisb.html

Go:   len(arr);  len(m)
来源：http://hz.havefunace.top/gtticgxjew.html

Ruby: x.length;  x.size
来源：http://hz.tian-w.cn/gtgodwhpif.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shanyushiyangkeji.top/gtmujvngit.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yongpay.top/gtzkforrdy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jinyuanbaomall.cn/gthxmyxohd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jqgfzy.top/gtgxmpemju.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenjidiqi.icu/gtbzgrshrk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.fengsongda.top/gtpeyukhzx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhengqikj.top/gtgrzkyhzo.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jinghuilouyu.cn/gtlugsjdry.html

Ruby: a == b
来源：http://hz.zdqjudy.top/gtkznmtjko.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ivvv.top/gterfwcgkl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jqgfzy.top/gtmcfytjop.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.fengsongda.top/gtrzjobcti.html

PHP:  if (empty($x)) {}
来源：http://hz.zhengqikj.top/gtalmlirbq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yvedp.cn/gtwcgrfsci.html

TS:   if (x == null) {}
来源：http://hz.hywenlv.cn/gtkpgsnyon.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jqgufenzy.top/gtkdqcmfay.html

Go:   if x == nil {}
来源：http://hz.hnqzz.top/gtuvdrxiow.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.mhx1999.top/gtzsxffrbh.html

C#:   if (x is null) {}
来源：http://hz.wangshuangyany.cn/gtgctfvcqx.html

[P07] 防抖与节流
来源：http://hz.tian-w.cn/gtixdhxgon.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yvedp.cn/gtbpnvtefn.html

PHP:  // 手写时间戳比较
来源：http://hz.zhixingplan.top/gtdmpjwobq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cucudq.cn/gtlmsuhqyg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sxryk.cn/gtmbckluxo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hywenlv.cn/gttbbqbhzn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.daria6918.cn/gtbnthfnqv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.iojbl.cn/gtutlpxiab.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.quarkkingdee.top/gtbdbsyjen.html

[P08] 处理浮点精度问题
来源：http://hz.hfpthk.cn/gtbgrxcdym.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhiwuduotai.top/gtcgvrjhut.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.vqdsnc.cn/gtxaxunfyl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gotoacloud.top/gtwfhbqwsc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jinqigfzy.top/gtrdosjdtz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.sweek.top/gtwtlvuwzn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.bjfxy.top/gtwpwhoyuf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.nwbrower.top/gtmukpmwpo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cheryme.top/gtqxhhllfe.html

================================================================================
来源：http://hz.nanxinkj.top/gtwfvczflm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.feifeiyinyue.top/gtsfjdupoi.html

================================================================================
来源：http://hz.9152youxi.cn/gtuvsoftbf.html

[Q01] 创建表
来源：http://hz.9152youxi.cn/gtilatjlmk.html

CREATE TABLE users (
来源：http://hz.mhx1999.top/gtbvklhrii.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.iojbl.cn/gtydfxojqj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.vqdsnc.cn/gtgmlcplkd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jqgfzy.top/gtctyzljuy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.snrcjt.cn/gtxlcthkal.html

);
来源：http://hz.jlsjyb.cn/gtwobwtdsv.html

[Q02] 创建带外键的表
来源：http://hz.yonumen.top/gtyhpidqrw.html

CREATE TABLE orders (
来源：http://hz.sysykeji.top/gtzmkonyaw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.pengpengdd.cyou/gtmusnfgup.html

user_id INT NOT NULL,
来源：http://hz.xuetiantiany.cn/gtzwscitxr.html

amount DECIMAL(10, 2),
来源：http://hz.tian-w.cn/gtigvwamos.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hfpthk.cn/gtdicrpdrx.html

);
来源：http://hz.yuxming.cn/gtqkmgirmm.html

[Q03] 增加列
来源：http://hz.jyoumei.cn/gtdzxirzcf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xuanzx.com/gteagtcttr.html

[Q04] 修改列类型
来源：http://hz.9152youxi.cn/gttuhnvsha.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.aibaodan.cn/gtiwxcsxrt.html

[Q05] 重命名列
来源：http://hz.ydjk.org.cn/gtzglujaxn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.aibaodan.cn/gtdodlflnc.html

[Q06] 删除列
来源：http://hz.ppjwa.cn/gtgslmsnzh.html


<!-- 参考信息 -->