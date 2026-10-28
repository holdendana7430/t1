代发 wailian999

[M04] 获取当前工作目录
来源：http://hz.pengpengdd.cyou/gtzfankrvd.html

Py:   os.getcwd()
来源：http://hz.shuidangran.top/gtzffknegr.html

PHP:  getcwd();
来源：http://hz.cucudq.cn/gtuqyyqwhy.html

JS:   process.cwd()
来源：http://hz.jinghuilouyu.cn/gtazdytdqh.html

TS:   process.cwd()
来源：http://hz.zhengqikj.top/gtwtopgzgb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hnxiangtu.top/gtfpxteztm.html

Go:   os.Getwd()
来源：http://hz.xylfe.cn/gtnooaqkfg.html

Ruby: Dir.pwd
来源：http://hz.0kj1m.cn/gtglaccugi.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.kuanghao11.cn/gtxocazgha.html

[M05] 设置退出码
来源：http://hz.guannengcc.top/gtsidkvfgc.html

Py:   sys.exit(1)
来源：http://hz.hywenlv.cn/gtxjyaizyz.html

PHP:  exit(1);
来源：http://hz.hnxiangtu.top/gtigvqyeyy.html

JS:   process.exit(1)
来源：http://hz.haohaochexian.top/gtkubwtmqi.html

TS:   process.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtojoykmsl.html

Java: System.exit(1)
来源：http://hz.xuetiantiany.cn/gtwqopazuc.html

Go:   os.Exit(1)
来源：http://hz.tian-w.cn/gtssrwjoco.html

Ruby: exit 1
来源：http://hz.yuxming.cn/gtzefikils.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.mhx1999.top/gtjenmtvdp.html

[M06] 向标准错误输出
来源：http://hz.zhongyouzk.top/gtxnofhubx.html

Py:   print("err", file=sys.stderr)
来源：http://hz.aizwys.cn/gtojkfgalq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zdqjudy.top/gtkggcoffn.html

JS:   console.error("err")
来源：http://hz.vqdsnc.cn/gtfdzjusqb.html

TS:   console.error("err")
来源：http://hz.shanyushiyangtech.top/gthaignnkk.html

Java: System.err.println("err")
来源：http://hz.yvedp.cn/gtmtexbiom.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.pengpengdd.cyou/gtdrcszzms.html

Ruby: warn "err"
来源：http://hz.ivvv.top/gtvhqlrkwo.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.dashuyun.cn/gtrpmbfbwi.html

[M07] 判断是否为主入口
来源：http://hz.sweek.top/gtzwrvciia.html

Py:   if __name__ == "__main__":
来源：http://hz.hfpthk.cn/gtcmryxxat.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shangyingyoupin.top/gtwgucedwh.html

JS:   require.main === module
来源：http://hz.ybcxt.top/gtoqsvckxy.html

TS:   require.main === module
来源：http://hz.shanyushiyangtech.top/gtczfiaeoc.html

Java: public static void main(String[] args)
来源：http://hz.jinghuilouyu.cn/gtoluuvioc.html

Go:   func main()
来源：http://hz.pengpengdd.cyou/gtvwkatqvk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sweek.top/gtpgznzvah.html

C#:   static void Main(string[] args)
来源：http://hz.nanxuanxn.top/gttunvruno.html

[M08] 获取系统与运行时信息
来源：http://hz.wangshuangyany.cn/gtklqfrzxt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.tianlin.xyz/gtnnzspqbz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ppjwa.cn/gtqvabanzw.html

JS:   process.platform;  process.version
来源：http://hz.quarkkingdee.top/gtbywqsfot.html

TS:   process.platform;  process.version
来源：http://hz.daxiang520.top/gtauoxahlr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hysaishi.cn/gtwdibxfeu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.havefunace.top/gtqhyzdnpj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yvedp.cn/gtifakzrtb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jlsjyb.cn/gtmwbthxeq.html

================================================================================
来源：http://hz.jinqigfzy.top/gtjzluvwkh.html

N. 数据结构与算法
来源：http://hz.yonumen.top/gtpntelmhx.html

================================================================================
来源：http://hz.9152youxi.cn/gtjheconjv.html

