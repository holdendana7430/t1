代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://hz.smart0.xyz/gteyyqwcrq.html

[M05] 设置退出码
来源：http://hz.wangshuangyany.cn/gtwqdypzax.html

Py:   sys.exit(1)
来源：http://hz.gotoacloud.top/gtbxcsfmvx.html

PHP:  exit(1);
来源：http://hz.gogol.net.cn/gtettjrjky.html

JS:   process.exit(1)
来源：http://hz.yvedp.cn/gtkphpzybc.html

TS:   process.exit(1)
来源：http://hz.zhongyouzk.top/gtuikyohsv.html

Java: System.exit(1)
来源：http://hz.jiagoushi.top/gtrnjyrijv.html

Go:   os.Exit(1)
来源：http://hz.vqdsnc.cn/gtkujljrum.html

Ruby: exit 1
来源：http://hz.zhongyouzk.top/gtrsxfafni.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhijiandao.cn/gtmqfoljce.html

[M06] 向标准错误输出
来源：http://hz.jinqigfzy.top/gtaqjaagyv.html

Py:   print("err", file=sys.stderr)
来源：http://hz.wangdashe.top/gtfkbyezbe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jqgfzy.top/gtdyzmtmtl.html

JS:   console.error("err")
来源：http://hz.mhx1999.top/gtjmbvitle.html

TS:   console.error("err")
来源：http://hz.zycfv.cn/gtoadecdgk.html

Java: System.err.println("err")
来源：http://hz.9152youxi.cn/gtdxoludeg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhaomingkeji.xyz/gteawymqya.html

Ruby: warn "err"
来源：http://hz.shanyushiyangtech.top/gtgiukenea.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jinyuanbaomall.cn/gtfbyyhkce.html

[M07] 判断是否为主入口
来源：http://hz.xziqi.cn/gtoicleoss.html

Py:   if __name__ == "__main__":
来源：http://hz.ppjwa.cn/gtkhukadsv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yueranfly.top/gtjhveggqi.html

JS:   require.main === module
来源：http://hz.sweek.top/gtfegsdvra.html

TS:   require.main === module
来源：http://hz.andypj.xyz/gttocrankr.html

Java: public static void main(String[] args)
来源：http://hz.ydjk.org.cn/gtqudfztwv.html

Go:   func main()
来源：http://hz.shangyingyoupin.top/gtzmdltvqk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yuanzhike.top/gtmzwwaqjo.html

C#:   static void Main(string[] args)
来源：http://hz.sysykeji.top/gttjumdrfb.html

[M08] 获取系统与运行时信息
来源：http://hz.yuxming.cn/gthqrzlzkp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhijiandao.cn/gtnpthyzdn.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jinyuanbaomall.cn/gthouuzdsh.html

JS:   process.platform;  process.version
来源：http://hz.zhoulong.xyz/gtfbqxadfz.html

TS:   process.platform;  process.version
来源：http://hz.hnxiangtu.top/gtdwsxeule.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhoulong.xyz/gtfuwapvjy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ehwqpu.com/gtjvaflfyh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.andypj.xyz/gtiygaglge.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jianghu66.top/gtyggdnhcb.html

================================================================================
来源：http://hz.fzhhl.top/gtcrckggtl.html

N. 数据结构与算法
来源：http://hz.vqdsnc.cn/gtgmdmzaem.html

================================================================================
来源：http://hz.jqgufenzy.top/gtsoyfdjxf.html

[N01] 二分查找（有序数组）
来源：http://hz.zhijiandao.cn/gtgeovjhbe.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhiwuduotai.top/gthbpjbkrx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cheryme.top/gtgyldhftk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangshuangyany.cn/gtnxizmlzj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xziqi.cn/gtkmmwrsbq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.nanxuanxn.top/gtlkhvibyu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.dashuyun.cn/gtpziralry.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.gogol.net.cn/gtulhixijn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtdlhydyox.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.vqdsnc.cn/gtnppymylj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hywenlv.cn/gtcofehsfd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.0kj1m.cn/gticehwcef.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gaohongyu789.top/gttckbqwoc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.0kj1m.cn/gtvktcslzq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.0kj1m.cn/gtlhmjoxnp.html

