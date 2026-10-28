代发 wailian999

Java: public static void main(String[] args)
来源：http://hz.cdnleiting.top/gtmiuuatju.html

Go:   func main()
来源：http://hz.xingfuxueyuan.xyz/gtifiszyeq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ybcxt.top/gtyyxsrvow.html

C#:   static void Main(string[] args)
来源：http://hz.vqdsnc.cn/gtifcwjxlj.html

[M08] 获取系统与运行时信息
来源：http://hz.yonumen.top/gtmqheknta.html

Py:   platform.system();  platform.python_version()
来源：http://hz.sysykeji.top/gtmkcacyko.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jyoumei.cn/gtekgnbxjp.html

JS:   process.platform;  process.version
来源：http://hz.jinqigufen.top/gtfbfbnaxg.html

TS:   process.platform;  process.version
来源：http://hz.jinghuilouyu.cn/gteiyhidev.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.svipenyu.cn/gtnrdpsjzm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinghuilouyu.cn/gtornvcjmo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shangyingyoupin.top/gteblnpshu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.birdmap.top/gtkogobpky.html

================================================================================
来源：http://hz.zhengqikj.top/gtdfxgjnct.html

N. 数据结构与算法
来源：http://hz.nwbrower.top/gtamhgzwwr.html

================================================================================
来源：http://hz.svipenyu.cn/gtpixrxzan.html

[N01] 二分查找（有序数组）
来源：http://hz.ydjk.org.cn/gthmieuznz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.meibo888.top/gtzftmfckx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shanyushiyangkeji.top/gtechzbogn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yonumen.top/gtctazxmqy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zdqjudy.top/gtowplxoqm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yj20258888.top/gtqxtsmqwq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinqigfzy.top/gtmvhayibj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xuanzx.com/gtjralcupy.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xinyue.icu/gtklgccnrh.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.snrcjt.cn/gthxqiqaah.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fzhhl.top/gtznbdwfrs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhiwuduotai.top/gtlcmiivrq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ydzc1.top/gtfjbkpqrz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinyuanbaomall.cn/gtpbgmwiie.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yuxming.cn/gtwsjufsvi.html

Go:   slices.Sort(arr)
来源：http://hz.shanyushiyangtech.top/gttyjbamio.html

Ruby: arr.sort
来源：http://hz.quarkkingdee.top/gtjfwbladk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cheryme.top/gtcvqoqnfj.html

[N03] 快速排序（分治示例）
来源：http://hz.daria6918.cn/gtfirzreaw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yj202588.top/gtdqeywvfn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nanxuanxn.top/gtzbmtipgj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sweek.top/gtjnzlylzq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hnqzz.top/gtqiviragz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.gotoacloud.top/gtfgtybpeo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.snrcjt.cn/gtldhyukck.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sweek.top/gtbkqjmuty.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.aizwys.cn/gtqsdthrzw.html

[N04] 斐波那契数列
来源：http://hz.zhoulong.xyz/gtzcjqjgud.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yueranfly.top/gtwupcfbde.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sufxvd.cn/gtbsaetspv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hywenlv.cn/gtqpouhmrw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxuanxn.top/gtopkrmdlp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hfpthk.cn/gtxdbpzvar.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.mhx1999.top/gtokzifflk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.dashuyun.cn/gtqoymxsnp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenzaomai.com/gtlkjjecjd.html

[N05] 最大公约数
来源：http://hz.ppjwa.cn/gtmohwaplb.html

Py:   math.gcd(a, b)
来源：http://hz.dashuyun.cn/gtvgbyhxgb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.redwolf501.top/gtcrxmsvgt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jlsjyb.cn/gtsvtrkrjl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.vqdsnc.cn/gtrkphrnty.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jqgfzy.top/gtmealqkco.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinghuilouyu.cn/gtfqgrtagt.html

Ruby: a.gcd(b)
来源：http://hz.zhengqikj.top/gtynqusdbj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.aibaodan.cn/gtcjcuimad.html

[N06] 判断回文字符串
来源：http://hz.fengsongda.top/gtualqpdbs.html

Py:   s == s[::-1]
来源：http://hz.shanyushiyangtech.top/gtohsscbfx.html