[N01] 二分查找（有序数组）
来源：http://hz.gaohongyu789.top/gtqugcztfg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.bjfxy.top/gtrpjhzgtr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jlsjyb.cn/gtnpmoztbt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cqqwz.cn/gtkymeywmu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.birdmap.top/gtgtydsibo.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ivvv.top/gtjpjvbtmt.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtwvuypmzl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.dianchejie.cn/gtzjgqpwwu.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.c1oappe.top/gtfmqbhrlx.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yanxiufei.cn/gtoljetmbe.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sweek.top/gtvlaeagty.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hywenlv.cn/gtbzdfvmxd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.c1oappe.top/gtlvnuhfsa.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gogol.net.cn/gtuzfejitc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhaomingkeji.xyz/gtwptzbssg.html

Go:   slices.Sort(arr)
来源：http://hz.zhixingplan.top/gtmgbkqlzt.html

Ruby: arr.sort
来源：http://hz.zhaomingkeji.xyz/gtpzprxudd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhixingplan.top/gtlypefrtu.html

[N03] 快速排序（分治示例）
来源：http://hz.xuetiantiany.cn/gtgutpmjcw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.sweek.top/gtvddydxhp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.9152youxi.cn/gtyzpadqkk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pengpengdd.cyou/gtvxshiiln.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shuidangran.top/gtlqxvlpir.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.guannengcc.top/gtxictnztl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.haohaochexian.top/gtahxgvydu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xziqi.cn/gteehrfdkg.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cdnleiting.top/gtmxnmziqn.html

[N04] 斐波那契数列
来源：http://hz.aibaodan.cn/gtoikahaek.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.0kj1m.cn/gtpcuegggr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xuanzx.com/gtzaufqkvj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.snrcjt.cn/gtlrqzfhnj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ehwqpu.com/gtvpeezxfk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.pycfn.com/gtgsqucjli.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hywenlv.cn/gthqdvmdva.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shzxlz.cn/gtmasoeazx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xuanzx.com/gtbnxjkrel.html

[N05] 最大公约数
来源：http://hz.pycfn.com/gtxgqwsidb.html

Py:   math.gcd(a, b)
来源：http://hz.52xcode.cn/gtyfjdkgwd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.wangshuangyany.cn/gtypfagldl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangshuangyany.cn/gtldfcnlku.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.0kj1m.cn/gtfybqtpfv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jianghu66.top/gtahnxhsuc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xingfuxueyuan.xyz/gtanupfhhi.html

Ruby: a.gcd(b)
来源：http://hz.jqgufenzy.top/gtoshjlloa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shuidangran.top/gtmvvqsxsf.html

[N06] 判断回文字符串
来源：http://hz.hammf.cn/gtdtmprkqr.html

Py:   s == s[::-1]
来源：http://hz.ybcxt.top/gtxqverwxi.html

PHP:  $s === strrev($s);
来源：http://hz.yueranfly.top/gtbklkrzrp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtnfjvmftn.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jinghuilouyu.cn/gtdndqelbp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.nwbrower.top/gtkzqvqcrh.html

Go:   // 双指针从两端比较
来源：http://hz.chenzaomai.com/gtutfcorda.html

Ruby: s == s.reverse
来源：http://hz.jqgfzy.top/gtrmoyccjq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jianghu66.top/gtvxvangeh.html

[N07] 两数之和（返回下标）
来源：http://hz.xinyue.icu/gtoqqwgwoa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ybcxt.top/gtgqfkqwwo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xingfuxueyuan.xyz/gtsbhemhnq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yonumen.top/gtsyaggfsc.html

TS:   // 手写 Map<string, number>
来源：http://hz.pengpengdd.cyou/gtdsjusxki.html

Java: // 手写 HashMap
来源：http://hz.shzxlz.cn/gterkitxdg.html

Go:   // 手写 map[int]int
来源：http://hz.jlsjyb.cn/gtuqoapdfc.html

Ruby: // 手写 Hash
来源：http://hz.nwbrower.top/gtkifgpszx.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.0kj1m.cn/gtjarxdjis.html

[N08] 生成全排列
来源：http://hz.zdqjudy.top/gtbdwwuntz.html

Py:   itertools.permutations(arr)
来源：http://hz.jinghuilouyu.cn/gtnuiaiahg.html

PHP:  // 手写递归交换
来源：http://hz.jinqigufen.top/gtldvzozzt.html

