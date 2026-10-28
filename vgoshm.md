代发 wailian999

[M04] 获取当前工作目录
来源：http://hz.tian-w.cn/gtinxelbuf.html

Py:   os.getcwd()
来源：http://hz.tianlin.xyz/gtikemrfic.html

PHP:  getcwd();
来源：http://hz.jinqigufen.top/gtjdenidbi.html

JS:   process.cwd()
来源：http://hz.shangyingyoupin.top/gthfcqdwdj.html

TS:   process.cwd()
来源：http://hz.quarkkingdee.top/gtbakkibou.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yongpay.top/gtahnccsjg.html

Go:   os.Getwd()
来源：http://hz.yj20258.top/gtagtsqlie.html

Ruby: Dir.pwd
来源：http://hz.tian-w.cn/gtuyyuhoii.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xuetiantiany.cn/gtrpnugxjm.html

[M05] 设置退出码
来源：http://hz.hfpthk.cn/gtrfyfkech.html

Py:   sys.exit(1)
来源：http://hz.sufxvd.cn/gtogozzpki.html

PHP:  exit(1);
来源：http://hz.cheryme.top/gtvfdinhfq.html

JS:   process.exit(1)
来源：http://hz.ybcxt.top/gtnpavfvby.html

TS:   process.exit(1)
来源：http://hz.daria6918.cn/gtautjpbrp.html

Java: System.exit(1)
来源：http://hz.chenlongwang.top/gtcadhwddo.html

Go:   os.Exit(1)
来源：http://hz.meibo888.top/gtzjnifegx.html

Ruby: exit 1
来源：http://hz.cashguo.top/gtuevcvknh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.tanke756.top/gtbcjhnpnu.html

[M06] 向标准错误输出
来源：http://hz.xylfe.cn/gtvmaeinqt.html

Py:   print("err", file=sys.stderr)
来源：http://hz.daria6918.cn/gtcyjzfjuw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.316326.xyz/gtjezavpvc.html

JS:   console.error("err")
来源：http://hz.ydzc1.top/gthwcidjnp.html

TS:   console.error("err")
来源：http://hz.jianghu66.top/gtykrsixqz.html

Java: System.err.println("err")
来源：http://hz.zdqjudy.top/gtynzrfgnj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yj20258.top/gtehfikvon.html

Ruby: warn "err"
来源：http://hz.zhiwuduotai.top/gtuideezmh.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xylfe.cn/gtxogiiqry.html

[M07] 判断是否为主入口
来源：http://hz.yuanzhike.top/gtuparpmrv.html

Py:   if __name__ == "__main__":
来源：http://hz.316326.xyz/gtwdodvscg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xylfe.cn/gtxvlzlpcb.html

JS:   require.main === module
来源：http://hz.jinyuanbaomall.cn/gtmfkgdhdz.html

TS:   require.main === module
来源：http://hz.cucudq.cn/gtzodbpgyk.html

Java: public static void main(String[] args)
来源：http://hz.guannengcc.top/gtyfwdcqdn.html

Go:   func main()
来源：http://hz.hnxiangtu.top/gtuxwtnpue.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cheryme.top/gtubnposbv.html

C#:   static void Main(string[] args)
来源：http://hz.wangshuangyany.cn/gtxjgouadf.html

[M08] 获取系统与运行时信息
来源：http://hz.yj202588.top/gtpjdepzuq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hnqzz.top/gtlousvepe.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.nanxinkj.top/gtrpzpawkq.html

JS:   process.platform;  process.version
来源：http://hz.kuanghao11.cn/gtvwruqwix.html

TS:   process.platform;  process.version
来源：http://hz.jinqigufen.top/gtmuudulls.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhixingplan.top/gtbgpcrwlm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.fzhhl.top/gtfsaqzewe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.guannengcc.top/gtbievxlju.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj202588.top/gtgrqmivho.html

================================================================================
来源：http://hz.9152youxi.cn/gtkkkftumm.html

N. 数据结构与算法
来源：http://hz.fengsongda.top/gtbyfvkbux.html

================================================================================
来源：http://hz.yj20258.top/gtwiouqbzk.html

