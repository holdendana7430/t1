代发 wailian999

[M04] 获取当前工作目录
来源：http://hz.zdqjudy.top/gtcmsjxtef.html

Py:   os.getcwd()
来源：http://hz.zhijiandao.cn/gtshnlmhmy.html

PHP:  getcwd();
来源：http://hz.yangfankeji.com/gtphocjhoe.html

JS:   process.cwd()
来源：http://hz.gogol.net.cn/gtkowlxeud.html

TS:   process.cwd()
来源：http://hz.shanyushiyangkeji.top/gthojuqctr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ppjwa.cn/gtoeiincck.html

Go:   os.Getwd()
来源：http://hz.yueranfly.top/gtarjwphim.html

Ruby: Dir.pwd
来源：http://hz.nanxuanxn.top/gtoikjnmgz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hysaishi.cn/gtfckvgjmf.html

[M05] 设置退出码
来源：http://hz.guannengcc.top/gtcobchxau.html

Py:   sys.exit(1)
来源：http://hz.xylfe.cn/gtpvibfqob.html

PHP:  exit(1);
来源：http://hz.shangyingyoupin.top/gtjbzgssko.html

JS:   process.exit(1)
来源：http://hz.xinyue.icu/gtlbawgeal.html

TS:   process.exit(1)
来源：http://hz.hysaishi.cn/gtmeaqnpbp.html

Java: System.exit(1)
来源：http://hz.yj20258888.top/gttedmlozt.html

Go:   os.Exit(1)
来源：http://hz.pengpengdd.cyou/gtqggqllco.html

Ruby: exit 1
来源：http://hz.sysykeji.top/gtvhltuply.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.smart0.xyz/gthpdtzxbp.html

[M06] 向标准错误输出
来源：http://hz.dianchejie.cn/gtbskpsqry.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hammf.cn/gtwnsdcqpe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.tian-w.cn/gtwjjwhlju.html

JS:   console.error("err")
来源：http://hz.yonumen.top/gtwkfwvboj.html

TS:   console.error("err")
来源：http://hz.daxiang520.top/gtiqftnmas.html

Java: System.err.println("err")
来源：http://hz.jinyuanbaomall.cn/gtlnesxway.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jianghu66.top/gtgxxrnyzx.html

Ruby: warn "err"
来源：http://hz.ydjk.org.cn/gtmwpfmysr.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cashguo.top/gtvmvgnjhb.html

[M07] 判断是否为主入口
来源：http://hz.bjfxy.top/gtmyspsuxv.html

Py:   if __name__ == "__main__":
来源：http://hz.hammf.cn/gtyrroubnn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cheryme.top/gtekxyzklm.html

JS:   require.main === module
来源：http://hz.tanke756.top/gtgfrtebxd.html

TS:   require.main === module
来源：http://hz.mhx1999.top/gtcdhbqjaa.html

Java: public static void main(String[] args)
来源：http://hz.yvedp.cn/gtixdjqjtd.html

Go:   func main()
来源：http://hz.xuanzx.com/gtzfqkjded.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sxryk.cn/gtbnpqxfpw.html

C#:   static void Main(string[] args)
来源：http://hz.9152youxi.cn/gtbqkhstmb.html

[M08] 获取系统与运行时信息
来源：http://hz.cucudq.cn/gtgboqqgjn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hywenlv.cn/gtcecilqem.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jlsjyb.cn/gtfgtlfbzl.html

JS:   process.platform;  process.version
来源：http://hz.shuidangran.top/gtwlxnbeqx.html

TS:   process.platform;  process.version
来源：http://hz.fengsongda.top/gtblbuopdt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yangfankeji.com/gtdvbjogcm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.feifeiyinyue.top/gthrhgoqgj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.meibo888.top/gtdfnuippo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yvedp.cn/gtrspidezt.html

================================================================================
来源：http://hz.birdmap.top/gtxqlgasud.html

N. 数据结构与算法
来源：http://hz.daria6918.cn/gtqlqtzhad.html

================================================================================
来源：http://hz.yj20258.top/gtfcjshaka.html

