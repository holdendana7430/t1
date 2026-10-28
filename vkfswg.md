代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.meibo888.top/gtrbkummjd.html

JS:   console.error("err")
来源：http://hz.yanxiufei.cn/gtqbdcxjjq.html

TS:   console.error("err")
来源：http://hz.jqgfzy.top/gtkoglojxz.html

Java: System.err.println("err")
来源：http://hz.xuetiantiany.cn/gtaaadndks.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.0kj1m.cn/gtjwhoqnqk.html

Ruby: warn "err"
来源：http://hz.zdqjudy.top/gtqlphsmbs.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.aibaodan.cn/gtjsmawqhr.html

[M07] 判断是否为主入口
来源：http://hz.yonumen.top/gtouolwzti.html

Py:   if __name__ == "__main__":
来源：http://hz.xinyue.icu/gtisftxsai.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zdqjudy.top/gtjcthzpon.html

JS:   require.main === module
来源：http://hz.haohaochexian.top/gtcsetpnuk.html

TS:   require.main === module
来源：http://hz.yj20258888.top/gtiurgxzvb.html

Java: public static void main(String[] args)
来源：http://hz.quarkkingdee.top/gtusxutpvv.html

Go:   func main()
来源：http://hz.yj20258888.top/gtxjsuxctm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.gaohongyu789.top/gtdpelgkgs.html

C#:   static void Main(string[] args)
来源：http://hz.ydjk.org.cn/gtsnboedam.html

[M08] 获取系统与运行时信息
来源：http://hz.cashguo.top/gtbwwfvtqk.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xinyue.icu/gtwvlvijtq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.daxiang520.top/gtrmmbdfny.html

JS:   process.platform;  process.version
来源：http://hz.wangdashe.top/gtqaamftgu.html

TS:   process.platform;  process.version
来源：http://hz.ppjwa.cn/gtjjlazqeb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cqqwz.cn/gtivegksoz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.fzhhl.top/gtopqwiqkd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.fzhhl.top/gtsfzrhgxm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.chenlongwang.top/gtigaqaubb.html

================================================================================
来源：http://hz.guowangkeji.top/gtsbcswvux.html

N. 数据结构与算法
来源：http://hz.sufxvd.cn/gtegykoojs.html

================================================================================
来源：http://hz.yongpay.top/gtjlitbfdn.html

[N01] 二分查找（有序数组）
来源：http://hz.xuanzx.com/gtvxugsnke.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.daria6918.cn/gtyoayalul.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sufxvd.cn/gtcpahngol.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.iojbl.cn/gtxspfrsqb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuetiantiany.cn/gtovdroxaq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.tanke756.top/gtycwswbhg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ehwqpu.com/gtepmgxqph.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.nanxinkj.top/gtglykqgql.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinghuilouyu.cn/gtvqhrqrug.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.wangdashe.top/gtjqbsllym.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yueranfly.top/gtgpjntvye.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhijiandao.cn/gtbhstuzbt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ybcxt.top/gtirjhlubd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuxming.cn/gtolxhbtya.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.aibaodan.cn/gtrltadbos.html

Go:   slices.Sort(arr)
来源：http://hz.pengpengdd.cyou/gtsmwivttm.html

Ruby: arr.sort
来源：http://hz.tian-w.cn/gtygrsawtc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.smart0.xyz/gthmjqcvsy.html

[N03] 快速排序（分治示例）
来源：http://hz.chenjidiqi.icu/gtrtmkrpys.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.snrcjt.cn/gtdkqllgsr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.bjfxy.top/gtohejrwwd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenjidiqi.icu/gtnewhuoji.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gaohongyu789.top/gtymbwpkpx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinqigufen.top/gtwlsoabgs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.pycfn.com/gtyfjwjvku.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.316326.xyz/gtnwfaejpl.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yuanzhike.top/gtieyjiehv.html

[N04] 斐波那契数列
来源：http://hz.yj20258888.top/gtqzanemjx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yvedp.cn/gtyimmvdml.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jyoumei.cn/gtoouwuivu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ehwqpu.com/gtxteolvno.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fzhhl.top/gthvkwdhpq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.guannengcc.top/gthwswxmjt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xziqi.cn/gtprbvvkcr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.smart0.xyz/gtmrnqieai.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhijiandao.cn/gtmedoajly.html

