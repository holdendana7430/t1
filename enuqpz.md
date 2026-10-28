代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yj202588.top/gtkvrxbfto.html

JS:   console.error("err")
来源：http://hz.jinyuanbaomall.cn/gtdhgkhdac.html

TS:   console.error("err")
来源：http://hz.pengpengdd.cyou/gtrtpnztsa.html

Java: System.err.println("err")
来源：http://hz.iojbl.cn/gtvcmbcvbt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.birdmap.top/gtgzcmmwvj.html

Ruby: warn "err"
来源：http://hz.xinyue.icu/gthrdidehp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cqqwz.cn/gtvebsoqlr.html

[M07] 判断是否为主入口
来源：http://hz.aizwys.cn/gtkidrkfsu.html

Py:   if __name__ == "__main__":
来源：http://hz.xuetiantiany.cn/gtcdvhaczx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.havefunace.top/gtodbqrxir.html

JS:   require.main === module
来源：http://hz.wangdashe.top/gtpfgidjrk.html

TS:   require.main === module
来源：http://hz.zdqjudy.top/gtaciyxzzc.html

Java: public static void main(String[] args)
来源：http://hz.yonumen.top/gthaxhtjfc.html

Go:   func main()
来源：http://hz.ydjk.org.cn/gtzvxtbyst.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.wangshuangyany.cn/gtukccluzx.html

C#:   static void Main(string[] args)
来源：http://hz.shuidangran.top/gtxvbjwgep.html

[M08] 获取系统与运行时信息
来源：http://hz.yvedp.cn/gteygxtude.html

Py:   platform.system();  platform.python_version()
来源：http://hz.tanke756.top/gtjojwynue.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yj20258.top/gtcxoyygfc.html

JS:   process.platform;  process.version
来源：http://hz.xylfe.cn/gtjkphtnwe.html

TS:   process.platform;  process.version
来源：http://hz.jianghu66.top/gtnroowurb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.52xcode.cn/gttancgqvb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shuidangran.top/gtwpntzlzz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.tian-w.cn/gtswwsdrhr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yuanzhike.top/gtmzliuwwq.html

================================================================================
来源：http://hz.c1oappe.top/gtazepvrbk.html

N. 数据结构与算法
来源：http://hz.smart0.xyz/gtzuyimmxo.html

================================================================================
来源：http://hz.ehwqpu.com/gtzqihqcxk.html

[N01] 二分查找（有序数组）
来源：http://hz.pycfn.com/gtbamjalyp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jqgfzy.top/gtttdqptly.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jianghu66.top/gtkyopwebm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhijiandao.cn/gtqoxwpcid.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.havefunace.top/gtvdnwgdyh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.redwolf501.top/gtfdwhnqwz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.bjfxy.top/gtgsayxboi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.vqdsnc.cn/gtpmyrwmvp.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gtafpaofyw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jinqigfzy.top/gtiedbjvdc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cucudq.cn/gtknmpqazt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ydzc1.top/gtsxfglhhk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gtdpdkciwu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenjidiqi.icu/gtnbgzgsvu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.316326.xyz/gtvglrzybr.html

Go:   slices.Sort(arr)
来源：http://hz.shzxlz.cn/gtgbkmcoln.html

Ruby: arr.sort
来源：http://hz.jyoumei.cn/gtkmvzzvty.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yongpay.top/gttctyxtke.html

[N03] 快速排序（分治示例）
来源：http://hz.pycfn.com/gtpovavbpe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hysaishi.cn/gtqzpndwdy.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhengqikj.top/gtkiwlckls.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yvedp.cn/gtoswjpvzd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hongshengwenyu.top/gtrxhputtr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shuidangran.top/gtruyorotp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yuanzhike.top/gtalrqbjzm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hammf.cn/gttgufmhcc.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yj202588.top/gtvhzpecqs.html

[N04] 斐波那契数列
来源：http://hz.yonumen.top/gtxdozavhe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.redwolf501.top/gtzqhhgfim.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.smart0.xyz/gtpelgfdem.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ydzc1.top/gtrbxbjkkw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.havefunace.top/gtxykuitvf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sxryk.cn/gtqlrbvhle.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sufxvd.cn/gtofkxcboq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cheryme.top/gtfamrrazs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.daria6918.cn/gtbmosdupe.html

