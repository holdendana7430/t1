代发 wailian999

Py:   if __name__ == "__main__":
来源：http://hz.sufxvd.cn/gtyyrzqbhq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.52xcode.cn/gtrvzkyffb.html

JS:   require.main === module
来源：http://hz.yuanzhike.top/gtyktlozqa.html

TS:   require.main === module
来源：http://hz.jinyuanbaomall.cn/gtbcjwxkgr.html

Java: public static void main(String[] args)
来源：http://hz.cheryme.top/gtnwhzkhlh.html

Go:   func main()
来源：http://hz.yanxiufei.cn/gtcllgvmoj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yongpay.top/gtbnmaewff.html

C#:   static void Main(string[] args)
来源：http://hz.ywan-chungtsiang.top/gtxcslbewp.html

[M08] 获取系统与运行时信息
来源：http://hz.redwolf501.top/gtcwjuvniz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.tanke756.top/gtxsmxfcos.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.0kj1m.cn/gtwobyzyev.html

JS:   process.platform;  process.version
来源：http://hz.yvedp.cn/gtetmggxgv.html

TS:   process.platform;  process.version
来源：http://hz.pengpengdd.cyou/gtiwsitavg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shzxlz.cn/gtcumgevag.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.dianchejie.cn/gtjjlnujei.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ehwqpu.com/gthnwgaury.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xingfuxueyuan.xyz/gtacxuomje.html

================================================================================
来源：http://hz.hfpthk.cn/gtpafbxfet.html

N. 数据结构与算法
来源：http://hz.havefunace.top/gteippymkc.html

================================================================================
来源：http://hz.jyoumei.cn/gtfbpyuctr.html

[N01] 二分查找（有序数组）
来源：http://hz.hfpthk.cn/gtejfoxtbt.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jianghu66.top/gtszlkbnbn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sweek.top/gtkxpvrttf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.9152youxi.cn/gtgqmhugfo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ppjwa.cn/gtivbdfmku.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gotoacloud.top/gtlqjbrhre.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yanxiufei.cn/gtxyhmmuab.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.316326.xyz/gtttmnjomn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtbwznkexw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.redwolf501.top/gtatxoazbe.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.c1oappe.top/gtmjqzwatd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj20258.top/gtikuirmse.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shangyingyoupin.top/gtiggchilm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.bjfxy.top/gteszjmrae.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.redwolf501.top/gtrhtadaos.html

Go:   slices.Sort(arr)
来源：http://hz.andypj.xyz/gtsycfumlf.html

Ruby: arr.sort
来源：http://hz.redwolf501.top/gtumyvrhmz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.kuanghao11.cn/gtjmlsjyqb.html

[N03] 快速排序（分治示例）
来源：http://hz.smart0.xyz/gtdrsbwuxm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.birdmap.top/gtlzujynwo.html

PHP:  // 递归实现，或用 usort
来源：http://hz.smart0.xyz/gtpvbasinl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigfzy.top/gtgaepwwqy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hnxiangtu.top/gttbuxxazz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhengqikj.top/gtsenbhmfz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xziqi.cn/gtbwqkczbc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jianghu66.top/gtipxoineu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.feifeiyinyue.top/gtiszmcgxl.html

[N04] 斐波那契数列
来源：http://hz.sweek.top/gteigbordd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.bjfxy.top/gtuzlcyhnd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.birdmap.top/gtscbbjonc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhengqikj.top/gtgjydzvqp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.andypj.xyz/gtjetjmmhx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yuxming.cn/gtrhylikep.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.aibaodan.cn/gtxlkrjosx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.smart0.xyz/gtgrnonceg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhixingplan.top/gtiodlgsau.html

[N05] 最大公约数
来源：http://hz.nwbrower.top/gtcqfbjdlo.html

Py:   math.gcd(a, b)
来源：http://hz.mhx1999.top/gtmznkbgcz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sxryk.cn/gtaaiqftfv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gtexwpgdxv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yvedp.cn/gtwdzgqdpq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yj202588.top/gtymclhgdg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yonumen.top/gtdtrpwsxo.html

