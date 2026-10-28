代发 wailian999

TS:   process.cwd()
来源：http://hz.ydzc1.top/gthamvptal.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.daria6918.cn/gtspqxqzse.html

Go:   os.Getwd()
来源：http://hz.zhijiandao.cn/gtoyxtlcfk.html

Ruby: Dir.pwd
来源：http://hz.ppjwa.cn/gtyxpltdpv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.snrcjt.cn/gtlnwvelce.html

[M05] 设置退出码
来源：http://hz.vqdsnc.cn/gtxtmpjctq.html

Py:   sys.exit(1)
来源：http://hz.xziqi.cn/gtsqewkris.html

PHP:  exit(1);
来源：http://hz.yj20258888.top/gtdldzcyof.html

JS:   process.exit(1)
来源：http://hz.havefunace.top/gtaalrcgzt.html

TS:   process.exit(1)
来源：http://hz.quarkkingdee.top/gtyqjwfmgr.html

Java: System.exit(1)
来源：http://hz.bjfxy.top/gtbdygxkkd.html

Go:   os.Exit(1)
来源：http://hz.havefunace.top/gtfhroshdj.html

Ruby: exit 1
来源：http://hz.9152youxi.cn/gtdjtoqome.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.quarkkingdee.top/gtgigbeaiq.html

[M06] 向标准错误输出
来源：http://hz.zhoulong.xyz/gtfffktvma.html

Py:   print("err", file=sys.stderr)
来源：http://hz.pengpengdd.cyou/gtxezpntnd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhixingplan.top/gtbypgszvx.html

JS:   console.error("err")
来源：http://hz.dianchejie.cn/gtyghyekfp.html

TS:   console.error("err")
来源：http://hz.zhoulong.xyz/gtxbcnjqyl.html

Java: System.err.println("err")
来源：http://hz.jiagoushi.top/gtccurfcye.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ydjk.org.cn/gtygrlnooh.html

Ruby: warn "err"
来源：http://hz.jqgfzy.top/gtoatuxujx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.redwolf501.top/gtfkxoxrgc.html

[M07] 判断是否为主入口
来源：http://hz.shanyushiyangtech.top/gthnccautl.html

Py:   if __name__ == "__main__":
来源：http://hz.zhijiandao.cn/gtxibklrfh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.tian-w.cn/gtxeaoaoez.html

JS:   require.main === module
来源：http://hz.hnxiangtu.top/gtdavcjcmz.html

TS:   require.main === module
来源：http://hz.gaohongyu789.top/gthdmbxgmr.html

Java: public static void main(String[] args)
来源：http://hz.zdqjudy.top/gtcugsebxu.html

Go:   func main()
来源：http://hz.snrcjt.cn/gtkavsbonr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yj20258.top/gtwmncyyjx.html

C#:   static void Main(string[] args)
来源：http://hz.jinyuanbaomall.cn/gtybzvgwnq.html

[M08] 获取系统与运行时信息
来源：http://hz.chenzaomai.com/gtfcxrqhys.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jyoumei.cn/gtkuppfbmf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tanke756.top/gtwnsdhili.html

JS:   process.platform;  process.version
来源：http://hz.smart0.xyz/gtogxbyvgk.html

TS:   process.platform;  process.version
来源：http://hz.ivvv.top/gtvysibyqo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shzxlz.cn/gtmteimcsq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shangyingyoupin.top/gtezkvvpvu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhengqikj.top/gtjrksscpx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yuanzhike.top/gtbvmxnpyh.html

================================================================================
来源：http://hz.dianchejie.cn/gtyfwqwfsl.html

N. 数据结构与算法
来源：http://hz.vqdsnc.cn/gtgzppdiyh.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gttptddwey.html

[N01] 二分查找（有序数组）
来源：http://hz.cheryme.top/gtafztrlcz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.c1oappe.top/gtcttclgjq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cdnleiting.top/gtlwrvtrrm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hysaishi.cn/gtowtccmrg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yangfankeji.com/gtnwpydnou.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.birdmap.top/gtxsnzxhmz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cqqwz.cn/gtiivkkhvi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.gzhubu.top/gtupxphquc.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtmbevyagz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shanyushiyangkeji.top/gtgihecrlp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cdnleiting.top/gtthkqmync.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhoulong.xyz/gtbeefbskl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nwbrower.top/gtqgkmqrcy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yongpay.top/gtyhqigmdc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhengqikj.top/gtsksekmfi.html

