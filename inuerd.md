代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.pycfn.com/gtqnmednrd.html

Ruby: warn "err"
来源：http://hz.quarkkingdee.top/gtlrnaoisy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ydjk.org.cn/gtvhbjifra.html

[M07] 判断是否为主入口
来源：http://hz.yuxming.cn/gtuqolnmdj.html

Py:   if __name__ == "__main__":
来源：http://hz.bjfxy.top/gtzeucwitd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cheryme.top/gtxhbzeutl.html

JS:   require.main === module
来源：http://hz.aibaodan.cn/gtfqyzytto.html

TS:   require.main === module
来源：http://hz.jinqigufen.top/gtmytkvgws.html

Java: public static void main(String[] args)
来源：http://hz.yuanzhike.top/gttglbvppx.html

Go:   func main()
来源：http://hz.jinghuilouyu.cn/gtioxrxsgw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.dianchejie.cn/gtgoonygrr.html

C#:   static void Main(string[] args)
来源：http://hz.gaohongyu789.top/gtrommpykk.html

[M08] 获取系统与运行时信息
来源：http://hz.gotoacloud.top/gtooaolqkr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhiwuduotai.top/gtbmlckstq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ivvv.top/gtxujqaoko.html

JS:   process.platform;  process.version
来源：http://hz.haohaochexian.top/gtfjremiga.html

TS:   process.platform;  process.version
来源：http://hz.zhaomingkeji.xyz/gtezhjxipp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.chenjidiqi.icu/gtfwnsuumo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gotoacloud.top/gtgnvcedqx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.birdmap.top/gtgljsjptr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cashguo.top/gtzoenzifp.html

================================================================================
来源：http://hz.bjfxy.top/gtjkobuygb.html

N. 数据结构与算法
来源：http://hz.nwbrower.top/gtdseythxm.html

================================================================================
来源：http://hz.sysykeji.top/gtphgwgzuv.html

[N01] 二分查找（有序数组）
来源：http://hz.xuetiantiany.cn/gtmdldklog.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nanxinkj.top/gtazqcvmbb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jqgfzy.top/gtbkbebgrp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.bjfxy.top/gtomqztaot.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shanyushiyangtech.top/gtevmupsrn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.vqdsnc.cn/gtinxurrht.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yj20258888.top/gttzuqfmfl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ydzc1.top/gtgtvjgzyg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gtvmtokpyv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.dianchejie.cn/gtsahqdlth.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.haohaochexian.top/gtokssoqhn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nwbrower.top/gtvruhhivb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.pycfn.com/gtqnpuzwwy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.smart0.xyz/gtnnqmisdj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hnqzz.top/gtyqpgcjin.html

Go:   slices.Sort(arr)
来源：http://hz.ybcxt.top/gtdndpdnef.html

Ruby: arr.sort
来源：http://hz.quarkkingdee.top/gtprjchoye.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ywan-chungtsiang.top/gtkqlgwdhc.html

[N03] 快速排序（分治示例）
来源：http://hz.zycfv.cn/gtnjyfnfrh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinyuanbaomall.cn/gtxeurkrhi.html

PHP:  // 递归实现，或用 usort
来源：http://hz.dashuyun.cn/gtjixdbckt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgufenzy.top/gtnamvogdn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.havefunace.top/gthubhvxdd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.haohaochexian.top/gtditwgxuh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ppjwa.cn/gtukgaeizf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.quarkkingdee.top/gtgftacsat.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shanyushiyangkeji.top/gtlysvjtkk.html

[N04] 斐波那契数列
来源：http://hz.zhijiandao.cn/gtdxtzixlz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.snrcjt.cn/gtfnbbetlk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinghuilouyu.cn/gtvrrkvmmt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xuetiantiany.cn/gtbuuqlbce.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gogol.net.cn/gtbspusvrb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.smart0.xyz/gtsnluyicm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.c1oappe.top/gtaikorcka.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ivvv.top/gtzgrmnrpw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yvedp.cn/gtznunbutz.html

[N05] 最大公约数
来源：http://hz.jinyuanbaomall.cn/gtgjceotgj.html

