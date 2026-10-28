代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenlongwang.top/gtpntwanbw.html

JS:   console.error("err")
来源：http://hz.snrcjt.cn/gtputobypx.html

TS:   console.error("err")
来源：http://hz.yj20258888.top/gtajnsxtrj.html

Java: System.err.println("err")
来源：http://hz.cucudq.cn/gtnbvvshqz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhoulong.xyz/gtxqygvcvh.html

Ruby: warn "err"
来源：http://hz.quarkkingdee.top/gtxcbsdcds.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yj20258.top/gtqedaqfoz.html

[M07] 判断是否为主入口
来源：http://hz.xylfe.cn/gtkecpzumr.html

Py:   if __name__ == "__main__":
来源：http://hz.yj202588.top/gttmpliiyp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yuanzhike.top/gtjidesfgu.html

JS:   require.main === module
来源：http://hz.redwolf501.top/gtvoqspfvr.html

TS:   require.main === module
来源：http://hz.xylfe.cn/gtwhinrrbw.html

Java: public static void main(String[] args)
来源：http://hz.jinghuilouyu.cn/gtzmyylypn.html

Go:   func main()
来源：http://hz.jinyuanbaomall.cn/gtgxkuzedi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.redwolf501.top/gtpfryvtio.html

C#:   static void Main(string[] args)
来源：http://hz.ivvv.top/gtwlllpjht.html

[M08] 获取系统与运行时信息
来源：http://hz.tianlin.xyz/gtzxnivwaz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cqqwz.cn/gtqlptfruu.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xziqi.cn/gtunfwyrwv.html

JS:   process.platform;  process.version
来源：http://hz.ywan-chungtsiang.top/gtteckpqdg.html

TS:   process.platform;  process.version
来源：http://hz.jinqigfzy.top/gtnmbvewnu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yonumen.top/gtfisycwme.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yvedp.cn/gtqcnwnjbr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ppjwa.cn/gtjkisfxlu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hfpthk.cn/gtpkbitszo.html

================================================================================
来源：http://hz.hnqzz.top/gtgdjlsesf.html

N. 数据结构与算法
来源：http://hz.kuanghao11.cn/gthwemxeyj.html

================================================================================
来源：http://hz.jyoumei.cn/gtnjvmshkq.html

[N01] 二分查找（有序数组）
来源：http://hz.yuanzhike.top/gtauhjoeaj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinghuilouyu.cn/gtnfgynpgf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ybcxt.top/gtfbinxedk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cheryme.top/gtcitdcqxf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.0kj1m.cn/gtlbtvkwkz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.svipenyu.cn/gtoujpyrqu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ywan-chungtsiang.top/gttocztrxo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.quarkkingdee.top/gtibxbqzcy.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtjynekjhr.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhixingplan.top/gtjgkmuwgj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hywenlv.cn/gttiqkmiva.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yueranfly.top/gtwbkwebnt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jqgfzy.top/gtfkhmqhrt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.pycfn.com/gtmnbcycio.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jlsjyb.cn/gtvxfsydct.html

Go:   slices.Sort(arr)
来源：http://hz.svipenyu.cn/gtysglymgb.html

Ruby: arr.sort
来源：http://hz.chenlongwang.top/gtocgkhenf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.nanxuanxn.top/gtdsliulkv.html

[N03] 快速排序（分治示例）
来源：http://hz.hnxiangtu.top/gtesdtxolz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhoulong.xyz/gtyyzxuing.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinghuilouyu.cn/gthhjsgfrk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigfzy.top/gtgyxyosxf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigufen.top/gtklephdwo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.pycfn.com/gtewpmvylh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yvedp.cn/gtivfkguqa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.snrcjt.cn/gtdpwmnexm.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ydjk.org.cn/gtbgfcgada.html

[N04] 斐波那契数列
来源：http://hz.guannengcc.top/gtdzjtvtqr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.fzhhl.top/gtdoxwbuxh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.chenjidiqi.icu/gtuefihvqr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hammf.cn/gtifzxoyym.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.guannengcc.top/gtbnxqssvl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sysykeji.top/gtlxqqisnz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhoulong.xyz/gtzyzkepcw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258.top/gtanogkjzt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj20258888.top/gtqlrftmqr.html