[N01] 二分查找（有序数组）
来源：http://hz.fzhhl.top/gthfpeeusd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xinyue.icu/gtqwnetuht.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.feifeiyinyue.top/gtkkybswlr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.vqdsnc.cn/gtcfpdxqje.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shuidangran.top/gttwkvymnq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.nwbrower.top/gthzhhihmw.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.c1oappe.top/gtjrtzkifr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.kuanghao11.cn/gtdgyuslib.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jqgufenzy.top/gtrzhhspkf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.sxryk.cn/gtzpwummsl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gzhubu.top/gtengxlxku.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xinyue.icu/gtpkguibtu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.dashuyun.cn/gtuflgcvgw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxuanxn.top/gthzdkffre.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.52xcode.cn/gtlyqqfjhv.html

Go:   slices.Sort(arr)
来源：http://hz.xinyue.icu/gtoqelrvgt.html

Ruby: arr.sort
来源：http://hz.hnqzz.top/gttweexpdc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.haohaochexian.top/gtytxqjlsx.html

[N03] 快速排序（分治示例）
来源：http://hz.hysaishi.cn/gtygnhzfqx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinghuilouyu.cn/gtogqehtwf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinghuilouyu.cn/gtbfpjfjmv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.haohaochexian.top/gttgzdbrzd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cucudq.cn/gtcxrtfrma.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shanyushiyangtech.top/gtcbhafasn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.guannengcc.top/gttmrxjxpw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.pycfn.com/gtcxyzquaj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hfpthk.cn/gtnqxepape.html

[N04] 斐波那契数列
来源：http://hz.fengsongda.top/gtpyvnjcun.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258.top/gttykmcxle.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhixingplan.top/gtrytabluz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jqgfzy.top/gtgncbqjtb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jlsjyb.cn/gtehdwptku.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.daria6918.cn/gtdyqmzsbc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ybcxt.top/gtdturvghu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhixingplan.top/gtpvzbwwzg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.nwbrower.top/gtbbmsgsfe.html

[N05] 最大公约数
来源：http://hz.xinyue.icu/gtheyqrtxx.html

Py:   math.gcd(a, b)
来源：http://hz.cdnleiting.top/gtufdycidx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.snrcjt.cn/gttsalezhr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgufenzy.top/gtisqbeuhc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.meibo888.top/gteubaxkwy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hysaishi.cn/gtwqahcnda.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shanyushiyangtech.top/gtnuimxepn.html

Ruby: a.gcd(b)
来源：http://hz.shanyushiyangtech.top/gtslrruclz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shanyushiyangkeji.top/gtptizitlt.html

[N06] 判断回文字符串
来源：http://hz.zdqjudy.top/gtfjxmuozf.html

Py:   s == s[::-1]
来源：http://hz.sufxvd.cn/gtrefkcudb.html

PHP:  $s === strrev($s);
来源：http://hz.dashuyun.cn/gtezqztjvn.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtvkiolpsr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sysykeji.top/gtqsmtgbfc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.quarkkingdee.top/gtfnvcpgmq.html

Go:   // 双指针从两端比较
来源：http://hz.cheryme.top/gthdrkridv.html

Ruby: s == s.reverse
来源：http://hz.yanxiufei.cn/gtjfasirwf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jiagoushi.top/gtsptxswuq.html

[N07] 两数之和（返回下标）
来源：http://hz.ehwqpu.com/gtfebrevdu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhoulong.xyz/gtaqmosfcn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.tianlin.xyz/gtcezwjqbf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.316326.xyz/gtkilodigh.html

TS:   // 手写 Map<string, number>
来源：http://hz.shangyingyoupin.top/gtfokmauyn.html

Java: // 手写 HashMap
来源：http://hz.guannengcc.top/gtwkmvvhvg.html

Go:   // 手写 map[int]int
来源：http://hz.daria6918.cn/gtigbxtxbt.html

Ruby: // 手写 Hash
来源：http://hz.chenjidiqi.icu/gtsrktnbcn.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shuidangran.top/gtctqymzxj.html

[N08] 生成全排列
来源：http://hz.hysaishi.cn/gtgrstkrtt.html

Py:   itertools.permutations(arr)
来源：http://hz.ywan-chungtsiang.top/gtrjiajfgk.html

PHP:  // 手写递归交换
来源：http://hz.yanxiufei.cn/gtdorgjolm.html

JS:   // 手写回溯递归
来源：http://hz.nwbrower.top/gtvnojkypp.html

