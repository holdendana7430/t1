代发 wailian999

Ruby: exit 1
来源：http://hz.dashuyun.cn/gtedgmkmbj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ydjk.org.cn/gtsxfofscj.html

[M06] 向标准错误输出
来源：http://hz.quarkkingdee.top/gtcvonolde.html

Py:   print("err", file=sys.stderr)
来源：http://hz.wangshuangyany.cn/gtbatkowwf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hnqzz.top/gtnsjllbeu.html

JS:   console.error("err")
来源：http://hz.ehwqpu.com/gtuvucipqa.html

TS:   console.error("err")
来源：http://hz.sweek.top/gtfbgckbpe.html

Java: System.err.println("err")
来源：http://hz.yuanzhike.top/gtkxqgitmh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.9152youxi.cn/gtiavdnsaq.html

Ruby: warn "err"
来源：http://hz.ehwqpu.com/gtwhomtrza.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yongpay.top/gtmcofihom.html

[M07] 判断是否为主入口
来源：http://hz.yueranfly.top/gttdxubgqw.html

Py:   if __name__ == "__main__":
来源：http://hz.sysykeji.top/gteinbrekg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shangyingyoupin.top/gtjlmpnaxb.html

JS:   require.main === module
来源：http://hz.yangfankeji.com/gtpsowtopu.html

TS:   require.main === module
来源：http://hz.nanxinkj.top/gtkygnqvwl.html

Java: public static void main(String[] args)
来源：http://hz.yuanzhike.top/gtjrhvxebk.html

Go:   func main()
来源：http://hz.svipenyu.cn/gtkzbhfqei.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jyoumei.cn/gtkfavxntl.html

C#:   static void Main(string[] args)
来源：http://hz.svipenyu.cn/gtuziajaud.html

[M08] 获取系统与运行时信息
来源：http://hz.jinqigufen.top/gtltjgaofj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.havefunace.top/gtbuuymqie.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cheryme.top/gtemswbbvd.html

JS:   process.platform;  process.version
来源：http://hz.hnxiangtu.top/gtfntulajf.html

TS:   process.platform;  process.version
来源：http://hz.hywenlv.cn/gtczxacydc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.smart0.xyz/gtjmpuxfej.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jyoumei.cn/gtouehljrm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.kuanghao11.cn/gtvjfqncaf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnqzz.top/gtskutivmc.html

================================================================================
来源：http://hz.chenlongwang.top/gtmdumseta.html

N. 数据结构与算法
来源：http://hz.xinyue.icu/gtjgaaqedl.html

================================================================================
来源：http://hz.cashguo.top/gtzgjwelyz.html

[N01] 二分查找（有序数组）
来源：http://hz.sufxvd.cn/gtxpcjrwnh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhengqikj.top/gtzzkpynyy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hysaishi.cn/gteorxsilw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.pengpengdd.cyou/gtynajsxoj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydjk.org.cn/gtiakkkwti.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.snrcjt.cn/gtiylgrtzu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhoulong.xyz/gtvwdiodkf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.wangshuangyany.cn/gtyvghnsbg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.aizwys.cn/gthmgazwhg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xylfe.cn/gtnlhkycvn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.mhx1999.top/gtllejgpjm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ybcxt.top/gtqlghnqou.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gteugmrary.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cucudq.cn/gtbocsguze.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yvedp.cn/gtxnaesjof.html

Go:   slices.Sort(arr)
来源：http://hz.hnqzz.top/gtlrmkbyzg.html

Ruby: arr.sort
来源：http://hz.jiagoushi.top/gtjwbqzijg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhixingplan.top/gtsvnyabcl.html

[N03] 快速排序（分治示例）
来源：http://hz.chenjidiqi.icu/gtayiklufg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.chenjidiqi.icu/gtofyffveg.html

PHP:  // 递归实现，或用 usort
来源：http://hz.pycfn.com/gtlwushufc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hongshengwenyu.top/gtvxpnymjt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.haohaochexian.top/gtnnerwbof.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shzxlz.cn/gtvykvmthn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.feifeiyinyue.top/gtfiflgjab.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jiagoushi.top/gtcdmovjut.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.pengpengdd.cyou/gtwhwnlzaj.html

