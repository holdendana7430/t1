代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gaohongyu789.top/gtdxlihhgz.html

Ruby: warn "err"
来源：http://hz.guannengcc.top/gtzubeoesl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ywan-chungtsiang.top/gtjkfrxxho.html

[M07] 判断是否为主入口
来源：http://hz.zhiwuduotai.top/gtovnlphfg.html

Py:   if __name__ == "__main__":
来源：http://hz.yj20258.top/gtwtdptoay.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhaomingkeji.xyz/gtidtnjdtw.html

JS:   require.main === module
来源：http://hz.zhixingplan.top/gtrratyvet.html

TS:   require.main === module
来源：http://hz.9152youxi.cn/gtemicibzf.html

Java: public static void main(String[] args)
来源：http://hz.yj202588.top/gthnvpxlxf.html

Go:   func main()
来源：http://hz.sufxvd.cn/gtzlgooqnj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yongpay.top/gtmakugkpg.html

C#:   static void Main(string[] args)
来源：http://hz.pengpengdd.cyou/gtxxytbdio.html

[M08] 获取系统与运行时信息
来源：http://hz.feifeiyinyue.top/gtnvoeuwhv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.316326.xyz/gtqvaomoau.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yanxiufei.cn/gthsqogbdr.html

JS:   process.platform;  process.version
来源：http://hz.birdmap.top/gtpynfckwr.html

TS:   process.platform;  process.version
来源：http://hz.feifeiyinyue.top/gtpzfdeifd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.redwolf501.top/gtedybqwhb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.kuanghao11.cn/gtyootpwxx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hywenlv.cn/gtsaykwcyo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.svipenyu.cn/gteoagnjky.html

================================================================================
来源：http://hz.yuxming.cn/gtgsvpcwkj.html

N. 数据结构与算法
来源：http://hz.quarkkingdee.top/gtcfodnmqa.html

================================================================================
来源：http://hz.aizwys.cn/gtswccyfpv.html

[N01] 二分查找（有序数组）
来源：http://hz.chenjidiqi.icu/gtjjxcqdvx.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sweek.top/gtfqoynjtz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yueranfly.top/gtnqjxnzgj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cashguo.top/gtuwyxdups.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.quarkkingdee.top/gtgpnedsem.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ppjwa.cn/gtingazanh.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.nanxinkj.top/gterqeqjut.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jyoumei.cn/gtgwhjokwt.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinqigufen.top/gtdkduqumi.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jiagoushi.top/gtszooqfck.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fengsongda.top/gtfsiepsua.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.chenzaomai.com/gtadkpnidy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhixingplan.top/gtqyfgdrmi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jiagoushi.top/gtbspfjoia.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jyoumei.cn/gtnusfwfct.html

Go:   slices.Sort(arr)
来源：http://hz.iojbl.cn/gtokhbcijp.html

Ruby: arr.sort
来源：http://hz.jinqigfzy.top/gtccmudagw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.haohaochexian.top/gttagtxwba.html

[N03] 快速排序（分治示例）
来源：http://hz.jqgfzy.top/gthciuavfk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.sysykeji.top/gtyckeigaa.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tanke756.top/gtieenchdx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.fengsongda.top/gtntwuavyz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgfzy.top/gtpvwuutpy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.haohaochexian.top/gtoaetfoio.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.gzhubu.top/gtdcflrxhy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.nanxuanxn.top/gtzctcuwrx.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ppjwa.cn/gtsnypxnly.html

[N04] 斐波那契数列
来源：http://hz.xuanzx.com/gtxkrykxaq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.kuanghao11.cn/gttmdyrqhj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.gogol.net.cn/gtvcfihvbt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xylfe.cn/gtqstdvete.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.52xcode.cn/gtskqytwhs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.tianlin.xyz/gtqhmgbdst.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yuanzhike.top/gtfdougyqd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhoulong.xyz/gtjyaemvqs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.bjfxy.top/gtxuntdjrw.html

[N05] 最大公约数
来源：http://hz.meibo888.top/gtinohrgyn.html

Py:   math.gcd(a, b)
来源：http://hz.yangfankeji.com/gtlqohvxme.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yj20258.top/gttqsomvcz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ivvv.top/gtydundcpm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zycfv.cn/gthkgladej.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.guowangkeji.top/gtnanfmlbe.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sufxvd.cn/gtebgkahzp.html