Py:   math.gcd(a, b)
来源：http://hz.hongshengwenyu.top/gtlwqbqfin.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hongshengwenyu.top/gtrwjmkyyi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangtech.top/gtzxcyuovf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pengpengdd.cyou/gtipeqwcpq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cashguo.top/gtlrahcfjt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.0kj1m.cn/gtypcqnzbl.html

Ruby: a.gcd(b)
来源：http://hz.sweek.top/gtgmpmksbg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yj20258.top/gtrbislvvv.html

[N06] 判断回文字符串
来源：http://hz.sufxvd.cn/gtxusfvchv.html

Py:   s == s[::-1]
来源：http://hz.daria6918.cn/gtwyckkigf.html

PHP:  $s === strrev($s);
来源：http://hz.zhixingplan.top/gtbaoqvjmm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cheryme.top/gtvlaweviy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.wangdashe.top/gtkrdsvxxw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zdqjudy.top/gtigoqbure.html

Go:   // 双指针从两端比较
来源：http://hz.gaohongyu789.top/gtshaoiihb.html

Ruby: s == s.reverse
来源：http://hz.xingfuxueyuan.xyz/gtkhhtcqui.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.sufxvd.cn/gttilqtjkj.html

[N07] 两数之和（返回下标）
来源：http://hz.zhixingplan.top/gtftfnnoax.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.mhx1999.top/gtngczattl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.aizwys.cn/gtavaswgvm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jlsjyb.cn/gtsjaerikm.html

TS:   // 手写 Map<string, number>
来源：http://hz.fzhhl.top/gtwoibtmhe.html

Java: // 手写 HashMap
来源：http://hz.zhiwuduotai.top/gtcptyzcpj.html

Go:   // 手写 map[int]int
来源：http://hz.ivvv.top/gtycnszodv.html

Ruby: // 手写 Hash
来源：http://hz.tian-w.cn/gtubhchyum.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shuidangran.top/gtccwnfpwk.html

[N08] 生成全排列
来源：http://hz.hywenlv.cn/gtilnoxjag.html

Py:   itertools.permutations(arr)
来源：http://hz.ybcxt.top/gtgosojrnu.html

PHP:  // 手写递归交换
来源：http://hz.cqqwz.cn/gtigbgmuhz.html

JS:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtcnhkvmtr.html

TS:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtzczbqgaq.html

Java: // 手写回溯递归
来源：http://hz.tianlin.xyz/gtgjlauhld.html

Go:   // 手写回溯递归
来源：http://hz.ydzc1.top/gtunalodqa.html

Ruby: arr.permutation.to_a
来源：http://hz.aizwys.cn/gtvqccdghc.html

C#:   // 手写回溯递归
来源：http://hz.sysykeji.top/gtpxdpcunr.html

[N09] 栈与队列
来源：http://hz.ydzc1.top/gtavqotsjx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.guannengcc.top/gtbueuwivt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhengqikj.top/gtclqwguob.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.9152youxi.cn/gtlpibhlli.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhijiandao.cn/gtkkabmanm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.iojbl.cn/gtuhgyxplr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ybcxt.top/gtxagjwavm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhengqikj.top/gtoxvvehdl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.9152youxi.cn/gtgfzizjos.html

[N10] 链表节点定义
来源：http://hz.ywan-chungtsiang.top/gtjjyltwmt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.chenlongwang.top/gtooteeief.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhaomingkeji.xyz/gtbcerqjxi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xziqi.cn/gtvkphdbyy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cheryme.top/gtgaitikzh.html

Java: class Node { int v; Node next; }
来源：http://hz.aibaodan.cn/gtbxmajzgd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ydzc1.top/gtplwqdeft.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.chenjidiqi.icu/gtgegzxxsv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nanxinkj.top/gtfnbebijr.html

[N11] 二叉树中序遍历
来源：http://hz.jlsjyb.cn/gtnleltvfq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shangyingyoupin.top/gtkvpnzdtz.html

PHP:  // 手写递归函数
来源：http://hz.yanxiufei.cn/gtlkfthxrh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shanyushiyangkeji.top/gtqtrmuukm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.meibo888.top/gttyzmsnei.html

Java: // 手写递归
来源：http://hz.hammf.cn/gtroaptfye.html

