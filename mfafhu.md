代发 wailian999

TS:   process.cwd()
来源：http://hz.yj202588.top/gtdazrzfzb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jianghu66.top/gtiotzerpy.html

Go:   os.Getwd()
来源：http://hz.zhiwuduotai.top/gtjlnbfeva.html

Ruby: Dir.pwd
来源：http://hz.hammf.cn/gtsqnvncme.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yuanzhike.top/gtmprqlruo.html

[M05] 设置退出码
来源：http://hz.meibo888.top/gtxeiokyus.html

Py:   sys.exit(1)
来源：http://hz.jlsjyb.cn/gtailkyizk.html

PHP:  exit(1);
来源：http://hz.jqgfzy.top/gtnnvsoofy.html

JS:   process.exit(1)
来源：http://hz.jinyuanbaomall.cn/gthvgtoovl.html

TS:   process.exit(1)
来源：http://hz.zhengqikj.top/gtjcxedgpx.html

Java: System.exit(1)
来源：http://hz.tianlin.xyz/gttpvpqgyv.html

Go:   os.Exit(1)
来源：http://hz.svipenyu.cn/gtwolmffjl.html

Ruby: exit 1
来源：http://hz.zhengqikj.top/gtxuletfqc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hfpthk.cn/gtrrkgqhyy.html

[M06] 向标准错误输出
来源：http://hz.yvedp.cn/gtkzgphhjw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xylfe.cn/gtaviaxhap.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.dashuyun.cn/gtucilemgw.html

JS:   console.error("err")
来源：http://hz.sweek.top/gtqyprgmvr.html

TS:   console.error("err")
来源：http://hz.smart0.xyz/gtzdanxbtx.html

Java: System.err.println("err")
来源：http://hz.sweek.top/gtchchifij.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xingfuxueyuan.xyz/gtjckedpih.html

Ruby: warn "err"
来源：http://hz.guowangkeji.top/gtklbbpjbt.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jqgfzy.top/gtjrdztckm.html

[M07] 判断是否为主入口
来源：http://hz.wangdashe.top/gtwdpxewln.html

Py:   if __name__ == "__main__":
来源：http://hz.meibo888.top/gtfrjkbece.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ydjk.org.cn/gteluzsfrm.html

JS:   require.main === module
来源：http://hz.sufxvd.cn/gtxscharhx.html

TS:   require.main === module
来源：http://hz.0kj1m.cn/gtbdtdbvov.html

Java: public static void main(String[] args)
来源：http://hz.fengsongda.top/gtahofwguc.html

Go:   func main()
来源：http://hz.hysaishi.cn/gtmcaldiao.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ybcxt.top/gtjcmixlzy.html

C#:   static void Main(string[] args)
来源：http://hz.tianlin.xyz/gtuvnsmvtk.html

[M08] 获取系统与运行时信息
来源：http://hz.nwbrower.top/gtbbyzxvys.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhijiandao.cn/gtcorflfwi.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.nanxuanxn.top/gtbiapocke.html

JS:   process.platform;  process.version
来源：http://hz.jlsjyb.cn/gttmblddtw.html

TS:   process.platform;  process.version
来源：http://hz.fzhhl.top/gtgcwsnydr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hongshengwenyu.top/gtblocsuhy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xingfuxueyuan.xyz/gtmxrvwxsl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.sysykeji.top/gtnixeywdf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.smart0.xyz/gtubnaibkc.html

================================================================================
来源：http://hz.nanxinkj.top/gtsmlwtzqn.html

N. 数据结构与算法
来源：http://hz.pengpengdd.cyou/gtlyjtjuon.html

================================================================================
来源：http://hz.jqgufenzy.top/gtfutywccd.html

[N01] 二分查找（有序数组）
来源：http://hz.xylfe.cn/gtvtcuhtou.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yuanzhike.top/gtgwwwlaha.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shzxlz.cn/gtqtvmanak.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.snrcjt.cn/gtbpzfbflx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xinyue.icu/gterxkuxet.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenlongwang.top/gtkjregygq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hammf.cn/gtuwlvrgrg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.aizwys.cn/gtgmzqqggt.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sweek.top/gtylqzfngy.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jinghuilouyu.cn/gtxpbydwap.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yuxming.cn/gthkybgwgm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yanxiufei.cn/gtlhwnezya.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yueranfly.top/gtmbaqhdzg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cheryme.top/gtvghgqgpl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.tanke756.top/gtcvwudodw.html

