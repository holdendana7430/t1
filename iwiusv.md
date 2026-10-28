代发 wailian999

Ruby: exit 1
来源：http://hz.zhixingplan.top/gtwyoiprlc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.feifeiyinyue.top/gtassznywl.html

[M06] 向标准错误输出
来源：http://hz.zhongyouzk.top/gtpvumutnl.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ehwqpu.com/gtmtqloach.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yuanzhike.top/gtrclspzvc.html

JS:   console.error("err")
来源：http://hz.sufxvd.cn/gtthgzcbvj.html

TS:   console.error("err")
来源：http://hz.zycfv.cn/gthmwpzoow.html

Java: System.err.println("err")
来源：http://hz.yonumen.top/gtljnjlfzd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.316326.xyz/gtqgczpsus.html

Ruby: warn "err"
来源：http://hz.jinyuanbaomall.cn/gtupesvubl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xylfe.cn/gtttbmxrnu.html

[M07] 判断是否为主入口
来源：http://hz.xuanzx.com/gtdercznfr.html

Py:   if __name__ == "__main__":
来源：http://hz.xziqi.cn/gtkdvqvaah.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.bjfxy.top/gtvpqcxqfh.html

JS:   require.main === module
来源：http://hz.jyoumei.cn/gtxcgningw.html

TS:   require.main === module
来源：http://hz.yuanzhike.top/gtcraluwkq.html

Java: public static void main(String[] args)
来源：http://hz.xuetiantiany.cn/gtcehfkqxl.html

Go:   func main()
来源：http://hz.sxryk.cn/gtcxscxnwo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.chenlongwang.top/gtwoatrefm.html

C#:   static void Main(string[] args)
来源：http://hz.yuxming.cn/gtvjyxawxx.html

[M08] 获取系统与运行时信息
来源：http://hz.jinqigfzy.top/gthgysspzu.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinqigfzy.top/gtzapbeclc.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sweek.top/gtgqccddzu.html

JS:   process.platform;  process.version
来源：http://hz.jiagoushi.top/gtmpczsxjg.html

TS:   process.platform;  process.version
来源：http://hz.hongshengwenyu.top/gtdamwhahm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.0kj1m.cn/gtvihynusn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.dianchejie.cn/gtwsgxjaaq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xylfe.cn/gthcpqwlxn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.gotoacloud.top/gtggyawcvs.html

================================================================================
来源：http://hz.jqgufenzy.top/gtesirtvma.html

N. 数据结构与算法
来源：http://hz.chenlongwang.top/gtwgwgfpir.html

================================================================================
来源：http://hz.zycfv.cn/gtsutsiqlw.html

[N01] 二分查找（有序数组）
来源：http://hz.yueranfly.top/gtwshvyguj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhaomingkeji.xyz/gttggoyoop.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cucudq.cn/gtpzhcrfza.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258888.top/gtnbpypacn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yueranfly.top/gtqkiremkj.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shangyingyoupin.top/gtuhcjndlm.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hysaishi.cn/gtessejqwk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinghuilouyu.cn/gtcrmxwqet.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.bjfxy.top/gtnixzglvu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yanxiufei.cn/gtvqnsocar.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jyoumei.cn/gtzvjfztus.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.wangdashe.top/gtiflddtbo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinqigufen.top/gtduqmzncj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ydzc1.top/gtcxpijcsu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinghuilouyu.cn/gtcpvdfgpf.html

Go:   slices.Sort(arr)
来源：http://hz.quarkkingdee.top/gtwagjjyek.html

Ruby: arr.sort
来源：http://hz.yonumen.top/gtduiykook.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yonumen.top/gtexduzevl.html

[N03] 快速排序（分治示例）
来源：http://hz.yj202588.top/gtiocdjllj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shanyushiyangtech.top/gtqnftigyx.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gzhubu.top/gtkshvmovg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yvedp.cn/gtfebanxqx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydzc1.top/gtuwadvypi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.aizwys.cn/gthvsbpgvz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xuanzx.com/gtvndvavls.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hongshengwenyu.top/gthwvmyhvc.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.svipenyu.cn/gtczgdmeac.html

