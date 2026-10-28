代发 wailian999

Ruby: exit 1
来源：http://hz.xuanzx.com/gtimahpffq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jyoumei.cn/gtfwempvoc.html

[M06] 向标准错误输出
来源：http://hz.snrcjt.cn/gtfwogurtw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nwbrower.top/gtvtwlrnbb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jlsjyb.cn/gtwbgbxesp.html

JS:   console.error("err")
来源：http://hz.guannengcc.top/gtejvwleuv.html

TS:   console.error("err")
来源：http://hz.tanke756.top/gtewnfxusc.html

Java: System.err.println("err")
来源：http://hz.tian-w.cn/gthsujxhdt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.316326.xyz/gtwigvjznj.html

Ruby: warn "err"
来源：http://hz.jinyuanbaomall.cn/gtoevdsmnx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.nanxuanxn.top/gtxcrhfvgu.html

[M07] 判断是否为主入口
来源：http://hz.feifeiyinyue.top/gtqafsvjya.html

Py:   if __name__ == "__main__":
来源：http://hz.ybcxt.top/gtrvaxcvdi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.0kj1m.cn/gtpfhbsshx.html

JS:   require.main === module
来源：http://hz.xziqi.cn/gtmjnnauay.html

TS:   require.main === module
来源：http://hz.ehwqpu.com/gtguoqwrdd.html

Java: public static void main(String[] args)
来源：http://hz.ydzc1.top/gtuicljbkg.html

Go:   func main()
来源：http://hz.bjfxy.top/gtzcvizlpt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.316326.xyz/gtzgnxihhw.html

C#:   static void Main(string[] args)
来源：http://hz.yuxming.cn/gtxkqbyxwq.html

[M08] 获取系统与运行时信息
来源：http://hz.yongpay.top/gtjwkxhpyr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.guannengcc.top/gtivjqvddt.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gotoacloud.top/gtoqrukgog.html

JS:   process.platform;  process.version
来源：http://hz.gotoacloud.top/gtyxwlfoek.html

TS:   process.platform;  process.version
来源：http://hz.dianchejie.cn/gteqqrtahg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.nanxinkj.top/gtqgoucaar.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ehwqpu.com/gtsopmczdi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zdqjudy.top/gtqaryukfb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.gotoacloud.top/gtfvyuicgg.html

================================================================================
来源：http://hz.yj20258888.top/gtzzjhllxr.html

N. 数据结构与算法
来源：http://hz.yj20258.top/gtbvpqvmvy.html

================================================================================
来源：http://hz.shuidangran.top/gteqhkeqof.html

[N01] 二分查找（有序数组）
来源：http://hz.hnqzz.top/gtbsqwsbbd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sysykeji.top/gttzuozwst.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhiwuduotai.top/gtjexzoomx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ywan-chungtsiang.top/gteoohqorm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.9152youxi.cn/gtoyoasuck.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ydjk.org.cn/gtykuwevup.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinqigufen.top/gtiocajjok.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sufxvd.cn/gtdzvraeaz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.daria6918.cn/gthaejqacq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jinghuilouyu.cn/gtnhlgzpsf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.feifeiyinyue.top/gtqnngipha.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.chenjidiqi.icu/gtwrcgvabn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.haohaochexian.top/gtubjzsoat.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.bjfxy.top/gtwduytvni.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhongyouzk.top/gtjwegawpb.html

Go:   slices.Sort(arr)
来源：http://hz.zhiwuduotai.top/gtjucdxrur.html

Ruby: arr.sort
来源：http://hz.redwolf501.top/gtnigfykfj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.kuanghao11.cn/gtypjhgphu.html

[N03] 快速排序（分治示例）
来源：http://hz.tian-w.cn/gtswrqrawn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.fengsongda.top/gthgjzesso.html

PHP:  // 递归实现，或用 usort
来源：http://hz.kuanghao11.cn/gtsuiclkrx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgufenzy.top/gtuoiidghx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhaomingkeji.xyz/gtbwnccqji.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.sxryk.cn/gtuhohrulw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.gotoacloud.top/gtyoolgbpo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.52xcode.cn/gtlwchuqek.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yonumen.top/gtmxvhjifi.html