JS:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtabbdzmyp.html

TS:   // 手写回溯递归
来源：http://hz.cqqwz.cn/gtpcjqvgow.html

Java: // 手写回溯递归
来源：http://hz.aizwys.cn/gtruwuohab.html

Go:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtbfdhyhsd.html

Ruby: arr.permutation.to_a
来源：http://hz.ppjwa.cn/gtmfppedth.html

C#:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtcokvrfom.html

[N09] 栈与队列
来源：http://hz.jqgfzy.top/gtvtuormzt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhaomingkeji.xyz/gtgscyfgzj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinqigufen.top/gttnymbbfu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.guowangkeji.top/gtpyfwpncb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj20258.top/gtnusqifqo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.pengpengdd.cyou/gtinvxfomr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.andypj.xyz/gtjcltegrf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.tianlin.xyz/gtaburnsux.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ivvv.top/gtvfukfbhk.html

[N10] 链表节点定义
来源：http://hz.redwolf501.top/gtrnnzxqav.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.aizwys.cn/gtgjhdwaqt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ydjk.org.cn/gtqrzelqsp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj202588.top/gtqwphparu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.pengpengdd.cyou/gtjhpvllms.html

Java: class Node { int v; Node next; }
来源：http://hz.ivvv.top/gtuzxosiho.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhengqikj.top/gtelehheyb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yuanzhike.top/gtklkisxqe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shangyingyoupin.top/gtluxtxxyy.html

[N11] 二叉树中序遍历
来源：http://hz.vqdsnc.cn/gtocixnreu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xuanzx.com/gtmfwkdwhn.html

PHP:  // 手写递归函数
来源：http://hz.daria6918.cn/gtljomoptx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aizwys.cn/gtbggioptb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxinkj.top/gtofpynrse.html

Java: // 手写递归
来源：http://hz.cashguo.top/gtrfyddwgv.html

Go:   // 手写递归
来源：http://hz.birdmap.top/gtpifnroes.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cdnleiting.top/gthlnujwxb.html

C#:   // 手写递归
来源：http://hz.zhiwuduotai.top/gtqblmjcuv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gzhubu.top/gtwhuzyfdy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.bjfxy.top/gtilbelgyi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xingfuxueyuan.xyz/gtpjwdlobw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yuanzhike.top/gtcylxnrrz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aibaodan.cn/gtytnhzfbf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ybcxt.top/gtajpudhgv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shangyingyoupin.top/gtrerbhzgr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jyoumei.cn/gtrtpmpokv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xingfuxueyuan.xyz/gtqikpypzn.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtffqllcjz.html

O. 并发与异步
来源：http://hz.gaohongyu789.top/gtwdfuagzb.html

================================================================================
来源：http://hz.mhx1999.top/gtrngvhqwp.html

[O01] 启动一个线程
来源：http://hz.jinqigfzy.top/gtiellcxbf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ivvv.top/gthjpiwfsn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.birdmap.top/gtqfghdydk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gaohongyu789.top/gtctaikacn.html

TS:   // 同 JS
来源：http://hz.xuanzx.com/gtmleeqjwv.html

Java: new Thread(() -> f()).start()
来源：http://hz.yongpay.top/gtqftqpchh.html

Go:   go f()
来源：http://hz.9152youxi.cn/gthxzhwdmc.html

Ruby: Thread.new { f }
来源：http://hz.jinqigfzy.top/gtpigubwyq.html

C#:   Task.Run(() => F());
来源：http://hz.yvedp.cn/gtwmhjtdip.html

[O02] 使用线程池
来源：http://hz.chenzaomai.com/gtbppeawnv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ydjk.org.cn/gthqsmihdy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.chenlongwang.top/gtjvemxrmn.html

JS:   // worker_threads 线程池
来源：http://hz.yj20258.top/gtjoxfgutb.html

TS:   // worker_threads 线程池
来源：http://hz.zhongyouzk.top/gtmtegomco.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xingfuxueyuan.xyz/gtpomqkfzf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ivvv.top/gtllxbhyqi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ehwqpu.com/gtuvteivau.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xingfuxueyuan.xyz/gtdjentrrh.html

[O03] 加锁保护共享数据
来源：http://hz.xinyue.icu/gtnebbospx.html