[N05] 最大公约数
来源：http://hz.jinyuanbaomall.cn/gtupnpeyvj.html

Py:   math.gcd(a, b)
来源：http://hz.hnqzz.top/gtitvskjne.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ppjwa.cn/gthznufsob.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj20258.top/gtggukmcfp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigufen.top/gtlqyykhxs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yongpay.top/gttzhjwqan.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shanyushiyangkeji.top/gtvyrrzmku.html

Ruby: a.gcd(b)
来源：http://hz.yanxiufei.cn/gtwbyxjqgw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jiagoushi.top/gtchvdrfiz.html

[N06] 判断回文字符串
来源：http://hz.ywan-chungtsiang.top/gtszxttmyw.html

Py:   s == s[::-1]
来源：http://hz.hysaishi.cn/gtgqvlurhy.html

PHP:  $s === strrev($s);
来源：http://hz.iojbl.cn/gtygvjxzdr.html

JS:   s === [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtkwfqtndr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtjujwsyxz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yj20258888.top/gthhhfjhmc.html

Go:   // 双指针从两端比较
来源：http://hz.hysaishi.cn/gtoudckslo.html

Ruby: s == s.reverse
来源：http://hz.jlsjyb.cn/gtqjfwwoba.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.havefunace.top/gtpwnpumfr.html

[N07] 两数之和（返回下标）
来源：http://hz.jiagoushi.top/gttcwihcfg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinghuilouyu.cn/gtjadrhkgo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.nanxuanxn.top/gtfulfnudt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ybcxt.top/gtpfeuueyu.html

TS:   // 手写 Map<string, number>
来源：http://hz.jyoumei.cn/gtextdisbp.html

Java: // 手写 HashMap
来源：http://hz.ydzc1.top/gtjjqjwqnq.html

Go:   // 手写 map[int]int
来源：http://hz.zhongyouzk.top/gtttnncbje.html

Ruby: // 手写 Hash
来源：http://hz.316326.xyz/gtozqrhrwc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yanxiufei.cn/gtakbtcfxc.html

[N08] 生成全排列
来源：http://hz.yj202588.top/gtoqylyjju.html

Py:   itertools.permutations(arr)
来源：http://hz.jqgfzy.top/gtwfpsaspi.html

PHP:  // 手写递归交换
来源：http://hz.cucudq.cn/gtqbxhkfyd.html

JS:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtoumafqra.html

TS:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtkrvqatcj.html

Java: // 手写回溯递归
来源：http://hz.0kj1m.cn/gtstaxootj.html

Go:   // 手写回溯递归
来源：http://hz.quarkkingdee.top/gtbdnpohfy.html

Ruby: arr.permutation.to_a
来源：http://hz.zhoulong.xyz/gtayimzutj.html

C#:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtyhmkqldi.html

[N09] 栈与队列
来源：http://hz.zycfv.cn/gtjbbdqzro.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.aizwys.cn/gtoijfcxbz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.shuidangran.top/gtzufqyupl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.daxiang520.top/gtgjgzogia.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xinyue.icu/gtlhbdxsyx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.svipenyu.cn/gtsjlxakcr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yj20258888.top/gtpcrvseju.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xziqi.cn/gtjvvfcrku.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.sysykeji.top/gtwilqhmyy.html

[N10] 链表节点定义
来源：http://hz.0kj1m.cn/gtjsvxqgnj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.meibo888.top/gtduusjmfi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.guannengcc.top/gteqpmggee.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.shuidangran.top/gtptujlcvt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hnqzz.top/gtuacpbfmh.html

Java: class Node { int v; Node next; }
来源：http://hz.jinqigufen.top/gtdzpalwnl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zdqjudy.top/gtpthcjdgx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yuxming.cn/gtpaiimmku.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yvedp.cn/gtdntljigr.html

[N11] 二叉树中序遍历
来源：http://hz.tanke756.top/gtumtmnfoh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yonumen.top/gtotztvaus.html

PHP:  // 手写递归函数
来源：http://hz.wangshuangyany.cn/gtiedrxarq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.c1oappe.top/gtyrcojzjx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gzhubu.top/gtueosnjbp.html

Java: // 手写递归
来源：http://hz.hammf.cn/gtlxmmffay.html

Go:   // 手写递归
来源：http://hz.xinyue.icu/gtyqmadocj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xylfe.cn/gtzwflifwz.html

C#:   // 手写递归
来源：http://hz.tian-w.cn/gtjxralkwa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yonumen.top/gtxbhdbzty.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yueranfly.top/gtfgyvilxi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.316326.xyz/gtydzcxtea.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sufxvd.cn/gteshcllkc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sweek.top/gtdtlhlgax.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangshuangyany.cn/gtjqfubtxw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenjidiqi.icu/gtcbotkify.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hammf.cn/gtlasfqohx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuetiantiany.cn/gtbntfcese.html

================================================================================
来源：http://hz.andypj.xyz/gttgkioeqw.html

O. 并发与异步
来源：http://hz.zhiwuduotai.top/gtyarhvayv.html

================================================================================
来源：http://hz.sxryk.cn/gtlptcppvz.html

[O01] 启动一个线程
来源：http://hz.iojbl.cn/gtodbxiwfk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.vqdsnc.cn/gtuxtpvhhi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ehwqpu.com/gtnuiqtqin.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.daxiang520.top/gtemprwpjs.html

TS:   // 同 JS
来源：http://hz.guannengcc.top/gtjuqagdra.html

Java: new Thread(() -> f()).start()
来源：http://hz.fengsongda.top/gtlhzovwkw.html

Go:   go f()
来源：http://hz.ywan-chungtsiang.top/gtvmbphtxq.html

Ruby: Thread.new { f }
来源：http://hz.yuxming.cn/gtaknwcsdz.html

C#:   Task.Run(() => F());
来源：http://hz.sufxvd.cn/gtjkfmwlit.html

[O02] 使用线程池
来源：http://hz.hnqzz.top/gtpyfppiuh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xinyue.icu/gtsldztfpz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ywan-chungtsiang.top/gtmwqdwlsm.html

JS:   // worker_threads 线程池
来源：http://hz.tanke756.top/gtjtjidbia.html

TS:   // worker_threads 线程池
来源：http://hz.chenlongwang.top/gtdovehaow.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.aibaodan.cn/gtwqhockum.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yonumen.top/gtumespfaa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xylfe.cn/gtlngsgnqw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.0kj1m.cn/gtfvtvonsx.html

[O03] 加锁保护共享数据
来源：http://hz.smart0.xyz/gtmvcmacer.html

Py:   with lock: shared += 1
来源：http://hz.yj20258.top/gtguhywnfi.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.vqdsnc.cn/gtenajfgaa.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.mhx1999.top/gtjveneyrl.html

TS:   // 同 JS
来源：http://hz.hysaishi.cn/gtsclvyvmf.html

Java: synchronized (this) { shared++; }
来源：http://hz.gaohongyu789.top/gtlqnbffzo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.sxryk.cn/gtjnyedttn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cucudq.cn/gtugikkura.html

C#:   lock (gate) { shared++; }
来源：http://hz.shanyushiyangtech.top/gthirrmmgn.html

[O04] 定义异步函数并等待
来源：http://hz.ydzc1.top/gtzsjzlebs.html

Py:   async def f():⏎    await g()
来源：http://hz.tianlin.xyz/gtefpifgvf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.daxiang520.top/gtymxulzpc.html

JS:   async function f() { await g(); }
来源：http://hz.cheryme.top/gtkbopzllq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yj20258.top/gtyoksxsef.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ppjwa.cn/gthnhfttyp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.svipenyu.cn/gtewjdvagt.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.vqdsnc.cn/gtkbsswknl.html

C#:   async Task F() { await G(); }
来源：http://hz.jinghuilouyu.cn/gtrpubdtnq.html

[O05] 并发执行并等待全部完成
来源：http://hz.wangdashe.top/gtznvpiysh.html

Py:   asyncio.gather(*tasks)
来源：http://hz.vqdsnc.cn/gtbezkchuf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xingfuxueyuan.xyz/gtfrjckdvq.html

JS:   await Promise.all(tasks)
来源：http://hz.tian-w.cn/gtkqadtfhd.html

TS:   await Promise.all(tasks)
来源：http://hz.ydzc1.top/gtcjuvikiw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ybcxt.top/gtdeujrsju.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cqqwz.cn/gtlskyechm.html

Ruby: threads.map(&:join)
来源：http://hz.cdnleiting.top/gtglkyjssw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ywan-chungtsiang.top/gtazhosytz.html

[O06] 使用进程池
来源：http://hz.gaohongyu789.top/gthpmmtlqw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yueranfly.top/gtucherpim.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.smart0.xyz/gtfsilzmps.html

JS:   // child_process / cluster 模块
来源：http://hz.sufxvd.cn/gtcynmwiow.html

TS:   // child_process / cluster 模块
来源：http://hz.gogol.net.cn/gtjnsuxxbh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cashguo.top/gtbeaxtlmv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.smart0.xyz/gtwokqrbie.html

Ruby: // fork 块
来源：http://hz.nanxuanxn.top/gtnerexbgw.html

C#:   Parallel.For
来源：http://hz.tanke756.top/gtxzgmyrwd.html

================================================================================
来源：http://hz.ydjk.org.cn/gtsiyhrnoq.html

P. 常用工具函数
来源：http://hz.yj20258.top/gtqcrkblsc.html

================================================================================
来源：http://hz.tianlin.xyz/gtxcxvuhwj.html

[P01] 生成 UUID
来源：http://hz.jinqigufen.top/gtdynfwgaf.html

Py:   str(uuid.uuid4())
来源：http://hz.yanxiufei.cn/gtcgjaqfdd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhongyouzk.top/gtsfpgdlmz.html

JS:   crypto.randomUUID()
来源：http://hz.daxiang520.top/gtiifcbnnc.html

TS:   crypto.randomUUID()
来源：http://hz.jiagoushi.top/gtqysloixn.html

Java: UUID.randomUUID().toString()
来源：http://hz.xziqi.cn/gtiwifbysb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ydjk.org.cn/gteeaixxjj.html

Ruby: SecureRandom.uuid
来源：http://hz.pengpengdd.cyou/gtkczmmjzm.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinyuanbaomall.cn/gtzvtlwnjj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.wangshuangyany.cn/gtnaxdtdzl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gzhubu.top/gtdibwmmxe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.aibaodan.cn/gtqnkcfmfw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jqgufenzy.top/gtidvadqsm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jinqigufen.top/gtlizetffp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.pycfn.com/gtlqqlfxkp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cucudq.cn/gtiecmmozv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.aizwys.cn/gtiiztcmsk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.bjfxy.top/gtbfqvwxvu.html

[P03] 生成短随机字符串
来源：http://hz.9152youxi.cn/gtxrrzsosd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.9152youxi.cn/gtjpvwvnek.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.nwbrower.top/gtuzleoyfd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuxming.cn/gtkwwuznus.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dianchejie.cn/gthdevhlxy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ivvv.top/gtfntnffmy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shanyushiyangkeji.top/gtrlydzvaz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.tanke756.top/gtveywnvbs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gogol.net.cn/gtccnssfob.html

[P04] 求长度
来源：http://hz.kuanghao11.cn/gthriyurqf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.chenzaomai.com/gtpgwqhlrj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.bjfxy.top/gtenbzrndh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yanxiufei.cn/gtxkbpfnke.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shanyushiyangkeji.top/gtwtyygruc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.pycfn.com/gtvvrydwxr.html

Go:   len(arr);  len(m)
来源：http://hz.zhaomingkeji.xyz/gtyeahciou.html

Ruby: x.length;  x.size
来源：http://hz.vqdsnc.cn/gthplvcsat.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.daria6918.cn/gtalztjshg.html

[P05] 判断两个对象内容是否相等
来源：http://hz.cdnleiting.top/gtkrohvdlf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.wangdashe.top/gtjvlfwuhi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cdnleiting.top/gthivlmmge.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jqgfzy.top/gteccvjxrf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cucudq.cn/gtrgwmkuzo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yonumen.top/gtmozzddpi.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.dashuyun.cn/gtgxtnaacy.html

Ruby: a == b
来源：http://hz.yj20258888.top/gtzkjorcbm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zdqjudy.top/gthegslcmi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cashguo.top/gtzedapijy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xuetiantiany.cn/gtxbgivvrk.html

PHP:  if (empty($x)) {}
来源：http://hz.hnxiangtu.top/gtffwqsntb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cucudq.cn/gtzuadlaxy.html

TS:   if (x == null) {}
来源：http://hz.yangfankeji.com/gtzrakcbvy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shangyingyoupin.top/gtphniuoiz.html

Go:   if x == nil {}
来源：http://hz.shuidangran.top/gtumckkxdq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yangfankeji.com/gtdcuohkti.html

C#:   if (x is null) {}
来源：http://hz.vqdsnc.cn/gtrxwaaboa.html

[P07] 防抖与节流
来源：http://hz.daxiang520.top/gtuszzpqqe.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhaomingkeji.xyz/gtwirpbukm.html

PHP:  // 手写时间戳比较
来源：http://hz.shangyingyoupin.top/gtbctrwqzh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.svipenyu.cn/gtnhpnoukp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258888.top/gtzgtzymga.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.snrcjt.cn/gtgpkcoqmx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hnxiangtu.top/gtunndrnnx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cheryme.top/gtvrmgbpwe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hnqzz.top/gtuhnlpoqe.html

[P08] 处理浮点精度问题
来源：http://hz.aizwys.cn/gtxchbzjnd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.wangshuangyany.cn/gtpjlfpvjq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhengqikj.top/gthbvzvqpj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.kuanghao11.cn/gtdxtyvgao.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.meibo888.top/gtlxoyljiw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yangfankeji.com/gtddpziszi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jiagoushi.top/gtyuddumfr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yonumen.top/gtplasffhd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ehwqpu.com/gtwskgszsz.html

================================================================================
来源：http://hz.9152youxi.cn/gtlfmarlcd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.chenzaomai.com/gtwvgytlpi.html

================================================================================
来源：http://hz.yj20258.top/gtubuzeyra.html

[Q01] 创建表
来源：http://hz.zhijiandao.cn/gtkdnwcvof.html

CREATE TABLE users (
来源：http://hz.ehwqpu.com/gtjyaokbon.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.haohaochexian.top/gtpqqoafey.html

name VARCHAR(50) NOT NULL,
来源：http://hz.gogol.net.cn/gtxmmnohve.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yongpay.top/gtpnbeuxok.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yanxiufei.cn/gtvhhflqam.html

);
来源：http://hz.gogol.net.cn/gtoglsmwpg.html

[Q02] 创建带外键的表
来源：http://hz.chenlongwang.top/gturgtavjt.html

CREATE TABLE orders (
来源：http://hz.hnqzz.top/gtmqzzeccq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.0kj1m.cn/gtzwgpnqdc.html

user_id INT NOT NULL,
来源：http://hz.yonumen.top/gtnymlktni.html

amount DECIMAL(10, 2),
来源：http://hz.zhongyouzk.top/gtfzxnriyz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cheryme.top/gtwldgaekk.html

);
来源：http://hz.hammf.cn/gtmsumrdog.html

[Q03] 增加列
来源：http://hz.cqqwz.cn/gtkzqjrmou.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yonumen.top/gttkggyxym.html

[Q04] 修改列类型
来源：http://hz.zhengqikj.top/gthyfbqtmg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yonumen.top/gtvoqpgagx.html

[Q05] 重命名列
来源：http://hz.hysaishi.cn/gtiuqfgeri.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nwbrower.top/gtjukrcffj.html

[Q06] 删除列
来源：http://hz.guannengcc.top/gtayqhxzrg.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.dashuyun.cn/gttsztragx.html

[Q07] 删除表
来源：http://hz.gzhubu.top/gtrkrifatg.html

DROP TABLE IF EXISTS orders;
来源：http://hz.haohaochexian.top/gtqvwlmihd.html

[Q08] 创建普通索引
来源：http://hz.yj20258888.top/gtkxgmdqgx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.chenjidiqi.icu/gtgagitbup.html

[Q09] 创建唯一索引
来源：http://hz.jinyuanbaomall.cn/gtzsftwqgc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.guowangkeji.top/gtoeheaiww.html

[Q10] 插入单行
来源：http://hz.hywenlv.cn/gtevkomrsa.html


<!-- 参考信息 -->