PHP:  $s === strrev($s);
来源：http://hz.ywan-chungtsiang.top/gtwotggzok.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtirxijwze.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shuidangran.top/gtounhijrt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sxryk.cn/gtxctsitsz.html

Go:   // 双指针从两端比较
来源：http://hz.sweek.top/gtiukomydy.html

Ruby: s == s.reverse
来源：http://hz.sxryk.cn/gtzlxmhghk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gaohongyu789.top/gtpobyeihr.html

[N07] 两数之和（返回下标）
来源：http://hz.snrcjt.cn/gttksmapor.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ppjwa.cn/gtwayccagv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.chenzaomai.com/gtutgmphgl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.fengsongda.top/gtutzfbcvz.html

TS:   // 手写 Map<string, number>
来源：http://hz.gzhubu.top/gtmiqfrvtk.html

Java: // 手写 HashMap
来源：http://hz.yvedp.cn/gthtrxesem.html

Go:   // 手写 map[int]int
来源：http://hz.sufxvd.cn/gttbzfkxsl.html

Ruby: // 手写 Hash
来源：http://hz.xylfe.cn/gthyfbdqis.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.dashuyun.cn/gthxbhlmdf.html

[N08] 生成全排列
来源：http://hz.yueranfly.top/gtyjfcbqsn.html

Py:   itertools.permutations(arr)
来源：http://hz.gotoacloud.top/gtiaaurmmf.html

PHP:  // 手写递归交换
来源：http://hz.sufxvd.cn/gtcrgwmtao.html

JS:   // 手写回溯递归
来源：http://hz.xziqi.cn/gtbfyvpffn.html

TS:   // 手写回溯递归
来源：http://hz.chenlongwang.top/gtulufgybh.html

Java: // 手写回溯递归
来源：http://hz.andypj.xyz/gttcfsvgbj.html

Go:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtkfadecwm.html

Ruby: arr.permutation.to_a
来源：http://hz.vqdsnc.cn/gtvuvxzqoi.html

C#:   // 手写回溯递归
来源：http://hz.yj202588.top/gtmapbgdwd.html

[N09] 栈与队列
来源：http://hz.wangdashe.top/gtesdsxfaa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.svipenyu.cn/gtxnvqjcys.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.havefunace.top/gtgqmunnjw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.wangdashe.top/gtyjufowpa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinghuilouyu.cn/gtxqeydfya.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hfpthk.cn/gtvpynpqah.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.svipenyu.cn/gtbiziiweg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.wangshuangyany.cn/gtzzbmhfqz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.bjfxy.top/gtistgewmw.html

[N10] 链表节点定义
来源：http://hz.snrcjt.cn/gtfqkhbezn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yanxiufei.cn/gtyixhxqso.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.redwolf501.top/gtzscbupvr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.meibo888.top/gttabzvnvv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.svipenyu.cn/gtkwcjqutb.html

Java: class Node { int v; Node next; }
来源：http://hz.quarkkingdee.top/gtkwbgwfpl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xylfe.cn/gthortksog.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.guowangkeji.top/gtjqcjcokn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.mhx1999.top/gtfrrprolo.html

[N11] 二叉树中序遍历
来源：http://hz.xuanzx.com/gtvqxmcdtj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.chenzaomai.com/gtercpgtqo.html

PHP:  // 手写递归函数
来源：http://hz.zhaomingkeji.xyz/gtifdeojec.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgfzy.top/gthpvwxxlb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hongshengwenyu.top/gtrsxekosv.html

Java: // 手写递归
来源：http://hz.shzxlz.cn/gtoigtftzy.html

Go:   // 手写递归
来源：http://hz.gotoacloud.top/gtfjkazcvg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.snrcjt.cn/gtkmzfqqpv.html

C#:   // 手写递归
来源：http://hz.iojbl.cn/gtmtbzdtez.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinqigufen.top/gttaqtpqgi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ydzc1.top/gtpvgjjzqq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jqgufenzy.top/gtupfcmlrp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nwbrower.top/gtuyccjqgl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.pengpengdd.cyou/gtpumpjhet.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.havefunace.top/gtxjlmkrla.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.tanke756.top/gtsybenuhx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ppjwa.cn/gtuqcacgio.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fzhhl.top/gtioebpker.html