[N04] 斐波那契数列
来源：http://hz.hysaishi.cn/gtypbxguox.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.chenzaomai.com/gtcqockxds.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.bjfxy.top/gthzolcmts.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jqgufenzy.top/gtdksphajw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sysykeji.top/gthofytxak.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.pengpengdd.cyou/gtzdyllgyb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shzxlz.cn/gtjcjighez.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.pengpengdd.cyou/gtcaitvvzv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.nanxuanxn.top/gtmebzffwa.html

[N05] 最大公约数
来源：http://hz.yuxming.cn/gtfwwjltjq.html

Py:   math.gcd(a, b)
来源：http://hz.hfpthk.cn/gtvhtoqrtr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.wangshuangyany.cn/gtqnegojzu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangtech.top/gtqsijognq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shzxlz.cn/gtidmtvote.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.guowangkeji.top/gtbbflnwub.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.dianchejie.cn/gtigpykhcx.html

Ruby: a.gcd(b)
来源：http://hz.sufxvd.cn/gtstzhhugq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hammf.cn/gtbkjqxegp.html

[N06] 判断回文字符串
来源：http://hz.yj20258.top/gtxmxnhmik.html

Py:   s == s[::-1]
来源：http://hz.wangdashe.top/gteygqwlox.html

PHP:  $s === strrev($s);
来源：http://hz.redwolf501.top/gtvkamyidw.html

JS:   s === [...s].reverse().join("")
来源：http://hz.tanke756.top/gtmevfjzsq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jinghuilouyu.cn/gtsajrkeaf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hysaishi.cn/gtvijpwrsu.html

Go:   // 双指针从两端比较
来源：http://hz.jinqigufen.top/gttqwkqkwe.html

Ruby: s == s.reverse
来源：http://hz.aizwys.cn/gtdfjkuadq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yj20258.top/gtrutaewfr.html

[N07] 两数之和（返回下标）
来源：http://hz.jinghuilouyu.cn/gtjhbyhjvx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhoulong.xyz/gtnytwtmqu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhongyouzk.top/gtfyukxzly.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhijiandao.cn/gtqwldbzvl.html

TS:   // 手写 Map<string, number>
来源：http://hz.shanyushiyangkeji.top/gtstcsfnqv.html

Java: // 手写 HashMap
来源：http://hz.52xcode.cn/gtfowmkare.html

Go:   // 手写 map[int]int
来源：http://hz.mhx1999.top/gtuatlmydh.html

Ruby: // 手写 Hash
来源：http://hz.yj20258888.top/gttcezllvs.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhiwuduotai.top/gtywyjbols.html

[N08] 生成全排列
来源：http://hz.yvedp.cn/gthsmbcpsw.html

Py:   itertools.permutations(arr)
来源：http://hz.havefunace.top/gtvdyavwvv.html

PHP:  // 手写递归交换
来源：http://hz.nwbrower.top/gtlqxysxie.html

JS:   // 手写回溯递归
来源：http://hz.yongpay.top/gtoxfssajn.html

TS:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtbdosaflm.html

Java: // 手写回溯递归
来源：http://hz.tianlin.xyz/gtzrumzrxg.html

Go:   // 手写回溯递归
来源：http://hz.chenlongwang.top/gtzduiuoop.html

Ruby: arr.permutation.to_a
来源：http://hz.zycfv.cn/gtqwqyvafv.html

C#:   // 手写回溯递归
来源：http://hz.xziqi.cn/gthcbjigio.html

[N09] 栈与队列
来源：http://hz.xziqi.cn/gtmuhbgiek.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xingfuxueyuan.xyz/gtsiozqswg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.52xcode.cn/gtxsuvmzfh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.chenzaomai.com/gtzzamndsn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yueranfly.top/gtluqspovm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.redwolf501.top/gtmncqqwmu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.pycfn.com/gtrjudmwby.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.316326.xyz/gtfxqrzret.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhaomingkeji.xyz/gtltqyyptz.html

[N10] 链表节点定义
来源：http://hz.jqgufenzy.top/gtlrxbvyvj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.daxiang520.top/gtzvtqcabm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.tanke756.top/gtlvunlvcb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xziqi.cn/gtlmxausuf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.meibo888.top/gtekkweake.html