[N05] 最大公约数
来源：http://hz.dianchejie.cn/gtqzpdvnhe.html

Py:   math.gcd(a, b)
来源：http://hz.jqgfzy.top/gtzjyqbxuh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.andypj.xyz/gtifnpqqvg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangtech.top/gtxxgrbbfu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.kuanghao11.cn/gttrskkxju.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gaohongyu789.top/gtzjvqwhyt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yj20258888.top/gtxnudanep.html

Ruby: a.gcd(b)
来源：http://hz.jqgfzy.top/gtkvqkvwbc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinqigfzy.top/gtsxhogvfy.html

[N06] 判断回文字符串
来源：http://hz.shanyushiyangkeji.top/gtlzsszktl.html

Py:   s == s[::-1]
来源：http://hz.xuanzx.com/gtzwnyczxh.html

PHP:  $s === strrev($s);
来源：http://hz.jyoumei.cn/gttcwwpihs.html

JS:   s === [...s].reverse().join("")
来源：http://hz.0kj1m.cn/gtbqyjdubk.html

TS:   s === [...s].reverse().join("")
来源：http://hz.chenjidiqi.icu/gtgnvjndar.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.smart0.xyz/gtrizkphgc.html

Go:   // 双指针从两端比较
来源：http://hz.hfpthk.cn/gtiberqjda.html

Ruby: s == s.reverse
来源：http://hz.jinghuilouyu.cn/gtpobheeve.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tian-w.cn/gtatffsbsj.html

[N07] 两数之和（返回下标）
来源：http://hz.svipenyu.cn/gtquyrulhf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.smart0.xyz/gtezwswqay.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sysykeji.top/gtwkusnvbl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.snrcjt.cn/gtqaketcvu.html

TS:   // 手写 Map<string, number>
来源：http://hz.shzxlz.cn/gtwhypdewo.html

Java: // 手写 HashMap
来源：http://hz.pycfn.com/gtsiysojnq.html

Go:   // 手写 map[int]int
来源：http://hz.yj202588.top/gtkllmywnx.html

Ruby: // 手写 Hash
来源：http://hz.cashguo.top/gtnrdrsuyj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hfpthk.cn/gtmajxeiey.html

[N08] 生成全排列
来源：http://hz.wangdashe.top/gteiaodjsd.html

Py:   itertools.permutations(arr)
来源：http://hz.shuidangran.top/gtscsdahzy.html

PHP:  // 手写递归交换
来源：http://hz.yonumen.top/gtrmbrqyuy.html

JS:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtveuqaqdq.html

TS:   // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtgntdepux.html

Java: // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtylmiqdap.html

Go:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtciwxqsgx.html

Ruby: arr.permutation.to_a
来源：http://hz.sxryk.cn/gtmeiqahsq.html

C#:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtcwvyaznm.html

[N09] 栈与队列
来源：http://hz.hammf.cn/gttbmcqzqo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.tianlin.xyz/gtftfaoqde.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.haohaochexian.top/gtdiinelzl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhengqikj.top/gtgavwyfvq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.fzhhl.top/gturhymlkn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinyuanbaomall.cn/gtsvhcsqbz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.daria6918.cn/gtgojdnyvk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yuxming.cn/gtkqvptrbp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.meibo888.top/gtbnitygiy.html

[N10] 链表节点定义
来源：http://hz.hnqzz.top/gtxvzcqlbk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jyoumei.cn/gtvpyvydad.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jqgufenzy.top/gtvfkarpaf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ydzc1.top/gtgyjiwbxh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.mhx1999.top/gtxtdfpzsp.html

Java: class Node { int v; Node next; }
来源：http://hz.yj20258888.top/gtjjucdkdk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.daxiang520.top/gtlvszljbq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hnxiangtu.top/gtvxszmfww.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yongpay.top/gteejrhzdd.html

[N11] 二叉树中序遍历
来源：http://hz.gaohongyu789.top/gtnvwdsfrq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhoulong.xyz/gtenfivxyn.html

PHP:  // 手写递归函数
来源：http://hz.jyoumei.cn/gthxucexjs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sufxvd.cn/gtlymixihc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.andypj.xyz/gteqervaql.html

