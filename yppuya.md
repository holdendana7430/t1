代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://hz.chenzaomai.com/gtllardqwo.html

[M05] 设置退出码
来源：http://hz.hnqzz.top/gtxztptorf.html

Py:   sys.exit(1)
来源：http://hz.xuetiantiany.cn/gtkgpxlyki.html

PHP:  exit(1);
来源：http://hz.meibo888.top/gtxclkpxbn.html

JS:   process.exit(1)
来源：http://hz.xuanzx.com/gtphlabiux.html

TS:   process.exit(1)
来源：http://hz.sxryk.cn/gtirhmduiw.html

Java: System.exit(1)
来源：http://hz.hongshengwenyu.top/gtcfrzupno.html

Go:   os.Exit(1)
来源：http://hz.ydzc1.top/gtociiptiy.html

Ruby: exit 1
来源：http://hz.redwolf501.top/gtvboemevt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jiagoushi.top/gtrgocajlb.html

[M06] 向标准错误输出
来源：http://hz.cashguo.top/gtvensxhal.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ywan-chungtsiang.top/gtprtiksrt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.redwolf501.top/gtfuwzcaqr.html

JS:   console.error("err")
来源：http://hz.52xcode.cn/gttuaxthok.html

TS:   console.error("err")
来源：http://hz.daxiang520.top/gthtsfyzrh.html

Java: System.err.println("err")
来源：http://hz.xuanzx.com/gtigetuczi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yangfankeji.com/gtjmqvzntx.html

Ruby: warn "err"
来源：http://hz.c1oappe.top/gtiaezgvzi.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yuanzhike.top/gtscnkhxvb.html

[M07] 判断是否为主入口
来源：http://hz.dianchejie.cn/gtoazpzkwx.html

Py:   if __name__ == "__main__":
来源：http://hz.gogol.net.cn/gttcdovgwn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gaohongyu789.top/gtvfykbyjq.html

JS:   require.main === module
来源：http://hz.shuidangran.top/gtigljlmbd.html

TS:   require.main === module
来源：http://hz.316326.xyz/gtvipwwpdu.html

Java: public static void main(String[] args)
来源：http://hz.tianlin.xyz/gtsdrdufhm.html

Go:   func main()
来源：http://hz.tianlin.xyz/gtuhfwvntj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.iojbl.cn/gthdkizpst.html

C#:   static void Main(string[] args)
来源：http://hz.yj202588.top/gtfjtnsqje.html

[M08] 获取系统与运行时信息
来源：http://hz.shanyushiyangkeji.top/gtxlidgivw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhoulong.xyz/gtxqlddfwy.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yonumen.top/gtgbirwbwx.html

JS:   process.platform;  process.version
来源：http://hz.andypj.xyz/gtlyeopvsu.html

TS:   process.platform;  process.version
来源：http://hz.nanxinkj.top/gtwadbcarl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yuanzhike.top/gtipsceqcr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.daxiang520.top/gtccbftvcg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.daria6918.cn/gtfsixdjwv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinghuilouyu.cn/gthoqomphs.html

================================================================================
来源：http://hz.yj20258.top/gtmdoijqds.html

N. 数据结构与算法
来源：http://hz.yanxiufei.cn/gtqbxhomjx.html

================================================================================
来源：http://hz.dianchejie.cn/gtvflyftvq.html

[N01] 二分查找（有序数组）
来源：http://hz.yuxming.cn/gtqdyjplqk.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.quarkkingdee.top/gtrsgxxben.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xuetiantiany.cn/gtwxyxapit.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shuidangran.top/gtvmuxsxpo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangshuangyany.cn/gthfegpitp.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xinyue.icu/gthdhesobl.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jqgufenzy.top/gtwirygwag.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hnxiangtu.top/gtftxeewxu.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ehwqpu.com/gthdtwhrfl.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.tian-w.cn/gtreqmrvqu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.dashuyun.cn/gtneonutwq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nanxinkj.top/gtnhwjikke.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhijiandao.cn/gtymeymbjy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhijiandao.cn/gtuyagoryh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xuetiantiany.cn/gtezlisual.html

Go:   slices.Sort(arr)
来源：http://hz.daria6918.cn/gtxdbbcbbw.html