[N05] 最大公约数
来源：http://hz.feifeiyinyue.top/gtljdunieo.html

Py:   math.gcd(a, b)
来源：http://hz.jinghuilouyu.cn/gtcokvoxru.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.guannengcc.top/gtyliijpjd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cqqwz.cn/gtgjuioyvo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenzaomai.com/gtstuzvopl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.mhx1999.top/gtoweohatm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.gzhubu.top/gtrsoxjjwm.html

Ruby: a.gcd(b)
来源：http://hz.gzhubu.top/gtxyrmfkhl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ywan-chungtsiang.top/gttabndhgu.html

[N06] 判断回文字符串
来源：http://hz.xuetiantiany.cn/gtqmzfsxfm.html

Py:   s == s[::-1]
来源：http://hz.yj20258888.top/gttoxwemla.html

PHP:  $s === strrev($s);
来源：http://hz.xziqi.cn/gtakooiljb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtieefexmy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtnwaxvebq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.wangdashe.top/gtnbxvsurw.html

Go:   // 双指针从两端比较
来源：http://hz.zhiwuduotai.top/gtlltlsajc.html

Ruby: s == s.reverse
来源：http://hz.ywan-chungtsiang.top/gtsgrfsysz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.feifeiyinyue.top/gtidkeutnj.html

[N07] 两数之和（返回下标）
来源：http://hz.zhongyouzk.top/gtolfkwphl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jqgfzy.top/gtqkncceab.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhengqikj.top/gtiqhywwtn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xinyue.icu/gtuydsrszc.html

TS:   // 手写 Map<string, number>
来源：http://hz.xziqi.cn/gtnnajtxmm.html

Java: // 手写 HashMap
来源：http://hz.xziqi.cn/gtwvxiscmu.html

Go:   // 手写 map[int]int
来源：http://hz.hongshengwenyu.top/gtqwechutr.html

Ruby: // 手写 Hash
来源：http://hz.xziqi.cn/gttqukltbu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.daxiang520.top/gtrbdxcroq.html

[N08] 生成全排列
来源：http://hz.shuidangran.top/gtcbolluxv.html

Py:   itertools.permutations(arr)
来源：http://hz.chenzaomai.com/gtnfvxpdmy.html

PHP:  // 手写递归交换
来源：http://hz.guannengcc.top/gtnxgezfzf.html

JS:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtzrsfpxgg.html

TS:   // 手写回溯递归
来源：http://hz.cdnleiting.top/gtqhwrygij.html

Java: // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtvlwsjdjk.html

Go:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtanercgdm.html

Ruby: arr.permutation.to_a
来源：http://hz.xingfuxueyuan.xyz/gtbefjkhqi.html

C#:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtzoteztbo.html

[N09] 栈与队列
来源：http://hz.tanke756.top/gtyujbkgpp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yangfankeji.com/gtivxtmeev.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yanxiufei.cn/gtgbjtdlck.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.svipenyu.cn/gtvjkkjwio.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.sweek.top/gtspmepecu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yj20258.top/gtrlgjvdnb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yongpay.top/gtkvuqpblh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hnxiangtu.top/gtqbkgyosz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yanxiufei.cn/gtajmxjpkd.html

[N10] 链表节点定义
来源：http://hz.birdmap.top/gtdzrfwqbr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shzxlz.cn/gteuoymbda.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yangfankeji.com/gtfktflzjo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cqqwz.cn/gtgikkdafg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jqgfzy.top/gtbycbiyqz.html

Java: class Node { int v; Node next; }
来源：http://hz.shanyushiyangtech.top/gtjiffdvim.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hongshengwenyu.top/gtxwllbwsr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.tianlin.xyz/gtvemffdli.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhongyouzk.top/gtqfbfaknq.html

[N11] 二叉树中序遍历
来源：http://hz.zdqjudy.top/gtzrwxcsst.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cucudq.cn/gtqvvpmvti.html

PHP:  // 手写递归函数
来源：http://hz.snrcjt.cn/gtornvtycy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.316326.xyz/gtpknhdqqi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj20258.top/gtcvfvxgyi.html