================================================================================
来源：http://hz.yvedp.cn/gtprwjfgdo.html

O. 并发与异步
来源：http://hz.snrcjt.cn/gtvvcumcgv.html

================================================================================
来源：http://hz.mhx1999.top/gthgcouzjf.html

[O01] 启动一个线程
来源：http://hz.gzhubu.top/gtasnbcnij.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yuxming.cn/gtfdwggqrh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shanyushiyangtech.top/gthzslizcf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yuanzhike.top/gtmivybauj.html

TS:   // 同 JS
来源：http://hz.shanyushiyangtech.top/gtxpgnhcks.html

Java: new Thread(() -> f()).start()
来源：http://hz.wangdashe.top/gtudytebzx.html

Go:   go f()
来源：http://hz.zhoulong.xyz/gtsrunaavl.html

Ruby: Thread.new { f }
来源：http://hz.hywenlv.cn/gtkxqadfdx.html

C#:   Task.Run(() => F());
来源：http://hz.shangyingyoupin.top/gtzpiqaqdm.html

[O02] 使用线程池
来源：http://hz.gogol.net.cn/gtynltguur.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yuanzhike.top/gtrmlapknq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.redwolf501.top/gtjyklwrhg.html

JS:   // worker_threads 线程池
来源：http://hz.wangshuangyany.cn/gthotnuyuv.html

TS:   // worker_threads 线程池
来源：http://hz.xingfuxueyuan.xyz/gtsjuzfzwn.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.c1oappe.top/gtyrmakwkh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.andypj.xyz/gtjyhycsvv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xziqi.cn/gtizdegyim.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinqigufen.top/gtavclmxyh.html

[O03] 加锁保护共享数据
来源：http://hz.zdqjudy.top/gtuzhdrmvj.html

Py:   with lock: shared += 1
来源：http://hz.yangfankeji.com/gtaakynvyu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cheryme.top/gtuvxpdyph.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.guannengcc.top/gtalqctqug.html

TS:   // 同 JS
来源：http://hz.vqdsnc.cn/gtleqzzxxr.html

Java: synchronized (this) { shared++; }
来源：http://hz.pengpengdd.cyou/gtpaudbkbn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.nanxinkj.top/gtosbwfnvz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.guannengcc.top/gtmmfkxgpr.html

C#:   lock (gate) { shared++; }
来源：http://hz.shanyushiyangkeji.top/gtiojydjeb.html

[O04] 定义异步函数并等待
来源：http://hz.dashuyun.cn/gtktqtuwtd.html

Py:   async def f():⏎    await g()
来源：http://hz.cqqwz.cn/gtklbhftdx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.tianlin.xyz/gtbcgsglef.html

JS:   async function f() { await g(); }
来源：http://hz.jianghu66.top/gtivcfgdos.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xinyue.icu/gtceierxky.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.birdmap.top/gtjcencurb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yuanzhike.top/gtbdbwicyu.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.chenjidiqi.icu/gtrposouor.html

C#:   async Task F() { await G(); }
来源：http://hz.ehwqpu.com/gtxeqpmyrp.html

[O05] 并发执行并等待全部完成
来源：http://hz.guowangkeji.top/gteoveqhxq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenzaomai.com/gtwxngbkyr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.guannengcc.top/gtaprdwjxa.html

JS:   await Promise.all(tasks)
来源：http://hz.yuanzhike.top/gtwxnqsrwh.html

TS:   await Promise.all(tasks)
来源：http://hz.yuanzhike.top/gtrcjarllo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.gogol.net.cn/gtizkaouvq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.snrcjt.cn/gtcvowqbvg.html

Ruby: threads.map(&:join)
来源：http://hz.shanyushiyangkeji.top/gtjmviqvjo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jyoumei.cn/gtexjukojp.html

[O06] 使用进程池
来源：http://hz.snrcjt.cn/gtztjjjcne.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xingfuxueyuan.xyz/gthvvyvzob.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xziqi.cn/gtxwlkkcfw.html

JS:   // child_process / cluster 模块
来源：http://hz.zycfv.cn/gtnvgkxnhl.html

