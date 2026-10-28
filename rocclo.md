代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://hz.aizwys.cn/gtjujnjmco.html

[M05] 设置退出码
来源：http://hz.shanyushiyangtech.top/gtehtylvdo.html

Py:   sys.exit(1)
来源：http://hz.andypj.xyz/gtckvcuugb.html

PHP:  exit(1);
来源：http://hz.ydzc1.top/gtuxopvwxf.html

JS:   process.exit(1)
来源：http://hz.iojbl.cn/gtwqzltfbj.html

TS:   process.exit(1)
来源：http://hz.xziqi.cn/gtqbknycfn.html

Java: System.exit(1)
来源：http://hz.ydzc1.top/gtqdrbqrdv.html

Go:   os.Exit(1)
来源：http://hz.jianghu66.top/gtruqcmahd.html

Ruby: exit 1
来源：http://hz.yj202588.top/gtauwjlicr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj20258.top/gtmrhumyys.html

[M06] 向标准错误输出
来源：http://hz.yuxming.cn/gtdvqimzpw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.kuanghao11.cn/gtnkokgdhg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenlongwang.top/gtwczpzyeh.html

JS:   console.error("err")
来源：http://hz.zhijiandao.cn/gtzifenzbj.html

TS:   console.error("err")
来源：http://hz.nwbrower.top/gtxerdzgpv.html

Java: System.err.println("err")
来源：http://hz.redwolf501.top/gtdwskfxuu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.tian-w.cn/gtdjqtmans.html

Ruby: warn "err"
来源：http://hz.xinyue.icu/gtlzqgebzs.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jqgfzy.top/gtpddioutx.html

[M07] 判断是否为主入口
来源：http://hz.bjfxy.top/gtopipwjxq.html

Py:   if __name__ == "__main__":
来源：http://hz.xziqi.cn/gtdikicxcp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.kuanghao11.cn/gtedtdwfsg.html

JS:   require.main === module
来源：http://hz.redwolf501.top/gtksnaftax.html

TS:   require.main === module
来源：http://hz.jinqigufen.top/gtbvmgceyp.html

Java: public static void main(String[] args)
来源：http://hz.jlsjyb.cn/gtkmjcyrhb.html

Go:   func main()
来源：http://hz.zhijiandao.cn/gttdkyssex.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinghuilouyu.cn/gtrnvttqik.html

C#:   static void Main(string[] args)
来源：http://hz.hysaishi.cn/gtbeuygtnf.html

[M08] 获取系统与运行时信息
来源：http://hz.ydjk.org.cn/gtzqxzorsv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.kuanghao11.cn/gturwtqric.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sysykeji.top/gtfpvettuk.html

JS:   process.platform;  process.version
来源：http://hz.cheryme.top/gteztikkdo.html

TS:   process.platform;  process.version
来源：http://hz.smart0.xyz/gtcnlxyjjd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhaomingkeji.xyz/gtpkoijulg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hammf.cn/gtwvowocjw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ehwqpu.com/gtwlxwysrg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sufxvd.cn/gtkgudhrfc.html

================================================================================
来源：http://hz.xinyue.icu/gtdbquezrq.html

N. 数据结构与算法
来源：http://hz.xuanzx.com/gtjkedapvh.html

================================================================================
来源：http://hz.zhengqikj.top/gtbsquwedy.html

[N01] 二分查找（有序数组）
来源：http://hz.dianchejie.cn/gtgrqbleso.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jqgufenzy.top/gtmctyixcr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.chenlongwang.top/gtuuukvctw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangshuangyany.cn/gtcdvymuxy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cucudq.cn/gtkhlrjoxd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.vqdsnc.cn/gtpezdpawc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yj20258.top/gtlqabohix.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ivvv.top/gtgmkmfcsk.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.tian-w.cn/gtmlkapgkc.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gogol.net.cn/gtnceahjzh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gotoacloud.top/gtogtngvrg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.andypj.xyz/gtjwtjefrv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gthselhdmm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinqigfzy.top/gtsdlecfqz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.redwolf501.top/gtxlhlhfuz.html

Go:   slices.Sort(arr)
来源：http://hz.xziqi.cn/gtqmldsuzs.html

Ruby: arr.sort
来源：http://hz.daxiang520.top/gtwyksrxxi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ppjwa.cn/gtvtgniitq.html