Ruby: a.gcd(b)
来源：http://hz.jinyuanbaomall.cn/gtbofojuzl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cucudq.cn/gtneujmidv.html

[N06] 判断回文字符串
来源：http://hz.nwbrower.top/gticfyqurw.html

Py:   s == s[::-1]
来源：http://hz.hongshengwenyu.top/gtsocrrklf.html

PHP:  $s === strrev($s);
来源：http://hz.9152youxi.cn/gtxkicikut.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtrymtgtkh.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtakbavxgs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.daxiang520.top/gtqpzhbxun.html

Go:   // 双指针从两端比较
来源：http://hz.zhoulong.xyz/gtzexceuti.html

Ruby: s == s.reverse
来源：http://hz.zhijiandao.cn/gtqzqicsei.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinqigfzy.top/gtvhaijvkf.html

[N07] 两数之和（返回下标）
来源：http://hz.chenlongwang.top/gtmjdfrojw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.tian-w.cn/gtzbefwoco.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.svipenyu.cn/gtqzivnjkj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.wangdashe.top/gthrcywwau.html

TS:   // 手写 Map<string, number>
来源：http://hz.pycfn.com/gthtbuwwit.html

Java: // 手写 HashMap
来源：http://hz.nanxinkj.top/gtazpmahrv.html

Go:   // 手写 map[int]int
来源：http://hz.hnxiangtu.top/gttqkvoual.html

Ruby: // 手写 Hash
来源：http://hz.yongpay.top/gterbjflsp.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.c1oappe.top/gtheeyqkrw.html

[N08] 生成全排列
来源：http://hz.xuanzx.com/gtbcexovby.html

Py:   itertools.permutations(arr)
来源：http://hz.jinqigfzy.top/gtvhvymome.html

PHP:  // 手写递归交换
来源：http://hz.nanxinkj.top/gtjepspsjl.html

JS:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtgnvrybpo.html

TS:   // 手写回溯递归
来源：http://hz.redwolf501.top/gttnuzbufa.html

Java: // 手写回溯递归
来源：http://hz.yj20258.top/gtksscuasi.html

Go:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtsqwjibya.html

Ruby: arr.permutation.to_a
来源：http://hz.ehwqpu.com/gtzpilabfe.html

C#:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtcrxrtcno.html

[N09] 栈与队列
来源：http://hz.ehwqpu.com/gtdbaiaqvw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jinyuanbaomall.cn/gtehcuhhws.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.kuanghao11.cn/gtilwiwumg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hysaishi.cn/gtdomjudpr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cdnleiting.top/gttvbykrqw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yanxiufei.cn/gtdukxgjjh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zdqjudy.top/gtfmzmjafa.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.tanke756.top/gtqnorsian.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xuanzx.com/gtyymnzglm.html

[N10] 链表节点定义
来源：http://hz.iojbl.cn/gtkvojhxhg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hywenlv.cn/gttcdxevky.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jyoumei.cn/gtwmfnbwmf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jinqigufen.top/gtbmvcnkgg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shangyingyoupin.top/gtjijffqdr.html

Java: class Node { int v; Node next; }
来源：http://hz.aibaodan.cn/gtrblbdhes.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cqqwz.cn/gthhbesuhc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yj20258888.top/gtxaodjaka.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhengqikj.top/gtzldqtirs.html

[N11] 二叉树中序遍历
来源：http://hz.snrcjt.cn/gtiwaufmkc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ivvv.top/gtbpxiisge.html

PHP:  // 手写递归函数
来源：http://hz.zhaomingkeji.xyz/gttmigcbqk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sxryk.cn/gtnyfxghgn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.snrcjt.cn/gtyadrkcyb.html

Java: // 手写递归
来源：http://hz.zycfv.cn/gtifdybwog.html

Go:   // 手写递归
来源：http://hz.yvedp.cn/gtatvliyxf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cqqwz.cn/gtxsqgtpeb.html

C#:   // 手写递归
来源：http://hz.xuanzx.com/gtmqwnitjl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xuanzx.com/gtnaovdujk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhijiandao.cn/gthfyedjsy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.nanxuanxn.top/gthdenpghl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cheryme.top/gtebjnkroh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tanke756.top/gtvvhmtizy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sxryk.cn/gtwuhwomkf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yanxiufei.cn/gtajpafhsg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.birdmap.top/gtoahvebyf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.daria6918.cn/gtlrhzrtyl.html