Go:   // 手写递归
来源：http://hz.zhengqikj.top/gtbarmzncl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.chenzaomai.com/gtfjvyliwq.html

C#:   // 手写递归
来源：http://hz.wangshuangyany.cn/gtzfreltea.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yvedp.cn/gtrqorteih.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hysaishi.cn/gtetjqrnbs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sufxvd.cn/gtokiqdgai.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.mhx1999.top/gtokrplfoo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhixingplan.top/gtcktlmygd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xylfe.cn/gtcgkdscqk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.guowangkeji.top/gtuxlnhwkj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinqigfzy.top/gteoesveoc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenjidiqi.icu/gtoiideiex.html

================================================================================
来源：http://hz.bjfxy.top/gtqniazzva.html

O. 并发与异步
来源：http://hz.hywenlv.cn/gtbxikdjux.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtpamsbwbs.html

[O01] 启动一个线程
来源：http://hz.cucudq.cn/gtxywnwurj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gogol.net.cn/gtnraeoyzo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.iojbl.cn/gtopgemwbd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jinghuilouyu.cn/gtidksgahn.html

TS:   // 同 JS
来源：http://hz.hammf.cn/gtbsrcoegu.html

Java: new Thread(() -> f()).start()
来源：http://hz.gzhubu.top/gttiqgdsow.html

Go:   go f()
来源：http://hz.gotoacloud.top/gtwehlfgmg.html

Ruby: Thread.new { f }
来源：http://hz.ydzc1.top/gtgskgnxdq.html

C#:   Task.Run(() => F());
来源：http://hz.cashguo.top/gtgsevhcum.html

[O02] 使用线程池
来源：http://hz.dianchejie.cn/gtvnfuymjv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.wangdashe.top/gtqhrwybig.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhiwuduotai.top/gtpimkzmio.html

JS:   // worker_threads 线程池
来源：http://hz.yuanzhike.top/gtgfqzkmvi.html

TS:   // worker_threads 线程池
来源：http://hz.pengpengdd.cyou/gtkshbykvu.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.chenlongwang.top/gtzniwvsyi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.guannengcc.top/gtfsubbbad.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yuanzhike.top/gtdghubesz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.guannengcc.top/gtxrwqtlbz.html

[O03] 加锁保护共享数据
来源：http://hz.jqgfzy.top/gtetexfhug.html

Py:   with lock: shared += 1
来源：http://hz.yangfankeji.com/gttlvgurmb.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhijiandao.cn/gtpthuwoxu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.meibo888.top/gtayivtppv.html

TS:   // 同 JS
来源：http://hz.snrcjt.cn/gtzaxtbhmi.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhaomingkeji.xyz/gtbwxxkitg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yuxming.cn/gtzfszavxg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.aibaodan.cn/gtbnktekmm.html

C#:   lock (gate) { shared++; }
来源：http://hz.shzxlz.cn/gtrrjpxmns.html

[O04] 定义异步函数并等待
来源：http://hz.yanxiufei.cn/gtcwcetfrf.html

Py:   async def f():⏎    await g()
来源：http://hz.jinqigfzy.top/gteqdsqaup.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nwbrower.top/gtfbvhkobb.html

JS:   async function f() { await g(); }
来源：http://hz.cashguo.top/gteformyqb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.sysykeji.top/gtdanbyixj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhoulong.xyz/gttjlhedkx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhixingplan.top/gtugntbkhs.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.52xcode.cn/gtvkbkxeoe.html

C#:   async Task F() { await G(); }
来源：http://hz.jyoumei.cn/gtdnhysrik.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinqigufen.top/gtghskgjoa.html

Py:   asyncio.gather(*tasks)
来源：http://hz.svipenyu.cn/gtvcwwcqpp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hongshengwenyu.top/gttxmowytg.html

JS:   await Promise.all(tasks)
来源：http://hz.hammf.cn/gtqmkplztf.html

TS:   await Promise.all(tasks)
来源：http://hz.bjfxy.top/gtmectwgva.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jiagoushi.top/gtkxzcsykc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.nanxuanxn.top/gtiekizhvu.html

Ruby: threads.map(&:join)
来源：http://hz.0kj1m.cn/gtnrdbhsoh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hnqzz.top/gtpmewacjq.html

