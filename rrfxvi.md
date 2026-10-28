代发 wailian999

TS:   process.cwd()
来源：http://hz.xziqi.cn/gtgrjoxvdq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhaomingkeji.xyz/gtrworpczx.html

Go:   os.Getwd()
来源：http://hz.nanxinkj.top/gthcspsayz.html

Ruby: Dir.pwd
来源：http://hz.dianchejie.cn/gtoeiztipz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cdnleiting.top/gttitilsbf.html

[M05] 设置退出码
来源：http://hz.aibaodan.cn/gtxysjsyth.html

Py:   sys.exit(1)
来源：http://hz.cucudq.cn/gtaxydoufm.html

PHP:  exit(1);
来源：http://hz.ppjwa.cn/gthaaocrqy.html

JS:   process.exit(1)
来源：http://hz.sysykeji.top/gtxjkwwqth.html

TS:   process.exit(1)
来源：http://hz.jqgufenzy.top/gtfmsckjha.html

Java: System.exit(1)
来源：http://hz.andypj.xyz/gtrujssfxn.html

Go:   os.Exit(1)
来源：http://hz.smart0.xyz/gtstjwtoym.html

Ruby: exit 1
来源：http://hz.tian-w.cn/gtmjxpliba.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.chenjidiqi.icu/gtnbhvvlqd.html

[M06] 向标准错误输出
来源：http://hz.chenlongwang.top/gttmumdhoy.html

Py:   print("err", file=sys.stderr)
来源：http://hz.birdmap.top/gtqveznzjm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zycfv.cn/gtnrntmfqw.html

JS:   console.error("err")
来源：http://hz.gzhubu.top/gtjijxoclm.html

TS:   console.error("err")
来源：http://hz.zdqjudy.top/gtluctxect.html

Java: System.err.println("err")
来源：http://hz.cqqwz.cn/gtntwacjtl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ehwqpu.com/gtfmlkdinw.html

Ruby: warn "err"
来源：http://hz.yuxming.cn/gtgtsaedns.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.sysykeji.top/gtlefmwdsh.html

[M07] 判断是否为主入口
来源：http://hz.chenjidiqi.icu/gtwdkjlffs.html

Py:   if __name__ == "__main__":
来源：http://hz.nanxinkj.top/gtomscuftg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yongpay.top/gtaeplyxug.html

JS:   require.main === module
来源：http://hz.cdnleiting.top/gtrobwpkif.html

TS:   require.main === module
来源：http://hz.cqqwz.cn/gtlxufohxb.html

Java: public static void main(String[] args)
来源：http://hz.nanxinkj.top/gtiajezeex.html

Go:   func main()
来源：http://hz.jqgufenzy.top/gtwcefunza.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.nwbrower.top/gtvimrxjjg.html

C#:   static void Main(string[] args)
来源：http://hz.redwolf501.top/gtysvuvihm.html

[M08] 获取系统与运行时信息
来源：http://hz.shanyushiyangtech.top/gtdxxucujt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xingfuxueyuan.xyz/gtbvdifhcx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yvedp.cn/gttwkgbmnv.html

JS:   process.platform;  process.version
来源：http://hz.sufxvd.cn/gtwelklqpu.html

TS:   process.platform;  process.version
来源：http://hz.havefunace.top/gtelddvojd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shzxlz.cn/gthafyysyo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.iojbl.cn/gtsqmghkrc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.nanxinkj.top/gtgizrhrig.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.nanxinkj.top/gtxdgzgfou.html

================================================================================
来源：http://hz.nanxinkj.top/gtogfdlbyv.html

N. 数据结构与算法
来源：http://hz.quarkkingdee.top/gtnujuubyj.html

================================================================================
来源：http://hz.shuidangran.top/gtkgoxpbuc.html

[N01] 二分查找（有序数组）
来源：http://hz.pengpengdd.cyou/gtutsuqugp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj202588.top/gtczmtqeoj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhengqikj.top/gtzlbntbpw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.bjfxy.top/gtylsjuvjy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhoulong.xyz/gtkicsxpfx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.dianchejie.cn/gtbkdiulem.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.nanxinkj.top/gtwkeekoli.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhaomingkeji.xyz/gtwezovpjq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zycfv.cn/gtilyqumgk.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.fzhhl.top/gtzkmpfuoh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.havefunace.top/gtjdswzpht.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cucudq.cn/gtnhchnlmj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.0kj1m.cn/gtustoqyhu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinqigfzy.top/gthrhzfivt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.gzhubu.top/gtnehnzvwt.html