Java: // 手写递归
来源：http://hz.dashuyun.cn/gtmdpgwkon.html

Go:   // 手写递归
来源：http://hz.tanke756.top/gtyuxcvfuz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hywenlv.cn/gtdilfjxep.html

C#:   // 手写递归
来源：http://hz.redwolf501.top/gtpjhqbcnl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.pengpengdd.cyou/gtnqpfllfz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.nanxinkj.top/gtjmsdqzfw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhiwuduotai.top/gtdpxvajih.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tanke756.top/gtqhdheyxc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yuanzhike.top/gthvhvyyqi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gtogznmaex.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.tian-w.cn/gtacrswdlr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.tanke756.top/gtmgulpjxq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cashguo.top/gtaabeuwxx.html

================================================================================
来源：http://hz.zhixingplan.top/gtujlmonmu.html

O. 并发与异步
来源：http://hz.zhaomingkeji.xyz/gtvpuqpshm.html

================================================================================
来源：http://hz.birdmap.top/gtnljnpmij.html

[O01] 启动一个线程
来源：http://hz.hysaishi.cn/gtfsyxnhee.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yonumen.top/gtgoncbcrp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ydzc1.top/gtqmkrwdiq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xziqi.cn/gtbztpjpet.html

TS:   // 同 JS
来源：http://hz.yongpay.top/gtyhgzczbh.html

Java: new Thread(() -> f()).start()
来源：http://hz.hywenlv.cn/gttyqeboca.html

Go:   go f()
来源：http://hz.daria6918.cn/gtyeyizynl.html

Ruby: Thread.new { f }
来源：http://hz.birdmap.top/gtfdtfptwy.html

C#:   Task.Run(() => F());
来源：http://hz.yj20258888.top/gtwrecoqjn.html

[O02] 使用线程池
来源：http://hz.nanxinkj.top/gthmnseypw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.52xcode.cn/gtxqejxeag.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jqgufenzy.top/gtdlfgnzpa.html

JS:   // worker_threads 线程池
来源：http://hz.hysaishi.cn/gtjsdbfifm.html

TS:   // worker_threads 线程池
来源：http://hz.cheryme.top/gtulfprxub.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.316326.xyz/gtqfcaqqyk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jqgufenzy.top/gttesxefrf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shanyushiyangkeji.top/gtqxpshgfb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.fzhhl.top/gtdfvutfez.html

[O03] 加锁保护共享数据
来源：http://hz.mhx1999.top/gtclehwqpo.html

Py:   with lock: shared += 1
来源：http://hz.xuanzx.com/gtcqrixjus.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.9152youxi.cn/gtwyfoxjzs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.daxiang520.top/gtbwzcvmmq.html

TS:   // 同 JS
来源：http://hz.jinghuilouyu.cn/gtvbndbgbq.html

Java: synchronized (this) { shared++; }
来源：http://hz.dianchejie.cn/gtbqauleba.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ppjwa.cn/gtxviaioad.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.nwbrower.top/gtzeoqmall.html

C#:   lock (gate) { shared++; }
来源：http://hz.pengpengdd.cyou/gtqprpgjeb.html

[O04] 定义异步函数并等待
来源：http://hz.c1oappe.top/gtkuiywtzv.html

Py:   async def f():⏎    await g()
来源：http://hz.andypj.xyz/gtgligandl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xuetiantiany.cn/gtontmkrqe.html

JS:   async function f() { await g(); }
来源：http://hz.shanyushiyangtech.top/gtdqfuzrmp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.nanxuanxn.top/gtuxadztkt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.guowangkeji.top/gtcfcyfvtn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zycfv.cn/gttinunbkk.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.daxiang520.top/gtxkpixfjh.html

C#:   async Task F() { await G(); }
来源：http://hz.sweek.top/gtaqrhwjol.html

[O05] 并发执行并等待全部完成
来源：http://hz.shanyushiyangkeji.top/gtxncfpvgd.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hongshengwenyu.top/gtddujynfo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jinghuilouyu.cn/gtqbvuanga.html

JS:   await Promise.all(tasks)
来源：http://hz.jqgfzy.top/gtnqojtvtb.html

