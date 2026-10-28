代发 wailian999

Py:   if __name__ == "__main__":
来源：http://hz.nanxuanxn.top/gtcxvmvixf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shuidangran.top/gtudiowezh.html

JS:   require.main === module
来源：http://hz.dashuyun.cn/gtendkpvlg.html

TS:   require.main === module
来源：http://hz.aibaodan.cn/gtzeoyrohk.html

Java: public static void main(String[] args)
来源：http://hz.nanxuanxn.top/gtjxoywfna.html

Go:   func main()
来源：http://hz.yj202588.top/gtixyjsznc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xylfe.cn/gtxxgdkarm.html

C#:   static void Main(string[] args)
来源：http://hz.kuanghao11.cn/gtyplfvcda.html

[M08] 获取系统与运行时信息
来源：http://hz.yj20258.top/gttvwyhvhf.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinghuilouyu.cn/gtilaexetu.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.aizwys.cn/gttkcymjva.html

JS:   process.platform;  process.version
来源：http://hz.guannengcc.top/gtdvghkvog.html

TS:   process.platform;  process.version
来源：http://hz.yuxming.cn/gtoflowodd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jlsjyb.cn/gttjyuwnlm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cqqwz.cn/gtjbasjdkp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.aibaodan.cn/gttzlqbxvl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.meibo888.top/gtpczhtbhx.html

================================================================================
来源：http://hz.tanke756.top/gtpkugjyhd.html

N. 数据结构与算法
来源：http://hz.iojbl.cn/gtsfoyfgqe.html

================================================================================
来源：http://hz.meibo888.top/gtohnzdcvj.html

[N01] 二分查找（有序数组）
来源：http://hz.zhongyouzk.top/gtsokkogzx.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nanxuanxn.top/gtwzxjnmqs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yuxming.cn/gtiobufzyu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnxiangtu.top/gtdxfrhpew.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.pycfn.com/gtweycxjzf.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.tianlin.xyz/gtgvezewxw.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cdnleiting.top/gtjwblzpjl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhaomingkeji.xyz/gtzolyxdgx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hfpthk.cn/gtomukcnhi.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ywan-chungtsiang.top/gtnnhuetkm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.feifeiyinyue.top/gtcmqjwdsq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.dashuyun.cn/gtrcxqtnsn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinyuanbaomall.cn/gthbcbtsoc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yanxiufei.cn/gtghvuomrf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hongshengwenyu.top/gtbzekrlyh.html

Go:   slices.Sort(arr)
来源：http://hz.cdnleiting.top/gtuuprqkwy.html

Ruby: arr.sort
来源：http://hz.xylfe.cn/gtgozleify.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.guannengcc.top/gtflmczjwg.html

[N03] 快速排序（分治示例）
来源：http://hz.chenjidiqi.icu/gtxulzstcg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.pycfn.com/gtjmkxmljc.html

PHP:  // 递归实现，或用 usort
来源：http://hz.316326.xyz/gtphhdpopf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shangyingyoupin.top/gtrubpmcbo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yongpay.top/gtnrkxiwrc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.dianchejie.cn/gtbieizgci.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jyoumei.cn/gtnjwpbjyg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yangfankeji.com/gtqreogvym.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.wangshuangyany.cn/gtjanawowd.html

[N04] 斐波那契数列
来源：http://hz.ivvv.top/gthuoqphxo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jqgfzy.top/gtogakffui.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.redwolf501.top/gtzxarsara.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jlsjyb.cn/gtplyfrmns.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yongpay.top/gtffumlizu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xuanzx.com/gtnmweflju.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.daxiang520.top/gtbcwzghrz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hnxiangtu.top/gtaxtazymt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xinyue.icu/gtskrssbfw.html

[N05] 最大公约数
来源：http://hz.cheryme.top/gtnnhykibc.html

Py:   math.gcd(a, b)
来源：http://hz.hammf.cn/gtmeaxvdbd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.0kj1m.cn/gtunhkekqc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.bjfxy.top/gtotqcpncw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pengpengdd.cyou/gtaiopnzbk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ywan-chungtsiang.top/gtnsgjrcqa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sysykeji.top/gtexrnerni.html