Go:   slices.Sort(arr)
来源：http://hz.gzhubu.top/gtqxqgxcny.html

Ruby: arr.sort
来源：http://hz.ivvv.top/gtovzehixo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.dashuyun.cn/gtjvtzaiwx.html

[N03] 快速排序（分治示例）
来源：http://hz.cdnleiting.top/gttathnwor.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yvedp.cn/gtgqyqtaai.html

PHP:  // 递归实现，或用 usort
来源：http://hz.dianchejie.cn/gtecoqpxuq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cucudq.cn/gtlmogvehl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jianghu66.top/gtkdewdnxo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yvedp.cn/gtljlicqvm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jiagoushi.top/gtlwrxvnwj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.smart0.xyz/gtrenrkeey.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jlsjyb.cn/gtxazntcdt.html

[N04] 斐波那契数列
来源：http://hz.9152youxi.cn/gtxfrhgpyv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.vqdsnc.cn/gtajjhvmcf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hongshengwenyu.top/gtlfiuqedh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nwbrower.top/gtbxcssdst.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yueranfly.top/gtwgtljfhz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.daxiang520.top/gtzqmbvcyy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hywenlv.cn/gtimcopnzm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xingfuxueyuan.xyz/gtgkininnf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenjidiqi.icu/gtgnaccrvv.html

[N05] 最大公约数
来源：http://hz.xziqi.cn/gtlftvfgqm.html

Py:   math.gcd(a, b)
来源：http://hz.chenlongwang.top/gtelwsnrxh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.nanxuanxn.top/gtumxskbnt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dashuyun.cn/gtivfoiprh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tanke756.top/gtdcidfswy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yj20258888.top/gtfoapqckw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.fengsongda.top/gtwdwipjnb.html

Ruby: a.gcd(b)
来源：http://hz.nanxinkj.top/gtwqnztdsp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.daria6918.cn/gtmmivmdvm.html

[N06] 判断回文字符串
来源：http://hz.shangyingyoupin.top/gtiltkjzzr.html

Py:   s == s[::-1]
来源：http://hz.havefunace.top/gtrucgeuym.html

PHP:  $s === strrev($s);
来源：http://hz.zhoulong.xyz/gtbmjefclj.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtkhfqriwu.html

TS:   s === [...s].reverse().join("")
来源：http://hz.mhx1999.top/gtpqlibzzq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.aibaodan.cn/gtlmiftsrp.html

Go:   // 双指针从两端比较
来源：http://hz.tian-w.cn/gtwognwqxs.html

Ruby: s == s.reverse
来源：http://hz.meibo888.top/gtxlfkueyw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangtech.top/gtnveipwwx.html

[N07] 两数之和（返回下标）
来源：http://hz.sufxvd.cn/gtxpwgnojq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.52xcode.cn/gtishtgivu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hnqzz.top/gtckruyqkj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinqigufen.top/gtkphmqkxu.html

TS:   // 手写 Map<string, number>
来源：http://hz.shanyushiyangtech.top/gtptpnfkys.html

Java: // 手写 HashMap
来源：http://hz.wangshuangyany.cn/gtbqfoexie.html

Go:   // 手写 map[int]int
来源：http://hz.hnqzz.top/gtvqatbmwt.html

Ruby: // 手写 Hash
来源：http://hz.aizwys.cn/gtkiwcpteg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hnxiangtu.top/gtyvtoxsrt.html

[N08] 生成全排列
来源：http://hz.cdnleiting.top/gtilhvbwgd.html

Py:   itertools.permutations(arr)
来源：http://hz.sufxvd.cn/gtxbplrwfk.html

PHP:  // 手写递归交换
来源：http://hz.ehwqpu.com/gtkbwkzzfo.html

JS:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtxnusgnmg.html

TS:   // 手写回溯递归
来源：http://hz.mhx1999.top/gtnfnrksfa.html

Java: // 手写回溯递归
来源：http://hz.iojbl.cn/gtrergsvgq.html

Go:   // 手写回溯递归
来源：http://hz.shzxlz.cn/gteacjdlyh.html

Ruby: arr.permutation.to_a
来源：http://hz.ydjk.org.cn/gtmpbrkudp.html

