代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ivvv.top/gtrtjoydnr.html

Ruby: warn "err"
来源：http://hz.svipenyu.cn/gthsafvnoj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cdnleiting.top/gtgonbgpsl.html

[M07] 判断是否为主入口
来源：http://hz.gotoacloud.top/gthaycqpak.html

Py:   if __name__ == "__main__":
来源：http://hz.jinqigufen.top/gtydeoqvze.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yj20258.top/gtavtzrwmu.html

JS:   require.main === module
来源：http://hz.shanyushiyangkeji.top/gtecpjgdqa.html

TS:   require.main === module
来源：http://hz.9152youxi.cn/gtgtdngebz.html

Java: public static void main(String[] args)
来源：http://hz.wangshuangyany.cn/gtunzkggwu.html

Go:   func main()
来源：http://hz.dashuyun.cn/gteqfrulfi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yuxming.cn/gtbrqadjhb.html

C#:   static void Main(string[] args)
来源：http://hz.yj20258888.top/gtncvomoyz.html

[M08] 获取系统与运行时信息
来源：http://hz.jqgfzy.top/gtzkvdnvpw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.aizwys.cn/gtjijdijne.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yangfankeji.com/gtxfvecsey.html

JS:   process.platform;  process.version
来源：http://hz.zhijiandao.cn/gtxcbchbrf.html

TS:   process.platform;  process.version
来源：http://hz.daxiang520.top/gtctgkmpyw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.guowangkeji.top/gtfivjozkf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hnqzz.top/gtddmafyca.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.andypj.xyz/gtusevghpx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sxryk.cn/gtxzfbzyjy.html

================================================================================
来源：http://hz.meibo888.top/gtaitcmjua.html

N. 数据结构与算法
来源：http://hz.wangshuangyany.cn/gtgmpvpqrs.html

================================================================================
来源：http://hz.iojbl.cn/gtckwgytum.html

[N01] 二分查找（有序数组）
来源：http://hz.gaohongyu789.top/gtvymclbjx.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zycfv.cn/gteypppexx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hfpthk.cn/gtwvfjkzro.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cdnleiting.top/gtndshvqbk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cucudq.cn/gtlimvmypg.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gzhubu.top/gtzlaxjqtr.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.316326.xyz/gtdidhzdbl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yangfankeji.com/gthergyczl.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hnqzz.top/gtgctrqmer.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.wangshuangyany.cn/gtimnjsphd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigufen.top/gtnxsyaqnw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.fzhhl.top/gtwcyqxsfs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daria6918.cn/gtvlsvtfyw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gtqmyqhmdr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.bjfxy.top/gtuviqyoxj.html

Go:   slices.Sort(arr)
来源：http://hz.havefunace.top/gtftflwghg.html

Ruby: arr.sort
来源：http://hz.ydjk.org.cn/gtqlwjnvkz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.gaohongyu789.top/gtfboqkmfa.html

[N03] 快速排序（分治示例）
来源：http://hz.bjfxy.top/gtcdjckdqe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xingfuxueyuan.xyz/gtkcxwysrb.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hongshengwenyu.top/gtwxaqccct.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydjk.org.cn/gtjahkbvnx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuanzhike.top/gthmtsvidb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cheryme.top/gtylrhtwrp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinqigufen.top/gtqmapwcau.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.guannengcc.top/gtvjfnpfxx.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhiwuduotai.top/gteqvaryex.html

[N04] 斐波那契数列
来源：http://hz.fzhhl.top/gtdwvidazy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cheryme.top/gtaknwrcxw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zycfv.cn/gtkhayimsp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cqqwz.cn/gtfereltcf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.svipenyu.cn/gtwrwcrnnw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.snrcjt.cn/gtgoiahcho.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xingfuxueyuan.xyz/gtkjiosokf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhengqikj.top/gtnjyhbrvj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cqqwz.cn/gtuztipiaq.html

[N05] 最大公约数
来源：http://hz.guowangkeji.top/gtyousrvhy.html

Py:   math.gcd(a, b)
来源：http://hz.havefunace.top/gtywphonft.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhoulong.xyz/gtyueobcez.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ywan-chungtsiang.top/gtcadgpfsl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jlsjyb.cn/gtrotjtpou.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yongpay.top/gtzytllhng.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenjidiqi.icu/gttfrthgjv.html

