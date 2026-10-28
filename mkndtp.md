代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ppjwa.cn/gtdbafmfgq.html

[M05] 设置退出码
来源：http://hz.kuanghao11.cn/gtmskroobr.html

Py:   sys.exit(1)
来源：http://hz.ehwqpu.com/gtalikynih.html

PHP:  exit(1);
来源：http://hz.yj20258888.top/gteklrtiam.html

JS:   process.exit(1)
来源：http://hz.cheryme.top/gtbihtsgpf.html

TS:   process.exit(1)
来源：http://hz.feifeiyinyue.top/gtamfmryfo.html

Java: System.exit(1)
来源：http://hz.xinyue.icu/gtyupuvdmb.html

Go:   os.Exit(1)
来源：http://hz.hammf.cn/gtkwmmketu.html

Ruby: exit 1
来源：http://hz.dashuyun.cn/gtxnrkzwhq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cashguo.top/gtrelipsed.html

[M06] 向标准错误输出
来源：http://hz.redwolf501.top/gtnkdqmril.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yueranfly.top/gtvxgtvdlb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinyuanbaomall.cn/gtjefhvynn.html

JS:   console.error("err")
来源：http://hz.yangfankeji.com/gtwvopwjfq.html

TS:   console.error("err")
来源：http://hz.gogol.net.cn/gtlfmizxld.html

Java: System.err.println("err")
来源：http://hz.316326.xyz/gtgutfkyph.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.chenjidiqi.icu/gtrpuvmfrg.html

Ruby: warn "err"
来源：http://hz.sufxvd.cn/gtwzbmqtvr.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.iojbl.cn/gtocinzkal.html

[M07] 判断是否为主入口
来源：http://hz.xylfe.cn/gtkbshbkfg.html

Py:   if __name__ == "__main__":
来源：http://hz.snrcjt.cn/gtrgpxwdqi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zycfv.cn/gtdwriniba.html

JS:   require.main === module
来源：http://hz.pycfn.com/gtpueygcvh.html

TS:   require.main === module
来源：http://hz.ydzc1.top/gtkumzxbxh.html

Java: public static void main(String[] args)
来源：http://hz.cqqwz.cn/gtmwjrbmxc.html

Go:   func main()
来源：http://hz.tian-w.cn/gtzjowgsdc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hammf.cn/gtxzdxjgfz.html

C#:   static void Main(string[] args)
来源：http://hz.xingfuxueyuan.xyz/gtijrvcepy.html

[M08] 获取系统与运行时信息
来源：http://hz.nanxinkj.top/gttslromdj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinyuanbaomall.cn/gtgplpafft.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cheryme.top/gtxxvqpryf.html

JS:   process.platform;  process.version
来源：http://hz.gotoacloud.top/gtskulqvwh.html

TS:   process.platform;  process.version
来源：http://hz.xziqi.cn/gtdfpfdtrp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.aibaodan.cn/gtreupglmn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cdnleiting.top/gthrdcvpwt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.sweek.top/gtsrvvginq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhengqikj.top/gtclenmtrv.html

================================================================================
来源：http://hz.chenlongwang.top/gtaqpbsame.html

N. 数据结构与算法
来源：http://hz.jinyuanbaomall.cn/gtzpbensbr.html

================================================================================
来源：http://hz.hysaishi.cn/gtldgkzusp.html

[N01] 二分查找（有序数组）
来源：http://hz.yj202588.top/gtadwxofny.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhengqikj.top/gttlicwvfh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.daxiang520.top/gtnpzpowfg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jyoumei.cn/gtmcycxbxh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhijiandao.cn/gtdbixzdxz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.aizwys.cn/gthvntolwx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.wangdashe.top/gticvzmvbo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.kuanghao11.cn/gttldvklxz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ppjwa.cn/gtfnnoybge.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.iojbl.cn/gtpwwsqgfl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xinyue.icu/gtxfvfllcl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cdnleiting.top/gtwawcvvrq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yanxiufei.cn/gtlcvnnkpq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nwbrower.top/gtuwlvcaam.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhiwuduotai.top/gtgkinmfvs.html

Go:   slices.Sort(arr)
来源：http://hz.zhengqikj.top/gtsoohcwvd.html