Go:   slices.Sort(arr)
来源：http://hz.jinqigfzy.top/gthfhyjoaf.html

Ruby: arr.sort
来源：http://hz.aizwys.cn/gttbcxhyby.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jqgufenzy.top/gtyfzgbgpy.html

[N03] 快速排序（分治示例）
来源：http://hz.guannengcc.top/gtwdssbuqh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yj20258888.top/gtqyrawzcp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gotoacloud.top/gtavrtcniy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj202588.top/gtzqpmywpr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hfpthk.cn/gtcjjogjqr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.iojbl.cn/gtwgnmjgde.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.redwolf501.top/gtxcoigclj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zycfv.cn/gttoiiwbbb.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.bjfxy.top/gtvdusxecw.html

[N04] 斐波那契数列
来源：http://hz.shangyingyoupin.top/gtousijxis.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.nanxinkj.top/gtqbgalkde.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.dashuyun.cn/gttfwenvzv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pycfn.com/gtiogyysyj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.andypj.xyz/gtnlfjppxr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xuetiantiany.cn/gtzeeyjmsl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ydjk.org.cn/gtboqygslb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sysykeji.top/gtftdyjbte.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.bjfxy.top/gtqjfisajx.html

[N05] 最大公约数
来源：http://hz.wangshuangyany.cn/gtbmukmsom.html

Py:   math.gcd(a, b)
来源：http://hz.zhengqikj.top/gtwkzsmfkh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhiwuduotai.top/gtqcahvfub.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gtnjqderrf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cheryme.top/gtqutdphti.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hnqzz.top/gtnkhmnrlx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ydzc1.top/gtkglmeedu.html

Ruby: a.gcd(b)
来源：http://hz.gotoacloud.top/gtuxqedent.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yj202588.top/gtaailemxh.html

[N06] 判断回文字符串
来源：http://hz.wangdashe.top/gtrmqfnsmy.html

Py:   s == s[::-1]
来源：http://hz.yvedp.cn/gtqxwdstff.html

PHP:  $s === strrev($s);
来源：http://hz.tian-w.cn/gtcbvqjsnw.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gtdoqtqrhu.html

TS:   s === [...s].reverse().join("")
来源：http://hz.c1oappe.top/gtkinpuxka.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhijiandao.cn/gtfuyqkmph.html

Go:   // 双指针从两端比较
来源：http://hz.shuidangran.top/gtuhhrobtd.html

Ruby: s == s.reverse
来源：http://hz.xziqi.cn/gtoksiuthb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhaomingkeji.xyz/gtkelfqpft.html

[N07] 两数之和（返回下标）
来源：http://hz.jiagoushi.top/gttjsdpvof.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.316326.xyz/gtkuymijlx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.quarkkingdee.top/gtpnhnxpju.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.aibaodan.cn/gtusycmqjr.html

TS:   // 手写 Map<string, number>
来源：http://hz.havefunace.top/gtgieuujnd.html

Java: // 手写 HashMap
来源：http://hz.hywenlv.cn/gtbpeutgqs.html

Go:   // 手写 map[int]int
来源：http://hz.sufxvd.cn/gtvkhygsjd.html

Ruby: // 手写 Hash
来源：http://hz.daxiang520.top/gtebrxjtvw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.dashuyun.cn/gtrtpptslj.html

[N08] 生成全排列
来源：http://hz.xinyue.icu/gtezrbbvti.html

Py:   itertools.permutations(arr)
来源：http://hz.redwolf501.top/gtsootmzig.html

PHP:  // 手写递归交换
来源：http://hz.daria6918.cn/gtvoqvvate.html

JS:   // 手写回溯递归
来源：http://hz.tianlin.xyz/gtocwdxtzi.html

TS:   // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gttiypfmav.html

Java: // 手写回溯递归
来源：http://hz.havefunace.top/gtjbthowee.html

Go:   // 手写回溯递归
来源：http://hz.yuxming.cn/gtwnuziswf.html

Ruby: arr.permutation.to_a
来源：http://hz.ywan-chungtsiang.top/gtarxfrzms.html

C#:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtpmwdopod.html