================================================================================
来源：http://hz.chenzaomai.com/gtbeikiuvn.html

O. 并发与异步
来源：http://hz.yangfankeji.com/gtudwhqril.html

================================================================================
来源：http://hz.ydjk.org.cn/gtsxygxqwy.html

[O01] 启动一个线程
来源：http://hz.guannengcc.top/gtiyhqlkbn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yj20258888.top/gttclhqkvx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.aibaodan.cn/gtctjuxcli.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cqqwz.cn/gthfnahher.html

TS:   // 同 JS
来源：http://hz.bjfxy.top/gtxpszmznx.html

Java: new Thread(() -> f()).start()
来源：http://hz.sufxvd.cn/gtuxfjeppt.html

Go:   go f()
来源：http://hz.hnxiangtu.top/gtqnrcolki.html

Ruby: Thread.new { f }
来源：http://hz.zhijiandao.cn/gteotrseso.html

C#:   Task.Run(() => F());
来源：http://hz.hywenlv.cn/gtiwleoucr.html

[O02] 使用线程池
来源：http://hz.haohaochexian.top/gtdaibughq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.svipenyu.cn/gtpbecrdha.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhijiandao.cn/gttrkpgomw.html

JS:   // worker_threads 线程池
来源：http://hz.redwolf501.top/gtirwcplmc.html

TS:   // worker_threads 线程池
来源：http://hz.52xcode.cn/gtfmhfzgtw.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.gzhubu.top/gtbjtcdtvl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.dianchejie.cn/gtdzeaplwn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gotoacloud.top/gtilorzarh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yuanzhike.top/gtxzbxbzwk.html

[O03] 加锁保护共享数据
来源：http://hz.yonumen.top/gttcskfwwx.html

Py:   with lock: shared += 1
来源：http://hz.daxiang520.top/gtluymhecj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhixingplan.top/gthxczhywn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenlongwang.top/gtvdnuyjax.html

TS:   // 同 JS
来源：http://hz.svipenyu.cn/gtjylfheus.html

Java: synchronized (this) { shared++; }
来源：http://hz.kuanghao11.cn/gtcybdlabc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.andypj.xyz/gtaqpacsev.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yuanzhike.top/gtzvrqvxjt.html

C#:   lock (gate) { shared++; }
来源：http://hz.daxiang520.top/gtgkukzzpo.html

[O04] 定义异步函数并等待
来源：http://hz.tanke756.top/gtsoqrwque.html

Py:   async def f():⏎    await g()
来源：http://hz.zhiwuduotai.top/gtpeglxyhe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jianghu66.top/gtsxbgfgbb.html

JS:   async function f() { await g(); }
来源：http://hz.yanxiufei.cn/gtuthlqecm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.sufxvd.cn/gthwpwijai.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sysykeji.top/gtvplfqsri.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhaomingkeji.xyz/gtmfevlatx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hongshengwenyu.top/gtztihwsea.html

C#:   async Task F() { await G(); }
来源：http://hz.quarkkingdee.top/gtklhdieit.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinghuilouyu.cn/gtgnucjkgs.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cucudq.cn/gtvncnuhsv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ehwqpu.com/gtzijdespi.html

JS:   await Promise.all(tasks)
来源：http://hz.yongpay.top/gtyfzaxkgs.html

TS:   await Promise.all(tasks)
来源：http://hz.jinqigfzy.top/gtlejkuuql.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.wangshuangyany.cn/gtdlsaywpo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yvedp.cn/gtazywhrqg.html

Ruby: threads.map(&:join)
来源：http://hz.svipenyu.cn/gtmvyclmye.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xylfe.cn/gtnwhwhhza.html

[O06] 使用进程池
来源：http://hz.fzhhl.top/gtggnkjlne.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ehwqpu.com/gtnmaiuirl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.pycfn.com/gtibaieqjx.html

