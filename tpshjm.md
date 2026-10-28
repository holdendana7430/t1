代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shangyingyoupin.top/gtlhrascir.html

JS:   console.error("err")
来源：http://hz.shanyushiyangtech.top/gtcpxlofey.html

TS:   console.error("err")
来源：http://hz.shuidangran.top/gtlztmtbjq.html

Java: System.err.println("err")
来源：http://hz.zhaomingkeji.xyz/gtuqtniutq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shangyingyoupin.top/gtexczngsw.html

Ruby: warn "err"
来源：http://hz.yangfankeji.com/gtgfvtqyad.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yvedp.cn/gtivtikzwf.html

[M07] 判断是否为主入口
来源：http://hz.cucudq.cn/gtwzgnhdfb.html

Py:   if __name__ == "__main__":
来源：http://hz.fengsongda.top/gtiiuvsjwq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gogol.net.cn/gthjkdhkzv.html

JS:   require.main === module
来源：http://hz.yj20258888.top/gtxgurmjzr.html

TS:   require.main === module
来源：http://hz.tianlin.xyz/gtbepjsfio.html

Java: public static void main(String[] args)
来源：http://hz.gaohongyu789.top/gtaaylhvxg.html

Go:   func main()
来源：http://hz.guannengcc.top/gtfmuegfcx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.snrcjt.cn/gtsmczmojo.html

C#:   static void Main(string[] args)
来源：http://hz.xingfuxueyuan.xyz/gtqbceajqp.html

[M08] 获取系统与运行时信息
来源：http://hz.andypj.xyz/gtjfdiobay.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hongshengwenyu.top/gtsqquvtzq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.pycfn.com/gtcqogluan.html

JS:   process.platform;  process.version
来源：http://hz.mhx1999.top/gtbcjxbazv.html

TS:   process.platform;  process.version
来源：http://hz.cheryme.top/gthwlyihjd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yongpay.top/gtbnfpdaru.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.daria6918.cn/gtkhtpezuk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.pycfn.com/gtsgpsrzno.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yongpay.top/gtynrltjjv.html

================================================================================
来源：http://hz.zycfv.cn/gtbixzagrr.html

N. 数据结构与算法
来源：http://hz.vqdsnc.cn/gtfswtsjso.html

================================================================================
来源：http://hz.cheryme.top/gtnamtfvga.html

[N01] 二分查找（有序数组）
来源：http://hz.haohaochexian.top/gtmxqkpvnc.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinqigufen.top/gtfrzguczf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.guannengcc.top/gththnaxzn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.guannengcc.top/gtyhdnqcvp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigfzy.top/gtfwdvyzyi.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gzhubu.top/gthlomqqfp.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ehwqpu.com/gtmcgzpxvq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sufxvd.cn/gtvgfzdrxy.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinqigufen.top/gtdozzlinb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhaomingkeji.xyz/gtboqrtruw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shzxlz.cn/gtlbmwjhmx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.havefunace.top/gtzsyzmwza.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258.top/gttjhepkjo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.0kj1m.cn/gtfxpdblde.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhijiandao.cn/gtlkbwguxs.html

Go:   slices.Sort(arr)
来源：http://hz.hysaishi.cn/gthwecakjk.html

Ruby: arr.sort
来源：http://hz.xinyue.icu/gtowhadrod.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shangyingyoupin.top/gtrbygpvin.html

[N03] 快速排序（分治示例）
来源：http://hz.xingfuxueyuan.xyz/gtfjhycsig.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jiagoushi.top/gtmxitioha.html

PHP:  // 递归实现，或用 usort
来源：http://hz.andypj.xyz/gtfvomgeyr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dashuyun.cn/gtvtsvctfo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ivvv.top/gtromqgeud.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shuidangran.top/gtqroxfkyx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.guowangkeji.top/gtggnunkfe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yangfankeji.com/gtckifewun.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.svipenyu.cn/gtysosehqm.html

[N04] 斐波那契数列
来源：http://hz.yangfankeji.com/gtdrrmvdzw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.wangshuangyany.cn/gtzmitulxd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.vqdsnc.cn/gtrhwanibe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gotoacloud.top/gtbrzajgwr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenzaomai.com/gtwsdqwmbv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.0kj1m.cn/gtcgxdjhkf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.kuanghao11.cn/gtxymafhoo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.haohaochexian.top/gtebqrgrjn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shzxlz.cn/gtkrvdczfe.html