Ruby: a.gcd(b)
来源：http://hz.hysaishi.cn/gtgqrhlpho.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.redwolf501.top/gtzhgbrizf.html

[N06] 判断回文字符串
来源：http://hz.jinyuanbaomall.cn/gtaihujfwo.html

Py:   s == s[::-1]
来源：http://hz.jlsjyb.cn/gtcsghvrxk.html

PHP:  $s === strrev($s);
来源：http://hz.chenlongwang.top/gtqaxvfufy.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jiagoushi.top/gtgxowmldw.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtysripfnw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shanyushiyangkeji.top/gtircwxhpb.html

Go:   // 双指针从两端比较
来源：http://hz.yonumen.top/gtnjdlqbbe.html

Ruby: s == s.reverse
来源：http://hz.cdnleiting.top/gtmotntzgq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shangyingyoupin.top/gttxjmnouq.html

[N07] 两数之和（返回下标）
来源：http://hz.hnqzz.top/gtugihlijf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jiagoushi.top/gtdpbqdpan.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cdnleiting.top/gtxklighcz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhoulong.xyz/gtyirxwsmm.html

TS:   // 手写 Map<string, number>
来源：http://hz.zdqjudy.top/gtbpihpqoo.html

Java: // 手写 HashMap
来源：http://hz.gzhubu.top/gtsnxadkzq.html

Go:   // 手写 map[int]int
来源：http://hz.chenzaomai.com/gtpaxuwrll.html

Ruby: // 手写 Hash
来源：http://hz.9152youxi.cn/gtekvvvwbz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.nanxinkj.top/gtwomgtrwa.html

[N08] 生成全排列
来源：http://hz.c1oappe.top/gtpoawmgvv.html

Py:   itertools.permutations(arr)
来源：http://hz.ivvv.top/gtfzlydpii.html

PHP:  // 手写递归交换
来源：http://hz.ybcxt.top/gtrrmirfld.html

JS:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gteyxurpvw.html

TS:   // 手写回溯递归
来源：http://hz.jinqigufen.top/gtupvlpgzg.html

Java: // 手写回溯递归
来源：http://hz.bjfxy.top/gteglpgmwv.html

Go:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtlmvrmlah.html

Ruby: arr.permutation.to_a
来源：http://hz.feifeiyinyue.top/gtibavoory.html

C#:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtivzffycp.html

[N09] 栈与队列
来源：http://hz.nwbrower.top/gtzkxxtxqn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yuxming.cn/gtjjpfwlft.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ppjwa.cn/gtujjzofdh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhiwuduotai.top/gtotjxannp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.gotoacloud.top/gtkqdurfdg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.smart0.xyz/gtqphwcpxj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yj20258.top/gtkemiffuh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.nanxuanxn.top/gtyhkegczo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.aizwys.cn/gtforxsiks.html

[N10] 链表节点定义
来源：http://hz.jinyuanbaomall.cn/gtbalavvyt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.daria6918.cn/gtprehhyfy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.kuanghao11.cn/gtntcwsvyi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ehwqpu.com/gtpobfnsos.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jyoumei.cn/gtxfgdxjht.html

Java: class Node { int v; Node next; }
来源：http://hz.cashguo.top/gtzcbjyngs.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.andypj.xyz/gtvfjipyhx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.chenzaomai.com/gtjuftjhvo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shangyingyoupin.top/gtnitonoaw.html

[N11] 二叉树中序遍历
来源：http://hz.yj20258.top/gtprwcqxrp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.svipenyu.cn/gtavkjwqmp.html

PHP:  // 手写递归函数
来源：http://hz.ivvv.top/gtiwatijtq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sweek.top/gtokxyjlqz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jyoumei.cn/gttvkpeddv.html

Java: // 手写递归
来源：http://hz.yonumen.top/gtnvrvliyl.html

Go:   // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtqaoxymvg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.nanxuanxn.top/gticalwwmo.html