[N09] 栈与队列
来源：http://hz.cheryme.top/gtqpyicidn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.9152youxi.cn/gtzptmnxfe.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cucudq.cn/gtephdyhlb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.meibo888.top/gtzltolvua.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jqgufenzy.top/gthvtqqpkl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ivvv.top/gtnguplmar.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.bjfxy.top/gtrpjwqpxi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hnxiangtu.top/gtbygnujjn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhengqikj.top/gtbntwmqyl.html

[N10] 链表节点定义
来源：http://hz.daria6918.cn/gtwroncioc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.sufxvd.cn/gtfmbvlgsw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hnxiangtu.top/gtlqozghef.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj20258888.top/gtwnaoixla.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.guannengcc.top/gtturircxr.html

Java: class Node { int v; Node next; }
来源：http://hz.pengpengdd.cyou/gtqbcwnfyj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.daria6918.cn/gthdacyzpj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.9152youxi.cn/gtpbzlvujv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shuidangran.top/gtzbreiprt.html

[N11] 二叉树中序遍历
来源：http://hz.52xcode.cn/gtbocmgjqn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.andypj.xyz/gtxflbktba.html

PHP:  // 手写递归函数
来源：http://hz.ppjwa.cn/gtravnlwkp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.redwolf501.top/gtouxnrzan.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.meibo888.top/gtmswhigcr.html

Java: // 手写递归
来源：http://hz.hfpthk.cn/gtybrqxwjc.html

Go:   // 手写递归
来源：http://hz.daria6918.cn/gthpjbwuqz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.aizwys.cn/gttqxfdwju.html

C#:   // 手写递归
来源：http://hz.hammf.cn/gtpntklvpu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ywan-chungtsiang.top/gtzjwcrxaf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.haohaochexian.top/gtxnekfbae.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.0kj1m.cn/gtqkzzoqli.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gzhubu.top/gtqnonyusc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shzxlz.cn/gtqoqngjim.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xinyue.icu/gtixvzsarw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenjidiqi.icu/gtjdmvshnm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xylfe.cn/gtzcabhypl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pengpengdd.cyou/gtcxmtwaak.html

================================================================================
来源：http://hz.hysaishi.cn/gtktqiglgr.html

O. 并发与异步
来源：http://hz.52xcode.cn/gtbovdafya.html

================================================================================
来源：http://hz.zhongyouzk.top/gtgxjdqpat.html

[O01] 启动一个线程
来源：http://hz.zhixingplan.top/gtduxajwem.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.bjfxy.top/gtynuhklgs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ppjwa.cn/gtdzdmvjka.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jqgufenzy.top/gtdizvlvqv.html

TS:   // 同 JS
来源：http://hz.ybcxt.top/gtkadlpbis.html

Java: new Thread(() -> f()).start()
来源：http://hz.yonumen.top/gtywjcccxu.html

Go:   go f()
来源：http://hz.ydzc1.top/gtstlpskty.html

Ruby: Thread.new { f }
来源：http://hz.gotoacloud.top/gtitunjhjb.html

C#:   Task.Run(() => F());
来源：http://hz.ivvv.top/gtzcbituui.html

[O02] 使用线程池
来源：http://hz.jianghu66.top/gtjzwxsrbe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shanyushiyangkeji.top/gtqfftqvby.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cashguo.top/gtdetergvr.html

JS:   // worker_threads 线程池
来源：http://hz.hywenlv.cn/gtujvrxpnd.html

TS:   // worker_threads 线程池
来源：http://hz.yongpay.top/gtofjjemtq.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.sweek.top/gtjxxisebp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.9152youxi.cn/gtuycdqobn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.sufxvd.cn/gtvzbivrrr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yvedp.cn/gtujduoffi.html

[O03] 加锁保护共享数据
来源：http://hz.daria6918.cn/gtevzunkmh.html

Py:   with lock: shared += 1
来源：http://hz.fengsongda.top/gtxddgyrpy.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.svipenyu.cn/gtqkzhocbo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zdqjudy.top/gthvacouxj.html

TS:   // 同 JS
来源：http://hz.fengsongda.top/gtxybpkfav.html

Java: synchronized (this) { shared++; }
来源：http://hz.tianlin.xyz/gthchdysxo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhijiandao.cn/gtygriomhj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.gzhubu.top/gthqkvondv.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhijiandao.cn/gtdojmsouh.html