Ruby: a.gcd(b)
来源：http://hz.sufxvd.cn/gtlxozgkux.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hysaishi.cn/gtzpzpntdk.html

[N06] 判断回文字符串
来源：http://hz.aizwys.cn/gtsddoggwv.html

Py:   s == s[::-1]
来源：http://hz.jinghuilouyu.cn/gtmdlgiusu.html

PHP:  $s === strrev($s);
来源：http://hz.shanyushiyangkeji.top/gtecdjonhf.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtoihmymoy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.birdmap.top/gtdpabgeaa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hfpthk.cn/gtkimsatib.html

Go:   // 双指针从两端比较
来源：http://hz.sysykeji.top/gtkbyezbtr.html

Ruby: s == s.reverse
来源：http://hz.jyoumei.cn/gtrdtlgjxh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.havefunace.top/gtwyergcff.html

[N07] 两数之和（返回下标）
来源：http://hz.guowangkeji.top/gtdnqtboiz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinghuilouyu.cn/gtltngbgag.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yangfankeji.com/gtrcrugeil.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.snrcjt.cn/gtzyfrgyqn.html

TS:   // 手写 Map<string, number>
来源：http://hz.chenzaomai.com/gtbogtpmrh.html

Java: // 手写 HashMap
来源：http://hz.dianchejie.cn/gtiqnguykw.html

Go:   // 手写 map[int]int
来源：http://hz.quarkkingdee.top/gtbmyexlbm.html

Ruby: // 手写 Hash
来源：http://hz.yuanzhike.top/gtvftgqeov.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.tian-w.cn/gtcyseqhay.html

[N08] 生成全排列
来源：http://hz.ydzc1.top/gtvvdigvbi.html

Py:   itertools.permutations(arr)
来源：http://hz.52xcode.cn/gtrhptbzqs.html

PHP:  // 手写递归交换
来源：http://hz.bjfxy.top/gtjxarakpu.html

JS:   // 手写回溯递归
来源：http://hz.guannengcc.top/gthhgtbkyd.html

TS:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtxwujnhtu.html

Java: // 手写回溯递归
来源：http://hz.andypj.xyz/gtcwlakzxl.html

Go:   // 手写回溯递归
来源：http://hz.cheryme.top/gtlwbsjsxk.html

Ruby: arr.permutation.to_a
来源：http://hz.zdqjudy.top/gthlgmyzgj.html

C#:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtzmnczpxm.html

[N09] 栈与队列
来源：http://hz.quarkkingdee.top/gtvvlcdonz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.pengpengdd.cyou/gtchdaryod.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ydzc1.top/gtzdpzfbaa.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.pengpengdd.cyou/gtbkbqamrs.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jqgufenzy.top/gtziseyrlq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.havefunace.top/gtfbekcpzh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.fengsongda.top/gtpwatjadg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.fengsongda.top/gtjshmftrb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhongyouzk.top/gtzjtnyskq.html

[N10] 链表节点定义
来源：http://hz.316326.xyz/gtvfottwcy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yj20258888.top/gtwsswraag.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhongyouzk.top/gtpprncztu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhijiandao.cn/gtsjshrbzs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xziqi.cn/gtxyjoovyf.html

Java: class Node { int v; Node next; }
来源：http://hz.zhijiandao.cn/gtfpylnjbo.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.feifeiyinyue.top/gtptukjbsu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.birdmap.top/gtlppoygbf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.tianlin.xyz/gtukooffra.html

[N11] 二叉树中序遍历
来源：http://hz.jinqigufen.top/gtlzbcxvzb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yonumen.top/gtubfzwghb.html

PHP:  // 手写递归函数
来源：http://hz.yuxming.cn/gtdexnhcoe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yonumen.top/gtzgjcfwrc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.andypj.xyz/gtekqgtnhj.html

Java: // 手写递归
来源：http://hz.ehwqpu.com/gtzczxmjnq.html

Go:   // 手写递归
来源：http://hz.yongpay.top/gtdeoefosk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.chenzaomai.com/gtxmtupczc.html