C#:   // 手写递归
来源：http://hz.cucudq.cn/gtpeztxnxe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinyuanbaomall.cn/gthwlumehk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.kuanghao11.cn/gtaqlnvghz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xuanzx.com/gtswijkmgk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.svipenyu.cn/gtmjveeoug.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhiwuduotai.top/gtlopmadml.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gtdvuybiye.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ivvv.top/gtszsokwug.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.wangdashe.top/gtfehyzirz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.snrcjt.cn/gtciddqumc.html

================================================================================
来源：http://hz.zhongyouzk.top/gtdxrvilim.html

O. 并发与异步
来源：http://hz.chenjidiqi.icu/gtgsgidhpf.html

================================================================================
来源：http://hz.dashuyun.cn/gtkxtiaszo.html

[O01] 启动一个线程
来源：http://hz.jiagoushi.top/gtsbrfuilj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yongpay.top/gtnogiudzt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cqqwz.cn/gtpkcrjomw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jianghu66.top/gtnyjzulzg.html

TS:   // 同 JS
来源：http://hz.gzhubu.top/gtgezdaaha.html

Java: new Thread(() -> f()).start()
来源：http://hz.quarkkingdee.top/gtlzfxksyb.html

Go:   go f()
来源：http://hz.0kj1m.cn/gthldzylud.html

Ruby: Thread.new { f }
来源：http://hz.guowangkeji.top/gtcmmmfelf.html

C#:   Task.Run(() => F());
来源：http://hz.shzxlz.cn/gteqfjsubl.html

[O02] 使用线程池
来源：http://hz.shanyushiyangtech.top/gtblwydrmr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.guowangkeji.top/gtkdxwcmxp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jqgufenzy.top/gtjwopsmdd.html

JS:   // worker_threads 线程池
来源：http://hz.guowangkeji.top/gtyhfypfsj.html

TS:   // worker_threads 线程池
来源：http://hz.quarkkingdee.top/gtuarnoanz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.pengpengdd.cyou/gtmmqvhvfs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.pengpengdd.cyou/gtbzlrmggn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xylfe.cn/gtbhrnedgc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gogol.net.cn/gtrumcyfqa.html

[O03] 加锁保护共享数据
来源：http://hz.yj20258.top/gthqbezqpu.html

Py:   with lock: shared += 1
来源：http://hz.ywan-chungtsiang.top/gtmpjaxcwg.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.smart0.xyz/gtlutfrfzk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shuidangran.top/gtbatxwqkh.html

TS:   // 同 JS
来源：http://hz.guowangkeji.top/gtbawkhlfi.html

Java: synchronized (this) { shared++; }
来源：http://hz.andypj.xyz/gtubvyxtbv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.wangdashe.top/gtzdopsnim.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cheryme.top/gtjlnecokp.html

C#:   lock (gate) { shared++; }
来源：http://hz.feifeiyinyue.top/gtuoqimcfx.html

[O04] 定义异步函数并等待
来源：http://hz.pengpengdd.cyou/gtguuxixnk.html

Py:   async def f():⏎    await g()
来源：http://hz.zhongyouzk.top/gtqrduyimb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.52xcode.cn/gtuvyuqkwy.html

JS:   async function f() { await g(); }
来源：http://hz.quarkkingdee.top/gtmwggyrwr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.tanke756.top/gtytcoxusx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhaomingkeji.xyz/gtrwadgjnc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yuxming.cn/gtwequcmua.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ehwqpu.com/gtxgqlntcz.html

C#:   async Task F() { await G(); }
来源：http://hz.xziqi.cn/gtpsnhktjz.html

[O05] 并发执行并等待全部完成
来源：http://hz.shuidangran.top/gtqxzyjmsl.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenlongwang.top/gtwghtozkq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zycfv.cn/gtbntfasrl.html

JS:   await Promise.all(tasks)
来源：http://hz.pycfn.com/gtimkchlkz.html

TS:   await Promise.all(tasks)
来源：http://hz.zhixingplan.top/gtkqiwokfi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.haohaochexian.top/gtdqjmcisp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cucudq.cn/gtsdmrwouc.html

Ruby: threads.map(&:join)
来源：http://hz.yonumen.top/gtiehjbvxi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.andypj.xyz/gtmiznwoci.html

[O06] 使用进程池
来源：http://hz.kuanghao11.cn/gterylzugj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jyoumei.cn/gtrdirjbej.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ivvv.top/gtfjzsvvfv.html