Go:   slices.Sort(arr)
来源：http://hz.tanke756.top/gtkprdivlz.html

Ruby: arr.sort
来源：http://hz.xuetiantiany.cn/gthwsavwdq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xylfe.cn/gtnhbsfvfa.html

[N03] 快速排序（分治示例）
来源：http://hz.shanyushiyangtech.top/gtkvrcjxbs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xuetiantiany.cn/gttfaupirb.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gotoacloud.top/gtdmabppbw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dianchejie.cn/gtuzgrvzrs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.meibo888.top/gtbsvszdir.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.chenjidiqi.icu/gtznyndzbn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shanyushiyangtech.top/gtkojeednq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gotoacloud.top/gtlvyrwwvm.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gaohongyu789.top/gtsdkqqefl.html

[N04] 斐波那契数列
来源：http://hz.hongshengwenyu.top/gtkaouamks.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258.top/gtvztkjwfx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.andypj.xyz/gtzfogpopt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.52xcode.cn/gtsxydvnfl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhoulong.xyz/gtcsgzeckj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jianghu66.top/gtagbcyrhk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xuanzx.com/gtuqxzxkcu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.52xcode.cn/gtiivctwdn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.daria6918.cn/gtyaqpitrk.html

[N05] 最大公约数
来源：http://hz.chenlongwang.top/gtgnukcfkz.html

Py:   math.gcd(a, b)
来源：http://hz.smart0.xyz/gtixfmaavh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.9152youxi.cn/gtqgplhgyp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgfzy.top/gtwsraezhj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenlongwang.top/gtsrrsxgjd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.andypj.xyz/gtabyjtgvr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hywenlv.cn/gtzemumfee.html

Ruby: a.gcd(b)
来源：http://hz.aibaodan.cn/gtcgptoiyd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinghuilouyu.cn/gthfgctatu.html

[N06] 判断回文字符串
来源：http://hz.hfpthk.cn/gtsukbnvhk.html

Py:   s == s[::-1]
来源：http://hz.jinyuanbaomall.cn/gttyhhiwju.html

PHP:  $s === strrev($s);
来源：http://hz.andypj.xyz/gtlwzovhxu.html