[O06] 使用进程池
来源：http://hz.smart0.xyz/gtrrsoblwi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.tian-w.cn/gtzwaiaxzo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hywenlv.cn/gtttaghlck.html

JS:   // child_process / cluster 模块
来源：http://hz.0kj1m.cn/gttdjjatyf.html

TS:   // child_process / cluster 模块
来源：http://hz.yuxming.cn/gtuvkknipu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhoulong.xyz/gtvhcuhptc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.chenjidiqi.icu/gtneizuaas.html

Ruby: // fork 块
来源：http://hz.shuidangran.top/gtdzhfyfcn.html

C#:   Parallel.For
来源：http://hz.vqdsnc.cn/gtjagcllib.html

================================================================================
来源：http://hz.cdnleiting.top/gtgmkzpyel.html

P. 常用工具函数
来源：http://hz.zycfv.cn/gtpeyvataa.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtzmhiteyx.html

[P01] 生成 UUID
来源：http://hz.ivvv.top/gtzpdpiaxn.html

Py:   str(uuid.uuid4())
来源：http://hz.yj20258.top/gtvwpkakgi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.0kj1m.cn/gtyzrexzef.html

JS:   crypto.randomUUID()
来源：http://hz.pengpengdd.cyou/gtoacebipw.html

TS:   crypto.randomUUID()
来源：http://hz.ydjk.org.cn/gtysdsiatq.html

Java: UUID.randomUUID().toString()
来源：http://hz.wangshuangyany.cn/gtykbossbr.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hongshengwenyu.top/gttgxjukzq.html

Ruby: SecureRandom.uuid
来源：http://hz.hnxiangtu.top/gtrffxngne.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenjidiqi.icu/gtuqerkiog.html

[P02] MD5 / SHA256 摘要
来源：http://hz.mhx1999.top/gtyxlqnkki.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ydzc1.top/gtqylrtviq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.snrcjt.cn/gtvslhicti.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.iojbl.cn/gttbzwdiqo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xingfuxueyuan.xyz/gtywhvzlfq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj20258.top/gtbkpyrpse.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shuidangran.top/gttsthfkka.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cheryme.top/gtutmkyxxh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yonumen.top/gtotrueklm.html

[P03] 生成短随机字符串
来源：http://hz.wangdashe.top/gtprvoipyk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gaohongyu789.top/gtjrpxpybm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yonumen.top/gtjrzumyve.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yangfankeji.com/gtoobeutas.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenjidiqi.icu/gthlcsfocx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.andypj.xyz/gtfyrcdwum.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.wangshuangyany.cn/gtqnzcyfnv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jiagoushi.top/gtsstgyjve.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ehwqpu.com/gtfclcqebo.html

[P04] 求长度
来源：http://hz.hnxiangtu.top/gtzyevchmw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.daria6918.cn/gtzuyykbmg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tian-w.cn/gtjqgeynii.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gotoacloud.top/gtlxsdtyeg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xziqi.cn/gtmdsdvmes.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xinyue.icu/gtflfwyrep.html

Go:   len(arr);  len(m)
来源：http://hz.gotoacloud.top/gtqzvzxkqc.html

Ruby: x.length;  x.size
来源：http://hz.yonumen.top/gtkdivtqvp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhaomingkeji.xyz/gtuyydzfzp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yj20258.top/gtiupwzzdv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tanke756.top/gtjilxtcqq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xingfuxueyuan.xyz/gtrmlvvnki.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.gzhubu.top/gtgvijsfip.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hongshengwenyu.top/gtfnhjvwgf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinyuanbaomall.cn/gtmvwurgyv.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jlsjyb.cn/gtchfmcnwu.html

Ruby: a == b
来源：http://hz.sweek.top/gtawsixtbb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yangfankeji.com/gtshmubpsu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.snrcjt.cn/gthmgqpijn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.meibo888.top/gtrmccqkme.html

PHP:  if (empty($x)) {}
来源：http://hz.xuanzx.com/gtvuoxkqin.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yj20258.top/gtfcvqvyhf.html