JS:   // child_process / cluster 模块
来源：http://hz.cqqwz.cn/gtwhsvmpkb.html

TS:   // child_process / cluster 模块
来源：http://hz.zhijiandao.cn/gthrptqvqy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sufxvd.cn/gtvzhgorrl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.redwolf501.top/gtlhypxtic.html

Ruby: // fork 块
来源：http://hz.sufxvd.cn/gtwyhnhygv.html

C#:   Parallel.For
来源：http://hz.cucudq.cn/gtzwwgnbsf.html

================================================================================
来源：http://hz.aibaodan.cn/gtuiezbizg.html

P. 常用工具函数
来源：http://hz.zhixingplan.top/gtivxkkqgd.html

================================================================================
来源：http://hz.cqqwz.cn/gtslyxqidf.html

[P01] 生成 UUID
来源：http://hz.ywan-chungtsiang.top/gtdwsxhtdc.html

Py:   str(uuid.uuid4())
来源：http://hz.0kj1m.cn/gtbcumxnqg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sysykeji.top/gtfxkixebt.html

JS:   crypto.randomUUID()
来源：http://hz.yj20258888.top/gtkgjzbkof.html

TS:   crypto.randomUUID()
来源：http://hz.hysaishi.cn/gtoeilkwcl.html

Java: UUID.randomUUID().toString()
来源：http://hz.yvedp.cn/gtqxfkhiio.html

Go:   // 用 github.com/google/uuid
来源：http://hz.c1oappe.top/gtrzpqnhbl.html

Ruby: SecureRandom.uuid
来源：http://hz.52xcode.cn/gtnjafienw.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ehwqpu.com/gtekzbzkxs.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yongpay.top/gtwveuffol.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.andypj.xyz/gtrjuhpwig.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhaomingkeji.xyz/gtbuegsztb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhaomingkeji.xyz/gtvnzrxuox.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yueranfly.top/gtkkbwhcwf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xziqi.cn/gtvugrakha.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ywan-chungtsiang.top/gtzrsinfhe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sufxvd.cn/gtrhlgdbll.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.mhx1999.top/gtffqgecyw.html

[P03] 生成短随机字符串
来源：http://hz.zhoulong.xyz/gtfsganzzj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.quarkkingdee.top/gttenxrmdk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ppjwa.cn/gtgkkwrylj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cqqwz.cn/gtfttlvtcf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.svipenyu.cn/gtawjopsuu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ehwqpu.com/gtyxphymuv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.gaohongyu789.top/gtlgjfnllx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cucudq.cn/gtdcmcxtjw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gaohongyu789.top/gtbrrjdufv.html

[P04] 求长度
来源：http://hz.aizwys.cn/gtvbfabrqb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xziqi.cn/gtczljzcaj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shangyingyoupin.top/gtocxkdxde.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nwbrower.top/gtqcvjojjj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cashguo.top/gtsypqqnhh.html

Java: list.size();  map.size();  s.length()
来源：http://hz.fzhhl.top/gtntzdmics.html

Go:   len(arr);  len(m)
来源：http://hz.sxryk.cn/gtgfgoimeh.html

Ruby: x.length;  x.size
来源：http://hz.zhiwuduotai.top/gtzspeoybz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.nwbrower.top/gthuohljae.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xziqi.cn/gtbpfxlzvt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yongpay.top/gtchlqmyfc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.wangdashe.top/gtalclment.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.pengpengdd.cyou/gtzdhjgtxf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgfzy.top/gtrcgbthop.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhoulong.xyz/gtsqoicdjx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhixingplan.top/gtldzqqurp.html

Ruby: a == b
来源：http://hz.gaohongyu789.top/gtvjtyffmv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.wangshuangyany.cn/gteipmzwlj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jinqigfzy.top/gtyzoskqlk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.chenzaomai.com/gtccytgywt.html

PHP:  if (empty($x)) {}
来源：http://hz.cdnleiting.top/gthezxwqrq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.0kj1m.cn/gtvchfnlfe.html

TS:   if (x == null) {}
来源：http://hz.birdmap.top/gtxtdhwcvk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yj20258888.top/gtdfedksww.html