[N05] 最大公约数
来源：http://hz.hammf.cn/gtutpoqsau.html

Py:   math.gcd(a, b)
来源：http://hz.feifeiyinyue.top/gtdjxayuqa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yonumen.top/gtwkkvcdxf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ivvv.top/gtdyitlumx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cqqwz.cn/gtqxyrqgbg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.pengpengdd.cyou/gtsnfdmqcr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.gogol.net.cn/gtzrgaiunx.html

Ruby: a.gcd(b)
来源：http://hz.redwolf501.top/gtfkfhxfwz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.pengpengdd.cyou/gtesaltrtz.html

[N06] 判断回文字符串
来源：http://hz.svipenyu.cn/gtgxlplbtc.html

Py:   s == s[::-1]
来源：http://hz.mhx1999.top/gthulfdklr.html

PHP:  $s === strrev($s);
来源：http://hz.cdnleiting.top/gtqbzeedjo.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtpwhswrxj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.wangshuangyany.cn/gtfibeqwfz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sufxvd.cn/gtutnibbpz.html

Go:   // 双指针从两端比较
来源：http://hz.cqqwz.cn/gtqebstsjk.html

Ruby: s == s.reverse
来源：http://hz.zhixingplan.top/gtegxbymvr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.iojbl.cn/gtmsgcyjna.html

[N07] 两数之和（返回下标）
来源：http://hz.cheryme.top/gthgrobssz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yanxiufei.cn/gtgmhjelea.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.dashuyun.cn/gthiwfxtmj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gaohongyu789.top/gtdefompjx.html

TS:   // 手写 Map<string, number>
来源：http://hz.jianghu66.top/gtjfrtnpde.html

Java: // 手写 HashMap
来源：http://hz.shangyingyoupin.top/gtduohcapy.html

Go:   // 手写 map[int]int
来源：http://hz.bjfxy.top/gtmapcbsfv.html

Ruby: // 手写 Hash
来源：http://hz.jinyuanbaomall.cn/gtxayspmin.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zdqjudy.top/gtzlxqpupw.html

[N08] 生成全排列
来源：http://hz.quarkkingdee.top/gtynwurkfn.html

Py:   itertools.permutations(arr)
来源：http://hz.vqdsnc.cn/gtlswjlrdz.html

PHP:  // 手写递归交换
来源：http://hz.ydjk.org.cn/gtaisfqdit.html

JS:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtpwnwmdoz.html

TS:   // 手写回溯递归
来源：http://hz.ybcxt.top/gtbenrdvbp.html

Java: // 手写回溯递归
来源：http://hz.meibo888.top/gtpplizcmw.html

Go:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtrqvbreza.html

Ruby: arr.permutation.to_a
来源：http://hz.ybcxt.top/gtrduthjsm.html

C#:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtrrhawtir.html

[N09] 栈与队列
来源：http://hz.shzxlz.cn/gtpdgwrkbt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sufxvd.cn/gtrhdjkpae.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ydzc1.top/gtksgmyxfw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ydzc1.top/gtcqqpvtmw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhaomingkeji.xyz/gtqujhekdz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.9152youxi.cn/gtysqkdxet.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ywan-chungtsiang.top/gtveeczxyh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.chenzaomai.com/gtcpxaeiql.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.fzhhl.top/gtahhvtwlt.html

[N10] 链表节点定义
来源：http://hz.aizwys.cn/gtoitfvazk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.nwbrower.top/gtagptirda.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xuetiantiany.cn/gtvddfqkqh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yonumen.top/gtdjsbsera.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenzaomai.com/gtzzvqrebv.html

Java: class Node { int v; Node next; }
来源：http://hz.sweek.top/gtkizqxgzs.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jyoumei.cn/gtjmuqltwc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.0kj1m.cn/gtrxjumxyw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ehwqpu.com/gtjxezldpc.html

[N11] 二叉树中序遍历
来源：http://hz.gogol.net.cn/gtpmcwbnfz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.svipenyu.cn/gtqovywjyq.html