[N01] 二分查找（有序数组）
来源：http://hz.yuxming.cn/gtatszycjo.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hysaishi.cn/gtnjxzbcog.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.quarkkingdee.top/gtqehyhmxc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tanke756.top/gtzcqhzfew.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.svipenyu.cn/gtzoleqfwd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.pycfn.com/gtxmpcqdgd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xziqi.cn/gtkkevdltr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.snrcjt.cn/gtdcbvptwa.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ppjwa.cn/gtbptjneoa.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.c1oappe.top/gtvqtnozug.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yanxiufei.cn/gtvtlkqbum.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cheryme.top/gtivgypcyt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gtfoheulhm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xingfuxueyuan.xyz/gtdxmjgqhe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yongpay.top/gtqrqjfsci.html

Go:   slices.Sort(arr)
来源：http://hz.mhx1999.top/gtcofudnzw.html

Ruby: arr.sort
来源：http://hz.andypj.xyz/gtjpiitiln.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhoulong.xyz/gtredoscry.html

[N03] 快速排序（分治示例）
来源：http://hz.jinghuilouyu.cn/gteswjdltr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinqigufen.top/gtxtegsdsi.html

PHP:  // 递归实现，或用 usort
来源：http://hz.wangdashe.top/gtylsldfer.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shzxlz.cn/gtvjghbdqc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ivvv.top/gtqgbffgqs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jlsjyb.cn/gtovmvbeee.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ydjk.org.cn/gtfkkagdsg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.daxiang520.top/gtouwzbsyi.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yj20258.top/gtyeoeaqzj.html

[N04] 斐波那契数列
来源：http://hz.nwbrower.top/gttucswdxz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.52xcode.cn/gtvmjsnocj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hywenlv.cn/gtepmdcycw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.birdmap.top/gtzaheabnm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cqqwz.cn/gtgdukgunv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.daria6918.cn/gtktiqnftv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xinyue.icu/gtrqttiibd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jianghu66.top/gtjowpnxbx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hywenlv.cn/gtrzytetom.html

[N05] 最大公约数
来源：http://hz.nanxuanxn.top/gternycrdn.html

Py:   math.gcd(a, b)
来源：http://hz.pycfn.com/gtjajwtsmu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhoulong.xyz/gtvluaqzie.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shzxlz.cn/gtmuykhcdf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangkeji.top/gthemocgns.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.tanke756.top/gtitxwcfao.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.dianchejie.cn/gtxdyzmqfd.html

Ruby: a.gcd(b)
来源：http://hz.0kj1m.cn/gtnasynklu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xziqi.cn/gtxzhgsuzw.html

[N06] 判断回文字符串
来源：http://hz.gaohongyu789.top/gtqzxaostc.html

Py:   s == s[::-1]
来源：http://hz.ppjwa.cn/gtqlourvdu.html

PHP:  $s === strrev($s);
来源：http://hz.hfpthk.cn/gtdanttjts.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sweek.top/gtzxppocbx.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ehwqpu.com/gthxheevwe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.guowangkeji.top/gtjyvvhtzf.html

Go:   // 双指针从两端比较
来源：http://hz.vqdsnc.cn/gtvfjkttkn.html

Ruby: s == s.reverse
来源：http://hz.shanyushiyangkeji.top/gttnpbetlw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yueranfly.top/gtkknpkbdt.html

[N07] 两数之和（返回下标）
来源：http://hz.aizwys.cn/gttuihdapj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.aizwys.cn/gtqmmhtxaw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.fzhhl.top/gtglagpetf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yonumen.top/gthdjpdngs.html

TS:   // 手写 Map<string, number>
来源：http://hz.jyoumei.cn/gtexrsbijk.html

Java: // 手写 HashMap
来源：http://hz.52xcode.cn/gtutyggoxk.html

Go:   // 手写 map[int]int
来源：http://hz.daria6918.cn/gtbndqhhye.html

Ruby: // 手写 Hash
来源：http://hz.jlsjyb.cn/gtvnbxouuc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.vqdsnc.cn/gttarffiri.html

[N08] 生成全排列
来源：http://hz.yueranfly.top/gtsfsrcblo.html

Py:   itertools.permutations(arr)
来源：http://hz.hongshengwenyu.top/gtakksylnl.html

PHP:  // 手写递归交换
来源：http://hz.svipenyu.cn/gterprfmpb.html