[N03] 快速排序（分治示例）
来源：http://hz.vqdsnc.cn/gtxbnlpwsb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhongyouzk.top/gtsrobhgsc.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gaohongyu789.top/gthtovokme.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinghuilouyu.cn/gtywigkaki.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yueranfly.top/gtklrkropo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cqqwz.cn/gtduqxqmsi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhongyouzk.top/gtkbrrvyrf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.pengpengdd.cyou/gtvuduawrj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shuidangran.top/gtssoaxwni.html

[N04] 斐波那契数列
来源：http://hz.jianghu66.top/gtnllqxgnm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.nanxuanxn.top/gtuugtvgkd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.0kj1m.cn/gttxuxznem.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.birdmap.top/gtbuzzbgjk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xingfuxueyuan.xyz/gtozemkdnk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.feifeiyinyue.top/gtbtpplbks.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhixingplan.top/gttdnssjrh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hongshengwenyu.top/gtzwzewimd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinqigufen.top/gtwqfpatqb.html

[N05] 最大公约数
来源：http://hz.ppjwa.cn/gtxcshwgqd.html

Py:   math.gcd(a, b)
来源：http://hz.meibo888.top/gtwaorttkx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yonumen.top/gtyhlfzrrl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.316326.xyz/gtfngwdhqg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhijiandao.cn/gtivrecuud.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.52xcode.cn/gtjeoeogsp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.havefunace.top/gtpxhoewfb.html

Ruby: a.gcd(b)
来源：http://hz.cashguo.top/gtjsyepyjt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinqigufen.top/gtyaejtjvq.html

[N06] 判断回文字符串
来源：http://hz.sxryk.cn/gtynczxlhy.html

Py:   s == s[::-1]
来源：http://hz.tian-w.cn/gtpzxzdmbr.html

PHP:  $s === strrev($s);
来源：http://hz.zhijiandao.cn/gtpwkdqoqf.html