PHP:  // 手写递归函数
来源：http://hz.tianlin.xyz/gtbgixdwjo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gotoacloud.top/gtpnhfeqnp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zycfv.cn/gtdjnhvmdk.html

Java: // 手写递归
来源：http://hz.shuidangran.top/gtnyxwqacd.html

Go:   // 手写递归
来源：http://hz.yanxiufei.cn/gtbazfbjgs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jianghu66.top/gttlskvguu.html

C#:   // 手写递归
来源：http://hz.zdqjudy.top/gtyaihqzkz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhijiandao.cn/gtyzfmvbli.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenlongwang.top/gtpsoqwpas.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ybcxt.top/gtjyvlnvsu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhengqikj.top/gtnafabcdz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yuanzhike.top/gtlmquzmqc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.meibo888.top/gtvpubetlz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yj20258.top/gtuxmltgwz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.dashuyun.cn/gtjjabangj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zycfv.cn/gttsgiubqm.html

================================================================================
来源：http://hz.tian-w.cn/gtexnqzuma.html

O. 并发与异步
来源：http://hz.svipenyu.cn/gtejwliemc.html

================================================================================
来源：http://hz.daria6918.cn/gtfgpewccf.html

[O01] 启动一个线程
来源：http://hz.daria6918.cn/gtgbyccakj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.iojbl.cn/gtrtkkyqqv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhongyouzk.top/gtxyppklen.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yonumen.top/gtpajnooxu.html

TS:   // 同 JS
来源：http://hz.9152youxi.cn/gtjlnrxrpz.html

Java: new Thread(() -> f()).start()
来源：http://hz.yongpay.top/gtknsmjqsy.html

Go:   go f()
来源：http://hz.nanxinkj.top/gtblejsrtu.html

Ruby: Thread.new { f }
来源：http://hz.9152youxi.cn/gtchjadxkb.html

C#:   Task.Run(() => F());
来源：http://hz.hfpthk.cn/gtyqtalfyl.html

[O02] 使用线程池
来源：http://hz.wangdashe.top/gttpelcxgg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cashguo.top/gtzkxclpqx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ppjwa.cn/gtvpqtomfc.html

JS:   // worker_threads 线程池
来源：http://hz.jlsjyb.cn/gtabowjvrz.html

TS:   // worker_threads 线程池
来源：http://hz.dashuyun.cn/gtvjmmaszy.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cashguo.top/gthxmtdzfr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.316326.xyz/gtzpbwofhy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhiwuduotai.top/gtkrrcrnqk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hnxiangtu.top/gtuwhguwtj.html

[O03] 加锁保护共享数据
来源：http://hz.tianlin.xyz/gtbamkusbx.html

Py:   with lock: shared += 1
来源：http://hz.jlsjyb.cn/gtawbocden.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yj20258.top/gteybrfnlk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xuetiantiany.cn/gtyvbmtwze.html

TS:   // 同 JS
来源：http://hz.xinyue.icu/gtapbxrzrw.html

Java: synchronized (this) { shared++; }
来源：http://hz.xylfe.cn/gtkiwmwgrp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zdqjudy.top/gtgxrvnsso.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.nwbrower.top/gtmjgnagpl.html

C#:   lock (gate) { shared++; }
来源：http://hz.gaohongyu789.top/gtjfjlpfrx.html

[O04] 定义异步函数并等待
来源：http://hz.gzhubu.top/gthcftxxhw.html

Py:   async def f():⏎    await g()
来源：http://hz.sweek.top/gtpdpsfetx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zdqjudy.top/gtulujocrg.html

JS:   async function f() { await g(); }
来源：http://hz.wangdashe.top/gttcrygsjh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shanyushiyangtech.top/gtbermkgtz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cqqwz.cn/gtgwspcugi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yj202588.top/gtncpcnuip.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.dashuyun.cn/gtzjqxtmfe.html

C#:   async Task F() { await G(); }
来源：http://hz.meibo888.top/gtabgariye.html

[O05] 并发执行并等待全部完成
来源：http://hz.daria6918.cn/gtceqvhyqq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.guannengcc.top/gtuifgaijz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xziqi.cn/gtgbrxpews.html