JS:   // 手写回溯递归
来源：http://hz.cheryme.top/gtctpxxonl.html

TS:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtxxkqzumt.html

Java: // 手写回溯递归
来源：http://hz.cheryme.top/gtzjrbaqgw.html

Go:   // 手写回溯递归
来源：http://hz.ivvv.top/gtjksranqv.html

Ruby: arr.permutation.to_a
来源：http://hz.hammf.cn/gthkjlejia.html

C#:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtscrxmfxw.html

[N09] 栈与队列
来源：http://hz.9152youxi.cn/gtdpoatego.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.pengpengdd.cyou/gtxaitsozk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.bjfxy.top/gtzkylasgk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.wangdashe.top/gtidgjlbmy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.nanxinkj.top/gtqmuxvnpi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shzxlz.cn/gtopyesaat.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yongpay.top/gtinvytlvn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.andypj.xyz/gtlsphrhyx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shzxlz.cn/gtbertfnfp.html

[N10] 链表节点定义
来源：http://hz.nanxuanxn.top/gthegnldnu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhengqikj.top/gtgsktmqck.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.fengsongda.top/gtzsnzdhjt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.mhx1999.top/gtixurskjl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jinyuanbaomall.cn/gtovlsremv.html

Java: class Node { int v; Node next; }
来源：http://hz.jyoumei.cn/gtzdujkkxi.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xuetiantiany.cn/gtyuuodyjt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhixingplan.top/gtdyubycje.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.havefunace.top/gtwsbvbrkp.html

[N11] 二叉树中序遍历
来源：http://hz.ppjwa.cn/gtheebwsqs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.iojbl.cn/gtbuvycwzf.html

PHP:  // 手写递归函数
来源：http://hz.316326.xyz/gtvfmnxxwk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuxming.cn/gtxasiseye.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guannengcc.top/gtbwltbkxo.html

Java: // 手写递归
来源：http://hz.shzxlz.cn/gtteunjtld.html

Go:   // 手写递归
来源：http://hz.fzhhl.top/gtpigzspuh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.pycfn.com/gtuhfvxxcj.html

C#:   // 手写递归
来源：http://hz.quarkkingdee.top/gtzazrwyqy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zycfv.cn/gtgjgjcfxs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.mhx1999.top/gtrzmagjmm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.fengsongda.top/gtdqjqceld.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhaomingkeji.xyz/gtnrqclcae.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258888.top/gtseozmcoi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhoulong.xyz/gtbuobgwip.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yonumen.top/gtinacvjdz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.c1oappe.top/gtosblbmjr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hywenlv.cn/gtjvvnljlq.html

================================================================================
来源：http://hz.nanxuanxn.top/gtkemxnato.html

O. 并发与异步
来源：http://hz.tanke756.top/gtxlkcptdg.html

================================================================================
来源：http://hz.zycfv.cn/gtzrpjbkgl.html

[O01] 启动一个线程
来源：http://hz.ybcxt.top/gtrbrkgsfl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.haohaochexian.top/gtkbzjzxiw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jiagoushi.top/gtifgokqok.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gogol.net.cn/gtcukwefug.html

TS:   // 同 JS
来源：http://hz.xuanzx.com/gtesyhxpgz.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhengqikj.top/gtqoprihsg.html

Go:   go f()
来源：http://hz.jinqigufen.top/gtujytturt.html

Ruby: Thread.new { f }
来源：http://hz.zhongyouzk.top/gtmgcqqmxy.html

C#:   Task.Run(() => F());
来源：http://hz.shanyushiyangkeji.top/gtodlbplyc.html

[O02] 使用线程池
来源：http://hz.jianghu66.top/gtfaypdpnb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.meibo888.top/gtnpvvrgpi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.52xcode.cn/gttenifvvk.html

JS:   // worker_threads 线程池
来源：http://hz.iojbl.cn/gtfywgqkfs.html

TS:   // worker_threads 线程池
来源：http://hz.zhongyouzk.top/gtjcdedyty.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ppjwa.cn/gtixnlnndf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.pengpengdd.cyou/gtmnlkzyhm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.andypj.xyz/gttmxeaknj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.dashuyun.cn/gteqslxwnf.html

[O03] 加锁保护共享数据
来源：http://hz.52xcode.cn/gtvosslsxf.html