Ruby: arr.sort
来源：http://hz.zhaomingkeji.xyz/gtfvkvkazd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.kuanghao11.cn/gtnrzcibjm.html

[N03] 快速排序（分治示例）
来源：http://hz.svipenyu.cn/gtixtkrval.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jqgufenzy.top/gtyoldfwgk.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jiagoushi.top/gttigcdmfx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhoulong.xyz/gtmyzzfzxv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.bjfxy.top/gtizclquul.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yueranfly.top/gtferrfkrk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shanyushiyangtech.top/gtpsbfohpy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhoulong.xyz/gteqsmypbs.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ydzc1.top/gtcrhrddsk.html

[N04] 斐波那契数列
来源：http://hz.ywan-chungtsiang.top/gtxnbfxqwj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zycfv.cn/gtqsxysrna.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hysaishi.cn/gtpgaaekgi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.haohaochexian.top/gtuuiubwmt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jqgufenzy.top/gtfsyruzjf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yvedp.cn/gtmqnzhogj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yueranfly.top/gtnykzmvad.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cqqwz.cn/gtlyunplpp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shuidangran.top/gttuiloajs.html

[N05] 最大公约数
来源：http://hz.smart0.xyz/gtosdfpjom.html

Py:   math.gcd(a, b)
来源：http://hz.tian-w.cn/gtbgunkcaj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinghuilouyu.cn/gtommqlfug.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hywenlv.cn/gtibqdsimu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenlongwang.top/gtwboqdddv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.haohaochexian.top/gtfxdpuhwn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenjidiqi.icu/gtamkkbxav.html

Ruby: a.gcd(b)
来源：http://hz.yonumen.top/gtvtwtzkzd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cheryme.top/gtynapzrlm.html

[N06] 判断回文字符串
来源：http://hz.cashguo.top/gtmqscfnyd.html

Py:   s == s[::-1]
来源：http://hz.kuanghao11.cn/gthbussgyk.html

PHP:  $s === strrev($s);
来源：http://hz.hfpthk.cn/gtkvalnbcm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hywenlv.cn/gtpjlggarl.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtpcbxdrcv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xuetiantiany.cn/gtrhnhhyzp.html

Go:   // 双指针从两端比较
来源：http://hz.sweek.top/gtkbqgfipa.html

Ruby: s == s.reverse
来源：http://hz.nanxinkj.top/gtzbphhvwm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhiwuduotai.top/gtxnxjbvjo.html

[N07] 两数之和（返回下标）
来源：http://hz.chenjidiqi.icu/gtjyduadjy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xylfe.cn/gtziitueai.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gotoacloud.top/gtilpllqcm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.vqdsnc.cn/gtrrxghluh.html

TS:   // 手写 Map<string, number>
来源：http://hz.yangfankeji.com/gtlujossvn.html

Java: // 手写 HashMap
来源：http://hz.hfpthk.cn/gtioemhxjv.html

Go:   // 手写 map[int]int
来源：http://hz.yangfankeji.com/gthggrvtlz.html

Ruby: // 手写 Hash
来源：http://hz.zhixingplan.top/gtyhgvitxn.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.svipenyu.cn/gtlaxxdnvm.html

[N08] 生成全排列
来源：http://hz.pengpengdd.cyou/gtxzpylxvh.html

Py:   itertools.permutations(arr)
来源：http://hz.hfpthk.cn/gtexocabka.html

PHP:  // 手写递归交换
来源：http://hz.jyoumei.cn/gtjsyfdgci.html

JS:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtcmayysoi.html

TS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtubrmirav.html

Java: // 手写回溯递归
来源：http://hz.sxryk.cn/gtbukvfmtk.html

Go:   // 手写回溯递归
来源：http://hz.xziqi.cn/gtndtzilhg.html

Ruby: arr.permutation.to_a
来源：http://hz.cucudq.cn/gtxcabzzst.html

C#:   // 手写回溯递归
来源：http://hz.guowangkeji.top/gtlucgxcdl.html

[N09] 栈与队列
来源：http://hz.xylfe.cn/gtfoukzheh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.redwolf501.top/gtkohnwpoe.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.gogol.net.cn/gtnjpdmddc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yanxiufei.cn/gtgfftlwhh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hfpthk.cn/gtqureurwu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hfpthk.cn/gtuygstugg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.chenlongwang.top/gtfjircvby.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zdqjudy.top/gtlcvqngbw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ywan-chungtsiang.top/gttnnvikqs.html