[N04] 斐波那契数列
来源：http://hz.guowangkeji.top/gttmnxsqft.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hysaishi.cn/gtgffxclnh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.pengpengdd.cyou/gtemxvancl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.wangdashe.top/gticwrwyey.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhiwuduotai.top/gtwbwuxuvd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zycfv.cn/gtljiqjugq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yj20258888.top/gtdfjsvajn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.0kj1m.cn/gtiogashxj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yonumen.top/gtvvqqcvnt.html

[N05] 最大公约数
来源：http://hz.ywan-chungtsiang.top/gtkxzmipgd.html

Py:   math.gcd(a, b)
来源：http://hz.ivvv.top/gtgohicltv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.cdnleiting.top/gtsniyuvpk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangdashe.top/gtzzeneskw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yueranfly.top/gtvuhdjofe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenzaomai.com/gtvzarydzd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.gaohongyu789.top/gtxlbhmrfr.html

Ruby: a.gcd(b)
来源：http://hz.ydjk.org.cn/gtsvadjvdt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zycfv.cn/gtgfhqyoxj.html

[N06] 判断回文字符串
来源：http://hz.quarkkingdee.top/gtbbnoouku.html

Py:   s == s[::-1]
来源：http://hz.nwbrower.top/gthufionsk.html

PHP:  $s === strrev($s);
来源：http://hz.316326.xyz/gtlzkhxuux.html

