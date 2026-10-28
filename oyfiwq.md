代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ivvv.top/gtgsygqbim.html

[M05] 设置退出码
来源：http://hz.hammf.cn/gtjovstpbz.html

Py:   sys.exit(1)
来源：http://hz.cucudq.cn/gtbzestaee.html

PHP:  exit(1);
来源：http://hz.jiagoushi.top/gtadobtlay.html

JS:   process.exit(1)
来源：http://hz.yvedp.cn/gtjbwpupbx.html

TS:   process.exit(1)
来源：http://hz.hnxiangtu.top/gtsficskkx.html

Java: System.exit(1)
来源：http://hz.yangfankeji.com/gtnpcdhdfv.html

Go:   os.Exit(1)
来源：http://hz.chenjidiqi.icu/gtcprihcse.html

Ruby: exit 1
来源：http://hz.9152youxi.cn/gtosfswpff.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.dianchejie.cn/gtliplrroa.html

[M06] 向标准错误输出
来源：http://hz.chenjidiqi.icu/gtcipfnsbf.html

Py:   print("err", file=sys.stderr)
来源：http://hz.guannengcc.top/gtohpqqnfg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenjidiqi.icu/gtwlxyxdke.html

JS:   console.error("err")
来源：http://hz.aibaodan.cn/gtmmebfypf.html

TS:   console.error("err")
来源：http://hz.wangshuangyany.cn/gtifjqwltc.html

Java: System.err.println("err")
来源：http://hz.andypj.xyz/gticcgkabm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ybcxt.top/gtilcbbxih.html

Ruby: warn "err"
来源：http://hz.ehwqpu.com/gtqeobemkd.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yongpay.top/gtluvpmdpd.html

[M07] 判断是否为主入口
来源：http://hz.jqgfzy.top/gtvjgbiyrh.html

Py:   if __name__ == "__main__":
来源：http://hz.svipenyu.cn/gttmklendm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xylfe.cn/gtkfxwhbie.html

JS:   require.main === module
来源：http://hz.dianchejie.cn/gtygdqlubk.html

TS:   require.main === module
来源：http://hz.tanke756.top/gtkplryhes.html

Java: public static void main(String[] args)
来源：http://hz.nanxuanxn.top/gtdfubdfha.html

Go:   func main()
来源：http://hz.iojbl.cn/gtxerxgczx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.snrcjt.cn/gtwakftfub.html

C#:   static void Main(string[] args)
来源：http://hz.zhaomingkeji.xyz/gthflgkvqq.html

[M08] 获取系统与运行时信息
来源：http://hz.fzhhl.top/gtamtroenv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xylfe.cn/gtlbxvhhcj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jinqigfzy.top/gthsbexffr.html

JS:   process.platform;  process.version
来源：http://hz.gzhubu.top/gtpnwrhnyp.html

TS:   process.platform;  process.version
来源：http://hz.ydjk.org.cn/gtnxraszsf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jlsjyb.cn/gtzyxrzrnt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yueranfly.top/gtcyvzefay.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinyuanbaomall.cn/gtwuwnawwp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj202588.top/gtnntrhofr.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtkapqxlpv.html

N. 数据结构与算法
来源：http://hz.iojbl.cn/gtowsloxwj.html

================================================================================
来源：http://hz.hysaishi.cn/gtynidpbrr.html

[N01] 二分查找（有序数组）
来源：http://hz.yuanzhike.top/gtisccbjge.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jqgfzy.top/gtpluzaouy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zycfv.cn/gtsljtueda.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.kuanghao11.cn/gtbvayfofc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258888.top/gtuhbmngwn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.dashuyun.cn/gtnqgsqxyz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.svipenyu.cn/gtjnqwahca.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhaomingkeji.xyz/gtbmdntzbe.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.aizwys.cn/gtgnevmnqw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xziqi.cn/gtuptrzwku.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydzc1.top/gtgchdmpjb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hfpthk.cn/gtsssovohv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cucudq.cn/gtnipzwlkm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xinyue.icu/gtmovcicdr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ehwqpu.com/gtmihbsugr.html

Go:   slices.Sort(arr)
来源：http://hz.zhijiandao.cn/gtaefzjqen.html