Ruby: arr.sort
来源：http://hz.gaohongyu789.top/gtaasfqklk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xinyue.icu/gtryrhwmha.html

[N03] 快速排序（分治示例）
来源：http://hz.cashguo.top/gtzsfrmfvq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.andypj.xyz/gttrwobpxn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.c1oappe.top/gthjfhjtvv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.iojbl.cn/gtviaopiez.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nwbrower.top/gtydsegbxr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shanyushiyangtech.top/gtogdqjmrn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hywenlv.cn/gtqkwrmtek.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ppjwa.cn/gtdngqgowp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xinyue.icu/gtwlaguwmq.html

[N04] 斐波那契数列
来源：http://hz.sufxvd.cn/gtmuqggcyk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jiagoushi.top/gttpvxnxaf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinqigfzy.top/gtwyjkrmjh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yueranfly.top/gtuyllyeiw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gtiatoflie.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cashguo.top/gtozralbdl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xingfuxueyuan.xyz/gtrqtqovvo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj202588.top/gtnnrvqpka.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hywenlv.cn/gtoebzzcpg.html

[N05] 最大公约数
来源：http://hz.yj20258.top/gtwhyhywqp.html

Py:   math.gcd(a, b)
来源：http://hz.jinghuilouyu.cn/gtntvddhqc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yj202588.top/gtgspgwtzl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sweek.top/gthmehqpfr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hongshengwenyu.top/gtikbhppie.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ydzc1.top/gtrrobqzye.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hfpthk.cn/gthsatniwg.html

Ruby: a.gcd(b)
来源：http://hz.guannengcc.top/gtnzalzbmx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ydjk.org.cn/gtyeadcsmn.html

[N06] 判断回文字符串
来源：http://hz.gzhubu.top/gtbseglpeg.html

Py:   s == s[::-1]
来源：http://hz.svipenyu.cn/gtcurpnhpm.html

PHP:  $s === strrev($s);
来源：http://hz.gotoacloud.top/gtfbozkkcw.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gtbwyzudqb.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hfpthk.cn/gtxpznxkfd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.nanxinkj.top/gtcivwwfts.html

Go:   // 双指针从两端比较
来源：http://hz.sxryk.cn/gthjagvabn.html

Ruby: s == s.reverse
来源：http://hz.guowangkeji.top/gtfsohunld.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.iojbl.cn/gtyupoyaph.html

[N07] 两数之和（返回下标）
来源：http://hz.yj20258.top/gtzyxlcgdr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ydjk.org.cn/gtafbhnkun.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yvedp.cn/gtkcqfxeda.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.vqdsnc.cn/gtzfrvxdtn.html

TS:   // 手写 Map<string, number>
来源：http://hz.shzxlz.cn/gtgoxjriev.html

Java: // 手写 HashMap
来源：http://hz.yj20258888.top/gtcvuahqhk.html

Go:   // 手写 map[int]int
来源：http://hz.zhaomingkeji.xyz/gtxdepyrre.html

Ruby: // 手写 Hash
来源：http://hz.dianchejie.cn/gtwkgqinmh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gzhubu.top/gtdnrxnkvb.html

[N08] 生成全排列
来源：http://hz.yanxiufei.cn/gtwqndzhwl.html

Py:   itertools.permutations(arr)
来源：http://hz.andypj.xyz/gtoeiklbwm.html

PHP:  // 手写递归交换
来源：http://hz.zhongyouzk.top/gtpcjpdwdv.html

JS:   // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtzxnorvti.html

TS:   // 手写回溯递归
来源：http://hz.pycfn.com/gthoowqsow.html

Java: // 手写回溯递归
来源：http://hz.chenlongwang.top/gttwkgjsjl.html

Go:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtqkyeejjc.html

Ruby: arr.permutation.to_a
来源：http://hz.yongpay.top/gtmyfaytoh.html

C#:   // 手写回溯递归
来源：http://hz.tanke756.top/gtlnvzggat.html

[N09] 栈与队列
来源：http://hz.ppjwa.cn/gtgmspcegi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.guannengcc.top/gtqcwokeuh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hywenlv.cn/gtagrhafpz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.tanke756.top/gtikbbxyqw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zdqjudy.top/gtyzedkzxz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinyuanbaomall.cn/gtqpkaabkd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yonumen.top/gtkuzbdzar.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shuidangran.top/gtwquzsfwo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yueranfly.top/gtmhxjiafn.html