Java: class Node { int v; Node next; }
来源：http://hz.yanxiufei.cn/gtmugslvis.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.sweek.top/gtsvroywyz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yonumen.top/gtogmubbzm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.52xcode.cn/gttnrveltl.html

[N11] 二叉树中序遍历
来源：http://hz.redwolf501.top/gtajwosatl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.tian-w.cn/gtkwhbyvkg.html

PHP:  // 手写递归函数
来源：http://hz.tian-w.cn/gtxozfzrge.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xylfe.cn/gtmlhubfxj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.kuanghao11.cn/gtfrkifsyl.html

Java: // 手写递归
来源：http://hz.xuetiantiany.cn/gtieikczqd.html

Go:   // 手写递归
来源：http://hz.dianchejie.cn/gttidorywb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.svipenyu.cn/gtwjcvqbut.html

C#:   // 手写递归
来源：http://hz.daria6918.cn/gtenveihvs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.nanxuanxn.top/gtgtpvyaub.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.kuanghao11.cn/gtkvjxkxci.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinqigufen.top/gtbqtutost.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258888.top/gtqyjkevsw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuetiantiany.cn/gtngohvqzj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zycfv.cn/gthjgctwvd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yuanzhike.top/gtnuzobcud.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.haohaochexian.top/gtxnpezrsw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fzhhl.top/gtitafgggf.html

================================================================================
来源：http://hz.pycfn.com/gtapqcmjkz.html

O. 并发与异步
来源：http://hz.c1oappe.top/gttujvzdfu.html

================================================================================
来源：http://hz.aizwys.cn/gtuuwlhual.html

[O01] 启动一个线程
来源：http://hz.hammf.cn/gtyarvhodk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gzhubu.top/gtjrvprcag.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yonumen.top/gtklpnmwzo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jinqigfzy.top/gtjufgbvwu.html

TS:   // 同 JS
来源：http://hz.chenjidiqi.icu/gtgmcvqxkx.html

Java: new Thread(() -> f()).start()
来源：http://hz.quarkkingdee.top/gtvvuugspr.html

Go:   go f()
来源：http://hz.c1oappe.top/gtmbkljmiy.html

Ruby: Thread.new { f }
来源：http://hz.ppjwa.cn/gtndrzxttg.html

C#:   Task.Run(() => F());
来源：http://hz.hammf.cn/gtbpfacmzy.html

[O02] 使用线程池
来源：http://hz.wangshuangyany.cn/gtfnwewqce.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yongpay.top/gthbpzbtke.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jyoumei.cn/gtqeeougyy.html

JS:   // worker_threads 线程池
来源：http://hz.kuanghao11.cn/gtpgojfzey.html

TS:   // worker_threads 线程池
来源：http://hz.jyoumei.cn/gtalqcjhtc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cheryme.top/gtqltwxmaw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.sufxvd.cn/gtdzhcymwh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhaomingkeji.xyz/gtewwtxzbl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.smart0.xyz/gtckuepkgi.html

[O03] 加锁保护共享数据
来源：http://hz.wangdashe.top/gtsytsdqpg.html

Py:   with lock: shared += 1
来源：http://hz.yangfankeji.com/gtzwnehwbf.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yuxming.cn/gtjtmjtdsb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinqigfzy.top/gtdjplrvat.html

TS:   // 同 JS
来源：http://hz.chenlongwang.top/gtdoppefyz.html

Java: synchronized (this) { shared++; }
来源：http://hz.sxryk.cn/gtjaarsoxs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ywan-chungtsiang.top/gtuhvhjcsk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.redwolf501.top/gtaytpfxwl.html

C#:   lock (gate) { shared++; }
来源：http://hz.yueranfly.top/gtwlldshpp.html

[O04] 定义异步函数并等待
来源：http://hz.ppjwa.cn/gtnbvkfkia.html

Py:   async def f():⏎    await g()
来源：http://hz.shzxlz.cn/gtnburffbx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gotoacloud.top/gtxighhhyw.html

JS:   async function f() { await g(); }
来源：http://hz.316326.xyz/gtisjqsvme.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hongshengwenyu.top/gtinltlopv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.guannengcc.top/gtqygnanbx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.wangdashe.top/gtunorazyn.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.dianchejie.cn/gtvggdpwzx.html