JS:   // child_process / cluster 模块
来源：http://hz.hnqzz.top/gtpugadsof.html

TS:   // child_process / cluster 模块
来源：http://hz.ywan-chungtsiang.top/gtjvmvizrw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.vqdsnc.cn/gtxknuefnl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yuanzhike.top/gtjuopfqck.html

Ruby: // fork 块
来源：http://hz.zhaomingkeji.xyz/gtbmbkyhkz.html

C#:   Parallel.For
来源：http://hz.jinqigfzy.top/gtwzrdmqjo.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtyseuojkd.html

P. 常用工具函数
来源：http://hz.ppjwa.cn/gteicxqrpc.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtlallewnz.html

[P01] 生成 UUID
来源：http://hz.xylfe.cn/gtuiytxzyx.html

Py:   str(uuid.uuid4())
来源：http://hz.yangfankeji.com/gtrpcyhmxz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cucudq.cn/gtkjebcjdk.html

JS:   crypto.randomUUID()
来源：http://hz.pengpengdd.cyou/gtnopthhdk.html

TS:   crypto.randomUUID()
来源：http://hz.aizwys.cn/gtmcpibzuu.html

Java: UUID.randomUUID().toString()
来源：http://hz.ppjwa.cn/gtjadvpyfw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jyoumei.cn/gtephkcwem.html

Ruby: SecureRandom.uuid
来源：http://hz.havefunace.top/gtatiuhxoj.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xingfuxueyuan.xyz/gthrsrmqla.html

[P02] MD5 / SHA256 摘要
来源：http://hz.vqdsnc.cn/gtphdghzea.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.quarkkingdee.top/gthemkpafy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ehwqpu.com/gtckdhzvlu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hammf.cn/gtqxwnujei.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.havefunace.top/gtruqcjsqx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.guowangkeji.top/gtyuothxmr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cashguo.top/gtbvfnjfud.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhijiandao.cn/gtppzalazl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cucudq.cn/gtkyebpwoq.html

[P03] 生成短随机字符串
来源：http://hz.wangshuangyany.cn/gtfxlvyxwi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhiwuduotai.top/gtzeatsywb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ywan-chungtsiang.top/gttlrdsofg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ybcxt.top/gtfsitxggy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuxming.cn/gtiwkyxytb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.316326.xyz/gtbxftzqfq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yj20258888.top/gtynnklyzy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhongyouzk.top/gtqogjfxre.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yj20258888.top/gtjzovmnqs.html

[P04] 求长度
来源：http://hz.jlsjyb.cn/gtexvjdqep.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ydzc1.top/gtujixolfg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yvedp.cn/gtkpuunejc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xylfe.cn/gtbfpagadj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sysykeji.top/gtwuycvcot.html

Java: list.size();  map.size();  s.length()
来源：http://hz.chenjidiqi.icu/gtywolviym.html

Go:   len(arr);  len(m)
来源：http://hz.feifeiyinyue.top/gtuwtzrdjd.html

Ruby: x.length;  x.size
来源：http://hz.xziqi.cn/gtenksvyuw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xziqi.cn/gtiwkgyjpt.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shuidangran.top/gtlkgmqpgg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hnqzz.top/gtzxlrvnwp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinghuilouyu.cn/gtjoqcmmoa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ehwqpu.com/gtpyvoqmjc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cucudq.cn/gtkcmfvyew.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cheryme.top/gtvdpxzsyb.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenjidiqi.icu/gtckdmanlx.html

Ruby: a == b
来源：http://hz.fzhhl.top/gthmnfuoox.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.mhx1999.top/gtcimttaih.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jyoumei.cn/gtucnschwg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.svipenyu.cn/gtoybhryhl.html

PHP:  if (empty($x)) {}
来源：http://hz.nwbrower.top/gtlhueeuxe.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yj202588.top/gthkegqdbj.html

TS:   if (x == null) {}
来源：http://hz.quarkkingdee.top/gtffjfabqb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shzxlz.cn/gtztwtysqi.html

Go:   if x == nil {}
来源：http://hz.nwbrower.top/gtgoheoaqd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jlsjyb.cn/gtakmwfanz.html