[N04] 斐波那契数列
来源：http://hz.0kj1m.cn/gtqplgughv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.dashuyun.cn/gtedwjngcu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hnxiangtu.top/gtxmamokkp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hammf.cn/gtvxttmocn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuanzhike.top/gtjcckocgy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gaohongyu789.top/gtfvbcqgbe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gotoacloud.top/gtpcpenoen.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj202588.top/gtblllzenl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.kuanghao11.cn/gtcakrzsqs.html

[N05] 最大公约数
来源：http://hz.shanyushiyangkeji.top/gtzxwqeezj.html

Py:   math.gcd(a, b)
来源：http://hz.316326.xyz/gttzeiuxng.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hammf.cn/gtqtsnqvmk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgfzy.top/gtjrttqlry.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.snrcjt.cn/gtfjoicyhi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.guannengcc.top/gtxpnwvwew.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sysykeji.top/gtvedttbat.html

Ruby: a.gcd(b)
来源：http://hz.svipenyu.cn/gtivedhtyt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.quarkkingdee.top/gtlihvcctg.html

[N06] 判断回文字符串
来源：http://hz.aibaodan.cn/gtxmecaghf.html

Py:   s == s[::-1]
来源：http://hz.zhijiandao.cn/gtlbzlryux.html

PHP:  $s === strrev($s);
来源：http://hz.xinyue.icu/gthltsjvlg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangtech.top/gtjfeuwedg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.fengsongda.top/gtbqivqgqp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ydzc1.top/gtvtiyvjob.html

Go:   // 双指针从两端比较
来源：http://hz.jianghu66.top/gtofdkfqjf.html

Ruby: s == s.reverse
来源：http://hz.cucudq.cn/gtfhpyijih.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.nanxinkj.top/gtwvjgohyo.html

[N07] 两数之和（返回下标）
来源：http://hz.pengpengdd.cyou/gtenrqvkvp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.316326.xyz/gtmoupisvf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.bjfxy.top/gtpyrfxebx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ywan-chungtsiang.top/gtatnphvlx.html

TS:   // 手写 Map<string, number>
来源：http://hz.dianchejie.cn/gtzlfjkyfk.html

Java: // 手写 HashMap
来源：http://hz.zhongyouzk.top/gtebqppchc.html

Go:   // 手写 map[int]int
来源：http://hz.jinqigufen.top/gtltyszrtu.html

Ruby: // 手写 Hash
来源：http://hz.zdqjudy.top/gtdifwnmmz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jianghu66.top/gtehfwcaeg.html

[N08] 生成全排列
来源：http://hz.ywan-chungtsiang.top/gtcfrpxjux.html

Py:   itertools.permutations(arr)
来源：http://hz.yvedp.cn/gtyjbarxpe.html

PHP:  // 手写递归交换
来源：http://hz.feifeiyinyue.top/gtenmzzdns.html

JS:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtdpjkalvh.html

TS:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtqjxhocaz.html

Java: // 手写回溯递归
来源：http://hz.hysaishi.cn/gtmutszhvm.html

Go:   // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtlhvwfsei.html

Ruby: arr.permutation.to_a
来源：http://hz.gaohongyu789.top/gtpyzcluxd.html

C#:   // 手写回溯递归
来源：http://hz.cheryme.top/gttppjdgbq.html

[N09] 栈与队列
来源：http://hz.pycfn.com/gttqbbjqpn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.wangdashe.top/gtvppitxpp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ydzc1.top/gthxkcgfht.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yvedp.cn/gthcjsdahs.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cdnleiting.top/gtsasmsbfc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hammf.cn/gtufgcqgrw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinghuilouyu.cn/gtqboriwqs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yangfankeji.com/gtcdiqpytb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.kuanghao11.cn/gtoiiblzmy.html

[N10] 链表节点定义
来源：http://hz.xziqi.cn/gtaghbnbss.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.wangdashe.top/gtqnlaistd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.wangshuangyany.cn/gtcnkqjpou.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hywenlv.cn/gtpvplaqte.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.fzhhl.top/gthdygcybv.html

Java: class Node { int v; Node next; }
来源：http://hz.hongshengwenyu.top/gtwyturnbp.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yj20258.top/gtzptwmqin.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.tianlin.xyz/gtuzukexzh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhongyouzk.top/gtsoixzysr.html