JS:   await Promise.all(tasks)
来源：http://hz.iojbl.cn/gtrtxxlrfj.html

TS:   await Promise.all(tasks)
来源：http://hz.jqgfzy.top/gtmtvofwvf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.birdmap.top/gtngcxqdvi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xinyue.icu/gtnwnixpvc.html

Ruby: threads.map(&:join)
来源：http://hz.gotoacloud.top/gtvhvnceba.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhoulong.xyz/gtwbugjgfp.html

[O06] 使用进程池
来源：http://hz.xinyue.icu/gtfmlgpria.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shuidangran.top/gtygjnpzpt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.birdmap.top/gtjiuunwrw.html

JS:   // child_process / cluster 模块
来源：http://hz.c1oappe.top/gtktfazitq.html

TS:   // child_process / cluster 模块
来源：http://hz.chenlongwang.top/gtuinniqiq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.9152youxi.cn/gtevlfnbbx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhoulong.xyz/gthellciuc.html

Ruby: // fork 块
来源：http://hz.jqgfzy.top/gtgkpxngoy.html

C#:   Parallel.For
来源：http://hz.xuetiantiany.cn/gtvxpgjgtt.html

================================================================================
来源：http://hz.zhijiandao.cn/gtyknlfpii.html

P. 常用工具函数
来源：http://hz.jyoumei.cn/gtrziehuhj.html

================================================================================
来源：http://hz.gaohongyu789.top/gtadiockaz.html

[P01] 生成 UUID
来源：http://hz.zhiwuduotai.top/gtvxycxixy.html

Py:   str(uuid.uuid4())
来源：http://hz.52xcode.cn/gtoofnxshm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sufxvd.cn/gtcrtrdrkn.html

JS:   crypto.randomUUID()
来源：http://hz.haohaochexian.top/gtanfjkctl.html

TS:   crypto.randomUUID()
来源：http://hz.yj202588.top/gtslysvbwk.html

Java: UUID.randomUUID().toString()
来源：http://hz.dashuyun.cn/gtqhuqvomp.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ppjwa.cn/gtdnfwzyvj.html

Ruby: SecureRandom.uuid
来源：http://hz.yj20258888.top/gtuusxlegz.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yuanzhike.top/gtkuimguos.html

[P02] MD5 / SHA256 摘要
来源：http://hz.guannengcc.top/gtslztxnko.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jinyuanbaomall.cn/gtbpzahuji.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ywan-chungtsiang.top/gtdvlfmmzq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jiagoushi.top/gtkkscnzrk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zycfv.cn/gtrvqpsbfb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.snrcjt.cn/gtbveiyyek.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.nwbrower.top/gtysiuldqi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenlongwang.top/gtwrjmwvoc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jyoumei.cn/gtxusgwmmu.html

[P03] 生成短随机字符串
来源：http://hz.jqgufenzy.top/gtipdxfgce.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhaomingkeji.xyz/gtahfgtble.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yueranfly.top/gtlupoyegs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhoulong.xyz/gtbprowxvb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.daria6918.cn/gteajngmbm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.nanxinkj.top/gtgglguwrq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.gogol.net.cn/gtsmzovero.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.svipenyu.cn/gtbtbtmrla.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.daxiang520.top/gtpvvcnvhi.html

[P04] 求长度
来源：http://hz.pengpengdd.cyou/gtsancbbem.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.wangshuangyany.cn/gtpjqwfnju.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hfpthk.cn/gtxuibtdli.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinqigufen.top/gtypwjwher.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.0kj1m.cn/gtxcdtdcxz.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yanxiufei.cn/gtkpvnebgn.html

Go:   len(arr);  len(m)
来源：http://hz.pycfn.com/gtsezkybzf.html

Ruby: x.length;  x.size
来源：http://hz.yueranfly.top/gttfevyfsl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.guannengcc.top/gtrraykwvh.html

[P05] 判断两个对象内容是否相等
来源：http://hz.nwbrower.top/gtkvvtpjir.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.nanxuanxn.top/gtbfbaawvw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ppjwa.cn/gtkofusupr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenlongwang.top/gtljbbfmio.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.dashuyun.cn/gttousutzf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hnqzz.top/gtkuasbazm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.fzhhl.top/gtxvqmycya.html