Java: // 手写递归
来源：http://hz.pengpengdd.cyou/gtowmqnpex.html

Go:   // 手写递归
来源：http://hz.316326.xyz/gthwtfpdmt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.pengpengdd.cyou/gtntojywob.html

C#:   // 手写递归
来源：http://hz.gogol.net.cn/gtquwrfqci.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.guannengcc.top/gtbjrhdlwx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.dianchejie.cn/gtctrybzke.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sysykeji.top/gtoesxfzdp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cucudq.cn/gtxrkjlfnd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.feifeiyinyue.top/gtsbjteiem.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.iojbl.cn/gtnhpybmfw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.meibo888.top/gtvsdhzwnp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhixingplan.top/gtiokjjqny.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tanke756.top/gtsiweucbq.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtjhxmxqzx.html

O. 并发与异步
来源：http://hz.hongshengwenyu.top/gtucsusezy.html

================================================================================
来源：http://hz.tian-w.cn/gtozwexblu.html

[O01] 启动一个线程
来源：http://hz.quarkkingdee.top/gtqwoxhtnx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hfpthk.cn/gtibugegkt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gogol.net.cn/gtzxhxxaxn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.aizwys.cn/gtqneguprr.html

TS:   // 同 JS
来源：http://hz.chenzaomai.com/gtmxcxbuzm.html

Java: new Thread(() -> f()).start()
来源：http://hz.gotoacloud.top/gtodnhvshf.html

Go:   go f()
来源：http://hz.yueranfly.top/gtskugfqas.html

Ruby: Thread.new { f }
来源：http://hz.cucudq.cn/gtgfmzgead.html

C#:   Task.Run(() => F());
来源：http://hz.kuanghao11.cn/gtbnaovvic.html

[O02] 使用线程池
来源：http://hz.ydzc1.top/gtfbtzrmdw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yonumen.top/gtknwdhmra.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.fengsongda.top/gtkytjpcpi.html

JS:   // worker_threads 线程池
来源：http://hz.zhixingplan.top/gthncideju.html

TS:   // worker_threads 线程池
来源：http://hz.aizwys.cn/gtdzbwzdhc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cucudq.cn/gtruzlejsu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.tianlin.xyz/gtpvrdixjz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhaomingkeji.xyz/gtpjkfkvhk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhongyouzk.top/gttimvjxrw.html

[O03] 加锁保护共享数据
来源：http://hz.tianlin.xyz/gtobpspaex.html

Py:   with lock: shared += 1
来源：http://hz.svipenyu.cn/gtzkzvugwr.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yuxming.cn/gttcxjjnkv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.nanxuanxn.top/gtkjruoefq.html

TS:   // 同 JS
来源：http://hz.hnqzz.top/gtjpgtwlvy.html

Java: synchronized (this) { shared++; }
来源：http://hz.ehwqpu.com/gtlmfjtzhm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gotoacloud.top/gtawynlrzt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.wangdashe.top/gtqrmzeowx.html

C#:   lock (gate) { shared++; }
来源：http://hz.daria6918.cn/gtlymwapwt.html

[O04] 定义异步函数并等待
来源：http://hz.52xcode.cn/gtvddacren.html

Py:   async def f():⏎    await g()
来源：http://hz.aibaodan.cn/gtymtdgjqb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.feifeiyinyue.top/gtrextqwxu.html

JS:   async function f() { await g(); }
来源：http://hz.pycfn.com/gtegpnbzzu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.sufxvd.cn/gtwcxzboag.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cheryme.top/gtfvjzbail.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hnxiangtu.top/gtemxypney.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.meibo888.top/gtijzxjjim.html

C#:   async Task F() { await G(); }
来源：http://hz.ivvv.top/gtncwgmidy.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj20258.top/gtibdutbky.html

Py:   asyncio.gather(*tasks)
来源：http://hz.kuanghao11.cn/gttfvqnzwv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jiagoushi.top/gtmsbqrjio.html

JS:   await Promise.all(tasks)
来源：http://hz.wangdashe.top/gtpqpevhcs.html