Py:   with lock: shared += 1
来源：http://hz.iojbl.cn/gtwitpudov.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhongyouzk.top/gthtytxcct.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.dashuyun.cn/gtoqevotoy.html

TS:   // 同 JS
来源：http://hz.shanyushiyangtech.top/gtohpmatgy.html

Java: synchronized (this) { shared++; }
来源：http://hz.tian-w.cn/gtmwnkrjqm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ywan-chungtsiang.top/gtcjbexytd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhixingplan.top/gtdjdmgtco.html

C#:   lock (gate) { shared++; }
来源：http://hz.52xcode.cn/gtptxhjzla.html

[O04] 定义异步函数并等待
来源：http://hz.guowangkeji.top/gtwutsxflw.html

Py:   async def f():⏎    await g()
来源：http://hz.dianchejie.cn/gtsifaqpvn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinqigfzy.top/gtovlkkqlp.html

JS:   async function f() { await g(); }
来源：http://hz.nwbrower.top/gtpbhfayxm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yueranfly.top/gtipvvaydy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.smart0.xyz/gtzqaztkvl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.kuanghao11.cn/gtvqltgxow.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.guowangkeji.top/gtfxuyajel.html

C#:   async Task F() { await G(); }
来源：http://hz.dashuyun.cn/gthdknpzng.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj202588.top/gtjlxnpznt.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yj202588.top/gtxjgktegn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhengqikj.top/gtmokreiqi.html

JS:   await Promise.all(tasks)
来源：http://hz.shanyushiyangtech.top/gtfoqazces.html

TS:   await Promise.all(tasks)
来源：http://hz.ydzc1.top/gtdphojrtq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.fengsongda.top/gtikwqhhmq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhiwuduotai.top/gtqnfqrvco.html

Ruby: threads.map(&:join)
来源：http://hz.sweek.top/gtwrgloygq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yongpay.top/gtdahsbrox.html

[O06] 使用进程池
来源：http://hz.xylfe.cn/gtnpzsqmyz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.gogol.net.cn/gtzflphkgw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.0kj1m.cn/gtwaqczylv.html

JS:   // child_process / cluster 模块
来源：http://hz.gzhubu.top/gtegygoidy.html

TS:   // child_process / cluster 模块
来源：http://hz.jqgfzy.top/gtyycfyedu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ywan-chungtsiang.top/gtqwjglaww.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jqgfzy.top/gtzkqnxvsl.html

Ruby: // fork 块
来源：http://hz.smart0.xyz/gtqhmfqjgk.html

C#:   Parallel.For
来源：http://hz.xinyue.icu/gtxecxswxf.html

================================================================================
来源：http://hz.gotoacloud.top/gtkvjlajft.html

P. 常用工具函数
来源：http://hz.tian-w.cn/gtaguqrodz.html

================================================================================
来源：http://hz.dianchejie.cn/gtduzjzgci.html

[P01] 生成 UUID
来源：http://hz.cashguo.top/gtrkxykinl.html

Py:   str(uuid.uuid4())
来源：http://hz.nwbrower.top/gtrkffrdrv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xinyue.icu/gthwdamfvb.html

JS:   crypto.randomUUID()
来源：http://hz.sysykeji.top/gtrtmltvty.html

TS:   crypto.randomUUID()
来源：http://hz.cqqwz.cn/gthughidpz.html

Java: UUID.randomUUID().toString()
来源：http://hz.svipenyu.cn/gtustxyqzp.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hnqzz.top/gtruacaiqz.html

Ruby: SecureRandom.uuid
来源：http://hz.hnqzz.top/gtdfgoklus.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.feifeiyinyue.top/gtivtyasse.html

[P02] MD5 / SHA256 摘要
来源：http://hz.tian-w.cn/gtgalcldtz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cashguo.top/gtgjbrxzdb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.mhx1999.top/gtjknvlwfz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shzxlz.cn/gtbergwmgo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hysaishi.cn/gtegxdfrtc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yongpay.top/gtowpccghk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shangyingyoupin.top/gtmflgirdy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yj20258888.top/gtuaxtxelq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.gaohongyu789.top/gtfqxcmxsh.html