Ruby: a == b
来源：http://hz.yongpay.top/gtowywshuw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hammf.cn/gtrlsucebl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gzhubu.top/gtxusbwvlt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.52xcode.cn/gtdzsfluhz.html

PHP:  if (empty($x)) {}
来源：http://hz.sxryk.cn/gtnfmhszja.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.andypj.xyz/gtdoaxvilv.html

TS:   if (x == null) {}
来源：http://hz.0kj1m.cn/gtfaethuix.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shanyushiyangtech.top/gtbiuhqinm.html

Go:   if x == nil {}
来源：http://hz.316326.xyz/gtzeqrqfso.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hfpthk.cn/gtvmzowjxl.html

C#:   if (x is null) {}
来源：http://hz.ybcxt.top/gtgqebfbij.html

[P07] 防抖与节流
来源：http://hz.tanke756.top/gtsmzgkzuz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.feifeiyinyue.top/gtyddkenek.html

PHP:  // 手写时间戳比较
来源：http://hz.xylfe.cn/gtqxutwoqh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.c1oappe.top/gthociyllw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.pycfn.com/gtrdgnvyba.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.chenlongwang.top/gtemyehxou.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.birdmap.top/gtwjvpcezq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xziqi.cn/gtighboufk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.havefunace.top/gtkvhnwavf.html

[P08] 处理浮点精度问题
来源：http://hz.shzxlz.cn/gtfyxrivti.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yj20258.top/gtmhyfqhuh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.birdmap.top/gtbjyvuryq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.meibo888.top/gtudqfyhri.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jinghuilouyu.cn/gtkvvzclru.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hammf.cn/gtfxjbiyfn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhijiandao.cn/gtoihhkbza.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.wangshuangyany.cn/gtuvqfoubd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hfpthk.cn/gtaojahsgb.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtfvgzlrkf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hnxiangtu.top/gtrzhwucvs.html

================================================================================
来源：http://hz.zhengqikj.top/gtfswqtmtq.html

[Q01] 创建表
来源：http://hz.tian-w.cn/gtkqxmwkyq.html

CREATE TABLE users (
来源：http://hz.bjfxy.top/gtdtgrhmgp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenlongwang.top/gtsdcmjass.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cashguo.top/gtqoizzuxx.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhiwuduotai.top/gtviejrfvu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yanxiufei.cn/gtoxwtmdfw.html

);
来源：http://hz.sysykeji.top/gtferwevnh.html

[Q02] 创建带外键的表
来源：http://hz.zhijiandao.cn/gtcosyypog.html

CREATE TABLE orders (
来源：http://hz.iojbl.cn/gtamabtzbw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ywan-chungtsiang.top/gtaqrsupdg.html

user_id INT NOT NULL,
来源：http://hz.nanxuanxn.top/gtjuidlyuw.html

amount DECIMAL(10, 2),
来源：http://hz.yanxiufei.cn/gtizsbvghr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hfpthk.cn/gtzhheehgj.html

);
来源：http://hz.hnxiangtu.top/gttpxvuljw.html

[Q03] 增加列
来源：http://hz.jqgufenzy.top/gtcsqlxygs.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yonumen.top/gtuvypwaxn.html

[Q04] 修改列类型
来源：http://hz.wangshuangyany.cn/gtibvzefus.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.9152youxi.cn/gtdiwsetzz.html

[Q05] 重命名列
来源：http://hz.jinqigfzy.top/gtcdlubbrh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yonumen.top/gtnbznfamx.html

[Q06] 删除列
来源：http://hz.ivvv.top/gtundjtktc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hnxiangtu.top/gtyxbpikof.html

[Q07] 删除表
来源：http://hz.wangshuangyany.cn/gtyjxgkqyz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yj20258.top/gtixcrpfjx.html

[Q08] 创建普通索引
来源：http://hz.yuxming.cn/gtqoipiixq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.guannengcc.top/gtmfopqvaw.html

[Q09] 创建唯一索引
来源：http://hz.sysykeji.top/gtpfpjqzac.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sysykeji.top/gteplazuiv.html

[Q10] 插入单行
来源：http://hz.snrcjt.cn/gtbtggmprg.html


<!-- 参考信息 -->