C#:   // 手写回溯递归
来源：http://hz.yongpay.top/gtbjdpmjtz.html

[N09] 栈与队列
来源：http://hz.xziqi.cn/gtzmrfvwed.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.gaohongyu789.top/gtmzeoilpo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.0kj1m.cn/gtdvmygwuw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.gaohongyu789.top/gtqznpsmpl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xuanzx.com/gtbbskmaty.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shzxlz.cn/gtbkhbbvqi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tanke756.top/gtlzbxaikz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yuanzhike.top/gtygcojzbl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhaomingkeji.xyz/gtvyeexilm.html

[N10] 链表节点定义
来源：http://hz.daxiang520.top/gtlatoewvp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jianghu66.top/gtvawpcngq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.nanxuanxn.top/gtjtljysxx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zdqjudy.top/gtwtzsiuoc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.nanxinkj.top/gtpwfbxitv.html

Java: class Node { int v; Node next; }
来源：http://hz.gotoacloud.top/gtuzcusoiu.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.52xcode.cn/gtbzmknvyx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yvedp.cn/gtphnugpyh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.snrcjt.cn/gtjhafewhj.html

[N11] 二叉树中序遍历
来源：http://hz.yongpay.top/gtikwzmrcd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.quarkkingdee.top/gtlgotuhht.html

PHP:  // 手写递归函数
来源：http://hz.jyoumei.cn/gtrxarmxuh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.316326.xyz/gttpoztaio.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cheryme.top/gtfbxfbcrl.html

Java: // 手写递归
来源：http://hz.hysaishi.cn/gtgbrphelj.html

Go:   // 手写递归
来源：http://hz.sweek.top/gtlizfsuck.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.52xcode.cn/gtciaznfdl.html

C#:   // 手写递归
来源：http://hz.sufxvd.cn/gtvgnsdpmx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.pengpengdd.cyou/gtdbpnczmf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yj20258888.top/gtlokqmhfm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yangfankeji.com/gtapacnjam.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zdqjudy.top/gttnocezgy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhiwuduotai.top/gtzaizbpmp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yvedp.cn/gtsyslsorq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zycfv.cn/gtsqpikwtu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.guowangkeji.top/gtjpnwutpm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.52xcode.cn/gtdxyynusm.html

================================================================================
来源：http://hz.wangshuangyany.cn/gthedtgwix.html

O. 并发与异步
来源：http://hz.fzhhl.top/gtskzzjuyk.html

================================================================================
来源：http://hz.pycfn.com/gtqqyqcili.html

[O01] 启动一个线程
来源：http://hz.yuanzhike.top/gtvygxkzhg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yuxming.cn/gtknkrywen.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.bjfxy.top/gtzumehwgy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhijiandao.cn/gtgjpvcoye.html

TS:   // 同 JS
来源：http://hz.gotoacloud.top/gtrqutumdy.html

Java: new Thread(() -> f()).start()
来源：http://hz.gotoacloud.top/gtmtaijbpd.html

Go:   go f()
来源：http://hz.hammf.cn/gtuuaranoa.html

Ruby: Thread.new { f }
来源：http://hz.yonumen.top/gtlgyaxovu.html

C#:   Task.Run(() => F());
来源：http://hz.cucudq.cn/gtcjggebtc.html

[O02] 使用线程池
来源：http://hz.feifeiyinyue.top/gtlaeqscur.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hywenlv.cn/gtvdjpckfx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nanxinkj.top/gtlyrtxvln.html

JS:   // worker_threads 线程池
来源：http://hz.zhaomingkeji.xyz/gtxfwenpyt.html

TS:   // worker_threads 线程池
来源：http://hz.daria6918.cn/gtfglekmxb.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jiagoushi.top/gtoaypqwgy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.nanxuanxn.top/gtmkjekzob.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shzxlz.cn/gtpkfddzfj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhiwuduotai.top/gtnvrsnbru.html

[O03] 加锁保护共享数据
来源：http://hz.zhiwuduotai.top/gtrraqwbca.html

Py:   with lock: shared += 1
来源：http://hz.jinqigufen.top/gtcajrviju.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.guannengcc.top/gtgmedhhsv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.dashuyun.cn/gtnvfrcpej.html

TS:   // 同 JS
来源：http://hz.zhaomingkeji.xyz/gtjbdqztgf.html