JS:   s === [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtxyzakgqz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtaubpizsf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yj20258.top/gtdcfvbvmn.html

Go:   // 双指针从两端比较
来源：http://hz.tian-w.cn/gtzvgxyrot.html

Ruby: s == s.reverse
来源：http://hz.hnqzz.top/gtodjyrxij.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.316326.xyz/gthpbklxpg.html

[N07] 两数之和（返回下标）
来源：http://hz.yongpay.top/gtspxkhzdu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jiagoushi.top/gtaeppmewi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.pengpengdd.cyou/gtnkdcivvi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yuxming.cn/gtalgzhfaj.html

TS:   // 手写 Map<string, number>
来源：http://hz.dianchejie.cn/gtjdftvfeo.html

Java: // 手写 HashMap
来源：http://hz.cashguo.top/gtfewzvcdo.html

Go:   // 手写 map[int]int
来源：http://hz.zhijiandao.cn/gtsasdgukk.html

Ruby: // 手写 Hash
来源：http://hz.yuanzhike.top/gtjyoowzde.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sweek.top/gtrozlmstb.html

[N08] 生成全排列
来源：http://hz.jqgfzy.top/gtbdywbzpg.html

Py:   itertools.permutations(arr)
来源：http://hz.zhoulong.xyz/gtbwpgpkfb.html

PHP:  // 手写递归交换
来源：http://hz.zycfv.cn/gtknqujlhw.html

JS:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtbdhorwtg.html

TS:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtaakqcqbn.html

Java: // 手写回溯递归
来源：http://hz.xinyue.icu/gtgkcdbfbs.html

Go:   // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtrltovhcr.html

Ruby: arr.permutation.to_a
来源：http://hz.mhx1999.top/gtwifemylv.html

C#:   // 手写回溯递归
来源：http://hz.hammf.cn/gtkqovdabl.html

[N09] 栈与队列
来源：http://hz.cheryme.top/gtjhcecimz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.mhx1999.top/gtcloiahxq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ivvv.top/gtrvtvynkf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yuanzhike.top/gtvjiuscbb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj20258.top/gtyzcvyyiu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gogol.net.cn/gtkzzwkukg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.mhx1999.top/gtxtdoogzo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.316326.xyz/gtrmzigclw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jianghu66.top/gtwsoknoju.html

[N10] 链表节点定义
来源：http://hz.tianlin.xyz/gtupceoeyj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jqgufenzy.top/gtmcvorvok.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.316326.xyz/gtwzlpplew.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.c1oappe.top/gtvyujghmi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.iojbl.cn/gtnasjpkhh.html

Java: class Node { int v; Node next; }
来源：http://hz.wangdashe.top/gtfwcjbwrj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.pengpengdd.cyou/gtsinzeogs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.andypj.xyz/gtjrjdvuec.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.chenzaomai.com/gtyuulcuei.html

[N11] 二叉树中序遍历
来源：http://hz.yongpay.top/gtpufcblpp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.chenlongwang.top/gtsajltpms.html

PHP:  // 手写递归函数
来源：http://hz.xingfuxueyuan.xyz/gtyjmowxqv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinghuilouyu.cn/gtnziubrel.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gotoacloud.top/gtevapkrtq.html

Java: // 手写递归
来源：http://hz.cqqwz.cn/gtmzktcxgj.html

Go:   // 手写递归
来源：http://hz.havefunace.top/gtjwzrnitn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.quarkkingdee.top/gtfismckvs.html

C#:   // 手写递归
来源：http://hz.hysaishi.cn/gttkmjlzem.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.tanke756.top/gtacyijfoy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hnqzz.top/gtwfgbkqdn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.meibo888.top/gtrddzavav.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shangyingyoupin.top/gtdfrbfqsw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xziqi.cn/gtwkmiwksl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.redwolf501.top/gtjqyejaal.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.quarkkingdee.top/gthsoffxdf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sysykeji.top/gtflhklmje.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hnqzz.top/gtkkutthgv.html

================================================================================
来源：http://hz.havefunace.top/gtvtyirwbd.html

O. 并发与异步
来源：http://hz.chenzaomai.com/gtxgtvracw.html

================================================================================
来源：http://hz.aizwys.cn/gttfysjcog.html

[O01] 启动一个线程
来源：http://hz.jqgufenzy.top/gtjhxadbft.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.wangshuangyany.cn/gthjfqwpsy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.aizwys.cn/gteyqifsoo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gaohongyu789.top/gtfafyaiad.html

TS:   // 同 JS
来源：http://hz.pengpengdd.cyou/gtnlraksbv.html

Java: new Thread(() -> f()).start()
来源：http://hz.yvedp.cn/gtexvscbqd.html

Go:   go f()
来源：http://hz.zhixingplan.top/gtxdaloemi.html

Ruby: Thread.new { f }
来源：http://hz.ybcxt.top/gtcbdhkdiw.html

C#:   Task.Run(() => F());
来源：http://hz.ehwqpu.com/gtalgqxfey.html

[O02] 使用线程池
来源：http://hz.chenlongwang.top/gtqahqoizz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xuetiantiany.cn/gtxwmgyfuu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yuxming.cn/gtnqphzjac.html

JS:   // worker_threads 线程池
来源：http://hz.jinqigfzy.top/gtfyylvggh.html

TS:   // worker_threads 线程池
来源：http://hz.hammf.cn/gtbxujohxe.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jiagoushi.top/gtmxmnnzei.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.quarkkingdee.top/gtviweafdc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.redwolf501.top/gtjaefdvwl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ehwqpu.com/gtkabdpfgr.html

[O03] 加锁保护共享数据
来源：http://hz.bjfxy.top/gtiazaebmk.html

Py:   with lock: shared += 1
来源：http://hz.316326.xyz/gtsafbjxwv.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jinqigfzy.top/gtjbfiplfl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.redwolf501.top/gtzpcktqhc.html

TS:   // 同 JS
来源：http://hz.0kj1m.cn/gtgvryqpks.html

Java: synchronized (this) { shared++; }
来源：http://hz.tianlin.xyz/gtquyohqfp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.guannengcc.top/gtxktqqozn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.fzhhl.top/gtdztvuwks.html

C#:   lock (gate) { shared++; }
来源：http://hz.316326.xyz/gtjhzzedjb.html

[O04] 定义异步函数并等待
来源：http://hz.jqgufenzy.top/gtignyrtsi.html

Py:   async def f():⏎    await g()
来源：http://hz.dashuyun.cn/gtfpzypvfl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ivvv.top/gtugotjsla.html

JS:   async function f() { await g(); }
来源：http://hz.yj20258888.top/gtsnfglhue.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cqqwz.cn/gtiixjsmqi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.snrcjt.cn/gtecjzxdvw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.0kj1m.cn/gtvbyehitg.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.chenlongwang.top/gtgckxmjdg.html

C#:   async Task F() { await G(); }
来源：http://hz.yangfankeji.com/gtvojartpl.html

[O05] 并发执行并等待全部完成
来源：http://hz.snrcjt.cn/gtksvbhagy.html

Py:   asyncio.gather(*tasks)
来源：http://hz.nanxinkj.top/gtaimglyhw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.chenlongwang.top/gtlzfyvbwl.html

JS:   await Promise.all(tasks)
来源：http://hz.chenjidiqi.icu/gtgzivebbl.html

TS:   await Promise.all(tasks)
来源：http://hz.sweek.top/gtdmrnmslp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hysaishi.cn/gtvenqsgpm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xuanzx.com/gtjrcunjvu.html

Ruby: threads.map(&:join)
来源：http://hz.cheryme.top/gtdwzccmxu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shzxlz.cn/gtwxoyzeiz.html

[O06] 使用进程池
来源：http://hz.yanxiufei.cn/gtmdzvxgte.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ehwqpu.com/gtyxnptksj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xuetiantiany.cn/gtbjncrpri.html

JS:   // child_process / cluster 模块
来源：http://hz.cdnleiting.top/gthocuwwlz.html

TS:   // child_process / cluster 模块
来源：http://hz.andypj.xyz/gtdvddcrbx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinghuilouyu.cn/gtpqcshvej.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.aibaodan.cn/gtrznakhdx.html

Ruby: // fork 块
来源：http://hz.yvedp.cn/gtcpcaxoau.html

C#:   Parallel.For
来源：http://hz.ivvv.top/gtrkjviblj.html

================================================================================
来源：http://hz.zdqjudy.top/gtkhzezeuj.html

P. 常用工具函数
来源：http://hz.guowangkeji.top/gtbglnplra.html

================================================================================
来源：http://hz.daxiang520.top/gtoyqedldi.html

[P01] 生成 UUID
来源：http://hz.bjfxy.top/gtkahfcuwb.html

Py:   str(uuid.uuid4())
来源：http://hz.dianchejie.cn/gtauoreapk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hongshengwenyu.top/gtuqlytbtn.html

JS:   crypto.randomUUID()
来源：http://hz.jiagoushi.top/gtfcsqsyzv.html

TS:   crypto.randomUUID()
来源：http://hz.0kj1m.cn/gtzltacqbk.html

Java: UUID.randomUUID().toString()
来源：http://hz.xinyue.icu/gtnmkbjgra.html

Go:   // 用 github.com/google/uuid
来源：http://hz.fzhhl.top/gtfirswfqg.html

Ruby: SecureRandom.uuid
来源：http://hz.zhijiandao.cn/gtplptvfow.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.daxiang520.top/gtbespgxwv.html

[P02] MD5 / SHA256 摘要
来源：http://hz.nwbrower.top/gtgncswpfk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jinqigufen.top/gtvktekdwn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.birdmap.top/gtodxwatwg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.9152youxi.cn/gtoimqdcyq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hywenlv.cn/gtwrpyatpg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhongyouzk.top/gtbkpuqdmp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jiagoushi.top/gtcbzbzdeg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.vqdsnc.cn/gtudymhiiq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ywan-chungtsiang.top/gtvjwpzcty.html

[P03] 生成短随机字符串
来源：http://hz.9152youxi.cn/gteutyulbz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhoulong.xyz/gtbbszhpxj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.sxryk.cn/gtkjxtdfsp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gaohongyu789.top/gtnqozkwjv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jiagoushi.top/gthexntwxt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.daria6918.cn/gtyouaanti.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.snrcjt.cn/gtugccrujb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shanyushiyangtech.top/gtynkrfzly.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gzhubu.top/gtmkzggdmc.html

[P04] 求长度
来源：http://hz.jlsjyb.cn/gtavfbyigy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jqgfzy.top/gteafsvvjk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.316326.xyz/gtgrkjycae.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.mhx1999.top/gtufbplcll.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ehwqpu.com/gthamfoewo.html

Java: list.size();  map.size();  s.length()
来源：http://hz.shanyushiyangkeji.top/gtznlkvxzl.html

Go:   len(arr);  len(m)
来源：http://hz.nanxinkj.top/gtljvzzukv.html

Ruby: x.length;  x.size
来源：http://hz.0kj1m.cn/gtxsnyiraa.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.chenjidiqi.icu/gtcjmonnbm.html

[P05] 判断两个对象内容是否相等
来源：http://hz.vqdsnc.cn/gtrfgmitge.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.wangshuangyany.cn/gtzpvijpik.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.svipenyu.cn/gtylhwhjqc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.fengsongda.top/gttsuopwgt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xziqi.cn/gtcpmqusri.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhongyouzk.top/gtydsvpffy.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zycfv.cn/gtwcwdnbkh.html

Ruby: a == b
来源：http://hz.shuidangran.top/gtluacfebn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.smart0.xyz/gtdclmjnjc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.mhx1999.top/gtgkixzhgn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.chenjidiqi.icu/gtjisjgrio.html

PHP:  if (empty($x)) {}
来源：http://hz.tianlin.xyz/gtdnvpggeu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.nanxuanxn.top/gtzxqsmzya.html

TS:   if (x == null) {}
来源：http://hz.zhengqikj.top/gtaclqtwkt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.kuanghao11.cn/gtffdcsgfj.html

Go:   if x == nil {}
来源：http://hz.hammf.cn/gtuaucxxhl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yangfankeji.com/gtqxedcvzl.html

C#:   if (x is null) {}
来源：http://hz.gzhubu.top/gtotzeitus.html

[P07] 防抖与节流
来源：http://hz.daxiang520.top/gtpvegccux.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.tianlin.xyz/gtndjasgwl.html

PHP:  // 手写时间戳比较
来源：http://hz.redwolf501.top/gtqaocagnc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yanxiufei.cn/gtreqqaepf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.c1oappe.top/gtcxempzjr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.pycfn.com/gtyoylwyru.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.chenzaomai.com/gtszhnckng.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yj20258.top/gtzytiyrwj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.chenjidiqi.icu/gttcjhrhyt.html

[P08] 处理浮点精度问题
来源：http://hz.xylfe.cn/gtmbxhjjbz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.pycfn.com/gtgkwxuysi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhongyouzk.top/gtldcjafis.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yuanzhike.top/gtqcukbdkt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cqqwz.cn/gterwgtomx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.andypj.xyz/gtdstvioof.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shanyushiyangtech.top/gtbsrswyoj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xuanzx.com/gtloskwhoo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.wangdashe.top/gtjyhdgwzh.html

================================================================================
来源：http://hz.shuidangran.top/gtwwghbvcn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.feifeiyinyue.top/gtljcwlyzf.html

================================================================================
来源：http://hz.hnxiangtu.top/gtqzvdufnx.html

[Q01] 创建表
来源：http://hz.cashguo.top/gtekmsxfos.html

CREATE TABLE users (
来源：http://hz.bjfxy.top/gthvryffkb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yongpay.top/gtqavlfpgp.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shzxlz.cn/gtehplmcrd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xingfuxueyuan.xyz/gtmattergz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gotoacloud.top/gtduxsyflu.html

);
来源：http://hz.tanke756.top/gtfbskzqql.html

[Q02] 创建带外键的表
来源：http://hz.daxiang520.top/gtxsewdyet.html

CREATE TABLE orders (
来源：http://hz.birdmap.top/gtmzamkpfu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258888.top/gtrraeczkn.html

user_id INT NOT NULL,
来源：http://hz.meibo888.top/gtijokorjl.html

amount DECIMAL(10, 2),
来源：http://hz.gotoacloud.top/gtqmjfzkxj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.quarkkingdee.top/gtosmcxvyg.html

);
来源：http://hz.52xcode.cn/gthkajzetx.html

[Q03] 增加列
来源：http://hz.feifeiyinyue.top/gtmlrycqrm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.meibo888.top/gtvaujkwsb.html

[Q04] 修改列类型
来源：http://hz.yanxiufei.cn/gtqxbhiemp.html


<!-- 参考信息 -->