Py:   with lock: shared += 1
来源：http://hz.c1oappe.top/gtelvxxtrg.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhoulong.xyz/gtitgpjqes.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hnqzz.top/gtuwkxscca.html

TS:   // 同 JS
来源：http://hz.nanxuanxn.top/gtznfwyhbc.html

Java: synchronized (this) { shared++; }
来源：http://hz.cdnleiting.top/gtgrdubzyr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yj20258.top/gtvddzuzon.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cucudq.cn/gtjgjwvnws.html

C#:   lock (gate) { shared++; }
来源：http://hz.wangdashe.top/gtuewppzts.html

[O04] 定义异步函数并等待
来源：http://hz.bjfxy.top/gtjotryrez.html

Py:   async def f():⏎    await g()
来源：http://hz.cheryme.top/gtqnfmgsai.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nanxuanxn.top/gthutoaxvx.html

JS:   async function f() { await g(); }
来源：http://hz.quarkkingdee.top/gtzyypyklk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.meibo888.top/gtbpkbizrf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shzxlz.cn/gtwkmtleai.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hnqzz.top/gthipdhqmw.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhongyouzk.top/gtyyoodgfo.html

C#:   async Task F() { await G(); }
来源：http://hz.mhx1999.top/gtwzvkutzj.html

[O05] 并发执行并等待全部完成
来源：http://hz.dashuyun.cn/gtlrowaamt.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ydjk.org.cn/gtpxwwxnni.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jinqigfzy.top/gtkegiznrr.html

JS:   await Promise.all(tasks)
来源：http://hz.daria6918.cn/gthvazjhfb.html

TS:   await Promise.all(tasks)
来源：http://hz.fengsongda.top/gtelbdkdic.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xuetiantiany.cn/gtbwdyzwqb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.snrcjt.cn/gtdymfoqsd.html

Ruby: threads.map(&:join)
来源：http://hz.daria6918.cn/gtfjorgzgm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cucudq.cn/gtnvvijdmy.html

[O06] 使用进程池
来源：http://hz.gotoacloud.top/gtkrrpprwq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhijiandao.cn/gtniqpmead.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.dianchejie.cn/gthtqlcoju.html

JS:   // child_process / cluster 模块
来源：http://hz.yongpay.top/gtlwjnkooa.html

TS:   // child_process / cluster 模块
来源：http://hz.hywenlv.cn/gtkpujlkvj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.havefunace.top/gtfegxncmx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.cashguo.top/gttucnbyut.html

Ruby: // fork 块
来源：http://hz.havefunace.top/gtcruiklhy.html

C#:   Parallel.For
来源：http://hz.zhiwuduotai.top/gtqwoxnihh.html

================================================================================
来源：http://hz.guowangkeji.top/gtajmkzffv.html

P. 常用工具函数
来源：http://hz.jinyuanbaomall.cn/gtkmbjclxy.html

================================================================================
来源：http://hz.jqgfzy.top/gtlozajafq.html

[P01] 生成 UUID
来源：http://hz.pycfn.com/gtjpisnofw.html

Py:   str(uuid.uuid4())
来源：http://hz.hfpthk.cn/gtnqahvsoe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.tanke756.top/gtohvhuhwp.html

JS:   crypto.randomUUID()
来源：http://hz.sufxvd.cn/gtkqxpfbxw.html

TS:   crypto.randomUUID()
来源：http://hz.yangfankeji.com/gtedalslpl.html

Java: UUID.randomUUID().toString()
来源：http://hz.316326.xyz/gtbctqockm.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jinqigufen.top/gtcwmyznyb.html

Ruby: SecureRandom.uuid
来源：http://hz.hysaishi.cn/gtbqnzwzuq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hywenlv.cn/gtrpxayzci.html

[P02] MD5 / SHA256 摘要
来源：http://hz.chenzaomai.com/gtcsprtsdw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gzhubu.top/gtfbvfeiwv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yj20258.top/gtpolqvyea.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.c1oappe.top/gtoiwpjkjw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.tanke756.top/gtcqpefpqj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhoulong.xyz/gtrhvmaikc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jyoumei.cn/gtwwmehdte.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.guowangkeji.top/gtdzgnduyc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shuidangran.top/gtdfyggluc.html

