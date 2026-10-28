代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhengqikj.top/gtzlkrnrqs.html

[M05] 设置退出码
来源：http://hz.nwbrower.top/gtpsfewocg.html

Py:   sys.exit(1)
来源：http://hz.chenlongwang.top/gtqitoxwoh.html

PHP:  exit(1);
来源：http://hz.zdqjudy.top/gtuaoetlpj.html

JS:   process.exit(1)
来源：http://hz.sxryk.cn/gtgjzbwjyk.html

TS:   process.exit(1)
来源：http://hz.dashuyun.cn/gtizjhtodc.html

Java: System.exit(1)
来源：http://hz.xylfe.cn/gtjxhoflfa.html

Go:   os.Exit(1)
来源：http://hz.yanxiufei.cn/gtrfvqyvfp.html

Ruby: exit 1
来源：http://hz.svipenyu.cn/gtpwbmzwof.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xingfuxueyuan.xyz/gteveamwhf.html

[M06] 向标准错误输出
来源：http://hz.xingfuxueyuan.xyz/gtugrcajnc.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xuetiantiany.cn/gtlacuzenu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cheryme.top/gtdcgokoop.html

JS:   console.error("err")
来源：http://hz.zhengqikj.top/gtkxpzavek.html

TS:   console.error("err")
来源：http://hz.hywenlv.cn/gtzkbttykh.html

Java: System.err.println("err")
来源：http://hz.shuidangran.top/gtslbaydfp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shangyingyoupin.top/gtxgtgfnam.html

Ruby: warn "err"
来源：http://hz.haohaochexian.top/gtbkthdqsv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.aizwys.cn/gtqquecpge.html

[M07] 判断是否为主入口
来源：http://hz.hysaishi.cn/gthwekfnde.html

Py:   if __name__ == "__main__":
来源：http://hz.hfpthk.cn/gtvhhfmczs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shzxlz.cn/gttlgmsaci.html

JS:   require.main === module
来源：http://hz.jinqigfzy.top/gtbiiftuxy.html

TS:   require.main === module
来源：http://hz.svipenyu.cn/gthuzsodxk.html

Java: public static void main(String[] args)
来源：http://hz.snrcjt.cn/gtagdavfdy.html

Go:   func main()
来源：http://hz.xingfuxueyuan.xyz/gtnhsczbtn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yuxming.cn/gtfyyghymp.html

C#:   static void Main(string[] args)
来源：http://hz.shanyushiyangkeji.top/gtiznbxjqc.html

[M08] 获取系统与运行时信息
来源：http://hz.yonumen.top/gtnkwdhbho.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gaohongyu789.top/gtbiwpshef.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.nanxinkj.top/gtouvudfyf.html

JS:   process.platform;  process.version
来源：http://hz.yj202588.top/gtisjqfzuf.html

TS:   process.platform;  process.version
来源：http://hz.ehwqpu.com/gtihukrfwv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.havefunace.top/gtxpjwjdkh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yangfankeji.com/gtaoqdtgbu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xuetiantiany.cn/gtpijtisfp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.dianchejie.cn/gtksiyrsvj.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtkemdlovj.html

N. 数据结构与算法
来源：http://hz.guannengcc.top/gtdnsitieo.html

================================================================================
来源：http://hz.sufxvd.cn/gtrtjqllvz.html

[N01] 二分查找（有序数组）
来源：http://hz.xuanzx.com/gtlanxbzai.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hongshengwenyu.top/gtecgtdcke.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.52xcode.cn/gtlhoxquge.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hammf.cn/gtcsmjswlb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xziqi.cn/gtfvsupstn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.quarkkingdee.top/gturxsfsbz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yangfankeji.com/gtlufeowtv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.cqqwz.cn/gtwjetsymi.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shangyingyoupin.top/gthfvfvevd.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhengqikj.top/gtfbohmjch.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xylfe.cn/gtdrhvugvo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.feifeiyinyue.top/gtdaihucsq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.redwolf501.top/gttoreyvjf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aibaodan.cn/gtxlbewdfj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xziqi.cn/gthrnckiiq.html

Go:   slices.Sort(arr)
来源：http://hz.fzhhl.top/gtuntlzzkf.html