Ruby: arr.sort
来源：http://hz.ppjwa.cn/gtzuflrqet.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.vqdsnc.cn/gtyfsvxwiu.html

[N03] 快速排序（分治示例）
来源：http://hz.hnqzz.top/gtmkcuaixj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.dashuyun.cn/gtcbnbzbqm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gogol.net.cn/gthpdzxxnc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hnqzz.top/gtlfapmzvp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj202588.top/gtyfczxcwg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.dianchejie.cn/gthpkayezq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.wangdashe.top/gtyxazyved.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.nanxinkj.top/gtblpsziau.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.aibaodan.cn/gtfloozmrb.html

[N04] 斐波那契数列
来源：http://hz.fengsongda.top/gtkmjiccgm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xuanzx.com/gthckkgedp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yj202588.top/gtxwnjrcmn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gogol.net.cn/gtaewrcojs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.haohaochexian.top/gtxxiklgwl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jlsjyb.cn/gtupwjwimw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.vqdsnc.cn/gtmbhjbyqo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhijiandao.cn/gtibipxoho.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.9152youxi.cn/gtkxbgccxv.html

[N05] 最大公约数
来源：http://hz.zhoulong.xyz/gtxciozhul.html

Py:   math.gcd(a, b)
来源：http://hz.yvedp.cn/gtbygdagna.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sysykeji.top/gturiyjaxl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangkeji.top/gtmnwmrhom.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhijiandao.cn/gtpwzmbucm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jianghu66.top/gtqisjyqks.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhaomingkeji.xyz/gtwsnmnbjx.html

Ruby: a.gcd(b)
来源：http://hz.zhengqikj.top/gtfydwydsp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yvedp.cn/gtftngzhoe.html

[N06] 判断回文字符串
来源：http://hz.yonumen.top/gtbkyezzbb.html

Py:   s == s[::-1]
来源：http://hz.nwbrower.top/gtijckkioh.html

PHP:  $s === strrev($s);
来源：http://hz.sufxvd.cn/gtkgckjjnm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtjjjvngaj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtibnabywu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.iojbl.cn/gtdskcfsnl.html

Go:   // 双指针从两端比较
来源：http://hz.jinyuanbaomall.cn/gtmjswtvcr.html

Ruby: s == s.reverse
来源：http://hz.aibaodan.cn/gtjadqxyet.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hysaishi.cn/gtglnwgkdo.html

[N07] 两数之和（返回下标）
来源：http://hz.ivvv.top/gtqjdbbojy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhongyouzk.top/gtzxvfuyxs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xziqi.cn/gteuhqdtcp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.aizwys.cn/gtbaljupnc.html

TS:   // 手写 Map<string, number>
来源：http://hz.andypj.xyz/gtbkyvutsy.html

Java: // 手写 HashMap
来源：http://hz.andypj.xyz/gtqdlpolhf.html

Go:   // 手写 map[int]int
来源：http://hz.shuidangran.top/gtkntetriv.html

Ruby: // 手写 Hash
来源：http://hz.ywan-chungtsiang.top/gtjituvxgo.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ydjk.org.cn/gtypgyymgy.html

[N08] 生成全排列
来源：http://hz.nanxinkj.top/gttwnoboud.html

Py:   itertools.permutations(arr)
来源：http://hz.xylfe.cn/gtmygycvbc.html

PHP:  // 手写递归交换
来源：http://hz.jinghuilouyu.cn/gtotbcjoci.html

JS:   // 手写回溯递归
来源：http://hz.yuxming.cn/gtlhsonjzi.html

TS:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtwniwkdpp.html

Java: // 手写回溯递归
来源：http://hz.jianghu66.top/gtvotxtydm.html

Go:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtkttzcbss.html

Ruby: arr.permutation.to_a
来源：http://hz.zhixingplan.top/gtjdheryry.html

C#:   // 手写回溯递归
来源：http://hz.cqqwz.cn/gtamuixkdr.html