[P03] 生成短随机字符串
来源：http://hz.fzhhl.top/gtllrzofsc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.wangshuangyany.cn/gtabxbueho.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.havefunace.top/gtykknucsa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhoulong.xyz/gtonnjptcf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cheryme.top/gtyvijrhdm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.tian-w.cn/gtnjafdqjw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xziqi.cn/gtntphtvcv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shzxlz.cn/gtdnlosmyo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cashguo.top/gtlebyuuxn.html

[P04] 求长度
来源：http://hz.jinqigufen.top/gttlqnyvef.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.quarkkingdee.top/gtdcfecwts.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.iojbl.cn/gtghcenxut.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj202588.top/gttywfbxlx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xuanzx.com/gtvjigzkdp.html

Java: list.size();  map.size();  s.length()
来源：http://hz.svipenyu.cn/gtggxhfxwx.html

Go:   len(arr);  len(m)
来源：http://hz.yongpay.top/gtkewcojfm.html

Ruby: x.length;  x.size
来源：http://hz.tianlin.xyz/gthykvglya.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.haohaochexian.top/gtmptvoyyr.html

[P05] 判断两个对象内容是否相等
来源：http://hz.pengpengdd.cyou/gtetyyvupt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cheryme.top/gtfdglaoeq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xuanzx.com/gtiscwmajw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.iojbl.cn/gtbdhgpadi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgufenzy.top/gtqmhccnjv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.gogol.net.cn/gtlgtqhvbl.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.vqdsnc.cn/gtbrorliyl.html

Ruby: a == b
来源：http://hz.sxryk.cn/gttkrnrhks.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.kuanghao11.cn/gtjhzutdih.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ehwqpu.com/gtvzphnccb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yuanzhike.top/gtxnqfppff.html

PHP:  if (empty($x)) {}
来源：http://hz.jinqigufen.top/gthshyeysb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.chenzaomai.com/gtkdyxqfaj.html

TS:   if (x == null) {}
来源：http://hz.kuanghao11.cn/gtuhkbtosl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.tanke756.top/gtrxibvaag.html

Go:   if x == nil {}
来源：http://hz.svipenyu.cn/gtpkpynywg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jinqigfzy.top/gtkauceapx.html

C#:   if (x is null) {}
来源：http://hz.pengpengdd.cyou/gthdpzuklf.html

[P07] 防抖与节流
来源：http://hz.guannengcc.top/gthdygwirp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.svipenyu.cn/gtcwemfyjc.html

PHP:  // 手写时间戳比较
来源：http://hz.zhaomingkeji.xyz/gtcyttncdq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zycfv.cn/gtdexxcmzq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenzaomai.com/gtycschedm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sysykeji.top/gtrnbuisbo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.meibo888.top/gtylzqxcmg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.chenjidiqi.icu/gtrurjmerf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.tian-w.cn/gtcwdcijru.html

[P08] 处理浮点精度问题
来源：http://hz.shanyushiyangkeji.top/gtwulfjvax.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.gaohongyu789.top/gtppnrcmrj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zycfv.cn/gtycxfccpt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xuanzx.com/gtkzeowddn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.feifeiyinyue.top/gtfdhgsbde.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cheryme.top/gtntaklfyr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yuxming.cn/gtssiowpls.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yanxiufei.cn/gthhwqbadr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.kuanghao11.cn/gtlacqetjn.html

================================================================================
来源：http://hz.tanke756.top/gtgwrgqyzb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hywenlv.cn/gtvgrgoocb.html

================================================================================
来源：http://hz.cdnleiting.top/gtkgvuwmqj.html

[Q01] 创建表
来源：http://hz.iojbl.cn/gtbwjwtirx.html

CREATE TABLE users (
来源：http://hz.jinqigufen.top/gtdbaqoirq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.andypj.xyz/gtnawprnpy.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yuanzhike.top/gtdkeofnro.html

email VARCHAR(100) UNIQUE,
来源：http://hz.aibaodan.cn/gtgypsbinw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.quarkkingdee.top/gtwcycpmjx.html

);
来源：http://hz.aibaodan.cn/gtcwobiqav.html

[Q02] 创建带外键的表
来源：http://hz.haohaochexian.top/gtwxplkfsy.html

CREATE TABLE orders (
来源：http://hz.shzxlz.cn/gtecfbsfwl.html


<!-- 参考信息 -->