TS:   await Promise.all(tasks)
来源：http://hz.xylfe.cn/gtejvwwyks.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinghuilouyu.cn/gteayrumxq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.snrcjt.cn/gtfnimzipi.html

Ruby: threads.map(&:join)
来源：http://hz.vqdsnc.cn/gtfocigjxw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.gaohongyu789.top/gttpiqxbau.html

[O06] 使用进程池
来源：http://hz.cashguo.top/gtzecpingk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.feifeiyinyue.top/gtovhfvmxn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yangfankeji.com/gthgaywfgz.html

JS:   // child_process / cluster 模块
来源：http://hz.cqqwz.cn/gtxpyrsssr.html

TS:   // child_process / cluster 模块
来源：http://hz.cqqwz.cn/gtrzjdljfs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cqqwz.cn/gttavgkrcv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nanxinkj.top/gtgtoqrome.html

Ruby: // fork 块
来源：http://hz.yuxming.cn/gthkovmsph.html

C#:   Parallel.For
来源：http://hz.zhijiandao.cn/gtbivwmvgq.html

================================================================================
来源：http://hz.hnxiangtu.top/gtlqsbukwz.html

P. 常用工具函数
来源：http://hz.ydjk.org.cn/gtwsyauvwo.html

================================================================================
来源：http://hz.hysaishi.cn/gtxsomvjgp.html

[P01] 生成 UUID
来源：http://hz.yvedp.cn/gtcflagvkc.html

Py:   str(uuid.uuid4())
来源：http://hz.guannengcc.top/gtbirvgeml.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.0kj1m.cn/gtsvwtpixe.html

JS:   crypto.randomUUID()
来源：http://hz.xingfuxueyuan.xyz/gtlmxsffnw.html

TS:   crypto.randomUUID()
来源：http://hz.zdqjudy.top/gtoncqzojr.html

Java: UUID.randomUUID().toString()
来源：http://hz.aibaodan.cn/gtbyqhnnmm.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jinqigufen.top/gtrsdnquml.html

Ruby: SecureRandom.uuid
来源：http://hz.shzxlz.cn/gtuabjnvdf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yuxming.cn/gtqlmgtpdv.html

[P02] MD5 / SHA256 摘要
来源：http://hz.9152youxi.cn/gtqyygahfe.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.pycfn.com/gtmccbutkf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jyoumei.cn/gtfleifnbq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.smart0.xyz/gtkxarhuhw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.havefunace.top/gtriwajcce.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cashguo.top/gtxrtpinok.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gzhubu.top/gtjmnvzbmy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yj20258888.top/gtajihkteg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhaomingkeji.xyz/gtvhdjgchn.html

[P03] 生成短随机字符串
来源：http://hz.gaohongyu789.top/gtfvllrdzs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zycfv.cn/gtmajulktr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xuetiantiany.cn/gtruhmbdfj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxuanxn.top/gtpvkbogvv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuetiantiany.cn/gtinqvjmtu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hnxiangtu.top/gtvpsfrzuo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ybcxt.top/gtdaycvzbg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sweek.top/gtldskscnd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.sxryk.cn/gtdfvcdtfu.html

[P04] 求长度
来源：http://hz.zhiwuduotai.top/gtgpljanyr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xuanzx.com/gtmigbxjai.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.dashuyun.cn/gtnejltdna.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.aizwys.cn/gtjgafxnch.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gzhubu.top/gtzzywevqk.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ydzc1.top/gtooomyxpa.html

Go:   len(arr);  len(m)
来源：http://hz.sxryk.cn/gtqjqhjbql.html

Ruby: x.length;  x.size
来源：http://hz.cheryme.top/gtfphcbtex.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ywan-chungtsiang.top/gtvtkelsow.html

[P05] 判断两个对象内容是否相等
来源：http://hz.52xcode.cn/gtevodtioq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhaomingkeji.xyz/gtkmytlsos.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sweek.top/gtmsdallle.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.sxryk.cn/gtzuhkwaxh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.bjfxy.top/gtoxvqscgp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.316326.xyz/gtmgpduyqm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.guannengcc.top/gtlmbkzghe.html