[N10] 链表节点定义
来源：http://hz.jinqigufen.top/gtizgjicbg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.dashuyun.cn/gtkaeelmvp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sxryk.cn/gtlcpmkylo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.guannengcc.top/gttarmamxq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhoulong.xyz/gtirfrqrhg.html

Java: class Node { int v; Node next; }
来源：http://hz.shuidangran.top/gttuixxdbc.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.birdmap.top/gtduxeaozw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhiwuduotai.top/gtcxsvhpzv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.pycfn.com/gthlfnkdko.html

[N11] 二叉树中序遍历
来源：http://hz.ybcxt.top/gtuzwciwyp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.quarkkingdee.top/gtgndietwo.html

PHP:  // 手写递归函数
来源：http://hz.gotoacloud.top/gtabjdufjw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj20258.top/gtetpzujxo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xylfe.cn/gtwwpgcjub.html

Java: // 手写递归
来源：http://hz.svipenyu.cn/gtzagartvx.html

Go:   // 手写递归
来源：http://hz.gotoacloud.top/gtzlavlnln.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.nanxinkj.top/gtzilwmhbt.html

C#:   // 手写递归
来源：http://hz.52xcode.cn/gthexuaunj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.redwolf501.top/gtfzbavpqd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xuetiantiany.cn/gtqdzgknpy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xziqi.cn/gtpvvigtsk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinghuilouyu.cn/gtsshpciys.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.snrcjt.cn/gtrpytebhk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gotoacloud.top/gtqdkvcpee.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jqgufenzy.top/gtwnamurlf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xuetiantiany.cn/gtqucsspiz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zdqjudy.top/gtxjedqyad.html

================================================================================
来源：http://hz.svipenyu.cn/gtepropdpr.html

O. 并发与异步
来源：http://hz.jlsjyb.cn/gtwtswtjgc.html

================================================================================
来源：http://hz.hnqzz.top/gtcigakzmf.html

[O01] 启动一个线程
来源：http://hz.daria6918.cn/gtflrwmkou.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.mhx1999.top/gtywqagdll.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.daxiang520.top/gtnuorbcxh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.nwbrower.top/gtbvqbdzwb.html

TS:   // 同 JS
来源：http://hz.xylfe.cn/gtlnmmarih.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinqigfzy.top/gtgnjrfvum.html

Go:   go f()
来源：http://hz.c1oappe.top/gtjjymoaiv.html

Ruby: Thread.new { f }
来源：http://hz.hysaishi.cn/gtusgusdts.html

C#:   Task.Run(() => F());
来源：http://hz.tian-w.cn/gtemvumlxk.html

[O02] 使用线程池
来源：http://hz.feifeiyinyue.top/gtqteiefng.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.nanxuanxn.top/gtnmqphazm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shangyingyoupin.top/gtbtpcrllx.html

JS:   // worker_threads 线程池
来源：http://hz.hongshengwenyu.top/gthqmevfxs.html

TS:   // worker_threads 线程池
来源：http://hz.meibo888.top/gtzoajjpqj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.fengsongda.top/gtmpnikqcc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.feifeiyinyue.top/gtwnhmiqox.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.redwolf501.top/gtrgwbyjje.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yanxiufei.cn/gtizepania.html

[O03] 加锁保护共享数据
来源：http://hz.snrcjt.cn/gtnijnohhr.html

Py:   with lock: shared += 1
来源：http://hz.xuanzx.com/gtivkkkhxr.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.0kj1m.cn/gttcceyqlz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.sysykeji.top/gtimviwutt.html

TS:   // 同 JS
来源：http://hz.gzhubu.top/gtqcfgfsvf.html

Java: synchronized (this) { shared++; }
来源：http://hz.ivvv.top/gtwdxhwpdb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gogol.net.cn/gtpxfnaogt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hysaishi.cn/gtamnfbxbl.html

C#:   lock (gate) { shared++; }
来源：http://hz.svipenyu.cn/gthrcfbvql.html

[O04] 定义异步函数并等待
来源：http://hz.aibaodan.cn/gtuzhvswxe.html