C#:   async Task F() { await G(); }
来源：http://hz.aibaodan.cn/gtupykddnv.html

[O05] 并发执行并等待全部完成
来源：http://hz.yonumen.top/gtfokeqnxy.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gogol.net.cn/gtdmmqjyaw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.svipenyu.cn/gtbmfkzepo.html

JS:   await Promise.all(tasks)
来源：http://hz.daria6918.cn/gtwxtmauce.html

TS:   await Promise.all(tasks)
来源：http://hz.fzhhl.top/gtjnztecjq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ybcxt.top/gtvvofyvzr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.chenjidiqi.icu/gtmmorvunb.html

Ruby: threads.map(&:join)
来源：http://hz.xziqi.cn/gtjhumpule.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinghuilouyu.cn/gttufxepcp.html

[O06] 使用进程池
来源：http://hz.9152youxi.cn/gtuqmwaytl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ywan-chungtsiang.top/gtimcigjxv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jinqigufen.top/gtpwldzuuc.html

JS:   // child_process / cluster 模块
来源：http://hz.birdmap.top/gthpyirxod.html

TS:   // child_process / cluster 模块
来源：http://hz.jianghu66.top/gtqbxxtyye.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.daxiang520.top/gteabywbuf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.aizwys.cn/gtezjwvbet.html

Ruby: // fork 块
来源：http://hz.xingfuxueyuan.xyz/gtonmhmsxz.html

C#:   Parallel.For
来源：http://hz.ywan-chungtsiang.top/gtxdmzuxwk.html

================================================================================
来源：http://hz.mhx1999.top/gtgmtfpwjw.html

P. 常用工具函数
来源：http://hz.xuetiantiany.cn/gtpgwdbbkw.html

================================================================================
来源：http://hz.zhijiandao.cn/gtshkefxnz.html

[P01] 生成 UUID
来源：http://hz.xingfuxueyuan.xyz/gtpdcwgzcj.html

Py:   str(uuid.uuid4())
来源：http://hz.nanxuanxn.top/gtwvxhpsyg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jlsjyb.cn/gtfpshsran.html

JS:   crypto.randomUUID()
来源：http://hz.kuanghao11.cn/gtmpmkwkcn.html

TS:   crypto.randomUUID()
来源：http://hz.tian-w.cn/gtuoodbahk.html

Java: UUID.randomUUID().toString()
来源：http://hz.ppjwa.cn/gtzdlxupmc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.fzhhl.top/gtbwdsofpw.html

Ruby: SecureRandom.uuid
来源：http://hz.yanxiufei.cn/gtyxqvdwcy.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jlsjyb.cn/gtkilhqrpb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhijiandao.cn/gtbxwzajdh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sufxvd.cn/gtgjlounwo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhixingplan.top/gtrpthfcec.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hfpthk.cn/gtiytumhic.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jinqigfzy.top/gtqotbjqfr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.tian-w.cn/gtomswtqxz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.guannengcc.top/gttgeqhxuq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zycfv.cn/gtmnafryls.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.daxiang520.top/gttezmgrak.html

[P03] 生成短随机字符串
来源：http://hz.jianghu66.top/gtvapqaeuf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.tanke756.top/gtjetltxkv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.snrcjt.cn/gttizcpmov.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sweek.top/gthjfchbbb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.haohaochexian.top/gttkfgxutz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinghuilouyu.cn/gtfhdbhwtt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.9152youxi.cn/gtmaumvqlm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhengqikj.top/gthgrrnoxh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.0kj1m.cn/gtjvulolqs.html

[P04] 求长度
来源：http://hz.quarkkingdee.top/gtrccpskst.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cqqwz.cn/gtiuworzlx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgfzy.top/gtthnbkurq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cashguo.top/gtydukrfim.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.andypj.xyz/gtulrlmsbg.html

Java: list.size();  map.size();  s.length()
来源：http://hz.52xcode.cn/gtdtsvprao.html

Go:   len(arr);  len(m)
来源：http://hz.andypj.xyz/gtmjahvzsv.html

Ruby: x.length;  x.size
来源：http://hz.ivvv.top/gtbcbrkprj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shanyushiyangtech.top/gtjpsuoazx.html