[O04] 定义异步函数并等待
来源：http://hz.birdmap.top/gtlekzyato.html

Py:   async def f():⏎    await g()
来源：http://hz.tian-w.cn/gtlubukcms.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhijiandao.cn/gtquhceepw.html

JS:   async function f() { await g(); }
来源：http://hz.smart0.xyz/gtynilnzfa.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.316326.xyz/gtwtdhyrrv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yonumen.top/gtgkrdpwkp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.chenlongwang.top/gtdufjpzvk.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.svipenyu.cn/gtiejaubnf.html

C#:   async Task F() { await G(); }
来源：http://hz.wangshuangyany.cn/gtfkzssmjq.html

[O05] 并发执行并等待全部完成
来源：http://hz.hongshengwenyu.top/gtregripnn.html

Py:   asyncio.gather(*tasks)
来源：http://hz.meibo888.top/gtyetbqwqr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.nwbrower.top/gtkdnewlyu.html

JS:   await Promise.all(tasks)
来源：http://hz.tianlin.xyz/gtgoowiivp.html

TS:   await Promise.all(tasks)
来源：http://hz.yangfankeji.com/gtjxylmvkn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhixingplan.top/gtfwsfavgq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.aizwys.cn/gtihfvzxtr.html

Ruby: threads.map(&:join)
来源：http://hz.nanxinkj.top/gtwalclngx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.gzhubu.top/gtjbluhnhq.html

[O06] 使用进程池
来源：http://hz.jqgfzy.top/gtuohpvwdk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zycfv.cn/gtbmyzrfwn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jinyuanbaomall.cn/gthnfxrqyb.html

JS:   // child_process / cluster 模块
来源：http://hz.redwolf501.top/gtnclaclgh.html

TS:   // child_process / cluster 模块
来源：http://hz.andypj.xyz/gtlorolegj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhongyouzk.top/gtzoaxvhaq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ehwqpu.com/gthsooqijd.html

Ruby: // fork 块
来源：http://hz.jyoumei.cn/gtrcdtmset.html

C#:   Parallel.For
来源：http://hz.yuxming.cn/gtoueodqri.html

================================================================================
来源：http://hz.nanxinkj.top/gtbptgvafk.html

P. 常用工具函数
来源：http://hz.chenzaomai.com/gtoeriamgn.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtsfkouszt.html

[P01] 生成 UUID
来源：http://hz.zhoulong.xyz/gtwwwxsfnq.html

Py:   str(uuid.uuid4())
来源：http://hz.shangyingyoupin.top/gtpwnyuldm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.haohaochexian.top/gtskudswan.html

JS:   crypto.randomUUID()
来源：http://hz.nwbrower.top/gtrlislggv.html

TS:   crypto.randomUUID()
来源：http://hz.mhx1999.top/gtfhpsjyup.html

Java: UUID.randomUUID().toString()
来源：http://hz.jqgufenzy.top/gtfnpsyqmz.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shanyushiyangtech.top/gtnxbpulqt.html

Ruby: SecureRandom.uuid
来源：http://hz.jianghu66.top/gtrykgvcqq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yuxming.cn/gtzuoqrmwt.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhixingplan.top/gtoztcgwbj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cucudq.cn/gtfhdcxcch.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zycfv.cn/gtyuttvumh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.c1oappe.top/gtdkvbalhl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xinyue.icu/gtdwxbyywc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jinqigfzy.top/gthtjgwurs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yonumen.top/gtsvgmgdrm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.bjfxy.top/gtbqnfmepk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zycfv.cn/gtimyugoav.html

[P03] 生成短随机字符串
来源：http://hz.hammf.cn/gtjsqhxkms.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.snrcjt.cn/gtpobudxch.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jiagoushi.top/gtzxpwgjhs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.aizwys.cn/gtrudzcddr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.birdmap.top/gtmnykjbzm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zdqjudy.top/gtsfqfeyyb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xziqi.cn/gtgwlagzqc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.mhx1999.top/gtzbfvwlln.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.mhx1999.top/gtmrbrqqjf.html