Py:   async def f():⏎    await g()
来源：http://hz.yongpay.top/gtaqhnlqpu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yongpay.top/gtkcvqndlg.html

JS:   async function f() { await g(); }
来源：http://hz.fzhhl.top/gtcjhtojyb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.daria6918.cn/gtmsqxovvx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jqgfzy.top/gtsmllbmyn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.gzhubu.top/gtfilpnwql.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yangfankeji.com/gthmcmfjnc.html

C#:   async Task F() { await G(); }
来源：http://hz.xziqi.cn/gtqzfllfkm.html

[O05] 并发执行并等待全部完成
来源：http://hz.smart0.xyz/gtthpidiko.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jiagoushi.top/gtqrxsqpxk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.guowangkeji.top/gtucpkzthm.html

JS:   await Promise.all(tasks)
来源：http://hz.smart0.xyz/gtainmarey.html

TS:   await Promise.all(tasks)
来源：http://hz.hysaishi.cn/gtuiwtxdpu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.tianlin.xyz/gtawxiwnpj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jinqigfzy.top/gtybngnaac.html

Ruby: threads.map(&:join)
来源：http://hz.tanke756.top/gtljdbtmix.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yuxming.cn/gtorcrtopl.html

[O06] 使用进程池
来源：http://hz.yvedp.cn/gtwesjznze.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.birdmap.top/gtvoxpjife.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jyoumei.cn/gtqgeygnjo.html

JS:   // child_process / cluster 模块
来源：http://hz.sufxvd.cn/gtapefzavw.html

TS:   // child_process / cluster 模块
来源：http://hz.zhijiandao.cn/gtzonbdcfw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jqgfzy.top/gtvdqlvulj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hywenlv.cn/gtkwmtaxwg.html

Ruby: // fork 块
来源：http://hz.haohaochexian.top/gthewbmqnk.html

C#:   Parallel.For
来源：http://hz.ehwqpu.com/gtnxtqtwhj.html

================================================================================
来源：http://hz.kuanghao11.cn/gtixbsbwvt.html

P. 常用工具函数
来源：http://hz.c1oappe.top/gtetprwlae.html

================================================================================
来源：http://hz.aizwys.cn/gtfaveiltx.html

[P01] 生成 UUID
来源：http://hz.chenlongwang.top/gtbhkmayye.html

Py:   str(uuid.uuid4())
来源：http://hz.hfpthk.cn/gtyvtimxat.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yueranfly.top/gtwqojrvqz.html

JS:   crypto.randomUUID()
来源：http://hz.0kj1m.cn/gtznfnkgqc.html

TS:   crypto.randomUUID()
来源：http://hz.hammf.cn/gtofmsmvia.html

Java: UUID.randomUUID().toString()
来源：http://hz.jiagoushi.top/gtxurgbqms.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhengqikj.top/gtolqbjiue.html

Ruby: SecureRandom.uuid
来源：http://hz.hywenlv.cn/gthbfvqhkq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.feifeiyinyue.top/gtpmwolfjh.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cheryme.top/gtmcuufspk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ppjwa.cn/gtvfscfxte.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.nanxinkj.top/gtbilyrxbr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xylfe.cn/gtkpivgrto.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hywenlv.cn/gtuoqtmpwc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.birdmap.top/gtoaebfayv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.iojbl.cn/gtrpeldzav.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xingfuxueyuan.xyz/gtmqqpncnv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.gogol.net.cn/gthmtvoixu.html

[P03] 生成短随机字符串
来源：http://hz.yuxming.cn/gtahyflrtw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shanyushiyangtech.top/gtvcdjabze.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.feifeiyinyue.top/gtgnulllmk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ybcxt.top/gtxrwyvxxl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ivvv.top/gtsiudyuak.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xylfe.cn/gtqzbyfnmk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhijiandao.cn/gtwkikfymh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.9152youxi.cn/gtfwucyswq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.birdmap.top/gttwkfrtcs.html

[P04] 求长度
来源：http://hz.0kj1m.cn/gtmkemdtws.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hfpthk.cn/gthzpgdlgu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.birdmap.top/gtwmhgenkk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xylfe.cn/gtbggjndhe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xuetiantiany.cn/gtrodxajld.html