Ruby: arr.sort
来源：http://hz.sufxvd.cn/gtrocnzlyi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sweek.top/gtyagyfkmd.html

[N03] 快速排序（分治示例）
来源：http://hz.tian-w.cn/gtrhepkbye.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xylfe.cn/gtohpzchft.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xylfe.cn/gtbiaffbuf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pengpengdd.cyou/gtsnhilzmh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydjk.org.cn/gtrmrudkvt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.nanxinkj.top/gtzdubwepa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.gzhubu.top/gtxvpbfipe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.316326.xyz/gtpaaicpcp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ydjk.org.cn/gtnuzqcxvf.html

[N04] 斐波那契数列
来源：http://hz.hfpthk.cn/gtfupmevlr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ydjk.org.cn/gtkejruvqd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sysykeji.top/gtwakpscmb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jianghu66.top/gtahhvyity.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ywan-chungtsiang.top/gtjltjkwsa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hnqzz.top/gtkepychmw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.pengpengdd.cyou/gtznelzftm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yueranfly.top/gtmbpspwsu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.tanke756.top/gthrmnjght.html

[N05] 最大公约数
来源：http://hz.haohaochexian.top/gtsnigspfp.html

Py:   math.gcd(a, b)
来源：http://hz.nwbrower.top/gtmepcqbws.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.wangshuangyany.cn/gturwgzjtd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.vqdsnc.cn/gtmvazcvyh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gtiwdzvvip.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.mhx1999.top/gtdktsmtdy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jlsjyb.cn/gtdabjwktw.html

Ruby: a.gcd(b)
来源：http://hz.pengpengdd.cyou/gtqywayppl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.chenzaomai.com/gtynqovuyh.html

[N06] 判断回文字符串
来源：http://hz.snrcjt.cn/gtbaklmwqc.html

Py:   s == s[::-1]
来源：http://hz.tanke756.top/gtlvjrirpu.html

PHP:  $s === strrev($s);
来源：http://hz.jqgfzy.top/gtpxpexrix.html