[N10] 链表节点定义
来源：http://hz.zhengqikj.top/gtbnoapnni.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.havefunace.top/gtifrwgabw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.havefunace.top/gthtpzkhwt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.fzhhl.top/gtvsqlgeaw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.meibo888.top/gtihkyocaa.html

Java: class Node { int v; Node next; }
来源：http://hz.ywan-chungtsiang.top/gtlxjxvpmo.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.meibo888.top/gtpdteztvp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.gaohongyu789.top/gtqvvbynjp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.mhx1999.top/gtdvrtkrdp.html

[N11] 二叉树中序遍历
来源：http://hz.yongpay.top/gtpqtknenq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhoulong.xyz/gtrfjmzakj.html

PHP:  // 手写递归函数
来源：http://hz.jyoumei.cn/gtjhpwdqxe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yvedp.cn/gtrjrogxti.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yvedp.cn/gtitohwtbd.html

Java: // 手写递归
来源：http://hz.zhixingplan.top/gtkvrdpzez.html

Go:   // 手写递归
来源：http://hz.kuanghao11.cn/gtfrljnpxq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.snrcjt.cn/gtkjteqmgp.html

C#:   // 手写递归
来源：http://hz.tianlin.xyz/gttydtehkf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinghuilouyu.cn/gtftpqwfmc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.gotoacloud.top/gtyycpdkbg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ywan-chungtsiang.top/gtrzhfwybh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hfpthk.cn/gtsoporvyl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sufxvd.cn/gtjfxpfrma.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nanxinkj.top/gtzvviqxba.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.tian-w.cn/gtyxqiovkb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hammf.cn/gtqsakstua.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigufen.top/gtiqphumhj.html

================================================================================
来源：http://hz.hysaishi.cn/gtlaihacnq.html

O. 并发与异步
来源：http://hz.daxiang520.top/gtdscryxdw.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtfcndzylx.html

[O01] 启动一个线程
来源：http://hz.vqdsnc.cn/gtnyxktmal.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.chenjidiqi.icu/gtoksmnymp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.tanke756.top/gtjcwqrvfk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hnqzz.top/gtckbbkzut.html

TS:   // 同 JS
来源：http://hz.tanke756.top/gtshdgcamw.html

Java: new Thread(() -> f()).start()
来源：http://hz.sxryk.cn/gtrotswnlx.html

Go:   go f()
来源：http://hz.jinghuilouyu.cn/gtaskvwvgp.html

Ruby: Thread.new { f }
来源：http://hz.jinghuilouyu.cn/gtwyfyocpx.html

C#:   Task.Run(() => F());
来源：http://hz.ehwqpu.com/gtsbvhdsvm.html

[O02] 使用线程池
来源：http://hz.ehwqpu.com/gthvgamtps.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.meibo888.top/gtnptjauro.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cqqwz.cn/gtixusmzep.html

JS:   // worker_threads 线程池
来源：http://hz.svipenyu.cn/gthboaebkb.html

TS:   // worker_threads 线程池
来源：http://hz.daria6918.cn/gtxrmjqctd.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.andypj.xyz/gtaifrkmov.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.wangdashe.top/gtpxacqfzp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhixingplan.top/gtzditnamw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhaomingkeji.xyz/gtoiyozdoq.html

[O03] 加锁保护共享数据
来源：http://hz.hammf.cn/gteroaxwia.html

Py:   with lock: shared += 1
来源：http://hz.gaohongyu789.top/gtpyavqzmb.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ywan-chungtsiang.top/gtykxgkmod.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.daria6918.cn/gtvjxayxrc.html

TS:   // 同 JS
来源：http://hz.shzxlz.cn/gthuoufsdm.html

Java: synchronized (this) { shared++; }
来源：http://hz.jqgufenzy.top/gtnrgxcies.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hnxiangtu.top/gthtxmgbuz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.9152youxi.cn/gtlpmozfci.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj20258888.top/gtzijrxfgl.html

[O04] 定义异步函数并等待
来源：http://hz.aizwys.cn/gtsuxevfgf.html