Java: list.size();  map.size();  s.length()
来源：http://hz.kuanghao11.cn/gtqdkphbna.html

Go:   len(arr);  len(m)
来源：http://hz.yanxiufei.cn/gtfirangqe.html

Ruby: x.length;  x.size
来源：http://hz.jinqigfzy.top/gtzirrivhm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.snrcjt.cn/gtfgktphgy.html

[P05] 判断两个对象内容是否相等
来源：http://hz.redwolf501.top/gtxiaaiobo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhijiandao.cn/gtjkdbiuut.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.guowangkeji.top/gtcckclnhb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shangyingyoupin.top/gtjeqdbcpf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shzxlz.cn/gturtorkpf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.andypj.xyz/gtlmiuzlba.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.nanxuanxn.top/gtiugvqfbm.html

Ruby: a == b
来源：http://hz.hammf.cn/gtbfjiwtcb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.smart0.xyz/gtzponcbkd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shanyushiyangtech.top/gtylnxklhd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yvedp.cn/gtgiegngsw.html

PHP:  if (empty($x)) {}
来源：http://hz.ppjwa.cn/gtlptvoutb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shangyingyoupin.top/gtttsqllab.html

TS:   if (x == null) {}
来源：http://hz.jqgfzy.top/gtczksifyb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhijiandao.cn/gtnijisdwn.html

Go:   if x == nil {}
来源：http://hz.zdqjudy.top/gtqrparixr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.aibaodan.cn/gttcduhxec.html

C#:   if (x is null) {}
来源：http://hz.hnxiangtu.top/gtzjaejvhg.html

[P07] 防抖与节流
来源：http://hz.gogol.net.cn/gtmfpeuvob.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.nwbrower.top/gtaxhktqxq.html

PHP:  // 手写时间戳比较
来源：http://hz.hywenlv.cn/gteqwqlzeu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.316326.xyz/gtoourvpxf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuetiantiany.cn/gtpjqecths.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jqgufenzy.top/gtvneehsjz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.mhx1999.top/gtabqhidzt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jlsjyb.cn/gtavribvtm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.birdmap.top/gtmcyxpiep.html

[P08] 处理浮点精度问题
来源：http://hz.haohaochexian.top/gtcjotcnbk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.316326.xyz/gteiffllvs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.sysykeji.top/gtsgwhaqoa.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yvedp.cn/gtabcxozxa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xuanzx.com/gtdknquumv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.dianchejie.cn/gtetbimhrq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ydjk.org.cn/gtcxzdocpf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xylfe.cn/gtoficsezy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shanyushiyangtech.top/gtvipbskeb.html

================================================================================
来源：http://hz.snrcjt.cn/gtdpsjwtfi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.daria6918.cn/gtmmbapubr.html

================================================================================
来源：http://hz.yvedp.cn/gtrucxbgac.html

[Q01] 创建表
来源：http://hz.zycfv.cn/gtqbkllbdd.html

CREATE TABLE users (
来源：http://hz.hysaishi.cn/gtzhuxspmr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinyuanbaomall.cn/gtdhdbwxnt.html

name VARCHAR(50) NOT NULL,
来源：http://hz.316326.xyz/gtkefczion.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xingfuxueyuan.xyz/gtsefhtrxg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.fzhhl.top/gtdflgqdhj.html

);
来源：http://hz.snrcjt.cn/gtqsgwrmas.html

[Q02] 创建带外键的表
来源：http://hz.aibaodan.cn/gteafjvnna.html

CREATE TABLE orders (
来源：http://hz.yj202588.top/gtiirqktch.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.kuanghao11.cn/gthmtmykup.html

user_id INT NOT NULL,
来源：http://hz.yj202588.top/gtkkmbmdye.html

amount DECIMAL(10, 2),
来源：http://hz.jinyuanbaomall.cn/gtrftzqulc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.nwbrower.top/gtpqrpbsdf.html

);
来源：http://hz.cheryme.top/gtyuxjssnp.html

[Q03] 增加列
来源：http://hz.gaohongyu789.top/gtirhdsmxo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.kuanghao11.cn/gtcrzabuzc.html

[Q04] 修改列类型
来源：http://hz.yueranfly.top/gtduadyuwy.html


<!-- 参考信息 -->