JS:   s === [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gtqymjvybf.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jinyuanbaomall.cn/gtjwbqaizz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.kuanghao11.cn/gtmpjgvupx.html

Go:   // 双指针从两端比较
来源：http://hz.cashguo.top/gtwhhlcbfm.html

Ruby: s == s.reverse
来源：http://hz.sufxvd.cn/gtrravaigp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shangyingyoupin.top/gthyhyskjg.html

[N07] 两数之和（返回下标）
来源：http://hz.zycfv.cn/gtyqejrhnb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.mhx1999.top/gtanhzpblj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ybcxt.top/gtelxkprjc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ydzc1.top/gtizahgiyj.html

TS:   // 手写 Map<string, number>
来源：http://hz.chenjidiqi.icu/gttonjshzq.html

Java: // 手写 HashMap
来源：http://hz.nanxinkj.top/gtcwloyogv.html

Go:   // 手写 map[int]int
来源：http://hz.tanke756.top/gtedjxkdnk.html

Ruby: // 手写 Hash
来源：http://hz.redwolf501.top/gtvlsmjdxu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.daria6918.cn/gtduipykuw.html

[N08] 生成全排列
来源：http://hz.yongpay.top/gthadvmgat.html

Py:   itertools.permutations(arr)
来源：http://hz.wangshuangyany.cn/gtfczvjrfi.html

PHP:  // 手写递归交换
来源：http://hz.chenlongwang.top/gtqpzutqka.html

JS:   // 手写回溯递归
来源：http://hz.sxryk.cn/gtwcjxdbmw.html

TS:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtvtjxlgrh.html

Java: // 手写回溯递归
来源：http://hz.snrcjt.cn/gttsnzbjpg.html

Go:   // 手写回溯递归
来源：http://hz.ydzc1.top/gtfjakcfbz.html

Ruby: arr.permutation.to_a
来源：http://hz.fengsongda.top/gtlqmdzyoc.html

C#:   // 手写回溯递归
来源：http://hz.yj20258.top/gtapdngivz.html

[N09] 栈与队列
来源：http://hz.jianghu66.top/gtkztrvwkz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.gzhubu.top/gtruznxtxx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.daria6918.cn/gtcdsydtpq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.chenzaomai.com/gtvpqixzia.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hnxiangtu.top/gtfyhcjkbx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.mhx1999.top/gtziesnxyl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cucudq.cn/gtoiwsarsz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.9152youxi.cn/gtnftihfpj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.dianchejie.cn/gtetmsycha.html

[N10] 链表节点定义
来源：http://hz.nanxinkj.top/gtpachkiwq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.meibo888.top/gtdvxgutec.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shanyushiyangkeji.top/gtlwpvfikf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jinqigufen.top/gtgqrgxrwd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zdqjudy.top/gtbrgyygii.html

Java: class Node { int v; Node next; }
来源：http://hz.daria6918.cn/gtdwalhiaz.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tanke756.top/gtjjgpeusu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zycfv.cn/gtwzxvalpr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.chenjidiqi.icu/gtvdykrasx.html

[N11] 二叉树中序遍历
来源：http://hz.shuidangran.top/gtxojbcish.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ydzc1.top/gttccxxrtq.html

PHP:  // 手写递归函数
来源：http://hz.smart0.xyz/gtykikicvd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhoulong.xyz/gtyrbwqyeu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenzaomai.com/gtqtvftafy.html

Java: // 手写递归
来源：http://hz.xylfe.cn/gtmdmhsqid.html

Go:   // 手写递归
来源：http://hz.ehwqpu.com/gtictonuht.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ivvv.top/gtswyydfsm.html

C#:   // 手写递归
来源：http://hz.yuanzhike.top/gtfeniiqqo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.0kj1m.cn/gtsvnhjwrc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yuxming.cn/gtsogxvxck.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.nanxuanxn.top/gtcntljskt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yanxiufei.cn/gtlebdwkel.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hnqzz.top/gtaryolbgd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.316326.xyz/gtekqkppem.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shangyingyoupin.top/gtjceblmxe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.guannengcc.top/gtbkiqzwrw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.daxiang520.top/gtukdzsudp.html

================================================================================
来源：http://hz.daria6918.cn/gtvrnbadqu.html

O. 并发与异步
来源：http://hz.tian-w.cn/gtiidyafng.html

================================================================================
来源：http://hz.yvedp.cn/gttibugjvn.html

[O01] 启动一个线程
来源：http://hz.jqgufenzy.top/gtisubkgpo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.chenlongwang.top/gtrlibkqgj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yongpay.top/gtthqwdzth.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.pycfn.com/gtdfjuiafy.html

TS:   // 同 JS
来源：http://hz.zhixingplan.top/gtdvxbjlec.html

Java: new Thread(() -> f()).start()
来源：http://hz.wangdashe.top/gtbrisoivy.html

Go:   go f()
来源：http://hz.zhaomingkeji.xyz/gthvkixcbc.html

Ruby: Thread.new { f }
来源：http://hz.hnqzz.top/gtpkifijlr.html

C#:   Task.Run(() => F());
来源：http://hz.redwolf501.top/gtddxclbta.html

[O02] 使用线程池
来源：http://hz.vqdsnc.cn/gtsqwtsvsv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cashguo.top/gthjscihfo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cdnleiting.top/gtcqptszkd.html

JS:   // worker_threads 线程池
来源：http://hz.chenlongwang.top/gtkqwokxmc.html

TS:   // worker_threads 线程池
来源：http://hz.sweek.top/gtzqqcdpph.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zdqjudy.top/gtbjcnunzg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xuanzx.com/gtyspheqfb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.316326.xyz/gtxlicmwjn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinqigufen.top/gtgwfgxpfz.html

[O03] 加锁保护共享数据
来源：http://hz.kuanghao11.cn/gtxmehbepm.html

Py:   with lock: shared += 1
来源：http://hz.ehwqpu.com/gtzdbtizud.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yongpay.top/gtjtbympxl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yongpay.top/gtkqyfhriu.html

TS:   // 同 JS
来源：http://hz.sxryk.cn/gtzwconvbc.html

Java: synchronized (this) { shared++; }
来源：http://hz.nwbrower.top/gtivhwapxv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.pengpengdd.cyou/gtbymwqgvr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jqgufenzy.top/gtoqtqrwbd.html

C#:   lock (gate) { shared++; }
来源：http://hz.yongpay.top/gtefbwjjeq.html

[O04] 定义异步函数并等待
来源：http://hz.iojbl.cn/gtpsnuawge.html

Py:   async def f():⏎    await g()
来源：http://hz.ydjk.org.cn/gtnltdhuoj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xingfuxueyuan.xyz/gtdlqomlqz.html

JS:   async function f() { await g(); }
来源：http://hz.meibo888.top/gtymvumydk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.wangshuangyany.cn/gtczovyzpp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ybcxt.top/gtjtujlbir.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.pycfn.com/gtrfyatgyk.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.dashuyun.cn/gtqnzyolqr.html

C#:   async Task F() { await G(); }
来源：http://hz.xylfe.cn/gtbjnhianc.html

[O05] 并发执行并等待全部完成
来源：http://hz.shanyushiyangkeji.top/gtdzwyadrl.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinqigufen.top/gtcrjmyyzs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.sweek.top/gtowoyript.html

JS:   await Promise.all(tasks)
来源：http://hz.yangfankeji.com/gtznfyzrgr.html

TS:   await Promise.all(tasks)
来源：http://hz.jinqigfzy.top/gtrjoptkrs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xuetiantiany.cn/gttuihwvkj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.316326.xyz/gtybctmjzb.html

Ruby: threads.map(&:join)
来源：http://hz.fzhhl.top/gtqpbwlccl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.nanxuanxn.top/gtcexggmag.html

[O06] 使用进程池
来源：http://hz.zycfv.cn/gtwvxodzbx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yueranfly.top/gthqrbrazi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.sxryk.cn/gtecmlwovz.html

JS:   // child_process / cluster 模块
来源：http://hz.cheryme.top/gtnfmdngwl.html

TS:   // child_process / cluster 模块
来源：http://hz.hnxiangtu.top/gtnihfwazo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.316326.xyz/gtanjpvjun.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yuxming.cn/gtmsiotuji.html

Ruby: // fork 块
来源：http://hz.yongpay.top/gtbumzxacp.html

C#:   Parallel.For
来源：http://hz.hnqzz.top/gtdnugsmkd.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtgqdekrre.html

P. 常用工具函数
来源：http://hz.svipenyu.cn/gtgflwlqis.html

================================================================================
来源：http://hz.jinqigufen.top/gttwlqpbov.html

[P01] 生成 UUID
来源：http://hz.ydjk.org.cn/gtzjjeggrh.html

Py:   str(uuid.uuid4())
来源：http://hz.ehwqpu.com/gtiyuyucgs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ivvv.top/gtvvpbluqf.html

JS:   crypto.randomUUID()
来源：http://hz.ivvv.top/gtxwmztnaa.html

TS:   crypto.randomUUID()
来源：http://hz.pycfn.com/gtrreugddv.html

Java: UUID.randomUUID().toString()
来源：http://hz.shzxlz.cn/gtsomggonu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sweek.top/gtkrnvpwhk.html

Ruby: SecureRandom.uuid
来源：http://hz.fengsongda.top/gtwtkbaxic.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.gzhubu.top/gtsdectupe.html

[P02] MD5 / SHA256 摘要
来源：http://hz.iojbl.cn/gtcldmjiay.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenjidiqi.icu/gtuaziqkvx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.feifeiyinyue.top/gtonvlsvey.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.andypj.xyz/gthnyegwdv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jyoumei.cn/gtaqntukyo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yuxming.cn/gtttsaxuia.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yuanzhike.top/gtagnsdmck.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yangfankeji.com/gtbeuaymds.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zdqjudy.top/gtpkkninzl.html

[P03] 生成短随机字符串
来源：http://hz.jinqigufen.top/gtiykqcvsy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhoulong.xyz/gttcgadpqb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cashguo.top/gtzlkyyorx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhixingplan.top/gtuwsxjqan.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sysykeji.top/gtejyteoiy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jqgfzy.top/gtgsjbwahh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yvedp.cn/gtdgdtflbo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ybcxt.top/gtarjpvlbz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gaohongyu789.top/gtoljcmehn.html

[P04] 求长度
来源：http://hz.birdmap.top/gtulugiwer.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.pengpengdd.cyou/gtyxwrlfjk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgfzy.top/gtztufddcn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.birdmap.top/gtxsprbqar.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shanyushiyangkeji.top/gtsdkshcyr.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jiagoushi.top/gtgraqubpt.html

Go:   len(arr);  len(m)
来源：http://hz.zhaomingkeji.xyz/gtasfeepkd.html

Ruby: x.length;  x.size
来源：http://hz.xylfe.cn/gtrosloyjm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yangfankeji.com/gtbukhuuel.html

[P05] 判断两个对象内容是否相等
来源：http://hz.wangdashe.top/gtxzuyoega.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.aizwys.cn/gtlltrukzy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ppjwa.cn/gtqbzxcbee.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.gogol.net.cn/gtdiuyapqq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gogol.net.cn/gtpgqloesx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.meibo888.top/gtuqplpgte.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.pycfn.com/gtyiwacbxn.html

Ruby: a == b
来源：http://hz.aibaodan.cn/gtmclfklcs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.c1oappe.top/gtbcsuhwmq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.chenzaomai.com/gtfdovrxop.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.cucudq.cn/gtwcnumpjy.html

PHP:  if (empty($x)) {}
来源：http://hz.yvedp.cn/gteeyjpgyv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.quarkkingdee.top/gtklumhdmj.html

TS:   if (x == null) {}
来源：http://hz.bjfxy.top/gtvyksumud.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.chenjidiqi.icu/gtepeyvijb.html

Go:   if x == nil {}
来源：http://hz.vqdsnc.cn/gthxsxmbap.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.gaohongyu789.top/gtrgcxdvnm.html

C#:   if (x is null) {}
来源：http://hz.aizwys.cn/gtgttljhwz.html

[P07] 防抖与节流
来源：http://hz.cheryme.top/gtxraqcmvk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.aizwys.cn/gtvbnogdxd.html

PHP:  // 手写时间戳比较
来源：http://hz.wangdashe.top/gtdknzutrq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.redwolf501.top/gthrzwdvmr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258888.top/gtnhmfvfko.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jiagoushi.top/gtcoywjbgi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yvedp.cn/gticwsolzs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yvedp.cn/gtisibamrk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ybcxt.top/gtsccylxnl.html

[P08] 处理浮点精度问题
来源：http://hz.guannengcc.top/gtdjixvzcn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shanyushiyangtech.top/gtqrhiialz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinghuilouyu.cn/gtusfridtb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.mhx1999.top/gtounjdive.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yuxming.cn/gtnyksrdsg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.kuanghao11.cn/gtfmcqfxdg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.aibaodan.cn/gtlpjotthg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zycfv.cn/gtzseogxjz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.gzhubu.top/gtsfkcyhao.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtmzpqyryg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.haohaochexian.top/gteonrocou.html

================================================================================
来源：http://hz.cucudq.cn/gthkhjhriu.html

[Q01] 创建表
来源：http://hz.wangshuangyany.cn/gtozqzxpcn.html

CREATE TABLE users (
来源：http://hz.daria6918.cn/gtlkenbkne.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aizwys.cn/gtajkfmkvc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yj20258.top/gtnhhfxgrm.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sysykeji.top/gtrcpspuuk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yueranfly.top/gtqmtlzgcj.html

);
来源：http://hz.jinghuilouyu.cn/gtrpgwmluh.html

[Q02] 创建带外键的表
来源：http://hz.xziqi.cn/gtaqihzeph.html

CREATE TABLE orders (
来源：http://hz.xingfuxueyuan.xyz/gtvxqwjzuw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuanzx.com/gtjaldvqiq.html

user_id INT NOT NULL,
来源：http://hz.nwbrower.top/gtqsgecxst.html

amount DECIMAL(10, 2),
来源：http://hz.guannengcc.top/gtmirpdsed.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.kuanghao11.cn/gtlfgxnjwv.html

);
来源：http://hz.zhongyouzk.top/gtepanwamg.html

[Q03] 增加列
来源：http://hz.jinyuanbaomall.cn/gtffpzovyg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhengqikj.top/gtgggdorvy.html

[Q04] 修改列类型
来源：http://hz.fzhhl.top/gtstiqtnws.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.meibo888.top/gtnmkoasjk.html

[Q05] 重命名列
来源：http://hz.fengsongda.top/gtzgubfeun.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gzhubu.top/gtowmdoxcs.html

[Q06] 删除列
来源：http://hz.jqgufenzy.top/gtvwhanonf.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sweek.top/gtltlkzxae.html

[Q07] 删除表
来源：http://hz.zhixingplan.top/gtozpuctmy.html

DROP TABLE IF EXISTS orders;
来源：http://hz.meibo888.top/gtzzgepzfy.html

[Q08] 创建普通索引
来源：http://hz.zhijiandao.cn/gtwqzcxien.html


<!-- 参考信息 -->