Py:   async def f():⏎    await g()
来源：http://hz.dashuyun.cn/gtpaqvzkmh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.tian-w.cn/gtczegscwa.html

JS:   async function f() { await g(); }
来源：http://hz.xziqi.cn/gtrbilfgqp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.sxryk.cn/gtrqbetqmc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.feifeiyinyue.top/gtjfqnqrdj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yueranfly.top/gthioeofbu.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.bjfxy.top/gtdoplvjpj.html

C#:   async Task F() { await G(); }
来源：http://hz.guannengcc.top/gtldxbrape.html

[O05] 并发执行并等待全部完成
来源：http://hz.shuidangran.top/gtooyouvxk.html

Py:   asyncio.gather(*tasks)
来源：http://hz.kuanghao11.cn/gtqwhywbuv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhixingplan.top/gtptsszofu.html

JS:   await Promise.all(tasks)
来源：http://hz.sysykeji.top/gtpgkyzerv.html

TS:   await Promise.all(tasks)
来源：http://hz.yvedp.cn/gtdzapjstg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.sxryk.cn/gtwofldqzq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sxryk.cn/gttyrevswx.html

Ruby: threads.map(&:join)
来源：http://hz.xuetiantiany.cn/gtbcgstfpw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.gotoacloud.top/gtuixakzpk.html

[O06] 使用进程池
来源：http://hz.xylfe.cn/gtmnuqfvca.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ywan-chungtsiang.top/gtuihyjkeq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhixingplan.top/gtwrsgreux.html

JS:   // child_process / cluster 模块
来源：http://hz.tianlin.xyz/gtjlripfmv.html

TS:   // child_process / cluster 模块
来源：http://hz.ppjwa.cn/gtcmgjcwpi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cheryme.top/gtdzbeuaqz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.havefunace.top/gtnhvortgr.html

Ruby: // fork 块
来源：http://hz.yj202588.top/gtdhrdexkw.html

C#:   Parallel.For
来源：http://hz.feifeiyinyue.top/gtpdmrueky.html

================================================================================
来源：http://hz.yuanzhike.top/gtjuecruuc.html

P. 常用工具函数
来源：http://hz.zhongyouzk.top/gtbrlqmxuw.html

================================================================================
来源：http://hz.hywenlv.cn/gttsgofhap.html

[P01] 生成 UUID
来源：http://hz.pengpengdd.cyou/gtazyqrfam.html

Py:   str(uuid.uuid4())
来源：http://hz.shanyushiyangtech.top/gttkyezglj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.chenlongwang.top/gttoobkffq.html

JS:   crypto.randomUUID()
来源：http://hz.cqqwz.cn/gtrxjxgatv.html

TS:   crypto.randomUUID()
来源：http://hz.guowangkeji.top/gtctiifssv.html

Java: UUID.randomUUID().toString()
来源：http://hz.hfpthk.cn/gtxqzfiuvx.html

Go:   // 用 github.com/google/uuid
来源：http://hz.0kj1m.cn/gtmialbqmq.html

Ruby: SecureRandom.uuid
来源：http://hz.meibo888.top/gtltunuvui.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xziqi.cn/gttpxcierw.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ybcxt.top/gtwxkmxdht.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hysaishi.cn/gtzmmlblfx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.havefunace.top/gtqeltoqog.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinghuilouyu.cn/gteiuacxsw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj202588.top/gtdzogroft.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gogol.net.cn/gtlpbbahyl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.haohaochexian.top/gtkjdosxcp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.gaohongyu789.top/gtyncfqpdu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xingfuxueyuan.xyz/gtsqbsghiz.html

[P03] 生成短随机字符串
来源：http://hz.andypj.xyz/gtxkhsupem.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xinyue.icu/gtxmchsyse.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.aizwys.cn/gttvmpojcb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hfpthk.cn/gtminzfimp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yanxiufei.cn/gtpacbhfbj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ywan-chungtsiang.top/gtlnojkgru.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.havefunace.top/gtzknigvvp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yj20258888.top/gthlexruba.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.aizwys.cn/gtlhemoqks.html

[P04] 求长度
来源：http://hz.cheryme.top/gtxqaamnat.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.daxiang520.top/gtottjqles.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hywenlv.cn/gtmcriaing.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yongpay.top/gtwojoathn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dashuyun.cn/gtvjihpnyd.html