[N11] 二叉树中序遍历
来源：http://hz.aibaodan.cn/gtknpkmese.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.andypj.xyz/gtxnxkxpsx.html

PHP:  // 手写递归函数
来源：http://hz.xingfuxueyuan.xyz/gtigfyszhb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hywenlv.cn/gtggidsbhs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuanzhike.top/gtfrjdrlhb.html

Java: // 手写递归
来源：http://hz.hysaishi.cn/gtnwzjwugm.html

Go:   // 手写递归
来源：http://hz.redwolf501.top/gtpvfqapdd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hywenlv.cn/gtxhbqyzpr.html

C#:   // 手写递归
来源：http://hz.kuanghao11.cn/gtqnkgkugc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shanyushiyangtech.top/gtajhqzkmk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xinyue.icu/gtkvmjzzmn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.smart0.xyz/gtaoriyfwi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nwbrower.top/gtaocgljlx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xinyue.icu/gtqxjhbidt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hnxiangtu.top/gthmyunsnt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jinqigufen.top/gthiabxfum.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.mhx1999.top/gtkvgjbvyr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.smart0.xyz/gtwwrndmrn.html

================================================================================
来源：http://hz.hywenlv.cn/gtzlsbomuz.html

O. 并发与异步
来源：http://hz.sysykeji.top/gtbocjiufo.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtzgykrarn.html

[O01] 启动一个线程
来源：http://hz.bjfxy.top/gtntxolyki.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.fengsongda.top/gtjcygraat.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xylfe.cn/gtbdvziitz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.mhx1999.top/gtvlwmrkdt.html

TS:   // 同 JS
来源：http://hz.zhijiandao.cn/gtgypqqsmg.html

Java: new Thread(() -> f()).start()
来源：http://hz.yvedp.cn/gtnubkpmit.html

Go:   go f()
来源：http://hz.fengsongda.top/gtvqgdrkvx.html

Ruby: Thread.new { f }
来源：http://hz.yj202588.top/gtpmfswwjf.html

C#:   Task.Run(() => F());
来源：http://hz.aizwys.cn/gtetuvgtfv.html

[O02] 使用线程池
来源：http://hz.zhongyouzk.top/gttctvnscu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zycfv.cn/gtkmgjtysk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cashguo.top/gtxgxmvqdw.html

JS:   // worker_threads 线程池
来源：http://hz.quarkkingdee.top/gtyhcxxudh.html

TS:   // worker_threads 线程池
来源：http://hz.feifeiyinyue.top/gtatfdygpj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shanyushiyangtech.top/gttmfbtqhh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhongyouzk.top/gtnyilzprk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gogol.net.cn/gtzitlmzts.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.meibo888.top/gtrrgjtuwx.html

[O03] 加锁保护共享数据
来源：http://hz.jinqigfzy.top/gtvbmpwhmh.html

Py:   with lock: shared += 1
来源：http://hz.sufxvd.cn/gthmknrrvh.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.snrcjt.cn/gtpjwdeqha.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ppjwa.cn/gtwsjkeuqs.html

TS:   // 同 JS
来源：http://hz.aizwys.cn/gtndmgaawt.html

Java: synchronized (this) { shared++; }
来源：http://hz.chenjidiqi.icu/gtdgvkiimh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.quarkkingdee.top/gtelbuxnwv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.wangshuangyany.cn/gtagacjdnd.html

C#:   lock (gate) { shared++; }
来源：http://hz.tanke756.top/gtjapgojzt.html

[O04] 定义异步函数并等待
来源：http://hz.shuidangran.top/gtptftkocm.html

Py:   async def f():⏎    await g()
来源：http://hz.52xcode.cn/gtdplrzukz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.tanke756.top/gtpumxuscq.html

JS:   async function f() { await g(); }
来源：http://hz.guowangkeji.top/gtmvopdqbl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ivvv.top/gtnjvkkcpt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xylfe.cn/gtpaxxyurt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cdnleiting.top/gtlvzolkjw.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xziqi.cn/gtkbnjccwc.html