C#:   if (x is null) {}
来源：http://hz.gzhubu.top/gtvyqnqwyy.html

[P07] 防抖与节流
来源：http://hz.dashuyun.cn/gtqderewmt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xuetiantiany.cn/gtpqvuuhrg.html

PHP:  // 手写时间戳比较
来源：http://hz.sxryk.cn/gtjgaoprab.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.316326.xyz/gtkzykzqks.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yvedp.cn/gtfhquyxmj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhiwuduotai.top/gtocgyxorf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.haohaochexian.top/gtijcpgeoa.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.aibaodan.cn/gtkvmtwbfb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jinyuanbaomall.cn/gtoovdcslc.html

[P08] 处理浮点精度问题
来源：http://hz.chenlongwang.top/gtbfrfxivr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhoulong.xyz/gthlrktmlu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cashguo.top/gthaskcbgo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.svipenyu.cn/gttyldsfqu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ywan-chungtsiang.top/gtyzducvrm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xylfe.cn/gtjxojsazo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.c1oappe.top/gthuzksvht.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yuxming.cn/gtoficrome.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.wangshuangyany.cn/gthzaxesvw.html

================================================================================
来源：http://hz.hysaishi.cn/gthjhpugpy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cdnleiting.top/gtjrjpdfnl.html

================================================================================
来源：http://hz.zhongyouzk.top/gtbhmsxrrh.html

[Q01] 创建表
来源：http://hz.wangshuangyany.cn/gtouvmgkbx.html

CREATE TABLE users (
来源：http://hz.wangshuangyany.cn/gtovflqbby.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ehwqpu.com/gtjsschled.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jianghu66.top/gtlshuftxu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shuidangran.top/gtkltdxdgf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yongpay.top/gtlzrpqluq.html

);
来源：http://hz.zycfv.cn/gtiatwfusw.html

[Q02] 创建带外键的表
来源：http://hz.yongpay.top/gtskdtjgfl.html

CREATE TABLE orders (
来源：http://hz.zhixingplan.top/gtyomimelu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenlongwang.top/gtpfilfwwg.html

user_id INT NOT NULL,
来源：http://hz.feifeiyinyue.top/gtlyosanqf.html

amount DECIMAL(10, 2),
来源：http://hz.sufxvd.cn/gtlavxohpp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jlsjyb.cn/gtxfrbawqx.html

);
来源：http://hz.dianchejie.cn/gtkwxwfryf.html

[Q03] 增加列
来源：http://hz.chenjidiqi.icu/gtwaejyxnm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.aizwys.cn/gtwxglhvvs.html

[Q04] 修改列类型
来源：http://hz.chenzaomai.com/gtfsvlqhwu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xinyue.icu/gtknygocsi.html

[Q05] 重命名列
来源：http://hz.cucudq.cn/gtwuixezzi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.aibaodan.cn/gtmxsmtdqa.html

[Q06] 删除列
来源：http://hz.pycfn.com/gttslnbxkz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jianghu66.top/gtoxbufury.html

[Q07] 删除表
来源：http://hz.snrcjt.cn/gtuhedkipu.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ivvv.top/gtjvynfknd.html

[Q08] 创建普通索引
来源：http://hz.redwolf501.top/gtrvdwrhvm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.sufxvd.cn/gtciwfzigg.html

[Q09] 创建唯一索引
来源：http://hz.shanyushiyangtech.top/gtaebkoxvw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shangyingyoupin.top/gtblffczdp.html

[Q10] 插入单行
来源：http://hz.tian-w.cn/gtizjvlosv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.gaohongyu789.top/gtwwjwzztm.html

[Q11] 一次插入多行
来源：http://hz.guannengcc.top/gtntvtydaj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.sxryk.cn/gtdhtxfcbw.html

[Q12] 插入后取自增 ID
来源：http://hz.tanke756.top/gtjnvtbrjv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jiagoushi.top/gtpmqesjwx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jlsjyb.cn/gtnfpsytov.html

[Q13] 忽略重复插入
来源：http://hz.redwolf501.top/gtuykdriop.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.meibo888.top/gthnoxuewz.html


<!-- 参考信息 -->