TS:   // child_process / cluster 模块
来源：http://hz.quarkkingdee.top/gttkldopie.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sweek.top/gtpujejmht.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.52xcode.cn/gtxbuoapmh.html

Ruby: // fork 块
来源：http://hz.shangyingyoupin.top/gttaxvvnnz.html

C#:   Parallel.For
来源：http://hz.nwbrower.top/gtfiajvpad.html

================================================================================
来源：http://hz.zhongyouzk.top/gtrhidbocj.html

P. 常用工具函数
来源：http://hz.dashuyun.cn/gtszctlaly.html

================================================================================
来源：http://hz.xziqi.cn/gthgwiewsp.html

[P01] 生成 UUID
来源：http://hz.sysykeji.top/gtaaozumza.html

Py:   str(uuid.uuid4())
来源：http://hz.sweek.top/gtyglldxre.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ehwqpu.com/gtuinrezma.html

JS:   crypto.randomUUID()
来源：http://hz.jinqigufen.top/gtqwtremou.html

TS:   crypto.randomUUID()
来源：http://hz.cheryme.top/gtecvfxjun.html

Java: UUID.randomUUID().toString()
来源：http://hz.yangfankeji.com/gtyrzpeoly.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cashguo.top/gtvqsdvwkm.html

Ruby: SecureRandom.uuid
来源：http://hz.xylfe.cn/gtbxofmxsa.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhoulong.xyz/gtjmtmjwvu.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yuxming.cn/gtgdsfnsaa.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.kuanghao11.cn/gtognnogvg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.c1oappe.top/gtsetqmudg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.daria6918.cn/gtjzygkvqk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hywenlv.cn/gtywermqhg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.316326.xyz/gtogjjkgcn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.tanke756.top/gtmbketjcj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ydzc1.top/gtmymwvyom.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yongpay.top/gtittbbydd.html

[P03] 生成短随机字符串
来源：http://hz.fzhhl.top/gtfjgbzzfk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yuxming.cn/gtewoxcsbf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gzhubu.top/gtvxsvuxek.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xziqi.cn/gtjatipilu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jyoumei.cn/gtjamsxqdp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.c1oappe.top/gtqbatvtpl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ywan-chungtsiang.top/gteybydphh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yvedp.cn/gtykhjqudb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhaomingkeji.xyz/gtqiqffzqd.html

[P04] 求长度
来源：http://hz.316326.xyz/gtqdjmidrp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ydjk.org.cn/gtaiafajzy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sysykeji.top/gtetczxwer.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.svipenyu.cn/gtmpjhnnti.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenlongwang.top/gtjaojqurb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yvedp.cn/gteqshwigq.html

Go:   len(arr);  len(m)
来源：http://hz.9152youxi.cn/gtovswefby.html

Ruby: x.length;  x.size
来源：http://hz.hywenlv.cn/gtvskivssm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hywenlv.cn/gtnuonbntn.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yvedp.cn/gturypylly.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.gzhubu.top/gtmqhlvwsv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ivvv.top/gtfxlqsafy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.tanke756.top/gtwwzaxhpg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinyuanbaomall.cn/gtwxrsgqrg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.aibaodan.cn/gtysbkyywd.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.mhx1999.top/gtdbaphmek.html

Ruby: a == b
来源：http://hz.zycfv.cn/gtuhnlsimp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.chenzaomai.com/gtxsdhmeml.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.wangshuangyany.cn/gtbfvuzcxa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jiagoushi.top/gtrzbhzhaz.html

PHP:  if (empty($x)) {}
来源：http://hz.birdmap.top/gtjaaluzas.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinyuanbaomall.cn/gtsedicsiw.html

TS:   if (x == null) {}
来源：http://hz.316326.xyz/gtatoigjjb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhoulong.xyz/gtkzjejdlb.html

Go:   if x == nil {}
来源：http://hz.cheryme.top/gtgextphag.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.svipenyu.cn/gteiwtkbwa.html

C#:   if (x is null) {}
来源：http://hz.jqgufenzy.top/gtizmhzupk.html

[P07] 防抖与节流
来源：http://hz.zdqjudy.top/gtokigtaqk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hywenlv.cn/gtaxsebvws.html