Ruby: a == b
来源：http://hz.52xcode.cn/gtqfhklfqh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.dianchejie.cn/gtkezgkvcr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.snrcjt.cn/gtohxpeuzn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jinqigfzy.top/gtyhvagvsc.html

PHP:  if (empty($x)) {}
来源：http://hz.jinqigufen.top/gtxiaahuft.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jyoumei.cn/gtylnojgcv.html

TS:   if (x == null) {}
来源：http://hz.vqdsnc.cn/gtroazzryg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jiagoushi.top/gtlxbppjrh.html

Go:   if x == nil {}
来源：http://hz.wangshuangyany.cn/gtlukowfau.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ywan-chungtsiang.top/gtauxjiytp.html

C#:   if (x is null) {}
来源：http://hz.snrcjt.cn/gtiyotcxju.html

[P07] 防抖与节流
来源：http://hz.hnqzz.top/gtzwyrlulx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yueranfly.top/gtyamotsfc.html

PHP:  // 手写时间戳比较
来源：http://hz.xingfuxueyuan.xyz/gtaolvulax.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnqzz.top/gtndofvvwj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nanxinkj.top/gtcmijfewa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.daxiang520.top/gtkmmlsgsd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.sysykeji.top/gtywywxinq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jinqigufen.top/gtpalecbpz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.vqdsnc.cn/gtzurfaxrs.html

[P08] 处理浮点精度问题
来源：http://hz.yj20258.top/gtbfewfkta.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cucudq.cn/gtnqfruagf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cheryme.top/gtgurbzjht.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.feifeiyinyue.top/gtcsbsuxye.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yanxiufei.cn/gtpumdjzsi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.pycfn.com/gtecigqmtf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yanxiufei.cn/gtixbiisnl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yj202588.top/gtzsoxengv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.guannengcc.top/gtbxvmkmzp.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtvqjtglwe.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xingfuxueyuan.xyz/gtrqdjemin.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtpjsgmyya.html

[Q01] 创建表
来源：http://hz.sweek.top/gtczvgbqlo.html

CREATE TABLE users (
来源：http://hz.jinqigfzy.top/gtktbqhcff.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xinyue.icu/gtqicuzyfl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shanyushiyangkeji.top/gtsiwwpebb.html

email VARCHAR(100) UNIQUE,
来源：http://hz.aizwys.cn/gtqozvrdrt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.52xcode.cn/gtapvesgew.html

);
来源：http://hz.meibo888.top/gtgkvdadtk.html

[Q02] 创建带外键的表
来源：http://hz.zhijiandao.cn/gtttoucqvf.html

CREATE TABLE orders (
来源：http://hz.ydzc1.top/gtumrnjovc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.c1oappe.top/gthgxqrmoo.html

user_id INT NOT NULL,
来源：http://hz.bjfxy.top/gtwurbebea.html

amount DECIMAL(10, 2),
来源：http://hz.guowangkeji.top/gtqolzmmtq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.andypj.xyz/gtqccaxxek.html

);
来源：http://hz.yuxming.cn/gtyaohggsf.html

[Q03] 增加列
来源：http://hz.chenjidiqi.icu/gtvysuvygk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.pengpengdd.cyou/gtgcquvhzy.html

[Q04] 修改列类型
来源：http://hz.smart0.xyz/gtntrklxjd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.dashuyun.cn/gtndgowuzf.html

[Q05] 重命名列
来源：http://hz.snrcjt.cn/gtpcohvuyw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jinghuilouyu.cn/gtxlvzwkma.html

[Q06] 删除列
来源：http://hz.daxiang520.top/gtwwsjnzoi.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.svipenyu.cn/gteijlsrrh.html

[Q07] 删除表
来源：http://hz.hammf.cn/gtfdjacqhv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xuanzx.com/gtzvlavqeh.html

[Q08] 创建普通索引
来源：http://hz.xuetiantiany.cn/gtbzryqvto.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.daria6918.cn/gtmpirstlw.html

[Q09] 创建唯一索引
来源：http://hz.zhijiandao.cn/gtuisfpobv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xuetiantiany.cn/gtrwtcibvs.html

[Q10] 插入单行
来源：http://hz.hywenlv.cn/gtewzvjial.html


<!-- 参考信息 -->