TS:   if (x == null) {}
来源：http://hz.zhaomingkeji.xyz/gtrtgyshld.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.wangshuangyany.cn/gtwucxbcvk.html

Go:   if x == nil {}
来源：http://hz.9152youxi.cn/gtmatbswkt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.gogol.net.cn/gtgjdbvixn.html

C#:   if (x is null) {}
来源：http://hz.snrcjt.cn/gtsfazcmbb.html

[P07] 防抖与节流
来源：http://hz.meibo888.top/gtdusvvxsb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xylfe.cn/gtptmunrbn.html

PHP:  // 手写时间戳比较
来源：http://hz.xylfe.cn/gtbokqbrsd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.316326.xyz/gtqnsukkxh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gaohongyu789.top/gttpqyujsr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shanyushiyangkeji.top/gtrjnvpkqq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhixingplan.top/gtvwhrumel.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yj20258888.top/gtgaghfjjm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.snrcjt.cn/gtsnrrtuea.html

[P08] 处理浮点精度问题
来源：http://hz.hnqzz.top/gtmvykiyvi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.vqdsnc.cn/gtsmcnlolo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ehwqpu.com/gtekwwkfcc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.c1oappe.top/gtqjlcyicx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.bjfxy.top/gtcffxxrtb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ydzc1.top/gtgrloqlob.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.wangdashe.top/gtywoeehrw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.haohaochexian.top/gtrrvbjcvi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.meibo888.top/gtvexzhnxx.html

================================================================================
来源：http://hz.tanke756.top/gtrdpheohf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.wangdashe.top/gtiijsbehz.html

================================================================================
来源：http://hz.aibaodan.cn/gtuqazlplz.html

[Q01] 创建表
来源：http://hz.cucudq.cn/gtvjzosrzm.html

CREATE TABLE users (
来源：http://hz.xylfe.cn/gthcegwsgr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.iojbl.cn/gtrdwgcexh.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hammf.cn/gtrlhazrrf.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhengqikj.top/gtgwdblzyf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.nwbrower.top/gtvvtgqogc.html

);
来源：http://hz.ywan-chungtsiang.top/gtzlxpchld.html

[Q02] 创建带外键的表
来源：http://hz.aizwys.cn/gtyvnumzmj.html

CREATE TABLE orders (
来源：http://hz.sweek.top/gtwedzcjcz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xingfuxueyuan.xyz/gtolgmxvpp.html

user_id INT NOT NULL,
来源：http://hz.gaohongyu789.top/gtooztdmqp.html

amount DECIMAL(10, 2),
来源：http://hz.hongshengwenyu.top/gtrbvgzlkt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.c1oappe.top/gtysjqxreo.html

);
来源：http://hz.yuanzhike.top/gtzvzlsywi.html

[Q03] 增加列
来源：http://hz.haohaochexian.top/gtsvybhhnm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.wangshuangyany.cn/gtzzavspin.html

[Q04] 修改列类型
来源：http://hz.chenzaomai.com/gtnecjcrjj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xuanzx.com/gthhxiybim.html

[Q05] 重命名列
来源：http://hz.yvedp.cn/gtjbjehbei.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.aibaodan.cn/gtsnhzijhx.html

[Q06] 删除列
来源：http://hz.jlsjyb.cn/gtaafptcgz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.birdmap.top/gtyoxqxelm.html

[Q07] 删除表
来源：http://hz.zdqjudy.top/gtkejirett.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shangyingyoupin.top/gtusirvysy.html

[Q08] 创建普通索引
来源：http://hz.hongshengwenyu.top/gtycrztxmy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hongshengwenyu.top/gtnvozcsua.html

[Q09] 创建唯一索引
来源：http://hz.zhengqikj.top/gtqqskifml.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.svipenyu.cn/gtusnkvonz.html

[Q10] 插入单行
来源：http://hz.cqqwz.cn/gtkrjfbiok.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shanyushiyangtech.top/gtvucxosdq.html

[Q11] 一次插入多行
来源：http://hz.quarkkingdee.top/gtkoajfxny.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.wangdashe.top/gtganvgkts.html

[Q12] 插入后取自增 ID
来源：http://hz.xuanzx.com/gtekojxnop.html


<!-- 参考信息 -->