[N09] 栈与队列
来源：http://hz.ydjk.org.cn/gtkxpifdru.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yvedp.cn/gtfctcykhz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cqqwz.cn/gtvvpudvuc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jianghu66.top/gtmrmpjxry.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shanyushiyangtech.top/gtldojgazn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jqgufenzy.top/gtrusmyhxz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.0kj1m.cn/gtcniphvxu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sufxvd.cn/gtxtzctmrz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xylfe.cn/gtaeraaqtt.html

[N10] 链表节点定义
来源：http://hz.yj202588.top/gtvdhcwona.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.pengpengdd.cyou/gtmabtqyja.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.316326.xyz/gtgvblerom.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.daria6918.cn/gtkqsigorc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yuxming.cn/gthlzpdjjs.html

Java: class Node { int v; Node next; }
来源：http://hz.yj202588.top/gtuchothlr.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.birdmap.top/gttvscgorv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhongyouzk.top/gtujiunveq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xingfuxueyuan.xyz/gtjuymxmxu.html

[N11] 二叉树中序遍历
来源：http://hz.shuidangran.top/gtkwxcveud.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yongpay.top/gtxojlmsgx.html

PHP:  // 手写递归函数
来源：http://hz.cheryme.top/gtvdpiqsho.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yongpay.top/gtmyjxvqld.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.mhx1999.top/gthudmwfkt.html

Java: // 手写递归
来源：http://hz.cashguo.top/gtkuaqwmtp.html

Go:   // 手写递归
来源：http://hz.sufxvd.cn/gtkiypwumb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zycfv.cn/gtzvqeyqrg.html

C#:   // 手写递归
来源：http://hz.vqdsnc.cn/gtpygsgchk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cqqwz.cn/gtsyejsebn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.dashuyun.cn/gtnblzguvp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shzxlz.cn/gtcbwjaiob.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhaomingkeji.xyz/gtjytwcqpc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.redwolf501.top/gtjuaajicw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gtscjahpqd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.9152youxi.cn/gtvfjjklxd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ehwqpu.com/gttckwyjez.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj202588.top/gtscmcevir.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtartapwxv.html

O. 并发与异步
来源：http://hz.haohaochexian.top/gtnadvbjyu.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gttouiplmr.html

[O01] 启动一个线程
来源：http://hz.mhx1999.top/gtvubmjwkq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xinyue.icu/gtkujfuqta.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.mhx1999.top/gtfnrxkjje.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenjidiqi.icu/gtlsbkdlzt.html

TS:   // 同 JS
来源：http://hz.dashuyun.cn/gtggkwjqyo.html

Java: new Thread(() -> f()).start()
来源：http://hz.chenzaomai.com/gtubfsipsg.html

Go:   go f()
来源：http://hz.yongpay.top/gtkxxmxvoj.html

Ruby: Thread.new { f }
来源：http://hz.sysykeji.top/gtxetkbfhz.html

C#:   Task.Run(() => F());
来源：http://hz.fzhhl.top/gtvtdwcneo.html

[O02] 使用线程池
来源：http://hz.zhengqikj.top/gtahjlxwaw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cucudq.cn/gtffculseh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zdqjudy.top/gtqboeimjm.html

JS:   // worker_threads 线程池
来源：http://hz.316326.xyz/gtwfsshgml.html

TS:   // worker_threads 线程池
来源：http://hz.pengpengdd.cyou/gtdenwmzlg.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.316326.xyz/gtlzrvndfp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hywenlv.cn/gtvtyqmzty.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hnqzz.top/gtfkpolgyi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.pycfn.com/gtapuoqydy.html

[O03] 加锁保护共享数据
来源：http://hz.shanyushiyangtech.top/gtkqhdnfly.html

Py:   with lock: shared += 1
来源：http://hz.tanke756.top/gtabeylqij.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cucudq.cn/gthjtdqjuh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.kuanghao11.cn/gtlimxnmyc.html

TS:   // 同 JS
来源：http://hz.yueranfly.top/gtslijnasf.html

Java: synchronized (this) { shared++; }
来源：http://hz.gzhubu.top/gtieubukdm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ivvv.top/gtzrrpsjua.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ivvv.top/gtwznfhyox.html

C#:   lock (gate) { shared++; }
来源：http://hz.shzxlz.cn/gthtvtsaqe.html