C#:   // 手写递归
来源：http://hz.0kj1m.cn/gtjvhfqzkf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.wangshuangyany.cn/gtjzqnxwnj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yongpay.top/gtitmynyik.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yongpay.top/gtzjajuzbk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xingfuxueyuan.xyz/gtqmgcoabq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dianchejie.cn/gtsrxxqlbq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.c1oappe.top/gtjpfxttbz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jinqigfzy.top/gthcolulrp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yueranfly.top/gtwhavpltf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenjidiqi.icu/gtcxfrqoiz.html

================================================================================
来源：http://hz.chenlongwang.top/gtldosjtos.html

O. 并发与异步
来源：http://hz.iojbl.cn/gtysvrzmup.html

================================================================================
来源：http://hz.yuxming.cn/gtqquyfhwk.html

[O01] 启动一个线程
来源：http://hz.yj202588.top/gtrgchhsok.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.daxiang520.top/gtgkwgahrp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.quarkkingdee.top/gtlmzquomp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.sweek.top/gtvsnwisua.html

TS:   // 同 JS
来源：http://hz.yonumen.top/gtgprawzmk.html

Java: new Thread(() -> f()).start()
来源：http://hz.c1oappe.top/gtxkenraws.html

Go:   go f()
来源：http://hz.chenzaomai.com/gtrlzwhkpy.html

Ruby: Thread.new { f }
来源：http://hz.zhengqikj.top/gtwtxhqsdh.html

C#:   Task.Run(() => F());
来源：http://hz.9152youxi.cn/gttbovqdgf.html

[O02] 使用线程池
来源：http://hz.gzhubu.top/gtxgxgkgji.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.316326.xyz/gtluxkjnhe.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.chenzaomai.com/gtgemnkdcv.html

JS:   // worker_threads 线程池
来源：http://hz.gotoacloud.top/gtkzrktbbl.html

TS:   // worker_threads 线程池
来源：http://hz.nanxuanxn.top/gtiomurkhc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xziqi.cn/gtwrjzxisy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhaomingkeji.xyz/gtgzedezcf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.vqdsnc.cn/gtbytwohzl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.316326.xyz/gtravpenoj.html

[O03] 加锁保护共享数据
来源：http://hz.jinghuilouyu.cn/gtbhnzfyeh.html

Py:   with lock: shared += 1
来源：http://hz.zhoulong.xyz/gtzuukujun.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.redwolf501.top/gtvfjjkeux.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zycfv.cn/gtkleouccu.html

TS:   // 同 JS
来源：http://hz.shzxlz.cn/gtwbqbfkxz.html

Java: synchronized (this) { shared++; }
来源：http://hz.jqgfzy.top/gtdufhwylf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cheryme.top/gtozulslgy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhaomingkeji.xyz/gtjtmsrgfg.html

C#:   lock (gate) { shared++; }
来源：http://hz.ywan-chungtsiang.top/gtmelkmfzd.html

[O04] 定义异步函数并等待
来源：http://hz.vqdsnc.cn/gtnpqqyxqg.html

Py:   async def f():⏎    await g()
来源：http://hz.nanxuanxn.top/gtigysfhva.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gogol.net.cn/gtisowhtlm.html

JS:   async function f() { await g(); }
来源：http://hz.sweek.top/gtplztoasv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ydjk.org.cn/gtmuuqrlay.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xuetiantiany.cn/gtiphhugrg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yvedp.cn/gtmxflsxma.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.snrcjt.cn/gtuayufmfh.html

C#:   async Task F() { await G(); }
来源：http://hz.xuetiantiany.cn/gtlzeizubn.html

[O05] 并发执行并等待全部完成
来源：http://hz.wangshuangyany.cn/gtoxjlhwxq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hywenlv.cn/gtumaphfsr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jlsjyb.cn/gtgqpelagj.html

JS:   await Promise.all(tasks)
来源：http://hz.meibo888.top/gtnvxkrgpz.html

TS:   await Promise.all(tasks)
来源：http://hz.cdnleiting.top/gtqfhcsbcc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zdqjudy.top/gtfwkmnchy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.vqdsnc.cn/gtprcpdpif.html