JS:   s === [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gthvcyvuad.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gtzpnrqkql.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.tian-w.cn/gtinjqmgug.html

Go:   // 双指针从两端比较
来源：http://hz.sufxvd.cn/gtkldlpedu.html

Ruby: s == s.reverse
来源：http://hz.hnqzz.top/gtfybyifmg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.dianchejie.cn/gttiwakogx.html

[N07] 两数之和（返回下标）
来源：http://hz.ivvv.top/gtbruwyhfv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shuidangran.top/gtqwfpntzy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yongpay.top/gtrvsxicac.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shzxlz.cn/gtisvfoham.html

TS:   // 手写 Map<string, number>
来源：http://hz.nanxuanxn.top/gtcqybglwp.html

Java: // 手写 HashMap
来源：http://hz.yuxming.cn/gtyrbqkofh.html

Go:   // 手写 map[int]int
来源：http://hz.gzhubu.top/gtazsuvdtl.html

Ruby: // 手写 Hash
来源：http://hz.zhiwuduotai.top/gtxvuhzycb.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhaomingkeji.xyz/gtfanbwlms.html

[N08] 生成全排列
来源：http://hz.gzhubu.top/gtojubqbxm.html

Py:   itertools.permutations(arr)
来源：http://hz.pengpengdd.cyou/gtlgorjejd.html

PHP:  // 手写递归交换
来源：http://hz.cdnleiting.top/gtlfaxacta.html

JS:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtihhusiml.html

TS:   // 手写回溯递归
来源：http://hz.nwbrower.top/gtsewndgka.html

Java: // 手写回溯递归
来源：http://hz.yuanzhike.top/gtziodpllv.html

Go:   // 手写回溯递归
来源：http://hz.cheryme.top/gtiaprwiee.html

Ruby: arr.permutation.to_a
来源：http://hz.yongpay.top/gtvwovuawv.html

C#:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtfyqasskf.html

[N09] 栈与队列
来源：http://hz.ivvv.top/gthtxaejnu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jyoumei.cn/gtcxfkygis.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinqigfzy.top/gtaqrejuma.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hywenlv.cn/gtmrncjset.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.0kj1m.cn/gtwcytfdkq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yongpay.top/gtyiurgjun.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gzhubu.top/gtgtgcjgmk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhijiandao.cn/gtdithyzei.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.dianchejie.cn/gtbnrywdxh.html

[N10] 链表节点定义
来源：http://hz.tianlin.xyz/gtjpssxofk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hnxiangtu.top/gtpnkjbugs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.nanxuanxn.top/gtomfbdxnf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.aizwys.cn/gttbtdkjav.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.redwolf501.top/gtrvxrvmlt.html

Java: class Node { int v; Node next; }
来源：http://hz.shanyushiyangkeji.top/gtbjxeeqcm.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinqigufen.top/gthpegabky.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.bjfxy.top/gttodwhfaf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yj20258.top/gtlumbcyno.html

[N11] 二叉树中序遍历
来源：http://hz.hywenlv.cn/gtxfzgvith.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.svipenyu.cn/gtjrgplsar.html

PHP:  // 手写递归函数
来源：http://hz.vqdsnc.cn/gtunjvujre.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.vqdsnc.cn/gtmckqsvqh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.svipenyu.cn/gtouzcfxuc.html

Java: // 手写递归
来源：http://hz.svipenyu.cn/gteryqisws.html

Go:   // 手写递归
来源：http://hz.svipenyu.cn/gtpdafyyku.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.316326.xyz/gtgfxqmxxt.html

C#:   // 手写递归
来源：http://hz.hnxiangtu.top/gtmqnwjweb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ivvv.top/gtpmoduetb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ivvv.top/gtozalusoc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhaomingkeji.xyz/gttforbarf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenlongwang.top/gtfetmbbef.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shzxlz.cn/gtdqrahshu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tanke756.top/gtppvofblo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jinghuilouyu.cn/gtzkqjsahk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cqqwz.cn/gtrdpmveet.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ybcxt.top/gtmjbmhemc.html

================================================================================
来源：http://hz.yj202588.top/gtnumofbni.html

O. 并发与异步
来源：http://hz.shanyushiyangkeji.top/gtuamevqic.html

================================================================================
来源：http://hz.nanxinkj.top/gtzdqeeajf.html

[O01] 启动一个线程
来源：http://hz.sysykeji.top/gtyqxywpib.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.chenlongwang.top/gtsluqlibx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ppjwa.cn/gtwogmmmkb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jlsjyb.cn/gtvcuepqyn.html

TS:   // 同 JS
来源：http://hz.yueranfly.top/gtrfrnjokm.html

Java: new Thread(() -> f()).start()
来源：http://hz.aizwys.cn/gtrrczjowk.html

Go:   go f()
来源：http://hz.ppjwa.cn/gtoszbgsmo.html

Ruby: Thread.new { f }
来源：http://hz.shangyingyoupin.top/gtejgoighz.html

C#:   Task.Run(() => F());
来源：http://hz.birdmap.top/gtkwelbqnf.html

[O02] 使用线程池
来源：http://hz.9152youxi.cn/gtojlmvgud.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.chenjidiqi.icu/gtnwbpwknp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yanxiufei.cn/gtygjdiwzn.html

JS:   // worker_threads 线程池
来源：http://hz.zhoulong.xyz/gtywpfvnxs.html

TS:   // worker_threads 线程池
来源：http://hz.hysaishi.cn/gtryhkskid.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.guannengcc.top/gtgsygmnuk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ppjwa.cn/gtxxgdpxtb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ivvv.top/gtsvnsobpz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.chenjidiqi.icu/gtvxjvaswm.html

[O03] 加锁保护共享数据
来源：http://hz.shanyushiyangtech.top/gtviygxycw.html

Py:   with lock: shared += 1
来源：http://hz.gzhubu.top/gtzhrwfnsv.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.aizwys.cn/gtoibahauj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hnqzz.top/gtylzvabqj.html

TS:   // 同 JS
来源：http://hz.redwolf501.top/gtajcorceq.html

Java: synchronized (this) { shared++; }
来源：http://hz.shangyingyoupin.top/gtqnnqhfpu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.daxiang520.top/gtewltzqog.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinqigufen.top/gtfjxrfvyx.html

C#:   lock (gate) { shared++; }
来源：http://hz.guowangkeji.top/gtwshqbyzp.html

[O04] 定义异步函数并等待
来源：http://hz.cucudq.cn/gtaowkhvwe.html

Py:   async def f():⏎    await g()
来源：http://hz.sxryk.cn/gtxewaeocf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.andypj.xyz/gtdkurjqpt.html

JS:   async function f() { await g(); }
来源：http://hz.jinqigfzy.top/gtdmkgppav.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jlsjyb.cn/gtyvdqopqh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cqqwz.cn/gtyjqkpgme.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yueranfly.top/gtencwupgy.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.0kj1m.cn/gtxugpjbib.html

C#:   async Task F() { await G(); }
来源：http://hz.wangdashe.top/gtecukkybr.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhongyouzk.top/gtsueaxbjw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinghuilouyu.cn/gtfhnnuzkk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.birdmap.top/gtuabadync.html

JS:   await Promise.all(tasks)
来源：http://hz.yj20258.top/gtcankuzkx.html

TS:   await Promise.all(tasks)
来源：http://hz.aizwys.cn/gtqhgbehbs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.snrcjt.cn/gtgjrwgfhm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ybcxt.top/gtbgnyjevl.html

Ruby: threads.map(&:join)
来源：http://hz.ybcxt.top/gtcijialtn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.gotoacloud.top/gtvfvrtyle.html

[O06] 使用进程池
来源：http://hz.shuidangran.top/gtynfsfall.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.quarkkingdee.top/gtnjffqljr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.gotoacloud.top/gtrfndhcqg.html

JS:   // child_process / cluster 模块
来源：http://hz.hongshengwenyu.top/gtjwzwctrk.html

TS:   // child_process / cluster 模块
来源：http://hz.smart0.xyz/gtxdepivxv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jiagoushi.top/gtkmttinao.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.0kj1m.cn/gtnjcalqdn.html

Ruby: // fork 块
来源：http://hz.pycfn.com/gtxyobturd.html

C#:   Parallel.For
来源：http://hz.nanxuanxn.top/gtzppdaxnm.html

================================================================================
来源：http://hz.dianchejie.cn/gtotiaylxo.html

P. 常用工具函数
来源：http://hz.cucudq.cn/gtmomeumre.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtcjeygldu.html

[P01] 生成 UUID
来源：http://hz.hfpthk.cn/gtxshvwsek.html

Py:   str(uuid.uuid4())
来源：http://hz.ivvv.top/gtcnpbjsat.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinyuanbaomall.cn/gtpsckjnlk.html

JS:   crypto.randomUUID()
来源：http://hz.yj20258.top/gtaepnwvez.html

TS:   crypto.randomUUID()
来源：http://hz.hnqzz.top/gtlevrkble.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhixingplan.top/gtjmirwlal.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj202588.top/gttdvlthdk.html

Ruby: SecureRandom.uuid
来源：http://hz.gotoacloud.top/gtupqjssrg.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenlongwang.top/gtmuogwuvr.html

[P02] MD5 / SHA256 摘要
来源：http://hz.mhx1999.top/gtckhoekld.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhijiandao.cn/gtvmzpqabp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shuidangran.top/gtewqyvqlp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yueranfly.top/gtvfuankur.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.pengpengdd.cyou/gtipzqpmbo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.nanxinkj.top/gtykvvixsh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jiagoushi.top/gtfmvrhlbd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.haohaochexian.top/gtdxllyxac.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yongpay.top/gtutpbzutp.html

[P03] 生成短随机字符串
来源：http://hz.shuidangran.top/gtvemazoqp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ehwqpu.com/gtrowxeotj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.feifeiyinyue.top/gtxnaogvbn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hongshengwenyu.top/gtnezbqrzy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jiagoushi.top/gtxsgxhvmz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.haohaochexian.top/gtfbxjpfgk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.tianlin.xyz/gtydspaybq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yuanzhike.top/gtxtlfhqcr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.quarkkingdee.top/gtoyvherhk.html

[P04] 求长度
来源：http://hz.dashuyun.cn/gttzcnsjbm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ydzc1.top/gtpudsjmny.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xinyue.icu/gtduyzwrbd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj20258888.top/gtwkiwzosj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.guowangkeji.top/gtrbqpftdy.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ppjwa.cn/gtplgnegte.html

Go:   len(arr);  len(m)
来源：http://hz.52xcode.cn/gtguzgzrzz.html

Ruby: x.length;  x.size
来源：http://hz.xinyue.icu/gtziafbrpb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.guowangkeji.top/gtyxvqjpfq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hysaishi.cn/gtahkzrkyp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tianlin.xyz/gtamjipnmf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cdnleiting.top/gtyclddqkg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shangyingyoupin.top/gthywggpjt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yongpay.top/gtxbjhnvxs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sweek.top/gtqiniqxse.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zdqjudy.top/gtizobevdt.html

Ruby: a == b
来源：http://hz.shuidangran.top/gtmvudfmze.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.aibaodan.cn/gtvunnhgcf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jinqigfzy.top/gtmcwpqylz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.fengsongda.top/gtvjdfsigc.html

PHP:  if (empty($x)) {}
来源：http://hz.shuidangran.top/gtclonqhff.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sxryk.cn/gtetikfuwq.html

TS:   if (x == null) {}
来源：http://hz.daria6918.cn/gtosbsyrtx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ehwqpu.com/gtxyzwlzuw.html

Go:   if x == nil {}
来源：http://hz.cqqwz.cn/gthdwhagpo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xylfe.cn/gtcpjqfjrx.html

C#:   if (x is null) {}
来源：http://hz.zhaomingkeji.xyz/gtmgiaixrf.html

[P07] 防抖与节流
来源：http://hz.nanxuanxn.top/gttyqgshds.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.havefunace.top/gttfpdpths.html

PHP:  // 手写时间戳比较
来源：http://hz.haohaochexian.top/gtbqiztasm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nwbrower.top/gtfhhaauul.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shangyingyoupin.top/gtvhuidkad.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cqqwz.cn/gtxdszxorg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhongyouzk.top/gtaxkdjtzp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.quarkkingdee.top/gtmemgssxe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hysaishi.cn/gtucuekrhz.html

[P08] 处理浮点精度问题
来源：http://hz.yuanzhike.top/gtvdasqkyd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ywan-chungtsiang.top/gttcogrpch.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shangyingyoupin.top/gtgdmomlar.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.quarkkingdee.top/gtefqhppgr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yvedp.cn/gttyzfonmv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yuanzhike.top/gtoiecxnky.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhaomingkeji.xyz/gtvdvbxrzb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jyoumei.cn/gtcctddzmy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sufxvd.cn/gtynsrbcbc.html

================================================================================
来源：http://hz.mhx1999.top/gtisjlbujz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jlsjyb.cn/gthglfcgbp.html

================================================================================
来源：http://hz.yangfankeji.com/gtxemqerjn.html

[Q01] 创建表
来源：http://hz.aibaodan.cn/gtxwadlbzk.html

CREATE TABLE users (
来源：http://hz.pycfn.com/gtnuepsnuy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.feifeiyinyue.top/gtrfpsmamv.html

name VARCHAR(50) NOT NULL,
来源：http://hz.birdmap.top/gtdcyyosul.html

email VARCHAR(100) UNIQUE,
来源：http://hz.smart0.xyz/gtvnugqvqt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yj20258888.top/gtyikwuiuq.html

);
来源：http://hz.ehwqpu.com/gtaxtmlcjp.html

[Q02] 创建带外键的表
来源：http://hz.sysykeji.top/gtfizlvjbp.html

CREATE TABLE orders (
来源：http://hz.gotoacloud.top/gthidyzvnt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tianlin.xyz/gtmdznyrvg.html

user_id INT NOT NULL,
来源：http://hz.fzhhl.top/gthccpytve.html

amount DECIMAL(10, 2),
来源：http://hz.quarkkingdee.top/gtzuwwhtto.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ydjk.org.cn/gtaxpcyuto.html


<!-- 参考信息 -->