Go:   if x == nil {}
来源：http://hz.mhx1999.top/gtjvqvizll.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.fzhhl.top/gtfjfbjdej.html

C#:   if (x is null) {}
来源：http://hz.shzxlz.cn/gtmshzlrlo.html

[P07] 防抖与节流
来源：http://hz.dianchejie.cn/gtlcrirsue.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.meibo888.top/gtbexfkhrv.html

PHP:  // 手写时间戳比较
来源：http://hz.jlsjyb.cn/gtbfpcbwbk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yangfankeji.com/gtuoldqbrw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guannengcc.top/gtowwojlss.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.0kj1m.cn/gtoejxohwu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xziqi.cn/gtuvtdoawk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xylfe.cn/gtuasngebc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.meibo888.top/gtudxbvoww.html

[P08] 处理浮点精度问题
来源：http://hz.zhiwuduotai.top/gtqptsiucv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.pycfn.com/gtnrdqusoo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.dashuyun.cn/gtwltbnwfg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jyoumei.cn/gtqjcbkgda.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.0kj1m.cn/gtpniqbyss.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yanxiufei.cn/gterzzhofk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.wangshuangyany.cn/gtndjcqcmf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhongyouzk.top/gtusjpsxln.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.pycfn.com/gtomnwujdl.html

================================================================================
来源：http://hz.yueranfly.top/gtdsyegvdy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yueranfly.top/gtpbatxidc.html

================================================================================
来源：http://hz.aibaodan.cn/gtwcoplghw.html

[Q01] 创建表
来源：http://hz.ywan-chungtsiang.top/gthhlndkoq.html

CREATE TABLE users (
来源：http://hz.jlsjyb.cn/gtldtyvyxf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxinkj.top/gtypmziljk.html

name VARCHAR(50) NOT NULL,
来源：http://hz.pycfn.com/gtousfczqy.html

email VARCHAR(100) UNIQUE,
来源：http://hz.dashuyun.cn/gtnusexorz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xuetiantiany.cn/gtxmmxllze.html

);
来源：http://hz.jinqigfzy.top/gtbmxeahks.html

[Q02] 创建带外键的表
来源：http://hz.gzhubu.top/gttfcmdvgw.html

CREATE TABLE orders (
来源：http://hz.tian-w.cn/gtlsskchlq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zycfv.cn/gtimtshooh.html

user_id INT NOT NULL,
来源：http://hz.zhiwuduotai.top/gtjbyyzjzo.html

amount DECIMAL(10, 2),
来源：http://hz.jinqigfzy.top/gtkdrkpbbv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinghuilouyu.cn/gtcpwtfmav.html

);
来源：http://hz.zhaomingkeji.xyz/gtsgquekpq.html

[Q03] 增加列
来源：http://hz.9152youxi.cn/gtiqbvhwkk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinyuanbaomall.cn/gtzeeynfvy.html

[Q04] 修改列类型
来源：http://hz.aizwys.cn/gtrthjpona.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.c1oappe.top/gtndldokdu.html

[Q05] 重命名列
来源：http://hz.gogol.net.cn/gtolrsvfpn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hysaishi.cn/gtsqmowbzj.html

[Q06] 删除列
来源：http://hz.tian-w.cn/gtwnxqqeel.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ehwqpu.com/gtaxqdqpzb.html

[Q07] 删除表
来源：http://hz.cucudq.cn/gtqxuovjde.html

DROP TABLE IF EXISTS orders;
来源：http://hz.smart0.xyz/gtvispbgqd.html

[Q08] 创建普通索引
来源：http://hz.snrcjt.cn/gtmoilvfum.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.birdmap.top/gthztojdyn.html

[Q09] 创建唯一索引
来源：http://hz.redwolf501.top/gtrfvubdli.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zycfv.cn/gthzysiaya.html

[Q10] 插入单行
来源：http://hz.vqdsnc.cn/gtobbpohwh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.quarkkingdee.top/gtqxgqwdre.html

[Q11] 一次插入多行
来源：http://hz.ivvv.top/gtunbtmnge.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.birdmap.top/gtovxpzvij.html

[Q12] 插入后取自增 ID
来源：http://hz.xziqi.cn/gtnkuuabtm.html


<!-- 参考信息 -->