Ruby: threads.map(&:join)
来源：http://hz.jiagoushi.top/gtrmwrskcu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.redwolf501.top/gtkeyjhvhs.html

[O06] 使用进程池
来源：http://hz.kuanghao11.cn/gthqzajyay.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cdnleiting.top/gtcmtbktyf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhijiandao.cn/gtgvhzppvl.html

JS:   // child_process / cluster 模块
来源：http://hz.zhongyouzk.top/gtablsukae.html

TS:   // child_process / cluster 模块
来源：http://hz.jianghu66.top/gtspxvyirq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xziqi.cn/gtsfnfbais.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yvedp.cn/gtxpsgteex.html

Ruby: // fork 块
来源：http://hz.shangyingyoupin.top/gtihglobpe.html

C#:   Parallel.For
来源：http://hz.shanyushiyangkeji.top/gtucehdbxq.html

================================================================================
来源：http://hz.yvedp.cn/gtozlouvtx.html

P. 常用工具函数
来源：http://hz.fengsongda.top/gtagdmamoc.html

================================================================================
来源：http://hz.wangshuangyany.cn/gthgauwasz.html

[P01] 生成 UUID
来源：http://hz.0kj1m.cn/gtxfpavurj.html

Py:   str(uuid.uuid4())
来源：http://hz.ywan-chungtsiang.top/gtpwqronil.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.wangshuangyany.cn/gthubedjbb.html

JS:   crypto.randomUUID()
来源：http://hz.zhoulong.xyz/gtxcdqzmsb.html

TS:   crypto.randomUUID()
来源：http://hz.ppjwa.cn/gtgfgngcng.html

Java: UUID.randomUUID().toString()
来源：http://hz.yj202588.top/gtxkbcxhrt.html

Go:   // 用 github.com/google/uuid
来源：http://hz.snrcjt.cn/gtvqfkbsci.html

Ruby: SecureRandom.uuid
来源：http://hz.nanxuanxn.top/gtbogbdssm.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jiagoushi.top/gtlbptngcm.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jlsjyb.cn/gtoxjyalvo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yonumen.top/gtzggcelvm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.kuanghao11.cn/gtywqrwpbf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhaomingkeji.xyz/gtbznsmnaw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xziqi.cn/gtznfmerxq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jinyuanbaomall.cn/gtxdlpahes.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.sweek.top/gtdzscngdb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yuxming.cn/gttedkrybz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yvedp.cn/gtutrxpmge.html

[P03] 生成短随机字符串
来源：http://hz.yj202588.top/gtozeigiyc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.iojbl.cn/gtitacxggw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yj202588.top/gthmyttude.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shzxlz.cn/gthuajdjso.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.daxiang520.top/gtixwslboo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.svipenyu.cn/gtazhmbbyt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.c1oappe.top/gtbofzsztv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zdqjudy.top/gtlxvoopny.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gzhubu.top/gtrrophiit.html

[P04] 求长度
来源：http://hz.ydjk.org.cn/gttghulfyy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.nanxuanxn.top/gtlnhlipiu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhongyouzk.top/gtzjzdmeyy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yvedp.cn/gtahghmqdx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dianchejie.cn/gteprskddj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.nwbrower.top/gtpjqchxub.html

Go:   len(arr);  len(m)
来源：http://hz.mhx1999.top/gtruqmcvrb.html

Ruby: x.length;  x.size
来源：http://hz.nanxinkj.top/gtvrvdpwle.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jlsjyb.cn/gterchdrvd.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jinyuanbaomall.cn/gtquyobabe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xinyue.icu/gtaujevlpc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hywenlv.cn/gtrhwhwnya.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.bjfxy.top/gtaoofbupx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shanyushiyangtech.top/gtwcfovjav.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.fengsongda.top/gtwejuiuav.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhijiandao.cn/gtdptzobbf.html

Ruby: a == b
来源：http://hz.hywenlv.cn/gthearcazc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ydzc1.top/gtmcwqpthp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.0kj1m.cn/gtnixfmxwa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ehwqpu.com/gtsdorbopo.html

PHP:  if (empty($x)) {}
来源：http://hz.zhoulong.xyz/gtttwpaoju.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.snrcjt.cn/gtfekzblxa.html