[P05] 判断两个对象内容是否相等
来源：http://hz.vqdsnc.cn/gttsvghotf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.chenjidiqi.icu/gtdohynaor.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xuetiantiany.cn/gtrvrsjtsa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.cdnleiting.top/gtmblnnpzf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhaomingkeji.xyz/gtxikjdouy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.pycfn.com/gtnmakztsq.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.snrcjt.cn/gtolilbpzn.html

Ruby: a == b
来源：http://hz.hammf.cn/gtvifrdyut.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhixingplan.top/gthhavudgt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.nwbrower.top/gtqhklvwnf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ivvv.top/gtmkaetctj.html

PHP:  if (empty($x)) {}
来源：http://hz.gaohongyu789.top/gtpqmxdglr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.nanxuanxn.top/gtdcldxcou.html

TS:   if (x == null) {}
来源：http://hz.shanyushiyangkeji.top/gtszystsup.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.mhx1999.top/gtbpjjqkdw.html

Go:   if x == nil {}
来源：http://hz.shuidangran.top/gtldejqbiw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.kuanghao11.cn/gtjgkreuwl.html

C#:   if (x is null) {}
来源：http://hz.wangshuangyany.cn/gtfrkonvwa.html

[P07] 防抖与节流
来源：http://hz.316326.xyz/gtyszicjpj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zdqjudy.top/gtcocfayvj.html

PHP:  // 手写时间戳比较
来源：http://hz.fzhhl.top/gtbmxspxxu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shuidangran.top/gtnkvaomtt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gtwtqrgnng.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xuetiantiany.cn/gtvidaxiof.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.52xcode.cn/gtoykgtktv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.tianlin.xyz/gtkwdmayxt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.chenjidiqi.icu/gtedambijn.html

[P08] 处理浮点精度问题
来源：http://hz.zhijiandao.cn/gthasmqcjc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xuanzx.com/gtfixqhpln.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ydzc1.top/gtlaoklwke.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.guowangkeji.top/gtznarnrjf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hysaishi.cn/gtsdggcrzr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.dianchejie.cn/gtqubdxcbd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jqgufenzy.top/gtuvltsicx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xinyue.icu/gtrbrtvyxn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yuxming.cn/gtlqnqdcmb.html

================================================================================
来源：http://hz.9152youxi.cn/gtndneiuor.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jiagoushi.top/gtxqlsmpna.html

================================================================================
来源：http://hz.svipenyu.cn/gtshqpjkhc.html

[Q01] 创建表
来源：http://hz.jyoumei.cn/gtuihhjwbt.html

CREATE TABLE users (
来源：http://hz.sufxvd.cn/gtobbylven.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zdqjudy.top/gtyrfxbvav.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shzxlz.cn/gtfpvyilhk.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hfpthk.cn/gtdymotsmn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xziqi.cn/gtpozerksa.html

);
来源：http://hz.yonumen.top/gtumvvacde.html

[Q02] 创建带外键的表
来源：http://hz.shanyushiyangtech.top/gtpyohspqk.html

CREATE TABLE orders (
来源：http://hz.yongpay.top/gtggwvklgq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jianghu66.top/gtctfuxnvi.html

user_id INT NOT NULL,
来源：http://hz.gaohongyu789.top/gtwplzarwr.html

amount DECIMAL(10, 2),
来源：http://hz.jianghu66.top/gtbtnmvxtx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.sysykeji.top/gtoxacvvkf.html

);
来源：http://hz.shzxlz.cn/gtqggxxhpb.html

[Q03] 增加列
来源：http://hz.hnxiangtu.top/gtywngojng.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.daxiang520.top/gtwmfbumth.html

[Q04] 修改列类型
来源：http://hz.hnqzz.top/gtrlfrmvgf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.andypj.xyz/gtdkwdxman.html

[Q05] 重命名列
来源：http://hz.shanyushiyangtech.top/gtgxkbqzna.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.guannengcc.top/gtcgaoazwq.html

[Q06] 删除列
来源：http://hz.iojbl.cn/gtzhgaoyrl.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhengqikj.top/gtquauxstx.html

[Q07] 删除表
来源：http://hz.havefunace.top/gtbgukovme.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sxryk.cn/gtzsvnaakw.html

[Q08] 创建普通索引
来源：http://hz.yongpay.top/gtdtjyszpj.html


<!-- 参考信息 -->