TS:   await Promise.all(tasks)
来源：http://hz.jinqigufen.top/gtbayhinet.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.nanxuanxn.top/gtrtspqvrz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cdnleiting.top/gtvvxhcvlg.html

Ruby: threads.map(&:join)
来源：http://hz.havefunace.top/gtafrablac.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.52xcode.cn/gtxtccqsor.html

[O06] 使用进程池
来源：http://hz.yj202588.top/gtkkmxrwkl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shanyushiyangtech.top/gtyrncqsyi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.svipenyu.cn/gtujtongau.html

JS:   // child_process / cluster 模块
来源：http://hz.shanyushiyangtech.top/gtvcburoey.html

TS:   // child_process / cluster 模块
来源：http://hz.jiagoushi.top/gtlxtawqkk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.wangdashe.top/gtinckfzwe.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jqgufenzy.top/gtvnkmhidl.html

Ruby: // fork 块
来源：http://hz.ivvv.top/gtremjluga.html

C#:   Parallel.For
来源：http://hz.shanyushiyangtech.top/gtaeleqdqf.html

================================================================================
来源：http://hz.sufxvd.cn/gtsyrbafhu.html

P. 常用工具函数
来源：http://hz.52xcode.cn/gtqynaawpx.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtxpkoneex.html

[P01] 生成 UUID
来源：http://hz.aizwys.cn/gtunnyuybz.html

Py:   str(uuid.uuid4())
来源：http://hz.iojbl.cn/gtreqqpdip.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.aizwys.cn/gtuvevvwgr.html

JS:   crypto.randomUUID()
来源：http://hz.sysykeji.top/gthrvtoejk.html

TS:   crypto.randomUUID()
来源：http://hz.nanxuanxn.top/gtxdxdqfho.html

Java: UUID.randomUUID().toString()
来源：http://hz.sysykeji.top/gtbsjfwyhl.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hnxiangtu.top/gtzfgcsdro.html

Ruby: SecureRandom.uuid
来源：http://hz.zhiwuduotai.top/gtycyxiokp.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sweek.top/gtsuurxkxr.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yj20258888.top/gtvsnqbrhb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.meibo888.top/gtmsebcmxk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.cucudq.cn/gtmbmfgeed.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ppjwa.cn/gtzhyfbmzw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gotoacloud.top/gtrcngzzhd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.daria6918.cn/gtvxgiozsz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.sxryk.cn/gttbgqbffy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xingfuxueyuan.xyz/gtwzmonvmn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jinghuilouyu.cn/gtqbikvdur.html

[P03] 生成短随机字符串
来源：http://hz.jlsjyb.cn/gtfhdmvubw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jyoumei.cn/gtykptpypr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ywan-chungtsiang.top/gttudgqfha.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dashuyun.cn/gtmdwujwwk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuetiantiany.cn/gtzikyxgjo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cucudq.cn/gtkedqorvg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cheryme.top/gtaocwdzvx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.chenlongwang.top/gtktrbmrbv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yonumen.top/gtrnvppxqj.html

[P04] 求长度
来源：http://hz.yj202588.top/gtagckxaor.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ywan-chungtsiang.top/gtgzyuehxy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtdgjmnutk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.snrcjt.cn/gtutuenqhg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangshuangyany.cn/gtkdltexzv.html

Java: list.size();  map.size();  s.length()
来源：http://hz.smart0.xyz/gtfpwwfldm.html

Go:   len(arr);  len(m)
来源：http://hz.jyoumei.cn/gtrkrooznb.html

Ruby: x.length;  x.size
来源：http://hz.quarkkingdee.top/gtvvggihtp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.fzhhl.top/gtvtiszbfl.html

[P05] 判断两个对象内容是否相等
来源：http://hz.feifeiyinyue.top/gtvqomcjwb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yuxming.cn/gtgskjlbrf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.andypj.xyz/gtlawvfwju.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.daxiang520.top/gtsevkznxw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shuidangran.top/gtmtvpguiy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sxryk.cn/gtagczhpjl.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hongshengwenyu.top/gtrylnlczo.html

Ruby: a == b
来源：http://hz.shzxlz.cn/gtkrrchjkl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yanxiufei.cn/gtwisanomn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jyoumei.cn/gteidihlgx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jinghuilouyu.cn/gtdlyjaabc.html