C#:   async Task F() { await G(); }
来源：http://hz.ydzc1.top/gtdyslyvto.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj202588.top/gtbuhhcbzk.html

Py:   asyncio.gather(*tasks)
来源：http://hz.tanke756.top/gtylvxglqz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.pycfn.com/gthsolommz.html

JS:   await Promise.all(tasks)
来源：http://hz.haohaochexian.top/gtlmzuabfe.html

TS:   await Promise.all(tasks)
来源：http://hz.nanxinkj.top/gtechtblvi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.aizwys.cn/gtzymvyksu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.meibo888.top/gthofcyizi.html

Ruby: threads.map(&:join)
来源：http://hz.zhongyouzk.top/gtwoftxeiw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.gzhubu.top/gtinyefhvt.html

[O06] 使用进程池
来源：http://hz.hnxiangtu.top/gtvbbaoego.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shanyushiyangkeji.top/gtlbgzajpb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.snrcjt.cn/gtsyfjzcjx.html

JS:   // child_process / cluster 模块
来源：http://hz.ywan-chungtsiang.top/gtavmnhstc.html

TS:   // child_process / cluster 模块
来源：http://hz.xuetiantiany.cn/gtdlpjwkgx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ivvv.top/gtzzzmzqtt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.wangshuangyany.cn/gtuimtpamh.html

Ruby: // fork 块
来源：http://hz.nanxuanxn.top/gtlpygxfer.html

C#:   Parallel.For
来源：http://hz.hongshengwenyu.top/gtiohbbzkz.html

================================================================================
来源：http://hz.aibaodan.cn/gtozbsxudc.html

P. 常用工具函数
来源：http://hz.shangyingyoupin.top/gtdjvsaiyp.html

================================================================================
来源：http://hz.jqgfzy.top/gtcpgzbuap.html

[P01] 生成 UUID
来源：http://hz.ivvv.top/gttcuewurj.html

Py:   str(uuid.uuid4())
来源：http://hz.zdqjudy.top/gtzqotnfva.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yj202588.top/gtaykuvbmt.html

JS:   crypto.randomUUID()
来源：http://hz.xuanzx.com/gtuphdlfio.html

TS:   crypto.randomUUID()
来源：http://hz.snrcjt.cn/gtthkwbyhn.html

Java: UUID.randomUUID().toString()
来源：http://hz.wangshuangyany.cn/gtimccsega.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cqqwz.cn/gtxopbjfyw.html

Ruby: SecureRandom.uuid
来源：http://hz.ydzc1.top/gtuwwnirjw.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yj202588.top/gtbndqiddb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jyoumei.cn/gtrapbvdfh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gzhubu.top/gtqmytdycj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gogol.net.cn/gttbopzpop.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ydzc1.top/gtrfsdvcgw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xziqi.cn/gtvlhszubf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hnqzz.top/gtchovttfm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ehwqpu.com/gtetzpceyq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhongyouzk.top/gteqxqbrys.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.smart0.xyz/gtdxkjnslf.html

[P03] 生成短随机字符串
来源：http://hz.ydjk.org.cn/gtehiyeise.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hongshengwenyu.top/gtwncexmgw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.redwolf501.top/gtgiqzlzqr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuanzhike.top/gtvhgjkike.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.iojbl.cn/gtcnhjfeww.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhengqikj.top/gtxvdazwne.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yangfankeji.com/gtylvdodph.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.chenzaomai.com/gtcnqsygvq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.wangdashe.top/gtbegibgin.html

[P04] 求长度
来源：http://hz.smart0.xyz/gtcrgxupgf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ivvv.top/gtekyooump.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jyoumei.cn/gtwpgmsnkf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pycfn.com/gtznsyxacr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xuanzx.com/gttysygztb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.tian-w.cn/gtjmkmcmpd.html

Go:   len(arr);  len(m)
来源：http://hz.cdnleiting.top/gtszxnnqyg.html

Ruby: x.length;  x.size
来源：http://hz.aibaodan.cn/gtkprntrgi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.vqdsnc.cn/gtlfkdnvua.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhoulong.xyz/gtkbapgddo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yuxming.cn/gtdobxzvkz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hnqzz.top/gtlpyjbssf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yj20258888.top/gtburicjzv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgufenzy.top/gtqxuezyxh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.tian-w.cn/gtmaqzksjl.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.havefunace.top/gtjfkobiub.html