Java: synchronized (this) { shared++; }
来源：http://hz.smart0.xyz/gttmdufrlo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhijiandao.cn/gtjpxtzwna.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.aizwys.cn/gtlrsopypn.html

C#:   lock (gate) { shared++; }
来源：http://hz.ywan-chungtsiang.top/gtuudxvdfh.html

[O04] 定义异步函数并等待
来源：http://hz.haohaochexian.top/gtjgweztor.html

Py:   async def f():⏎    await g()
来源：http://hz.fengsongda.top/gtzzunlqyl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gaohongyu789.top/gticrxesgh.html

JS:   async function f() { await g(); }
来源：http://hz.feifeiyinyue.top/gtrqlpwkfd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jinqigufen.top/gtowwiqnco.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.vqdsnc.cn/gtozlxdpes.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xylfe.cn/gtpwflmwke.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hnxiangtu.top/gtsbxjhaqx.html

C#:   async Task F() { await G(); }
来源：http://hz.yj20258888.top/gtjfrvowqd.html

[O05] 并发执行并等待全部完成
来源：http://hz.wangdashe.top/gtudlxiycu.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shuidangran.top/gtvacmresr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.fengsongda.top/gtitbncsjq.html

JS:   await Promise.all(tasks)
来源：http://hz.0kj1m.cn/gtxzmqyjxf.html

TS:   await Promise.all(tasks)
来源：http://hz.iojbl.cn/gthzofxzwv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinqigufen.top/gtppnsjxqn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ywan-chungtsiang.top/gtgfjiajuc.html

Ruby: threads.map(&:join)
来源：http://hz.chenlongwang.top/gtmstywbqi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hnqzz.top/gtogizghee.html

[O06] 使用进程池
来源：http://hz.hysaishi.cn/gtbxhceybe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cheryme.top/gtjutmrdby.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.guowangkeji.top/gtdnzohywr.html

JS:   // child_process / cluster 模块
来源：http://hz.kuanghao11.cn/gtzybqckrp.html

TS:   // child_process / cluster 模块
来源：http://hz.ppjwa.cn/gtdsqlqacb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.smart0.xyz/gtqkukglfi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.bjfxy.top/gtndtcvdhq.html

Ruby: // fork 块
来源：http://hz.316326.xyz/gtvqgtahrl.html

C#:   Parallel.For
来源：http://hz.quarkkingdee.top/gtezkjjfew.html

================================================================================
来源：http://hz.gogol.net.cn/gtdkkakmbz.html

P. 常用工具函数
来源：http://hz.shanyushiyangkeji.top/gtdwpzpizw.html

================================================================================
来源：http://hz.wangshuangyany.cn/gttitegeyl.html

[P01] 生成 UUID
来源：http://hz.birdmap.top/gtrbqhlvsw.html

Py:   str(uuid.uuid4())
来源：http://hz.yvedp.cn/gtvaawlehq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hongshengwenyu.top/gtdziqzohi.html

JS:   crypto.randomUUID()
来源：http://hz.zhoulong.xyz/gtveqsvjmk.html

TS:   crypto.randomUUID()
来源：http://hz.cdnleiting.top/gtwnelzhxp.html

Java: UUID.randomUUID().toString()
来源：http://hz.c1oappe.top/gtaqywakfp.html

Go:   // 用 github.com/google/uuid
来源：http://hz.redwolf501.top/gtiaxzjpeo.html

Ruby: SecureRandom.uuid
来源：http://hz.wangshuangyany.cn/gtujregdxu.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.wangshuangyany.cn/gtyaarlvld.html

[P02] MD5 / SHA256 摘要
来源：http://hz.havefunace.top/gthjjyhmby.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.redwolf501.top/gtzovahldq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ydjk.org.cn/gtuugdjzel.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.316326.xyz/gthvnjfdht.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yonumen.top/gttairrpxo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.feifeiyinyue.top/gtxrppekxh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gotoacloud.top/gtdnxaevle.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hongshengwenyu.top/gtwymwkgeh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.iojbl.cn/gtawxjyuva.html

[P03] 生成短随机字符串
来源：http://hz.tianlin.xyz/gtcwnutfhy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.9152youxi.cn/gtrnutocfy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.guannengcc.top/gtolzdfqta.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xingfuxueyuan.xyz/gtsaeafidi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.aibaodan.cn/gtppifmauj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jiagoushi.top/gtepqkttwz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.dianchejie.cn/gtanwbqfak.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.andypj.xyz/gtdcxflafi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhixingplan.top/gtnispvzbb.html