JS:   s === [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtxzndxave.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jiagoushi.top/gtiouhzshr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.havefunace.top/gtkheuufvo.html

Go:   // 双指针从两端比较
来源：http://hz.hnxiangtu.top/gthbpybskm.html

Ruby: s == s.reverse
来源：http://hz.nanxinkj.top/gtajonkzyb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.dianchejie.cn/gtqddphrag.html

[N07] 两数之和（返回下标）
来源：http://hz.xinyue.icu/gtsunvsvvw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.iojbl.cn/gtsauxoono.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jianghu66.top/gtbsywxrwp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.cheryme.top/gtuvziziai.html

TS:   // 手写 Map<string, number>
来源：http://hz.hnqzz.top/gtwxkkquad.html

Java: // 手写 HashMap
来源：http://hz.nanxinkj.top/gtudmlvkqb.html

Go:   // 手写 map[int]int
来源：http://hz.vqdsnc.cn/gtzzkuheou.html

Ruby: // 手写 Hash
来源：http://hz.cheryme.top/gtttbwljau.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shzxlz.cn/gteopwjwzv.html

[N08] 生成全排列
来源：http://hz.cashguo.top/gtgaxusnwu.html

Py:   itertools.permutations(arr)
来源：http://hz.yongpay.top/gtnmktfqqd.html

PHP:  // 手写递归交换
来源：http://hz.yuxming.cn/gtyhjbeoiq.html

JS:   // 手写回溯递归
来源：http://hz.zhongyouzk.top/gtmongmktv.html

TS:   // 手写回溯递归
来源：http://hz.yueranfly.top/gttjtorxoe.html

Java: // 手写回溯递归
来源：http://hz.xuanzx.com/gtmgoolxuz.html

Go:   // 手写回溯递归
来源：http://hz.wangdashe.top/gtoomsfzgg.html

Ruby: arr.permutation.to_a
来源：http://hz.yj202588.top/gtheotbjyo.html

C#:   // 手写回溯递归
来源：http://hz.yuxming.cn/gticvbaxdm.html

[N09] 栈与队列
来源：http://hz.shzxlz.cn/gtbcyiyfrm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.wangdashe.top/gtfdsohlcq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zycfv.cn/gtwlmbrdyc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.havefunace.top/gtjtwffhfz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.kuanghao11.cn/gtsttivwff.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.nwbrower.top/gtkhcryroa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.daxiang520.top/gtmylrjmtq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hywenlv.cn/gthphdoqhh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xuanzx.com/gtdvekmlut.html

[N10] 链表节点定义
来源：http://hz.gogol.net.cn/gtbaokzayn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.daria6918.cn/gtrkjvtnlc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cqqwz.cn/gtclywogri.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.redwolf501.top/gtblbtlniy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.daria6918.cn/gttuskwnfg.html

Java: class Node { int v; Node next; }
来源：http://hz.birdmap.top/gtydrrsdal.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hfpthk.cn/gtuuhlxcwa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinghuilouyu.cn/gtmxelgdpn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cashguo.top/gtxqziukzj.html

[N11] 二叉树中序遍历
来源：http://hz.daria6918.cn/gtfkqzxkis.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.aibaodan.cn/gtrxmaacls.html

PHP:  // 手写递归函数
来源：http://hz.jqgufenzy.top/gtypdxiqld.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xziqi.cn/gtrzohrebc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sweek.top/gtxqlmswwg.html

Java: // 手写递归
来源：http://hz.birdmap.top/gtcqwdvich.html

Go:   // 手写递归
来源：http://hz.feifeiyinyue.top/gttemcjcuk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cashguo.top/gtkzagsjto.html

C#:   // 手写递归
来源：http://hz.xylfe.cn/gtzqjuybjw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.52xcode.cn/gtzphlyakj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinyuanbaomall.cn/gtotkzdjvg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yj20258888.top/gtssjbwtfl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.snrcjt.cn/gtddfrxssv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinqigufen.top/gtosegetia.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuetiantiany.cn/gtcdtowocp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhoulong.xyz/gtipbcfhuf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinqigufen.top/gttxtittrz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ivvv.top/gtwtakzvdh.html

================================================================================
来源：http://hz.jinqigufen.top/gtnqtlxnfw.html

O. 并发与异步
来源：http://hz.svipenyu.cn/gtspuayjdk.html

================================================================================
来源：http://hz.haohaochexian.top/gtmumqsjpm.html

[O01] 启动一个线程
来源：http://hz.cucudq.cn/gtoqvgemsf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sysykeji.top/gtefdqoyts.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hnxiangtu.top/gtthwlihhi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.guannengcc.top/gtsiptxpem.html

TS:   // 同 JS
来源：http://hz.snrcjt.cn/gttnrrwbnk.html

Java: new Thread(() -> f()).start()
来源：http://hz.cheryme.top/gtbltftgrt.html

Go:   go f()
来源：http://hz.ydzc1.top/gtwbcbwyuq.html

Ruby: Thread.new { f }
来源：http://hz.yj20258.top/gtmhepdvsp.html

C#:   Task.Run(() => F());
来源：http://hz.cqqwz.cn/gtxptdfcdk.html

[O02] 使用线程池
来源：http://hz.wangshuangyany.cn/gtbnbapuvf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ivvv.top/gtcoohalwn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yj202588.top/gtlbvgryud.html

JS:   // worker_threads 线程池
来源：http://hz.cashguo.top/gtikddzkpa.html

TS:   // worker_threads 线程池
来源：http://hz.hfpthk.cn/gtzfbaafzn.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.gotoacloud.top/gtkaqpwqni.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.dianchejie.cn/gtqgtjvtmw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gaohongyu789.top/gtdwgrwnzx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shanyushiyangtech.top/gtvgaqhjww.html

[O03] 加锁保护共享数据
来源：http://hz.cdnleiting.top/gtkxpjnxnx.html

Py:   with lock: shared += 1
来源：http://hz.shanyushiyangkeji.top/gttvdzfpgh.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yuxming.cn/gtblrekvcb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hammf.cn/gtpnbywfad.html

TS:   // 同 JS
来源：http://hz.zhiwuduotai.top/gteejfoiko.html

Java: synchronized (this) { shared++; }
来源：http://hz.kuanghao11.cn/gtwbttyhsh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hnqzz.top/gtmuyoqeqz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hfpthk.cn/gtuvmaxmzo.html

C#:   lock (gate) { shared++; }
来源：http://hz.jinghuilouyu.cn/gtlnrdqxej.html

[O04] 定义异步函数并等待
来源：http://hz.snrcjt.cn/gtmwkjbges.html

Py:   async def f():⏎    await g()
来源：http://hz.svipenyu.cn/gtshiwqkfg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nwbrower.top/gtswuydbss.html

JS:   async function f() { await g(); }
来源：http://hz.hnxiangtu.top/gtpsvbnmqp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jinyuanbaomall.cn/gtzjtdvwih.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.tian-w.cn/gtlslmexdm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.smart0.xyz/gtiqvuyrss.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.dianchejie.cn/gtvrfddecr.html

C#:   async Task F() { await G(); }
来源：http://hz.hnqzz.top/gtrgymxbch.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinghuilouyu.cn/gtykfbslbr.html

Py:   asyncio.gather(*tasks)
来源：http://hz.fzhhl.top/gthgjuqwsh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.guannengcc.top/gttveuoypn.html

JS:   await Promise.all(tasks)
来源：http://hz.dianchejie.cn/gtbbgbfrgp.html

TS:   await Promise.all(tasks)
来源：http://hz.gaohongyu789.top/gtytfaprvc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.guannengcc.top/gtpkltnala.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xylfe.cn/gtwdteomxg.html

Ruby: threads.map(&:join)
来源：http://hz.tanke756.top/gttwclndpv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhaomingkeji.xyz/gtzrkpvzkj.html

[O06] 使用进程池
来源：http://hz.jinqigfzy.top/gtcbhlcqim.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.52xcode.cn/gtsfvtrtgm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.chenzaomai.com/gtxjsnwbzo.html

JS:   // child_process / cluster 模块
来源：http://hz.zhoulong.xyz/gtzoiztroh.html

TS:   // child_process / cluster 模块
来源：http://hz.quarkkingdee.top/gtvvuwacgw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cheryme.top/gtvxldmnwl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.iojbl.cn/gtpghksrki.html

Ruby: // fork 块
来源：http://hz.guannengcc.top/gttdublqxk.html

C#:   Parallel.For
来源：http://hz.cqqwz.cn/gtggwlfnbr.html

================================================================================
来源：http://hz.ivvv.top/gtmizpiwoz.html

P. 常用工具函数
来源：http://hz.aibaodan.cn/gtghdgnmoe.html

================================================================================
来源：http://hz.jianghu66.top/gtjezizmzj.html

[P01] 生成 UUID
来源：http://hz.cashguo.top/gtjztlxxzc.html

Py:   str(uuid.uuid4())
来源：http://hz.dashuyun.cn/gtmrjgokhj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.mhx1999.top/gtbmocrsok.html

JS:   crypto.randomUUID()
来源：http://hz.yj202588.top/gtqkvvpawz.html

TS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtsklebwfo.html

Java: UUID.randomUUID().toString()
来源：http://hz.meibo888.top/gtdaikhths.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gogol.net.cn/gtiwzyppxz.html

Ruby: SecureRandom.uuid
来源：http://hz.zhixingplan.top/gtudjlgupv.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.guannengcc.top/gtirgfbqru.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xylfe.cn/gtvendamzk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shangyingyoupin.top/gtkgllbmaf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ydzc1.top/gtebllnavy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cucudq.cn/gtveanotla.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.guannengcc.top/gtxfmwaqpc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.snrcjt.cn/gtgnbpgbhi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cucudq.cn/gtzrhkedyu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hnxiangtu.top/gtmvdzjasy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.tian-w.cn/gtetfnwtij.html

[P03] 生成短随机字符串
来源：http://hz.yongpay.top/gtevfzogfz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shzxlz.cn/gtemzvabdn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gotoacloud.top/gtuqksoilj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.aizwys.cn/gthxmmpefx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenlongwang.top/gtcuqqqgsj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yongpay.top/gtskbejjbf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jinyuanbaomall.cn/gteeywfxah.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sweek.top/gtqnzbgzwt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hnxiangtu.top/gtdefgthmw.html

[P04] 求长度
来源：http://hz.tanke756.top/gtvrkqzhcc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.52xcode.cn/gtzqivygei.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.c1oappe.top/gtccqaysfb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xinyue.icu/gtiduxopnb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnxiangtu.top/gtwxcjcpsv.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yj202588.top/gtfaqhdiyg.html

Go:   len(arr);  len(m)
来源：http://hz.zhiwuduotai.top/gtyrhrytvt.html

Ruby: x.length;  x.size
来源：http://hz.sufxvd.cn/gtracddedd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yuxming.cn/gtzccokvfq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhoulong.xyz/gtcaipdosi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xinyue.icu/gtvmliopkf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sysykeji.top/gtvnhvdqfh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jinghuilouyu.cn/gtfvxiojvn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.birdmap.top/gtbdvrrkff.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.snrcjt.cn/gtkjbvcgwz.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.nwbrower.top/gtotqgudmb.html

Ruby: a == b
来源：http://hz.0kj1m.cn/gtxjepkfwq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.birdmap.top/gtpvhbrrgs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xuanzx.com/gtjsoktepk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hnqzz.top/gtrhxddykt.html

PHP:  if (empty($x)) {}
来源：http://hz.yonumen.top/gtraltfpiv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhijiandao.cn/gtchvexxgc.html

TS:   if (x == null) {}
来源：http://hz.gaohongyu789.top/gtmhuxnmlo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.cqqwz.cn/gtphfsetjk.html

Go:   if x == nil {}
来源：http://hz.mhx1999.top/gtexktsrfl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xziqi.cn/gtqraosiok.html

C#:   if (x is null) {}
来源：http://hz.hnqzz.top/gtfvurxtho.html

[P07] 防抖与节流
来源：http://hz.zhongyouzk.top/gtngzrjyax.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xziqi.cn/gtxazanjjr.html

PHP:  // 手写时间戳比较
来源：http://hz.zhaomingkeji.xyz/gtaffdpbxl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhaomingkeji.xyz/gtnbxsrprv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.0kj1m.cn/gtmsgrmgiz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.havefunace.top/gttytwhkek.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.chenlongwang.top/gtxvipasch.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhengqikj.top/gtgbtkagqv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.aizwys.cn/gtbmizhnfl.html

[P08] 处理浮点精度问题
来源：http://hz.ehwqpu.com/gtfcpbjmjk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.bjfxy.top/gtpzgxpbrc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.daria6918.cn/gtgnvrbfbj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cdnleiting.top/gtzrchdgcf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.svipenyu.cn/gtovyhratr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.0kj1m.cn/gtylzbywvc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hfpthk.cn/gtjtwawisq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.daxiang520.top/gtcwvhxycr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.dashuyun.cn/gtwkkzkcay.html

================================================================================
来源：http://hz.jqgufenzy.top/gtksfltwri.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yongpay.top/gttpuqtaqn.html

================================================================================
来源：http://hz.guowangkeji.top/gtdbpqcsdk.html

[Q01] 创建表
来源：http://hz.zhongyouzk.top/gthpfjaabc.html

CREATE TABLE users (
来源：http://hz.yanxiufei.cn/gtajkvdqub.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aibaodan.cn/gtlsonxfln.html

name VARCHAR(50) NOT NULL,
来源：http://hz.dianchejie.cn/gtfrcqtvod.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jqgfzy.top/gtyhosjown.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hfpthk.cn/gtgswgubkk.html

);
来源：http://hz.jinqigufen.top/gtpotxywxj.html

[Q02] 创建带外键的表
来源：http://hz.yueranfly.top/gtzwtcigra.html

CREATE TABLE orders (
来源：http://hz.zhiwuduotai.top/gtqgnqqukt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.pengpengdd.cyou/gtubncvpms.html

user_id INT NOT NULL,
来源：http://hz.cdnleiting.top/gtjpvxzohk.html

amount DECIMAL(10, 2),
来源：http://hz.jianghu66.top/gtvhnycwtl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jianghu66.top/gtmbswpwci.html

);
来源：http://hz.fengsongda.top/gtgzapsbtj.html

[Q03] 增加列
来源：http://hz.chenzaomai.com/gtbufugchx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xziqi.cn/gtxrdghbjq.html

[Q04] 修改列类型
来源：http://hz.ehwqpu.com/gtgnwdpakk.html


<!-- 参考信息 -->