Ruby: a == b
来源：http://hz.yongpay.top/gtwrgpzxvj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xziqi.cn/gtiahzslqd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zycfv.cn/gtpqtuujrp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.aibaodan.cn/gtpmuexboq.html

PHP:  if (empty($x)) {}
来源：http://hz.sxryk.cn/gtilirsbal.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.gzhubu.top/gtrraooyuo.html

TS:   if (x == null) {}
来源：http://hz.sufxvd.cn/gtqmszfalk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shangyingyoupin.top/gtonpomgig.html

Go:   if x == nil {}
来源：http://hz.zhengqikj.top/gtxgqthdgz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yueranfly.top/gtmsnmffoy.html

C#:   if (x is null) {}
来源：http://hz.pycfn.com/gtfdlupogz.html

[P07] 防抖与节流
来源：http://hz.jqgfzy.top/gtaoqlzbyg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xingfuxueyuan.xyz/gtnbgtjnkn.html

PHP:  // 手写时间戳比较
来源：http://hz.hnxiangtu.top/gtjtvkmivj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.meibo888.top/gtnnnueiri.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daria6918.cn/gtszpcvhgz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.chenjidiqi.icu/gtehiglvht.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yj20258.top/gtdirascng.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jiagoushi.top/gtqzhyjhzj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jyoumei.cn/gtgfrodugq.html

[P08] 处理浮点精度问题
来源：http://hz.hfpthk.cn/gtnhlpspks.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yonumen.top/gtbajmkvse.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yueranfly.top/gtiyvfpbfe.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.wangdashe.top/gtlejjflht.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xingfuxueyuan.xyz/gtwnxeehif.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.andypj.xyz/gtdjzrswql.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hysaishi.cn/gtaonpnwaq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ehwqpu.com/gtkmrlpxge.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.iojbl.cn/gttwerseia.html

================================================================================
来源：http://hz.havefunace.top/gtwwshlsdw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hysaishi.cn/gtomhivmjb.html

================================================================================
来源：http://hz.shuidangran.top/gtsbkugpws.html

[Q01] 创建表
来源：http://hz.jlsjyb.cn/gtgzmeaybv.html

CREATE TABLE users (
来源：http://hz.zhiwuduotai.top/gtcieppkpw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cashguo.top/gtinvpcdlr.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shuidangran.top/gtnbwsmeds.html

email VARCHAR(100) UNIQUE,
来源：http://hz.c1oappe.top/gtxklitahx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hnqzz.top/gtwtwxogfv.html

);
来源：http://hz.9152youxi.cn/gtktyafuxz.html

[Q02] 创建带外键的表
来源：http://hz.yonumen.top/gtfoxbbwbq.html

CREATE TABLE orders (
来源：http://hz.shuidangran.top/gtsraohrej.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ehwqpu.com/gtezitzhtt.html

user_id INT NOT NULL,
来源：http://hz.ywan-chungtsiang.top/gtlslbjlbz.html

amount DECIMAL(10, 2),
来源：http://hz.zhoulong.xyz/gtpcebirgy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhongyouzk.top/gtpzkfpmss.html

);
来源：http://hz.yj202588.top/gtsvypvrgh.html

[Q03] 增加列
来源：http://hz.tanke756.top/gtqcezhdfc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.havefunace.top/gthjnxdkwx.html

[Q04] 修改列类型
来源：http://hz.ppjwa.cn/gtryawqcir.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yangfankeji.com/gtjvtrjpzt.html

[Q05] 重命名列
来源：http://hz.sweek.top/gtetragcey.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yuanzhike.top/gtlwvsgxfk.html

[Q06] 删除列
来源：http://hz.cdnleiting.top/gtqntuekbp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ywan-chungtsiang.top/gtrpztwtsn.html

[Q07] 删除表
来源：http://hz.guowangkeji.top/gtppiiaqkz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yongpay.top/gtjyhujbua.html

[Q08] 创建普通索引
来源：http://hz.dianchejie.cn/gtxjaibbeh.html


<!-- 参考信息 -->