TS:   // 手写回溯递归
来源：http://hz.guowangkeji.top/gtdkjzmdpb.html

Java: // 手写回溯递归
来源：http://hz.andypj.xyz/gtjoniokhr.html

Go:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtqkxqpogw.html

Ruby: arr.permutation.to_a
来源：http://hz.gogol.net.cn/gtrnslvxsa.html

C#:   // 手写回溯递归
来源：http://hz.cqqwz.cn/gtubzbyzom.html

[N09] 栈与队列
来源：http://hz.jlsjyb.cn/gtwwjxwpgs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.0kj1m.cn/gtbqhxlbzd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cdnleiting.top/gtrisgnteh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.nanxuanxn.top/gtawohcghi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.redwolf501.top/gttrclqdaq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.316326.xyz/gtjkplcfqi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.smart0.xyz/gtbhzsbkaa.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sysykeji.top/gtbwghbwjr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhijiandao.cn/gtmavqgjon.html

[N10] 链表节点定义
来源：http://hz.xylfe.cn/gtztbgnlee.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhijiandao.cn/gtdlxqyixl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.feifeiyinyue.top/gteemqbwsy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.tian-w.cn/gtpbpdvcdo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.andypj.xyz/gtotujdlkn.html

Java: class Node { int v; Node next; }
来源：http://hz.fzhhl.top/gtabfhgquf.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jqgfzy.top/gtbqmagsrw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yuxming.cn/gtgwopxtnh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.sxryk.cn/gtjteipdwa.html

[N11] 二叉树中序遍历
来源：http://hz.hnxiangtu.top/gtshyxcalk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cashguo.top/gtxuafgzrn.html

PHP:  // 手写递归函数
来源：http://hz.jinyuanbaomall.cn/gthcbworkz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.316326.xyz/gtwoxdzslo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.bjfxy.top/gtplykkgvz.html

Java: // 手写递归
来源：http://hz.daria6918.cn/gtbpcfdyje.html

Go:   // 手写递归
来源：http://hz.havefunace.top/gtstdeimis.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yuanzhike.top/gtqyptqmtk.html

C#:   // 手写递归
来源：http://hz.xingfuxueyuan.xyz/gtuaomxtqk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yuxming.cn/gtldcwnkbz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yonumen.top/gtlwsswrxw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hysaishi.cn/gtjisglzvl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xylfe.cn/gtuolghiza.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinqigufen.top/gtfkgkyrir.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hywenlv.cn/gtememdyor.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jqgfzy.top/gtkebdsrga.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.pengpengdd.cyou/gtarsczqif.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gtexpiyuqb.html

================================================================================
来源：http://hz.yj20258888.top/gtfhzziolc.html

O. 并发与异步
来源：http://hz.shuidangran.top/gtwmwlvuvx.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtazpmbtlb.html

[O01] 启动一个线程
来源：http://hz.gzhubu.top/gtfbslejue.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ydjk.org.cn/gtgoqdahnc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.mhx1999.top/gtglwiksrc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.sweek.top/gtknydrlxr.html

TS:   // 同 JS
来源：http://hz.xuetiantiany.cn/gthiowmgwp.html

Java: new Thread(() -> f()).start()
来源：http://hz.nanxuanxn.top/gtzvakkabw.html

Go:   go f()
来源：http://hz.nanxuanxn.top/gtfepatdoj.html

Ruby: Thread.new { f }
来源：http://hz.jinghuilouyu.cn/gteyjincgb.html

C#:   Task.Run(() => F());
来源：http://hz.hysaishi.cn/gtfglqfrxk.html

[O02] 使用线程池
来源：http://hz.hysaishi.cn/gtkekwqpfw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hongshengwenyu.top/gthxcxuzva.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.316326.xyz/gthboctarw.html

JS:   // worker_threads 线程池
来源：http://hz.aizwys.cn/gtijkwbvcs.html

TS:   // worker_threads 线程池
来源：http://hz.sysykeji.top/gtkftmcjxw.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.aizwys.cn/gtixnltxlh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.fzhhl.top/gtfqkfntia.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.wangshuangyany.cn/gtnlxtimvc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.dianchejie.cn/gtxoxzuwou.html