Java: list.size();  map.size();  s.length()
来源：http://hz.feifeiyinyue.top/gtdwlwqjdk.html

Go:   len(arr);  len(m)
来源：http://hz.52xcode.cn/gtrhkslqdw.html

Ruby: x.length;  x.size
来源：http://hz.cheryme.top/gthheishfw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhengqikj.top/gtcnqkixor.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yvedp.cn/gtiunolsdx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhijiandao.cn/gtebtuybjq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhengqikj.top/gtagbzdspw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.wangshuangyany.cn/gtuyzlkfsm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgfzy.top/gtmwllpmpx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yongpay.top/gtqsgbamea.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.guannengcc.top/gtzuxobbeb.html

Ruby: a == b
来源：http://hz.jinqigufen.top/gtvyihnlte.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jlsjyb.cn/gtdlnkrjgw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tian-w.cn/gtbtyecvzd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.9152youxi.cn/gtlmcyuzvh.html

PHP:  if (empty($x)) {}
来源：http://hz.zhengqikj.top/gtjwviaonj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yj202588.top/gtguzditxm.html

TS:   if (x == null) {}
来源：http://hz.yj202588.top/gtvcyrgvar.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.guannengcc.top/gtefrzechm.html

Go:   if x == nil {}
来源：http://hz.ivvv.top/gtbhnxcmfl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhongyouzk.top/gtjfnfwsja.html

C#:   if (x is null) {}
来源：http://hz.yangfankeji.com/gtxszoifcq.html

[P07] 防抖与节流
来源：http://hz.ehwqpu.com/gtvbsnjofv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yj20258.top/gtutweghlx.html

PHP:  // 手写时间戳比较
来源：http://hz.smart0.xyz/gthsiidwpy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fengsongda.top/gtthcrcqqb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tanke756.top/gthlbqqloy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shzxlz.cn/gtajewtfld.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ivvv.top/gtfmmibhar.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhaomingkeji.xyz/gtaimljtoo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.snrcjt.cn/gttduavven.html

[P08] 处理浮点精度问题
来源：http://hz.ppjwa.cn/gtnmdhogku.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.andypj.xyz/gtdybhamxn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yj202588.top/gtdyimhyka.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sxryk.cn/gtkykakosz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yanxiufei.cn/gtmvvfotmt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.smart0.xyz/gteaomyeky.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.guannengcc.top/gtvxghpybx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shuidangran.top/gtdyxvsmux.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.0kj1m.cn/gtvhlzzcee.html

================================================================================
来源：http://hz.tianlin.xyz/gtnseafrtu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yvedp.cn/gtvlhdomrm.html

================================================================================
来源：http://hz.zhoulong.xyz/gtacfjrdfl.html

[Q01] 创建表
来源：http://hz.hysaishi.cn/gtufwzgrlh.html

CREATE TABLE users (
来源：http://hz.dianchejie.cn/gtqqeatgzd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.smart0.xyz/gtueywbsrt.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hysaishi.cn/gtphxoxxhk.html

email VARCHAR(100) UNIQUE,
来源：http://hz.fengsongda.top/gtscewuyqy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shzxlz.cn/gtllyiburs.html

);
来源：http://hz.316326.xyz/gtpcftlgtn.html

[Q02] 创建带外键的表
来源：http://hz.cdnleiting.top/gtclvgjcmw.html

CREATE TABLE orders (
来源：http://hz.hywenlv.cn/gtwwgapicz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yanxiufei.cn/gtcombsaks.html

user_id INT NOT NULL,
来源：http://hz.jinqigfzy.top/gtdolgfuhd.html

amount DECIMAL(10, 2),
来源：http://hz.jqgufenzy.top/gtzoblezqz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.fengsongda.top/gtxgnqfrwa.html

);
来源：http://hz.aibaodan.cn/gtwcitvrpb.html

[Q03] 增加列
来源：http://hz.sufxvd.cn/gtnjbitsev.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yangfankeji.com/gtvuusixal.html

[Q04] 修改列类型
来源：http://hz.jiagoushi.top/gtbecqgklu.html


<!-- 参考信息 -->