Go:   slices.Sort(arr)
来源：http://hz.zhixingplan.top/gtlliqcnpp.html

Ruby: arr.sort
来源：http://hz.wangshuangyany.cn/gtufaiiefj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ppjwa.cn/gtrybakelh.html

[N03] 快速排序（分治示例）
来源：http://hz.bjfxy.top/gtdwbdsecq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.kuanghao11.cn/gtvmvoscyx.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nwbrower.top/gtvxnaavab.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ehwqpu.com/gtelgbvikq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jiagoushi.top/gtagatyaut.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.aibaodan.cn/gtspbwtalm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cqqwz.cn/gtlkjzfmdt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.dashuyun.cn/gtkchstzzd.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shuidangran.top/gtlflcxxwq.html

[N04] 斐波那契数列
来源：http://hz.guowangkeji.top/gtwfublekj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.c1oappe.top/gtqketcjkh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.wangshuangyany.cn/gtwzliuvsb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hfpthk.cn/gthwkkesmn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fzhhl.top/gtzmgzsyto.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.feifeiyinyue.top/gtjjibfytc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.daxiang520.top/gtzidqarbd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhiwuduotai.top/gtdrpqfvsk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.svipenyu.cn/gtfhzshytk.html

[N05] 最大公约数
来源：http://hz.sweek.top/gtdwnxljyr.html

Py:   math.gcd(a, b)
来源：http://hz.yanxiufei.cn/gtcrqpnmrl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.wangshuangyany.cn/gtporxttli.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgufenzy.top/gtmyacagbt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.mhx1999.top/gtrxinawha.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ybcxt.top/gtgtmthrsf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.pengpengdd.cyou/gtrmodbhoz.html

Ruby: a.gcd(b)
来源：http://hz.ivvv.top/gterqpwzpf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.iojbl.cn/gtjixqglfo.html

[N06] 判断回文字符串
来源：http://hz.52xcode.cn/gtwgqbaeup.html

Py:   s == s[::-1]
来源：http://hz.0kj1m.cn/gtbpsszkoy.html

PHP:  $s === strrev($s);
来源：http://hz.birdmap.top/gtzxvalrsv.html