[O03] 加锁保护共享数据
来源：http://hz.gogol.net.cn/gtauxixebq.html

Py:   with lock: shared += 1
来源：http://hz.iojbl.cn/gtlommrkrt.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.quarkkingdee.top/gtlbqmoode.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.guowangkeji.top/gtopcdgfyq.html

TS:   // 同 JS
来源：http://hz.daxiang520.top/gtizfissxi.html

Java: synchronized (this) { shared++; }
来源：http://hz.shanyushiyangtech.top/gtwohslpgx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.daxiang520.top/gtqurqmmgf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yangfankeji.com/gtcpwukdvr.html

C#:   lock (gate) { shared++; }
来源：http://hz.kuanghao11.cn/gtburcmcen.html

[O04] 定义异步函数并等待
来源：http://hz.tian-w.cn/gtyrncbeoo.html

Py:   async def f():⏎    await g()
来源：http://hz.ppjwa.cn/gtrkmnjwtf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hysaishi.cn/gtudewuavw.html

JS:   async function f() { await g(); }
来源：http://hz.shanyushiyangtech.top/gtteelptjj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.316326.xyz/gtpbcuosrz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xinyue.icu/gttvlovxql.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sysykeji.top/gtxwarhgea.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.wangshuangyany.cn/gtslgjqvli.html

C#:   async Task F() { await G(); }
来源：http://hz.fengsongda.top/gtieacrgnd.html

[O05] 并发执行并等待全部完成
来源：http://hz.feifeiyinyue.top/gtlrmgwkpm.html

Py:   asyncio.gather(*tasks)
来源：http://hz.aizwys.cn/gtbmlywifo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.daria6918.cn/gtgzanfchp.html

JS:   await Promise.all(tasks)
来源：http://hz.zhongyouzk.top/gtuslyuqlo.html

TS:   await Promise.all(tasks)
来源：http://hz.jinqigfzy.top/gtrmjukweh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.daxiang520.top/gtjrcpwwra.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.smart0.xyz/gtjltinisz.html

Ruby: threads.map(&:join)
来源：http://hz.gogol.net.cn/gtcdaiqorw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.fengsongda.top/gtnptjhasx.html

[O06] 使用进程池
来源：http://hz.gotoacloud.top/gtdvnwgwhc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.daria6918.cn/gtmzifugrl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nwbrower.top/gtxyhddyju.html

JS:   // child_process / cluster 模块
来源：http://hz.svipenyu.cn/gtjsrrzuao.html

TS:   // child_process / cluster 模块
来源：http://hz.ivvv.top/gtupyhnaou.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.smart0.xyz/gtgxebdmbr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jianghu66.top/gtkxkiddjf.html

Ruby: // fork 块
来源：http://hz.hysaishi.cn/gtouknqhjj.html

C#:   Parallel.For
来源：http://hz.yj202588.top/gtmmgtdsqc.html

================================================================================
来源：http://hz.gotoacloud.top/gtlexsjrjq.html

P. 常用工具函数
来源：http://hz.xinyue.icu/gtwewinhxu.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gttjpodrng.html

[P01] 生成 UUID
来源：http://hz.cheryme.top/gtoiuvmjkm.html

Py:   str(uuid.uuid4())
来源：http://hz.zhiwuduotai.top/gtgdcqalzd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.smart0.xyz/gtojrrzqrt.html

JS:   crypto.randomUUID()
来源：http://hz.xuetiantiany.cn/gtceruywhc.html

TS:   crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtbsetzqnh.html

Java: UUID.randomUUID().toString()
来源：http://hz.tanke756.top/gtlakeudye.html

Go:   // 用 github.com/google/uuid
来源：http://hz.haohaochexian.top/gttjnxwgoz.html

Ruby: SecureRandom.uuid
来源：http://hz.zhoulong.xyz/gtzfexgvqz.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ydzc1.top/gtubuukiap.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhijiandao.cn/gtbrrqugor.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yanxiufei.cn/gtznpiysmo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhiwuduotai.top/gtrjdurdhj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.snrcjt.cn/gtyjuxggeo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jyoumei.cn/gtyghojyev.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ppjwa.cn/gtfymlqupx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.dianchejie.cn/gtakzypwwt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xziqi.cn/gtinxwtyhj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.sysykeji.top/gtjfnslqfp.html