PHP:  // 手写时间戳比较
来源：http://hz.yonumen.top/gthtbwuowa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gotoacloud.top/gtuagvjuap.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zycfv.cn/gtaraxgzko.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cashguo.top/gtgmzjcsoj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shuidangran.top/gttalkqflb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gotoacloud.top/gtigirltxg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jinqigfzy.top/gtsydeikbl.html

[P08] 处理浮点精度问题
来源：http://hz.nanxinkj.top/gtsbfpegvd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhijiandao.cn/gtkzarcnov.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.sufxvd.cn/gtfsmceogb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jinqigufen.top/gttxlenfdq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.snrcjt.cn/gtmqufvrbb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cashguo.top/gtespratcz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sweek.top/gtmuwdaqyi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.316326.xyz/gtgefgznov.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.dashuyun.cn/gthmqfheaf.html

================================================================================
来源：http://hz.cqqwz.cn/gtspxbgucj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jqgfzy.top/gtphqfqmfa.html

================================================================================
来源：http://hz.haohaochexian.top/gtdxkebyub.html

[Q01] 创建表
来源：http://hz.quarkkingdee.top/gtwrtzkzcd.html

CREATE TABLE users (
来源：http://hz.birdmap.top/gtebyffxop.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xinyue.icu/gtwgyfmrmr.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cheryme.top/gtguhkuzwn.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xingfuxueyuan.xyz/gtabyezhvb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.pengpengdd.cyou/gtyuvyzwkd.html

);
来源：http://hz.yonumen.top/gtsrxcmwuj.html

[Q02] 创建带外键的表
来源：http://hz.snrcjt.cn/gtjeuiyvtm.html

CREATE TABLE orders (
来源：http://hz.svipenyu.cn/gtpaqffyps.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yonumen.top/gtbbifashp.html

user_id INT NOT NULL,
来源：http://hz.yanxiufei.cn/gtkqnkdgxt.html

amount DECIMAL(10, 2),
来源：http://hz.pycfn.com/gtugomenlx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhixingplan.top/gtydrzhice.html

);
来源：http://hz.sweek.top/gtwisznhtu.html

[Q03] 增加列
来源：http://hz.shuidangran.top/gthqpmamwl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhoulong.xyz/gtydvpjgrk.html

[Q04] 修改列类型
来源：http://hz.quarkkingdee.top/gtpqxrcjlf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yuanzhike.top/gttletixwy.html

[Q05] 重命名列
来源：http://hz.haohaochexian.top/gtjugkuhew.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nanxuanxn.top/gtmpvtttmy.html

[Q06] 删除列
来源：http://hz.xylfe.cn/gtrjxuiwff.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.xziqi.cn/gtydprrpzi.html

[Q07] 删除表
来源：http://hz.pycfn.com/gtflkfywfy.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhixingplan.top/gtctnohqsd.html

[Q08] 创建普通索引
来源：http://hz.hongshengwenyu.top/gtfyimlgyx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.kuanghao11.cn/gtesemamsh.html

[Q09] 创建唯一索引
来源：http://hz.hywenlv.cn/gtoqgcgxhc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.iojbl.cn/gtqpsernro.html

[Q10] 插入单行
来源：http://hz.vqdsnc.cn/gtarxdqtsg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hfpthk.cn/gtyarfnghk.html

[Q11] 一次插入多行
来源：http://hz.ehwqpu.com/gtahapmxby.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhijiandao.cn/gtnpzbnbha.html

[Q12] 插入后取自增 ID
来源：http://hz.xziqi.cn/gtbyesxpiw.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hnqzz.top/gtykvgvhxf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhongyouzk.top/gtyzdtbfjj.html

[Q13] 忽略重复插入
来源：http://hz.zhoulong.xyz/gtzqysoezu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.vqdsnc.cn/gtnferqgpc.html

[Q14] 存在则更新（upsert）
来源：http://hz.tian-w.cn/gtlqdsqjwq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hnxiangtu.top/gtimsbowhv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hnxiangtu.top/gtsrwwaqat.html

[Q15] 查询全部
来源：http://hz.ydjk.org.cn/gtwlcdtelv.html


<!-- 参考信息 -->