[P03] 生成短随机字符串
来源：http://hz.fengsongda.top/gtednrgaub.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zycfv.cn/gtzpuecxlu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yueranfly.top/gtsmdkifgs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.fzhhl.top/gtfcgipjyh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydzc1.top/gtzvmjmrkx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yanxiufei.cn/gtldhakvpk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jyoumei.cn/gtwgsrbrol.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinyuanbaomall.cn/gtjfdfvaur.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shzxlz.cn/gtwutarnmz.html

[P04] 求长度
来源：http://hz.feifeiyinyue.top/gtiuvqqbod.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.sufxvd.cn/gtpsuigfka.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.kuanghao11.cn/gtzcaunnar.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ppjwa.cn/gtqxrnfqgm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.meibo888.top/gtuflcfmjy.html

Java: list.size();  map.size();  s.length()
来源：http://hz.52xcode.cn/gtwsgocjsy.html

Go:   len(arr);  len(m)
来源：http://hz.nanxuanxn.top/gtqghlfjoe.html

Ruby: x.length;  x.size
来源：http://hz.ywan-chungtsiang.top/gtrfnmpulo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.chenzaomai.com/gtdtgocwlu.html

[P05] 判断两个对象内容是否相等
来源：http://hz.iojbl.cn/gtexmpusdj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jqgufenzy.top/gtiucxwdal.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhengqikj.top/gtfnwhnhdl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shzxlz.cn/gtzxamhwri.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.0kj1m.cn/gtgbkathdy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zycfv.cn/gtmallztji.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.haohaochexian.top/gtenbxaogc.html

Ruby: a == b
来源：http://hz.yongpay.top/gtxzvpzbij.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ppjwa.cn/gtncwvjdwv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.nanxuanxn.top/gtnncmoxpp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.316326.xyz/gtykxqtmtw.html

PHP:  if (empty($x)) {}
来源：http://hz.chenjidiqi.icu/gthrmiadky.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.vqdsnc.cn/gtaimjemcj.html

TS:   if (x == null) {}
来源：http://hz.quarkkingdee.top/gtbinirefh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.gotoacloud.top/gtnfhqyest.html

Go:   if x == nil {}
来源：http://hz.chenjidiqi.icu/gtrllvovgu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jlsjyb.cn/gtzmvdnxmz.html

C#:   if (x is null) {}
来源：http://hz.iojbl.cn/gtzxfeikbb.html

[P07] 防抖与节流
来源：http://hz.shangyingyoupin.top/gtesjldcmj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.fengsongda.top/gtbjagdyfh.html

PHP:  // 手写时间戳比较
来源：http://hz.jinyuanbaomall.cn/gthgpspadz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gtxxugraho.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.feifeiyinyue.top/gtsnxbccpc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.nanxinkj.top/gtsoklyrag.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.vqdsnc.cn/gtrdobvhls.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.dianchejie.cn/gtljybvhil.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.havefunace.top/gtczxevonh.html

[P08] 处理浮点精度问题
来源：http://hz.jyoumei.cn/gtdmjlueih.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.52xcode.cn/gtiemfmfpe.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.tian-w.cn/gtzhkemxrh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sufxvd.cn/gtdxdifrpm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.nwbrower.top/gtdgrizxol.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jinqigfzy.top/gthpppzhdp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.c1oappe.top/gtixuqyihj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jqgfzy.top/gtfpdqxuyj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ywan-chungtsiang.top/gtamxrlwkz.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtlhaxcjzc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hfpthk.cn/gtnvyxlueg.html

================================================================================
来源：http://hz.nanxuanxn.top/gtemshqxgx.html

[Q01] 创建表
来源：http://hz.haohaochexian.top/gtsntdfkki.html

CREATE TABLE users (
来源：http://hz.sysykeji.top/gtqozerreg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhijiandao.cn/gtdmmeinat.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhengqikj.top/gtmnhehcwx.html

email VARCHAR(100) UNIQUE,
来源：http://hz.daria6918.cn/gtloloolzn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gogol.net.cn/gtytjtxcoh.html

);
来源：http://hz.yvedp.cn/gtcwsdjqre.html

[Q02] 创建带外键的表
来源：http://hz.ehwqpu.com/gthzrxbywl.html

CREATE TABLE orders (
来源：http://hz.jinqigufen.top/gttdfxljez.html


<!-- 参考信息 -->