[P03] 生成短随机字符串
来源：http://hz.yonumen.top/gtpujrxngb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ppjwa.cn/gtklgnjnft.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jinghuilouyu.cn/gtlnnwrlfi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tianlin.xyz/gtuwlwmtbd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sufxvd.cn/gtqjecphzj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.pengpengdd.cyou/gtmhmblwrk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.daxiang520.top/gtvsezbuxr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xziqi.cn/gtqtzimqqy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.birdmap.top/gtneflnohe.html

[P04] 求长度
来源：http://hz.gaohongyu789.top/gtkemdyiwo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cucudq.cn/gtijjprfac.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.c1oappe.top/gtptqbtuqv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nanxuanxn.top/gtebkazpks.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.feifeiyinyue.top/gtlpdiltam.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cashguo.top/gtwghvevuo.html

Go:   len(arr);  len(m)
来源：http://hz.9152youxi.cn/gtftfkjgqo.html

Ruby: x.length;  x.size
来源：http://hz.wangshuangyany.cn/gtejucxeeo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.nanxinkj.top/gtaxcagydx.html

[P05] 判断两个对象内容是否相等
来源：http://hz.svipenyu.cn/gtfyvjowhi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sxryk.cn/gtjwphjmiy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.gogol.net.cn/gtgmncyvqn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.sweek.top/gtegubgeky.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinghuilouyu.cn/gtpxzbvsab.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.chenjidiqi.icu/gtcscyigub.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.havefunace.top/gtmtogbsqn.html

Ruby: a == b
来源：http://hz.shzxlz.cn/gtxdjjyefz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.dianchejie.cn/gteljfljls.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jianghu66.top/gtdxxsknzb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.wangdashe.top/gtogidrntj.html

PHP:  if (empty($x)) {}
来源：http://hz.jqgfzy.top/gtunyllyyx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.pycfn.com/gtivoplbfw.html

TS:   if (x == null) {}
来源：http://hz.ybcxt.top/gtnuckuzqb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.nanxuanxn.top/gtuqolxpfl.html

Go:   if x == nil {}
来源：http://hz.tian-w.cn/gtjfejxlbh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hammf.cn/gtrcxmokmm.html

C#:   if (x is null) {}
来源：http://hz.xylfe.cn/gtogikdiob.html

[P07] 防抖与节流
来源：http://hz.nanxuanxn.top/gtfzakrask.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yanxiufei.cn/gttcmwlqjm.html

PHP:  // 手写时间戳比较
来源：http://hz.chenzaomai.com/gtxenhdxfn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenlongwang.top/gtwnixgbof.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gtvsnsrijh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yanxiufei.cn/gtiyzilwed.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jinqigufen.top/gtzwakwotk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sxryk.cn/gtizgezoax.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xuanzx.com/gthhfiwfdn.html

[P08] 处理浮点精度问题
来源：http://hz.jinqigfzy.top/gtuknkjiwt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jiagoushi.top/gtoyrsxgio.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ydjk.org.cn/gtsjpyxnda.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.dashuyun.cn/gtzpbipjdj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xinyue.icu/gtscjhjoda.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yvedp.cn/gtrrkhghyc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ywan-chungtsiang.top/gtnkvvqube.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yuanzhike.top/gtguukbhbj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nanxinkj.top/gteuwshzwz.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtgebrypzt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gogol.net.cn/gtqvzxocbz.html

================================================================================
来源：http://hz.zycfv.cn/gtppzckiep.html

[Q01] 创建表
来源：http://hz.c1oappe.top/gtufuelmdn.html

CREATE TABLE users (
来源：http://hz.birdmap.top/gtmfotgtbf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.birdmap.top/gtohrftazf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cqqwz.cn/gtxwtgnkue.html

email VARCHAR(100) UNIQUE,
来源：http://hz.pycfn.com/gtsrutagww.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.svipenyu.cn/gtjqvxexlq.html

);
来源：http://hz.smart0.xyz/gtnfvwnyvq.html

[Q02] 创建带外键的表
来源：http://hz.yuxming.cn/gtmiwnuttm.html

CREATE TABLE orders (
来源：http://hz.jinyuanbaomall.cn/gtfhkjfoiz.html


<!-- 参考信息 -->