Ruby: a.gcd(b)
来源：http://hz.sufxvd.cn/gtditwkiqs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jyoumei.cn/gtraexhirs.html

[N06] 判断回文字符串
来源：http://hz.chenjidiqi.icu/gtcfliqoiz.html

Py:   s == s[::-1]
来源：http://hz.yuanzhike.top/gtyonjtcjt.html

PHP:  $s === strrev($s);
来源：http://hz.jqgfzy.top/gttpokthja.html

JS:   s === [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtiefxceme.html

TS:   s === [...s].reverse().join("")
来源：http://hz.iojbl.cn/gtbwoqucfa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shanyushiyangkeji.top/gtexhhkpkl.html

Go:   // 双指针从两端比较
来源：http://hz.hysaishi.cn/gtjtboicef.html

Ruby: s == s.reverse
来源：http://hz.jinqigufen.top/gtuewsaahg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jqgfzy.top/gtlojcefvz.html

[N07] 两数之和（返回下标）
来源：http://hz.yj202588.top/gtoaejpbea.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jqgfzy.top/gtpjpfxxls.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xinyue.icu/gtblkolhdr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jyoumei.cn/gtdzbhfsje.html

TS:   // 手写 Map<string, number>
来源：http://hz.316326.xyz/gtzqlshtbq.html

Java: // 手写 HashMap
来源：http://hz.xziqi.cn/gtzpmzsbjd.html

Go:   // 手写 map[int]int
来源：http://hz.aizwys.cn/gtxapmtwxg.html

Ruby: // 手写 Hash
来源：http://hz.iojbl.cn/gtmudipsae.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sweek.top/gtdrcsaoix.html

[N08] 生成全排列
来源：http://hz.dianchejie.cn/gtllneaxbq.html

Py:   itertools.permutations(arr)
来源：http://hz.zhoulong.xyz/gtwdlhwlic.html

PHP:  // 手写递归交换
来源：http://hz.vqdsnc.cn/gtvrbzmnlo.html

JS:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtfdytyuwx.html

TS:   // 手写回溯递归
来源：http://hz.cashguo.top/gtpahaddgg.html

Java: // 手写回溯递归
来源：http://hz.xuanzx.com/gtjmgbiqey.html

Go:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gthfpuegmv.html

Ruby: arr.permutation.to_a
来源：http://hz.zhongyouzk.top/gtyuuhmltk.html

C#:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtbpznyvnw.html

[N09] 栈与队列
来源：http://hz.pycfn.com/gtpjldjbey.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.pycfn.com/gtejwupewd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jiagoushi.top/gtzdwahkiu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cheryme.top/gtbfrunqhs.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinyuanbaomall.cn/gtagjmgpcv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.redwolf501.top/gttffmcmag.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hammf.cn/gtzkwwgruw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.chenjidiqi.icu/gtslhvpfad.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.nwbrower.top/gtbzzdznyz.html

[N10] 链表节点定义
来源：http://hz.svipenyu.cn/gticvdcpft.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhengqikj.top/gtvygqehat.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yj202588.top/gtwsiszxnz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.9152youxi.cn/gtkqdsngqd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhijiandao.cn/gtubwyhryc.html

Java: class Node { int v; Node next; }
来源：http://hz.cucudq.cn/gtdmcxwbgj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.0kj1m.cn/gtmtfegalm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinqigfzy.top/gtdfdldehi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhijiandao.cn/gtcvozzbnr.html

[N11] 二叉树中序遍历
来源：http://hz.dashuyun.cn/gtocxrzgrh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.tian-w.cn/gtzqvzezcx.html

PHP:  // 手写递归函数
来源：http://hz.zhixingplan.top/gtybzxwsaq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxinkj.top/gtxvwqqcsq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ehwqpu.com/gtbeqxsdxl.html

Java: // 手写递归
来源：http://hz.iojbl.cn/gtuzaoasnv.html

Go:   // 手写递归
来源：http://hz.fzhhl.top/gtwqmpkslz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.guowangkeji.top/gtasqgnxzw.html

C#:   // 手写递归
来源：http://hz.zhijiandao.cn/gtuohlfjrm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shuidangran.top/gtwrgqyrrb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.guannengcc.top/gtqzopklxd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.tanke756.top/gtlheqvgew.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangtech.top/gtfzmcuopa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tian-w.cn/gtfybhklth.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jiagoushi.top/gtotcihigw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.daria6918.cn/gtrbskpvyu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cucudq.cn/gtaxtiuoaw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gtqdmiwpyq.html

================================================================================
来源：http://hz.sysykeji.top/gttoammfuq.html

O. 并发与异步
来源：http://hz.xinyue.icu/gttsmxovqp.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtyutewalx.html

[O01] 启动一个线程
来源：http://hz.jinqigfzy.top/gtsvbxzuxy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.52xcode.cn/gtslowtnsx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.aizwys.cn/gtviepzwzu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.tanke756.top/gtsxntosbu.html

TS:   // 同 JS
来源：http://hz.yanxiufei.cn/gtoqchntjz.html

Java: new Thread(() -> f()).start()
来源：http://hz.gzhubu.top/gtnwgyxdtt.html

Go:   go f()
来源：http://hz.jinghuilouyu.cn/gtrxfcuiwl.html

Ruby: Thread.new { f }
来源：http://hz.cheryme.top/gtjqcdktbu.html

C#:   Task.Run(() => F());
来源：http://hz.cqqwz.cn/gtiwsxvsiv.html

[O02] 使用线程池
来源：http://hz.316326.xyz/gtnhgfxzfo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.svipenyu.cn/gtiwvjouiz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.meibo888.top/gtyyekbjat.html

JS:   // worker_threads 线程池
来源：http://hz.yuanzhike.top/gtarmlklpt.html

TS:   // worker_threads 线程池
来源：http://hz.andypj.xyz/gtgylqswik.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.sweek.top/gtoyxrjoty.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yongpay.top/gtjqfxqrdk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.nanxinkj.top/gtuegfpwwn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhaomingkeji.xyz/gtlrhbchki.html

[O03] 加锁保护共享数据
来源：http://hz.haohaochexian.top/gtqmonfgdf.html

Py:   with lock: shared += 1
来源：http://hz.yuanzhike.top/gtykhnmlqb.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cheryme.top/gthjiijvkz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.wangdashe.top/gteytgoxfj.html

TS:   // 同 JS
来源：http://hz.sysykeji.top/gtnxkbzzij.html

Java: synchronized (this) { shared++; }
来源：http://hz.fengsongda.top/gtdnzczbgc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shanyushiyangtech.top/gtvnepoffw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yj20258.top/gtoafyegmb.html

C#:   lock (gate) { shared++; }
来源：http://hz.pycfn.com/gtwzsuzsyy.html

[O04] 定义异步函数并等待
来源：http://hz.hnxiangtu.top/gtjmrwsvsu.html

Py:   async def f():⏎    await g()
来源：http://hz.nwbrower.top/gtfvivsuxw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.chenzaomai.com/gtnxolntej.html

JS:   async function f() { await g(); }
来源：http://hz.nanxuanxn.top/gthbutphxx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ywan-chungtsiang.top/gtosznnmkc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.nanxinkj.top/gtytpjkwuu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.redwolf501.top/gtmbecjmjc.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zdqjudy.top/gtquldkfao.html

C#:   async Task F() { await G(); }
来源：http://hz.cdnleiting.top/gtzifaupgm.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhixingplan.top/gtxdgsnnqf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.wangdashe.top/gtizbneeqi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cucudq.cn/gtqbhnhbvz.html

JS:   await Promise.all(tasks)
来源：http://hz.sweek.top/gtcbrabmkj.html

TS:   await Promise.all(tasks)
来源：http://hz.316326.xyz/gtnzgjdujg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ywan-chungtsiang.top/gtcwanxkys.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.chenzaomai.com/gtqgxmxnwu.html

Ruby: threads.map(&:join)
来源：http://hz.sysykeji.top/gtsbtiazru.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.tianlin.xyz/gtwidbbhtw.html

[O06] 使用进程池
来源：http://hz.hnxiangtu.top/gtywhykpjx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.sufxvd.cn/gtjgdawosb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ydzc1.top/gtsylyupxx.html

JS:   // child_process / cluster 模块
来源：http://hz.tian-w.cn/gtxosadejp.html

TS:   // child_process / cluster 模块
来源：http://hz.yueranfly.top/gtslpokkre.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hysaishi.cn/gtcusfphad.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shangyingyoupin.top/gtcvqdhkjw.html

Ruby: // fork 块
来源：http://hz.ehwqpu.com/gtnzxqkrrn.html

C#:   Parallel.For
来源：http://hz.guowangkeji.top/gtytfszbak.html

================================================================================
来源：http://hz.iojbl.cn/gtmomuqyoh.html

P. 常用工具函数
来源：http://hz.jiagoushi.top/gtqlogmmqy.html

================================================================================
来源：http://hz.cucudq.cn/gteyskklhb.html

[P01] 生成 UUID
来源：http://hz.chenlongwang.top/gtbdeynepx.html

Py:   str(uuid.uuid4())
来源：http://hz.316326.xyz/gtlviunllm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xylfe.cn/gtcdthpjhs.html

JS:   crypto.randomUUID()
来源：http://hz.xingfuxueyuan.xyz/gtbtkjnksc.html

TS:   crypto.randomUUID()
来源：http://hz.birdmap.top/gtctaqxxib.html

Java: UUID.randomUUID().toString()
来源：http://hz.cdnleiting.top/gtdlkmeegc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ybcxt.top/gtevkgcdtf.html

Ruby: SecureRandom.uuid
来源：http://hz.yonumen.top/gtmirnnsac.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinqigfzy.top/gtmtehujvy.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cashguo.top/gtoukjmlrg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.tianlin.xyz/gtfxyiymkd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.nanxinkj.top/gtxdvazbxa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinqigfzy.top/gtiazzmzyf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yuxming.cn/gtjrtvtcyr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.haohaochexian.top/gtwimvpjfj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.pengpengdd.cyou/gtfkmtkkmv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.iojbl.cn/gtlwqwdvhp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.iojbl.cn/gtosotxaph.html

[P03] 生成短随机字符串
来源：http://hz.svipenyu.cn/gtghaupqqp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xziqi.cn/gtsrsaqyev.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shzxlz.cn/gtrfjbizmo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxinkj.top/gtprdkzask.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenjidiqi.icu/gtvxnrulyz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.c1oappe.top/gtopuptccu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jqgfzy.top/gtznizscbu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jqgfzy.top/gtfedyygjm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ydjk.org.cn/gtmqdfwrbr.html

[P04] 求长度
来源：http://hz.xylfe.cn/gtdydukolk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.snrcjt.cn/gtxwigedqx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zdqjudy.top/gtwapejuvd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinyuanbaomall.cn/gtbbfiyqds.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhaomingkeji.xyz/gthkzvsqbh.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhoulong.xyz/gtqxomuaog.html

Go:   len(arr);  len(m)
来源：http://hz.hywenlv.cn/gtsobkfyvq.html

Ruby: x.length;  x.size
来源：http://hz.zhijiandao.cn/gtdzerreek.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.bjfxy.top/gtahdrsbzv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.dashuyun.cn/gtljpfdbyi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xingfuxueyuan.xyz/gtyyzjfcvg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.tianlin.xyz/gtkzhrgflu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jqgufenzy.top/gtuxlwsuqy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.kuanghao11.cn/gtxcbqhrfl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinghuilouyu.cn/gtqzzjhcss.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ydzc1.top/gtujliqvrn.html

Ruby: a == b
来源：http://hz.shanyushiyangtech.top/gtvnowjwwz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhoulong.xyz/gtkgnuwnjs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.fzhhl.top/gtkcfupbhs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.fzhhl.top/gtccmnpnta.html

PHP:  if (empty($x)) {}
来源：http://hz.jyoumei.cn/gtypqzvlgw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cucudq.cn/gtjcnnvugj.html

TS:   if (x == null) {}
来源：http://hz.ydzc1.top/gtophvsicv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.vqdsnc.cn/gtpvgkcfew.html

Go:   if x == nil {}
来源：http://hz.xylfe.cn/gtxrmmyuka.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.guowangkeji.top/gtybcbkvbl.html

C#:   if (x is null) {}
来源：http://hz.vqdsnc.cn/gtrfbmiutp.html

[P07] 防抖与节流
来源：http://hz.kuanghao11.cn/gtslybxykw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.fengsongda.top/gtjdzcvfbi.html

PHP:  // 手写时间戳比较
来源：http://hz.dianchejie.cn/gtvlksogeo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinyuanbaomall.cn/gtsytezddp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.andypj.xyz/gtvlnxfehl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.birdmap.top/gtdykiqoie.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hongshengwenyu.top/gtimyaamfb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sufxvd.cn/gtvxwsyule.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.nanxuanxn.top/gtkuiyyrqw.html

[P08] 处理浮点精度问题
来源：http://hz.jlsjyb.cn/gtfcxuyudi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ehwqpu.com/gtzbvaybsm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhoulong.xyz/gtieqsfxip.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jianghu66.top/gtctrdaqal.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xuanzx.com/gtjbrjbxzi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.aizwys.cn/gtjeqjdhdw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhongyouzk.top/gtizsqnuee.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shzxlz.cn/gtxtpoboqv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.gotoacloud.top/gttfvsbaqt.html

================================================================================
来源：http://hz.yj202588.top/gtmiqzyfgf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj20258888.top/gtfokppzhm.html

================================================================================
来源：http://hz.gotoacloud.top/gthlzbdddt.html

[Q01] 创建表
来源：http://hz.dashuyun.cn/gtzzairgsi.html

CREATE TABLE users (
来源：http://hz.sysykeji.top/gtqomckadx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinyuanbaomall.cn/gtngbscfir.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhixingplan.top/gtkcgeffps.html

email VARCHAR(100) UNIQUE,
来源：http://hz.kuanghao11.cn/gtumvlohoz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.dashuyun.cn/gtlxrpghzh.html

);
来源：http://hz.svipenyu.cn/gtyezasewb.html

[Q02] 创建带外键的表
来源：http://hz.sufxvd.cn/gttjozhzoo.html

CREATE TABLE orders (
来源：http://hz.vqdsnc.cn/gttocihagk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xziqi.cn/gtvbnyoosj.html

user_id INT NOT NULL,
来源：http://hz.jyoumei.cn/gttarcuxvu.html

amount DECIMAL(10, 2),
来源：http://hz.havefunace.top/gthpcsofxg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yanxiufei.cn/gtxfdsjalc.html

);
来源：http://hz.yonumen.top/gttmqqmrax.html

[Q03] 增加列
来源：http://hz.andypj.xyz/gtmjifooqs.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.gaohongyu789.top/gtaotrancp.html

[Q04] 修改列类型
来源：http://hz.cashguo.top/gtrwoyylls.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yuxming.cn/gtckccfapu.html

[Q05] 重命名列
来源：http://hz.jinqigufen.top/gtrgpjvcry.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ehwqpu.com/gtdogluqhn.html

[Q06] 删除列
来源：http://hz.sysykeji.top/gtguovalzd.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.iojbl.cn/gtlhakfcye.html

[Q07] 删除表
来源：http://hz.yangfankeji.com/gtmhgkfazh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.haohaochexian.top/gtxrebcwne.html

[Q08] 创建普通索引
来源：http://hz.daxiang520.top/gtxvedvhrd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yj20258888.top/gtglezdlln.html

[Q09] 创建唯一索引
来源：http://hz.snrcjt.cn/gtrlodsegs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cdnleiting.top/gtyzfalzmb.html

[Q10] 插入单行
来源：http://hz.gaohongyu789.top/gtcunitpnz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yuanzhike.top/gtcrvyrrxs.html

[Q11] 一次插入多行
来源：http://hz.guowangkeji.top/gttxajdjls.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hysaishi.cn/gtjcxibvau.html

[Q12] 插入后取自增 ID
来源：http://hz.yonumen.top/gtvqwxswmk.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.wangdashe.top/gtoqddbyna.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jiagoushi.top/gtvkikxygj.html

[Q13] 忽略重复插入
来源：http://hz.guannengcc.top/gtpssmmvdc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hysaishi.cn/gtqzxnmunu.html


<!-- 参考信息 -->