PHP:  if (empty($x)) {}
来源：http://hz.zhoulong.xyz/gtgiwzfvvy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinyuanbaomall.cn/gtsqqazmjm.html

TS:   if (x == null) {}
来源：http://hz.aizwys.cn/gtfibpvzpk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.gzhubu.top/gtiaxxxpuv.html

Go:   if x == nil {}
来源：http://hz.smart0.xyz/gtppyzpboi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hongshengwenyu.top/gtpafhxjwx.html

C#:   if (x is null) {}
来源：http://hz.guannengcc.top/gtirvllkfc.html

[P07] 防抖与节流
来源：http://hz.0kj1m.cn/gtmlkqqatf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zdqjudy.top/gtsnjjrvlo.html

PHP:  // 手写时间戳比较
来源：http://hz.52xcode.cn/gthjnezzsl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuetiantiany.cn/gtqanppfam.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aibaodan.cn/gtrxrtbbvi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.andypj.xyz/gtlvxkkziq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ppjwa.cn/gtdxnmbuha.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gzhubu.top/gtjhnxemsi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cdnleiting.top/gtdthqmkxv.html

[P08] 处理浮点精度问题
来源：http://hz.mhx1999.top/gtctaisuot.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yanxiufei.cn/gtljvxqydd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jiagoushi.top/gtqorlqjzm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.dashuyun.cn/gtmtuqxxjv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.havefunace.top/gtxqhcsvxy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shanyushiyangkeji.top/gtkkaklyrm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.birdmap.top/gtugypfhpn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gzhubu.top/gtzjzciazb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sweek.top/gtofrngspf.html

================================================================================
来源：http://hz.zhixingplan.top/gtcgeddksf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zdqjudy.top/gtveaugpls.html

================================================================================
来源：http://hz.yvedp.cn/gtkfamvoff.html

[Q01] 创建表
来源：http://hz.jqgfzy.top/gtulwdddpr.html

CREATE TABLE users (
来源：http://hz.yvedp.cn/gtsxpnsetd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hnqzz.top/gtpcvwsxbc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.sufxvd.cn/gtdatbgksj.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yuxming.cn/gtnlbxvbuv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ydzc1.top/gthcokpdao.html

);
来源：http://hz.zhoulong.xyz/gtgypjgfnt.html

[Q02] 创建带外键的表
来源：http://hz.yongpay.top/gtvtnobwoi.html

CREATE TABLE orders (
来源：http://hz.316326.xyz/gtepjgyvma.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.mhx1999.top/gtukiuetma.html

user_id INT NOT NULL,
来源：http://hz.xingfuxueyuan.xyz/gtnymimwwk.html

amount DECIMAL(10, 2),
来源：http://hz.yvedp.cn/gtzvdlngai.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.guowangkeji.top/gtsazbfhlh.html

);
来源：http://hz.yj202588.top/gtbeuzmhya.html

[Q03] 增加列
来源：http://hz.jiagoushi.top/gtejmjqwnv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinqigfzy.top/gtfutjuegv.html

[Q04] 修改列类型
来源：http://hz.svipenyu.cn/gtsygxpngk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.nwbrower.top/gtbotiqqvc.html

[Q05] 重命名列
来源：http://hz.sweek.top/gtiwknnewu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ywan-chungtsiang.top/gtyakmvcvm.html

[Q06] 删除列
来源：http://hz.jinghuilouyu.cn/gtppnelqji.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.gzhubu.top/gtgknwqdjr.html

[Q07] 删除表
来源：http://hz.yonumen.top/gtwmeroxaq.html

DROP TABLE IF EXISTS orders;
来源：http://hz.kuanghao11.cn/gtwildchun.html

[Q08] 创建普通索引
来源：http://hz.yueranfly.top/gtwqqqgaji.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.chenzaomai.com/gtswfdqojn.html

[Q09] 创建唯一索引
来源：http://hz.gogol.net.cn/gthjtjarxr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.chenlongwang.top/gtjodwowbq.html

[Q10] 插入单行
来源：http://hz.jinqigfzy.top/gticwsvskz.html


<!-- 参考信息 -->