[O04] 定义异步函数并等待
来源：http://hz.vqdsnc.cn/gtnyafufdi.html

Py:   async def f():⏎    await g()
来源：http://hz.guannengcc.top/gteberypfy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ydzc1.top/gtffxzxagb.html

JS:   async function f() { await g(); }
来源：http://hz.fengsongda.top/gtmgsykbdr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.nanxinkj.top/gtulhfdpyi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hywenlv.cn/gtusplwtlt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.gotoacloud.top/gtesiqvksc.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.9152youxi.cn/gtkvkxzyva.html

C#:   async Task F() { await G(); }
来源：http://hz.cheryme.top/gtwepknxsh.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj20258.top/gtxzgqeotf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zycfv.cn/gtqkzczims.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.guannengcc.top/gtumfxtvdf.html

JS:   await Promise.all(tasks)
来源：http://hz.quarkkingdee.top/gtojwnvckm.html

TS:   await Promise.all(tasks)
来源：http://hz.iojbl.cn/gtxzzfpdca.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yj20258.top/gttsxfmcbk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xuetiantiany.cn/gtjhtdtybs.html

Ruby: threads.map(&:join)
来源：http://hz.xylfe.cn/gtxmrknzvc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.tian-w.cn/gtrjdrhcch.html

[O06] 使用进程池
来源：http://hz.yj20258888.top/gtkkmywfjl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.nanxinkj.top/gtzrlvyctf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.dianchejie.cn/gtyvzcqgwx.html

JS:   // child_process / cluster 模块
来源：http://hz.andypj.xyz/gtpznsufvh.html

TS:   // child_process / cluster 模块
来源：http://hz.zdqjudy.top/gtzojdyqql.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.shangyingyoupin.top/gtiiehahbr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.sweek.top/gtrquqdyhx.html

Ruby: // fork 块
来源：http://hz.jiagoushi.top/gtstxwgdoh.html

C#:   Parallel.For
来源：http://hz.zhengqikj.top/gtropzlyum.html

================================================================================
来源：http://hz.jianghu66.top/gtdqvyuqun.html

P. 常用工具函数
来源：http://hz.andypj.xyz/gtrmchubdx.html

================================================================================
来源：http://hz.jiagoushi.top/gthlovvfpr.html

[P01] 生成 UUID
来源：http://hz.tian-w.cn/gtstnouakf.html

Py:   str(uuid.uuid4())
来源：http://hz.shuidangran.top/gtfsngoljc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yuxming.cn/gtsojpazea.html

JS:   crypto.randomUUID()
来源：http://hz.c1oappe.top/gtojngxkdv.html

TS:   crypto.randomUUID()
来源：http://hz.yonumen.top/gtmfnorohq.html

Java: UUID.randomUUID().toString()
来源：http://hz.guowangkeji.top/gtrpuwrqyd.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj20258888.top/gtyhcubszg.html

Ruby: SecureRandom.uuid
来源：http://hz.sysykeji.top/gtkxagnwxl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jyoumei.cn/gtjflziiva.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jiagoushi.top/gtmhrnzbem.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cheryme.top/gthuigcywp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinqigufen.top/gtguxgcunn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.sysykeji.top/gteqhgcwih.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gogol.net.cn/gtsxitpksl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.daxiang520.top/gtsezvhyjs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hnxiangtu.top/gttbyibnbq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zdqjudy.top/gtbsmbxyaz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.gaohongyu789.top/gtitolling.html

[P03] 生成短随机字符串
来源：http://hz.iojbl.cn/gtmvfudgbn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.9152youxi.cn/gtilbdkvzd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ehwqpu.com/gtofmsagfp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhongyouzk.top/gtmcdanwhh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258.top/gtonaewqfq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shuidangran.top/gtvhqavcie.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.daxiang520.top/gttycmylea.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.c1oappe.top/gtagpjzorf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.quarkkingdee.top/gtmoifxmtx.html

[P04] 求长度
来源：http://hz.yonumen.top/gtfahnpanl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hammf.cn/gtgeprgvtp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zdqjudy.top/gtnucnfqeb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gogol.net.cn/gtsiadtfnf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cheryme.top/gtnbjzkxue.html