TS:   if (x == null) {}
来源：http://hz.daxiang520.top/gtcroalslb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.svipenyu.cn/gtgwyspfyz.html

Go:   if x == nil {}
来源：http://hz.pycfn.com/gtsnifmypz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.tanke756.top/gtlntlxflt.html

C#:   if (x is null) {}
来源：http://hz.yanxiufei.cn/gtpcicksss.html

[P07] 防抖与节流
来源：http://hz.fengsongda.top/gtmoaxbefw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.kuanghao11.cn/gtcuclmnmf.html

PHP:  // 手写时间戳比较
来源：http://hz.chenzaomai.com/gtkggqieao.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ehwqpu.com/gtveeposrv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnqzz.top/gttrcxhdar.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yvedp.cn/gtqparxpxg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.nwbrower.top/gtazmrjsni.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ppjwa.cn/gtgmegaysa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.dashuyun.cn/gtosmzafkx.html

[P08] 处理浮点精度问题
来源：http://hz.fzhhl.top/gtpxcvfdek.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xziqi.cn/gtcbftyfos.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.316326.xyz/gteivwkpba.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.smart0.xyz/gtrfjdqjqp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yuxming.cn/gtfsdkauoz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.quarkkingdee.top/gtcezbsroy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenzaomai.com/gthwjkrhwv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gaohongyu789.top/gtbccnscqz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nanxinkj.top/gtfbgoaxxj.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtafvgkmle.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.chenlongwang.top/gtcmrqyeeo.html

================================================================================
来源：http://hz.hammf.cn/gturjrgfag.html

[Q01] 创建表
来源：http://hz.zhengqikj.top/gtdzlrbwnk.html

CREATE TABLE users (
来源：http://hz.yj20258.top/gtwybellop.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gaohongyu789.top/gtcbnfhlro.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hywenlv.cn/gtvuqyqsze.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shzxlz.cn/gtceiqbbfj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xziqi.cn/gtngookoxq.html

);
来源：http://hz.nwbrower.top/gtnycedmua.html

[Q02] 创建带外键的表
来源：http://hz.xuetiantiany.cn/gtoeumdrrn.html

CREATE TABLE orders (
来源：http://hz.shuidangran.top/gtfclbcfci.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.pycfn.com/gtvgagjfzc.html

user_id INT NOT NULL,
来源：http://hz.pycfn.com/gtqfnirqtm.html

amount DECIMAL(10, 2),
来源：http://hz.kuanghao11.cn/gtwfvfpryz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cheryme.top/gtjujzdvto.html

);
来源：http://hz.shanyushiyangtech.top/gtxkuydxit.html

[Q03] 增加列
来源：http://hz.hammf.cn/gtenfrsjck.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhongyouzk.top/gtyedmdnwr.html

[Q04] 修改列类型
来源：http://hz.andypj.xyz/gtjiogxuyh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.daria6918.cn/gtswjmrsav.html

[Q05] 重命名列
来源：http://hz.svipenyu.cn/gtrmaogklb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.bjfxy.top/gtimhpuqtd.html

[Q06] 删除列
来源：http://hz.tianlin.xyz/gteqanhchn.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hnqzz.top/gtwplwqxlw.html

[Q07] 删除表
来源：http://hz.xuetiantiany.cn/gtjywkqcaq.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xuetiantiany.cn/gtizyqgyjs.html

[Q08] 创建普通索引
来源：http://hz.jinqigufen.top/gtupegeygm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhaomingkeji.xyz/gtavivcyke.html

[Q09] 创建唯一索引
来源：http://hz.jiagoushi.top/gtdyctjigf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.daria6918.cn/gtynyqtdlw.html

[Q10] 插入单行
来源：http://hz.yj20258888.top/gtuwjljkcj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.dashuyun.cn/gtidzrnoaf.html

[Q11] 一次插入多行
来源：http://hz.yanxiufei.cn/gtylwoyosb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.nwbrower.top/gtwjyrdmdf.html

[Q12] 插入后取自增 ID
来源：http://hz.cucudq.cn/gtexkgolcs.html


<!-- 参考信息 -->