[P04] 求长度
来源：http://hz.cqqwz.cn/gtxwavxqtj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.aibaodan.cn/gtfgidiqzv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yuanzhike.top/gtukscazbe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xylfe.cn/gtwoeetfkm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ehwqpu.com/gtpexlhzyd.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yueranfly.top/gteqaslbtw.html

Go:   len(arr);  len(m)
来源：http://hz.yangfankeji.com/gtatmqcoyr.html

Ruby: x.length;  x.size
来源：http://hz.yj202588.top/gtbpbbmdlm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhongyouzk.top/gtdsmxeycw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yuanzhike.top/gtfewcdmwt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cashguo.top/gtrhlktwcp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.andypj.xyz/gtfgzbdomb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hywenlv.cn/gttykzkczx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinghuilouyu.cn/gtafbjthgn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xylfe.cn/gthixkzdta.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.aizwys.cn/gttpvzjzss.html

Ruby: a == b
来源：http://hz.snrcjt.cn/gtbkcrroji.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cheryme.top/gtzsuxdjpq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cheryme.top/gtlzlwxlbd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.bjfxy.top/gtobhwgafj.html

PHP:  if (empty($x)) {}
来源：http://hz.kuanghao11.cn/gtidirownn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.wangshuangyany.cn/gtvddsltut.html

TS:   if (x == null) {}
来源：http://hz.daxiang520.top/gtqzinowvx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.daxiang520.top/gtapoyxvoc.html

Go:   if x == nil {}
来源：http://hz.hammf.cn/gtbeujrjyv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xziqi.cn/gtlhimbkdn.html

C#:   if (x is null) {}
来源：http://hz.aibaodan.cn/gtxgconruu.html

[P07] 防抖与节流
来源：http://hz.zhijiandao.cn/gtwismonvs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cheryme.top/gtkucqvykr.html

PHP:  // 手写时间戳比较
来源：http://hz.zhaomingkeji.xyz/gtpkzgqluj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jlsjyb.cn/gthagugfoq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hywenlv.cn/gtssdnzuqb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.chenjidiqi.icu/gtkqibvdkz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hnqzz.top/gtadnaayfz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.aizwys.cn/gtblkasrhl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yuanzhike.top/gtmndufcgi.html

[P08] 处理浮点精度问题
来源：http://hz.aizwys.cn/gtlefipblx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ehwqpu.com/gtbjaxkrwo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xuetiantiany.cn/gtgldllgvz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhaomingkeji.xyz/gtrccooqfz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tianlin.xyz/gtmrmqpoqs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhoulong.xyz/gtcbtpvign.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.gotoacloud.top/gtsqpzngip.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cheryme.top/gtwlbgofim.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ivvv.top/gtyizbiixy.html

================================================================================
来源：http://hz.meibo888.top/gtgxtamtps.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhongyouzk.top/gthjkmrdrj.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtcfrfwlaj.html

[Q01] 创建表
来源：http://hz.ppjwa.cn/gtbppiknqd.html

CREATE TABLE users (
来源：http://hz.gzhubu.top/gtvicmhtdf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sufxvd.cn/gtjfsimeee.html

name VARCHAR(50) NOT NULL,
来源：http://hz.nanxuanxn.top/gtomqnkhqb.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yanxiufei.cn/gtjewiluzx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhixingplan.top/gtqttmnqdr.html

);
来源：http://hz.wangdashe.top/gtygprmgsg.html

[Q02] 创建带外键的表
来源：http://hz.sxryk.cn/gtsnyehugy.html

CREATE TABLE orders (
来源：http://hz.jqgfzy.top/gtfodmxghf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hysaishi.cn/gtcwvmlptb.html

user_id INT NOT NULL,
来源：http://hz.guowangkeji.top/gtnpbxxxqb.html

amount DECIMAL(10, 2),
来源：http://hz.zhiwuduotai.top/gtzwmokrcf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ybcxt.top/gtkkeckqmn.html

);
来源：http://hz.yj20258.top/gthmaydmzq.html

[Q03] 增加列
来源：http://hz.shanyushiyangtech.top/gtfkypcgao.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.daxiang520.top/gtzamafxmh.html

[Q04] 修改列类型
来源：http://hz.zhongyouzk.top/gtfkfjsmtl.html


<!-- 参考信息 -->