JS:   s === [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtgvvukbce.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gzhubu.top/gthktloezm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.haohaochexian.top/gtzltrxjub.html

Go:   // 双指针从两端比较
来源：http://hz.kuanghao11.cn/gtzetwvogl.html

Ruby: s == s.reverse
来源：http://hz.chenzaomai.com/gtzopwhwts.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tian-w.cn/gtgvqupxec.html

[N07] 两数之和（返回下标）
来源：http://hz.gogol.net.cn/gtrkspyscn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hysaishi.cn/gtgloylszk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cashguo.top/gtehqpwtvf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinghuilouyu.cn/gtoxttbjvg.html

TS:   // 手写 Map<string, number>
来源：http://hz.hfpthk.cn/gtzehhmucn.html

Java: // 手写 HashMap
来源：http://hz.xylfe.cn/gtebxoznar.html

Go:   // 手写 map[int]int
来源：http://hz.xinyue.icu/gtorpyoqsk.html

Ruby: // 手写 Hash
来源：http://hz.gzhubu.top/gtiafbdbne.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shanyushiyangtech.top/gttbwpgoaq.html

[N08] 生成全排列
来源：http://hz.tanke756.top/gtnlfmecvx.html

Py:   itertools.permutations(arr)
来源：http://hz.ivvv.top/gtnjutclua.html

PHP:  // 手写递归交换
来源：http://hz.yj202588.top/gtxqvlxdbs.html

JS:   // 手写回溯递归
来源：http://hz.zycfv.cn/gttkowcazq.html

TS:   // 手写回溯递归
来源：http://hz.tianlin.xyz/gtbibspebd.html

Java: // 手写回溯递归
来源：http://hz.andypj.xyz/gtslzuspra.html

Go:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtjzppacpj.html

Ruby: arr.permutation.to_a
来源：http://hz.zdqjudy.top/gtdotpoqwv.html

C#:   // 手写回溯递归
来源：http://hz.birdmap.top/gttfpjsgxk.html

[N09] 栈与队列
来源：http://hz.gaohongyu789.top/gtfquagzul.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.redwolf501.top/gtweoxpzyt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.bjfxy.top/gtopmmcedc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhijiandao.cn/gtsrnfaojz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yueranfly.top/gtagimthhr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinyuanbaomall.cn/gtffmnbinv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shanyushiyangtech.top/gtlrsfovco.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shanyushiyangkeji.top/gtvqyglmev.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jianghu66.top/gtxiqoxczd.html

[N10] 链表节点定义
来源：http://hz.jinqigufen.top/gtjmduhkym.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.dashuyun.cn/gtybymeieo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.smart0.xyz/gtxsenjnzf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xuanzx.com/gtizuwwiqa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jinyuanbaomall.cn/gtaowplzgh.html

Java: class Node { int v; Node next; }
来源：http://hz.shanyushiyangtech.top/gthjlpphak.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.dianchejie.cn/gtqouidjou.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinqigufen.top/gtdihmvphe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yvedp.cn/gtlhybbbwe.html

[N11] 二叉树中序遍历
来源：http://hz.yongpay.top/gtoahqpirc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yueranfly.top/gtolepnayk.html

PHP:  // 手写递归函数
来源：http://hz.dashuyun.cn/gttpxvihwi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tian-w.cn/gtvapevast.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cucudq.cn/gtuyaewugb.html

Java: // 手写递归
来源：http://hz.guowangkeji.top/gteqlunhsg.html

Go:   // 手写递归
来源：http://hz.ivvv.top/gtvtkamiec.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.sufxvd.cn/gtxcuzevyu.html

C#:   // 手写递归
来源：http://hz.jyoumei.cn/gtrgayucbq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yj20258.top/gtwklckadv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shanyushiyangkeji.top/gttbefoums.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ehwqpu.com/gtfggzqpxp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jyoumei.cn/gtvvewcsfj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuanzx.com/gtzovflmgg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zycfv.cn/gtbhsnlsxo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.gaohongyu789.top/gtwalbuccy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cdnleiting.top/gttzcjuuhq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ybcxt.top/gtjvwklakg.html

================================================================================
来源：http://hz.yongpay.top/gtiahcszal.html

O. 并发与异步
来源：http://hz.shangyingyoupin.top/gtsixmdbgy.html

================================================================================
来源：http://hz.sweek.top/gtwggrtggw.html

[O01] 启动一个线程
来源：http://hz.daria6918.cn/gtnpucazqx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ybcxt.top/gtzcsmikmx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinqigufen.top/gtmzjkumya.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fzhhl.top/gtiypoaecx.html

TS:   // 同 JS
来源：http://hz.jyoumei.cn/gtqakdadgr.html

Java: new Thread(() -> f()).start()
来源：http://hz.chenzaomai.com/gtgxejsksj.html

Go:   go f()
来源：http://hz.zhoulong.xyz/gtaqnxbjeq.html

Ruby: Thread.new { f }
来源：http://hz.9152youxi.cn/gtyxqlkfzf.html

C#:   Task.Run(() => F());
来源：http://hz.chenjidiqi.icu/gtuqvopsqt.html

[O02] 使用线程池
来源：http://hz.jinqigfzy.top/gtmkzqgney.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yangfankeji.com/gtinwiteqm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhijiandao.cn/gtyehqfsbs.html

JS:   // worker_threads 线程池
来源：http://hz.zhijiandao.cn/gtpwlgurzc.html

TS:   // worker_threads 线程池
来源：http://hz.ppjwa.cn/gtvfalvhyf.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ppjwa.cn/gtdclukdko.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shanyushiyangkeji.top/gtncxqqjkz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ppjwa.cn/gtqdljvzow.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.dianchejie.cn/gtciosmfpw.html

[O03] 加锁保护共享数据
来源：http://hz.tianlin.xyz/gtkiueuhwp.html

Py:   with lock: shared += 1
来源：http://hz.shanyushiyangtech.top/gtfbuaazqd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.iojbl.cn/gthfagkmrv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.haohaochexian.top/gtsxuuxdxx.html

TS:   // 同 JS
来源：http://hz.ybcxt.top/gtvtvrbdsx.html

Java: synchronized (this) { shared++; }
来源：http://hz.9152youxi.cn/gtflpxekcd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.aibaodan.cn/gtlkmuyebg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ydjk.org.cn/gttpynfqep.html

C#:   lock (gate) { shared++; }
来源：http://hz.aibaodan.cn/gtaukjgoln.html

[O04] 定义异步函数并等待
来源：http://hz.shzxlz.cn/gtsuzlkfnv.html

Py:   async def f():⏎    await g()
来源：http://hz.yuxming.cn/gtgkopnrve.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.havefunace.top/gttrkvleyo.html

JS:   async function f() { await g(); }
来源：http://hz.tian-w.cn/gtcdvfflvy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cashguo.top/gtsmbzmrar.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.52xcode.cn/gtdtmcemzl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jqgfzy.top/gtdeokauum.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.haohaochexian.top/gtofsmlubw.html

C#:   async Task F() { await G(); }
来源：http://hz.wangshuangyany.cn/gtzpqznidi.html

[O05] 并发执行并等待全部完成
来源：http://hz.kuanghao11.cn/gtsewsfgld.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cashguo.top/gtykeujekp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.guannengcc.top/gtrxwapryn.html

JS:   await Promise.all(tasks)
来源：http://hz.svipenyu.cn/gtmmtjpvzd.html

TS:   await Promise.all(tasks)
来源：http://hz.yj20258888.top/gtzauozmau.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yongpay.top/gtgsawqrww.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hysaishi.cn/gtfchamplt.html

Ruby: threads.map(&:join)
来源：http://hz.ehwqpu.com/gtvpqmtnnc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xuanzx.com/gtghhucnoa.html

[O06] 使用进程池
来源：http://hz.fzhhl.top/gtixfvwjnj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hnxiangtu.top/gtrubmztxi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.redwolf501.top/gtiilnlejn.html

JS:   // child_process / cluster 模块
来源：http://hz.mhx1999.top/gtlpbpdgfj.html

TS:   // child_process / cluster 模块
来源：http://hz.ppjwa.cn/gttenwwgyr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hywenlv.cn/gtsexnpofp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.haohaochexian.top/gtddoptmfg.html

Ruby: // fork 块
来源：http://hz.aizwys.cn/gtdwyxtovc.html

C#:   Parallel.For
来源：http://hz.gzhubu.top/gtntltwoxv.html

================================================================================
来源：http://hz.ydzc1.top/gtypnacjlf.html

P. 常用工具函数
来源：http://hz.sufxvd.cn/gtxfdmekry.html

================================================================================
来源：http://hz.jyoumei.cn/gtglckyieh.html

[P01] 生成 UUID
来源：http://hz.cheryme.top/gthvcooplq.html

Py:   str(uuid.uuid4())
来源：http://hz.vqdsnc.cn/gtelcisosy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinqigfzy.top/gtqqdedtep.html

JS:   crypto.randomUUID()
来源：http://hz.cashguo.top/gtczqkhurg.html

TS:   crypto.randomUUID()
来源：http://hz.jyoumei.cn/gtxdygrxtg.html

Java: UUID.randomUUID().toString()
来源：http://hz.dashuyun.cn/gtfpulhtgx.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj20258.top/gtxoubdrkk.html

Ruby: SecureRandom.uuid
来源：http://hz.aibaodan.cn/gtlrvyrexm.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hysaishi.cn/gtgkjwxfkr.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sufxvd.cn/gtcrwmzruz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sysykeji.top/gtvvefpkqx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.sysykeji.top/gtqkvwiueq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.0kj1m.cn/gtwjkngujt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yongpay.top/gtrnvshgle.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.kuanghao11.cn/gtzxwrxdyr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yvedp.cn/gtmvtjoveh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.quarkkingdee.top/gtojfxvqic.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ppjwa.cn/gtdtqhqemp.html

[P03] 生成短随机字符串
来源：http://hz.wangdashe.top/gtqvgrchdf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cheryme.top/gtbslkdvlp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yj20258888.top/gtijeorjag.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shangyingyoupin.top/gtcofebfwy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhongyouzk.top/gtnomcikrq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shanyushiyangkeji.top/gtlxbyfgwu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yangfankeji.com/gtwvvsnbcy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.tianlin.xyz/gtzjtcibnh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cdnleiting.top/gtdzgqftoe.html

[P04] 求长度
来源：http://hz.feifeiyinyue.top/gtfqqwfyok.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.smart0.xyz/gtddvpshpq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.quarkkingdee.top/gtyigwscwq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xinyue.icu/gtrbiwlcko.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ehwqpu.com/gtbbrddbqo.html

Java: list.size();  map.size();  s.length()
来源：http://hz.guannengcc.top/gtylzocblo.html

Go:   len(arr);  len(m)
来源：http://hz.hnqzz.top/gtvervgylw.html

Ruby: x.length;  x.size
来源：http://hz.tanke756.top/gteybhqzus.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jinqigfzy.top/gtdbebzljn.html

[P05] 判断两个对象内容是否相等
来源：http://hz.svipenyu.cn/gtmdnquhvt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yj20258888.top/gtfqnzkzkm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.316326.xyz/gtugbtnwrn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenzaomai.com/gtpskhsfde.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenjidiqi.icu/gtnlhgrovf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhaomingkeji.xyz/gtdylokcwo.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.meibo888.top/gttjoaucys.html

Ruby: a == b
来源：http://hz.aibaodan.cn/gtyktmsptx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.wangshuangyany.cn/gtnqfukhsy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.dianchejie.cn/gtkpytggfd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.tian-w.cn/gtynmmcwxr.html

PHP:  if (empty($x)) {}
来源：http://hz.hfpthk.cn/gtdguqjbav.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ppjwa.cn/gttwtzxbia.html

TS:   if (x == null) {}
来源：http://hz.cqqwz.cn/gtvzwejxie.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.dashuyun.cn/gthvegqfzk.html

Go:   if x == nil {}
来源：http://hz.sxryk.cn/gtkopeuumd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.316326.xyz/gteanvhjta.html

C#:   if (x is null) {}
来源：http://hz.0kj1m.cn/gthndqiaik.html

[P07] 防抖与节流
来源：http://hz.shanyushiyangtech.top/gtplijtjxo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jianghu66.top/gtslsfdzip.html

PHP:  // 手写时间戳比较
来源：http://hz.shuidangran.top/gteyjcmjok.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.birdmap.top/gtoelsvovs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.kuanghao11.cn/gtmbkvugxi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.tian-w.cn/gtpheeaeeh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hysaishi.cn/gtqxuwzhts.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.andypj.xyz/gtsncyilvb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yvedp.cn/gtyqynguek.html

[P08] 处理浮点精度问题
来源：http://hz.chenzaomai.com/gtiftakxcg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cheryme.top/gtwihwddda.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hfpthk.cn/gtkszdvrkk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hysaishi.cn/gtuumrrwiv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hysaishi.cn/gtjbmfyyko.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ppjwa.cn/gtlubpomhn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jyoumei.cn/gtqicazipp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dashuyun.cn/gtsviijhpk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nanxinkj.top/gtkrthfvpb.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtjlddthjz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yongpay.top/gtjblgpkaz.html

================================================================================
来源：http://hz.snrcjt.cn/gtagsbskoe.html

[Q01] 创建表
来源：http://hz.tian-w.cn/gtyqmgaibc.html

CREATE TABLE users (
来源：http://hz.jiagoushi.top/gtahsrpwep.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aizwys.cn/gtsgtirqhg.html

name VARCHAR(50) NOT NULL,
来源：http://hz.daxiang520.top/gtaudndkbb.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yueranfly.top/gtczbxdszp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shanyushiyangkeji.top/gtjxyqutoa.html

);
来源：http://hz.jinqigfzy.top/gtiqjypdhh.html

[Q02] 创建带外键的表
来源：http://hz.sysykeji.top/gtpkykuklq.html

CREATE TABLE orders (
来源：http://hz.c1oappe.top/gtfqjravas.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dashuyun.cn/gtjcksedyr.html

user_id INT NOT NULL,
来源：http://hz.0kj1m.cn/gthtwqrcrk.html

amount DECIMAL(10, 2),
来源：http://hz.fzhhl.top/gtgkeykgge.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ivvv.top/gthxhgjiqm.html


<!-- 参考信息 -->