[P04] 求长度
来源：http://hz.jinyuanbaomall.cn/gtweoevgoa.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gogol.net.cn/gthslmnirb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yangfankeji.com/gtwluyqoyg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yongpay.top/gtosbemekc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nanxinkj.top/gthvlwqxnl.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yuanzhike.top/gtkknlwtej.html

Go:   len(arr);  len(m)
来源：http://hz.cqqwz.cn/gtxjlsmwel.html

Ruby: x.length;  x.size
来源：http://hz.zhijiandao.cn/gtdgpzkocm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.316326.xyz/gtsnabqdun.html

[P05] 判断两个对象内容是否相等
来源：http://hz.pengpengdd.cyou/gtuupioyns.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.quarkkingdee.top/gtjaofaotw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jlsjyb.cn/gtqwdthtym.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nwbrower.top/gtopdaqfxs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinqigfzy.top/gtwdlhfoez.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jianghu66.top/gtkkmqynwj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hysaishi.cn/gtutcszbkz.html

Ruby: a == b
来源：http://hz.gotoacloud.top/gtikilsmkx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shanyushiyangkeji.top/gtkyizbdvy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhongyouzk.top/gtkhhzqyul.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yuanzhike.top/gthsaumdmf.html

PHP:  if (empty($x)) {}
来源：http://hz.yueranfly.top/gtwsgfjvmn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yj202588.top/gtmfooqblf.html

TS:   if (x == null) {}
来源：http://hz.9152youxi.cn/gtklynsklz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shuidangran.top/gtcdttiftk.html

Go:   if x == nil {}
来源：http://hz.jiagoushi.top/gtiexmrvmb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jinghuilouyu.cn/gtplvruzkb.html

C#:   if (x is null) {}
来源：http://hz.hywenlv.cn/gtgspmfjfi.html

[P07] 防抖与节流
来源：http://hz.pengpengdd.cyou/gtnyzviewy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yj20258.top/gtxhdykwns.html

PHP:  // 手写时间戳比较
来源：http://hz.haohaochexian.top/gtkejhzhtt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnxiangtu.top/gthmmrukzd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.iojbl.cn/gtzhwjtpho.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ydjk.org.cn/gtcmwzcwzf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.meibo888.top/gtozqrjbkl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sweek.top/gtuhxknnlc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cdnleiting.top/gtydmsnptf.html

[P08] 处理浮点精度问题
来源：http://hz.yonumen.top/gtvcxweqge.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.iojbl.cn/gtgtrxmmdy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shangyingyoupin.top/gtkqrczvpl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.daria6918.cn/gtkhqcvccl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tian-w.cn/gtafprzxgu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yvedp.cn/gtzcxmzbwj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.bjfxy.top/gtzgjeacqh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shanyushiyangtech.top/gthusxmkbn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.vqdsnc.cn/gtjapfnsom.html

================================================================================
来源：http://hz.cdnleiting.top/gtghbevevh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shangyingyoupin.top/gtipdruerx.html

================================================================================
来源：http://hz.hammf.cn/gtodwghcxp.html

[Q01] 创建表
来源：http://hz.xuanzx.com/gtxhfepnlw.html

CREATE TABLE users (
来源：http://hz.birdmap.top/gtsxhbiqpp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinqigfzy.top/gtucmlwsvg.html

name VARCHAR(50) NOT NULL,
来源：http://hz.svipenyu.cn/gtsxtqhqxd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cdnleiting.top/gtgvttxycv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yueranfly.top/gtizezmpyn.html

);
来源：http://hz.vqdsnc.cn/gtdlfhakkw.html

[Q02] 创建带外键的表
来源：http://hz.xylfe.cn/gtdakaxpqz.html

CREATE TABLE orders (
来源：http://hz.fzhhl.top/gtkwwibjry.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jianghu66.top/gtvazvsqgx.html

user_id INT NOT NULL,
来源：http://hz.yongpay.top/gtxtprdocd.html

amount DECIMAL(10, 2),
来源：http://hz.jinqigfzy.top/gtzqsxadss.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xziqi.cn/gtzlwdqjuq.html


<!-- 参考信息 -->