Java: list.size();  map.size();  s.length()
来源：http://hz.kuanghao11.cn/gtbksvlmfs.html

Go:   len(arr);  len(m)
来源：http://hz.iojbl.cn/gtyvzasloq.html

Ruby: x.length;  x.size
来源：http://hz.redwolf501.top/gtnsxwyqit.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhengqikj.top/gtnaugwoaz.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhiwuduotai.top/gtnlkxoyfb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.316326.xyz/gtivpjcjdq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.gotoacloud.top/gttdroqvdn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhengqikj.top/gtaejoyrrl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgfzy.top/gtednpeupk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.iojbl.cn/gtevkmeior.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hywenlv.cn/gtrxgnvaxi.html

Ruby: a == b
来源：http://hz.sweek.top/gtfoanmugt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cucudq.cn/gtfrybmobs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sufxvd.cn/gtmpeaquum.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yj202588.top/gtwcwvbttk.html

PHP:  if (empty($x)) {}
来源：http://hz.sxryk.cn/gtlzqeawyy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.gzhubu.top/gtkkxpenlc.html

TS:   if (x == null) {}
来源：http://hz.ydzc1.top/gtlzkvgvjq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hnqzz.top/gtjgbmyugn.html

Go:   if x == nil {}
来源：http://hz.ivvv.top/gtoigvdfco.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.sufxvd.cn/gtkhjinnic.html

C#:   if (x is null) {}
来源：http://hz.zhoulong.xyz/gtfplyxghc.html

[P07] 防抖与节流
来源：http://hz.hammf.cn/gtlcunmbgf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cqqwz.cn/gtlnwjptur.html

PHP:  // 手写时间戳比较
来源：http://hz.yueranfly.top/gtdputmoet.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yongpay.top/gtjmisrnwz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangkeji.top/gtrfpxvtwr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.52xcode.cn/gtvfpyopah.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.smart0.xyz/gtvcumphsv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cqqwz.cn/gtjyfaobdx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xylfe.cn/gtifbqqjbr.html

[P08] 处理浮点精度问题
来源：http://hz.xziqi.cn/gtuuslddch.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yj202588.top/gtueuzbfav.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.nanxuanxn.top/gthsbdaiul.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gaohongyu789.top/gtwcodbavm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.sysykeji.top/gtuuxplily.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zycfv.cn/gtynsbxwsg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.nanxuanxn.top/gtzijurcid.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.chenzaomai.com/gtxwkyvonm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenlongwang.top/gtabfttwfi.html

================================================================================
来源：http://hz.nanxinkj.top/gtpqgngtmv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.dianchejie.cn/gtrkynlsfp.html

================================================================================
来源：http://hz.tanke756.top/gtzrdaabfr.html

[Q01] 创建表
来源：http://hz.gotoacloud.top/gtecomtszg.html

CREATE TABLE users (
来源：http://hz.bjfxy.top/gtjzpumhgg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydjk.org.cn/gtgpiangxm.html

name VARCHAR(50) NOT NULL,
来源：http://hz.aibaodan.cn/gtzztzwoub.html

email VARCHAR(100) UNIQUE,
来源：http://hz.guannengcc.top/gtawywcdvt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.daria6918.cn/gtkmosmcuh.html

);
来源：http://hz.zhengqikj.top/gtjssmaflb.html

[Q02] 创建带外键的表
来源：http://hz.hammf.cn/gtqkrumnli.html

CREATE TABLE orders (
来源：http://hz.wangdashe.top/gtbnivprrv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yuxming.cn/gtdnohvwgz.html

user_id INT NOT NULL,
来源：http://hz.jinyuanbaomall.cn/gtawygshxb.html

amount DECIMAL(10, 2),
来源：http://hz.hammf.cn/gtbwhfbpxi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.vqdsnc.cn/gtespnxovw.html

);
来源：http://hz.zhongyouzk.top/gtbuewdqlk.html

[Q03] 增加列
来源：http://hz.yj20258888.top/gtcloqjevz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ywan-chungtsiang.top/gtgyujdgwp.html

[Q04] 修改列类型
来源：http://hz.xylfe.cn/gtessosman.html


<!-- 参考信息 -->