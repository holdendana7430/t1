代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xingfuxueyuan.xyz/gtmkjurtvj.html

[M05] 设置退出码
来源：http://hz.yongpay.top/gtntyotqqz.html

Py:   sys.exit(1)
来源：http://hz.iojbl.cn/gteokqepcs.html

PHP:  exit(1);
来源：http://hz.nanxinkj.top/gtrwqkslpa.html

JS:   process.exit(1)
来源：http://hz.guowangkeji.top/gtpiqrkywu.html

TS:   process.exit(1)
来源：http://hz.hnxiangtu.top/gtczeqwyfm.html

Java: System.exit(1)
来源：http://hz.zhongyouzk.top/gtcuxoaztc.html

Go:   os.Exit(1)
来源：http://hz.cqqwz.cn/gtalcxmurw.html

Ruby: exit 1
来源：http://hz.zhengqikj.top/gtlyayvgqz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.0kj1m.cn/gtdlepcpem.html

[M06] 向标准错误输出
来源：http://hz.chenlongwang.top/gtlahdhref.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinqigfzy.top/gthpydfpxz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gaohongyu789.top/gtsxhpmccp.html

JS:   console.error("err")
来源：http://hz.jqgufenzy.top/gtjcqbpqdd.html

TS:   console.error("err")
来源：http://hz.yuxming.cn/gtkfbgihyv.html

Java: System.err.println("err")
来源：http://hz.cucudq.cn/gtyiueksgy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.snrcjt.cn/gtugskugfj.html

Ruby: warn "err"
来源：http://hz.zhaomingkeji.xyz/gtgfooomqy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yvedp.cn/gtrsrwkzud.html

[M07] 判断是否为主入口
来源：http://hz.shanyushiyangtech.top/gtrwwgfldg.html

Py:   if __name__ == "__main__":
来源：http://hz.zhengqikj.top/gtljvogzhu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.daxiang520.top/gtarybwklp.html

JS:   require.main === module
来源：http://hz.tanke756.top/gtpzbipyex.html

TS:   require.main === module
来源：http://hz.jinqigufen.top/gtxktsmezt.html

Java: public static void main(String[] args)
来源：http://hz.yonumen.top/gthemkpizk.html

Go:   func main()
来源：http://hz.cucudq.cn/gtiizbthrz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhengqikj.top/gtscljvmlp.html

C#:   static void Main(string[] args)
来源：http://hz.jqgufenzy.top/gtdomqxmis.html

[M08] 获取系统与运行时信息
来源：http://hz.gaohongyu789.top/gtnubhppyo.html

Py:   platform.system();  platform.python_version()
来源：http://hz.sufxvd.cn/gtyodopizr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhoulong.xyz/gtorxzjzvv.html

JS:   process.platform;  process.version
来源：http://hz.gogol.net.cn/gteyabryte.html

TS:   process.platform;  process.version
来源：http://hz.jinyuanbaomall.cn/gtupsqquzr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cqqwz.cn/gtwejrrkja.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.andypj.xyz/gtxnkzqlht.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.aizwys.cn/gtuxsczdcq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hongshengwenyu.top/gtynqgygzg.html

================================================================================
来源：http://hz.xinyue.icu/gtyerekklr.html

N. 数据结构与算法
来源：http://hz.jianghu66.top/gtpmsezprf.html

================================================================================
来源：http://hz.chenlongwang.top/gtvlayqeul.html

[N01] 二分查找（有序数组）
来源：http://hz.zhiwuduotai.top/gtrjtofakt.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yuanzhike.top/gtcqsvikmu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gotoacloud.top/gtjfhabgpy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ivvv.top/gtuejzjbvz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgfzy.top/gtenpfzfzp.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ppjwa.cn/gtnfoskegx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.birdmap.top/gtzixaqwuw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.pycfn.com/gtoftfjjws.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.tanke756.top/gtlsznxpqz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zycfv.cn/gtjstuoita.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.dashuyun.cn/gtopfiafgt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.gzhubu.top/gtjdkvryyw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guowangkeji.top/gtmpcghkcb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.c1oappe.top/gtpcbzmzby.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.chenjidiqi.icu/gtpveogemt.html

Go:   slices.Sort(arr)
来源：http://hz.jinghuilouyu.cn/gtgrsugdwc.html

Ruby: arr.sort
来源：http://hz.nwbrower.top/gttfdtskxe.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sufxvd.cn/gtmixjvzvy.html

[N03] 快速排序（分治示例）
来源：http://hz.mhx1999.top/gtlcpcepmg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yanxiufei.cn/gtqhnalssa.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jianghu66.top/gtaxvuspkr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zycfv.cn/gtxdyzugqi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yvedp.cn/gtmgrnfmta.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hammf.cn/gtybcvuofb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.sysykeji.top/gtwpacbwdr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.andypj.xyz/gtqqsqfsiz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.daria6918.cn/gtxqawzjsq.html

[N04] 斐波那契数列
来源：http://hz.pengpengdd.cyou/gtcbqskeeq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangtech.top/gtfwgimqsb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xuanzx.com/gtwqruvybz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuxming.cn/gtldslwxai.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.feifeiyinyue.top/gtvetriugx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yj202588.top/gtkyunpmhx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.redwolf501.top/gtsmjtigql.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ivvv.top/gtrxvdjmyu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yangfankeji.com/gtxbroqdgi.html

[N05] 最大公约数
来源：http://hz.guowangkeji.top/gtdofivmcq.html

Py:   math.gcd(a, b)
来源：http://hz.jinghuilouyu.cn/gtmxmttpyk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.dashuyun.cn/gtewyaaiob.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenjidiqi.icu/gtpjrtqffc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daxiang520.top/gtwmercfoy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yj20258.top/gtptxhawsv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.andypj.xyz/gttxzpigpn.html

Ruby: a.gcd(b)
来源：http://hz.andypj.xyz/gtwkecwbml.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.snrcjt.cn/gtfkgzhqej.html

[N06] 判断回文字符串
来源：http://hz.wangshuangyany.cn/gtbilnlede.html

Py:   s == s[::-1]
来源：http://hz.jinyuanbaomall.cn/gtuvhkuvln.html

PHP:  $s === strrev($s);
来源：http://hz.shanyushiyangkeji.top/gtlzeqjohq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.gzhubu.top/gtaiqnofxy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ywan-chungtsiang.top/gtnokebpdu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.andypj.xyz/gtgltrhpcn.html

Go:   // 双指针从两端比较
来源：http://hz.yvedp.cn/gtwvsundya.html

Ruby: s == s.reverse
来源：http://hz.nwbrower.top/gtfckfduik.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.smart0.xyz/gtbflxvaxz.html

[N07] 两数之和（返回下标）
来源：http://hz.hongshengwenyu.top/gtvngujdkq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhengqikj.top/gtlebutvll.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yuxming.cn/gtlccutsxu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yuanzhike.top/gtghaljozl.html

TS:   // 手写 Map<string, number>
来源：http://hz.jyoumei.cn/gtckzmmwzu.html

Java: // 手写 HashMap
来源：http://hz.cashguo.top/gtowdbttrh.html

Go:   // 手写 map[int]int
来源：http://hz.yanxiufei.cn/gtbbrwyiue.html

Ruby: // 手写 Hash
来源：http://hz.nwbrower.top/gtlpylwsyt.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shuidangran.top/gthbgyedlu.html

[N08] 生成全排列
来源：http://hz.tianlin.xyz/gtoyfcbsfh.html

Py:   itertools.permutations(arr)
来源：http://hz.xylfe.cn/gtzdtcdama.html

PHP:  // 手写递归交换
来源：http://hz.guannengcc.top/gtkxckeusx.html

JS:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtverrzads.html

TS:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtwybvksaa.html

Java: // 手写回溯递归
来源：http://hz.aibaodan.cn/gtmpxaejbx.html

Go:   // 手写回溯递归
来源：http://hz.dianchejie.cn/gtfbqjanhe.html

Ruby: arr.permutation.to_a
来源：http://hz.c1oappe.top/gtazynhiuy.html

C#:   // 手写回溯递归
来源：http://hz.ivvv.top/gtmmxxryfl.html

[N09] 栈与队列
来源：http://hz.xinyue.icu/gtnzuoroxk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.aibaodan.cn/gtaifanrrl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.c1oappe.top/gtejbutdps.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.meibo888.top/gtyxjpynym.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yvedp.cn/gtgejfdais.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hywenlv.cn/gtrufpvmsm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.aizwys.cn/gtdrjwmfkk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.mhx1999.top/gtuvghfcvm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yj20258.top/gtyikwvdfc.html

[N10] 链表节点定义
来源：http://hz.jqgufenzy.top/gtydmpgnpe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ehwqpu.com/gthfvjwlen.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.smart0.xyz/gtedmgqatg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ybcxt.top/gtbjdtxpjm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sysykeji.top/gtxvihyhzq.html

Java: class Node { int v; Node next; }
来源：http://hz.cdnleiting.top/gttacghwdk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.aizwys.cn/gtptkcgqqe.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinqigufen.top/gtdhqwqoum.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.mhx1999.top/gtoxzwkiyc.html

[N11] 二叉树中序遍历
来源：http://hz.jqgfzy.top/gtxaaodule.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jianghu66.top/gtdydxmsut.html

PHP:  // 手写递归函数
来源：http://hz.kuanghao11.cn/gtlomjpwye.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.snrcjt.cn/gthmgoystn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.wangshuangyany.cn/gtkuvinnwo.html

Java: // 手写递归
来源：http://hz.hnqzz.top/gtdmwbvgmd.html

Go:   // 手写递归
来源：http://hz.xinyue.icu/gttisblroo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.wangshuangyany.cn/gtxmjfwkpk.html

C#:   // 手写递归
来源：http://hz.sysykeji.top/gtdxxihmdf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.wangshuangyany.cn/gtegoiwsfl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.havefunace.top/gtcwszhand.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.nanxinkj.top/gtxyfkxgyp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.52xcode.cn/gtnhzelnom.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cheryme.top/gteyuopknh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.quarkkingdee.top/gtomtdnrpu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhijiandao.cn/gtchjpfild.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.kuanghao11.cn/gtreathtdi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xylfe.cn/gtdfotolgj.html

================================================================================
来源：http://hz.jianghu66.top/gtuezohwbm.html

O. 并发与异步
来源：http://hz.zycfv.cn/gtihkqllfh.html

================================================================================
来源：http://hz.zhengqikj.top/gtiftmubsl.html

[O01] 启动一个线程
来源：http://hz.zhaomingkeji.xyz/gtehcypiqb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.316326.xyz/gtwxtetvzc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.pycfn.com/gtpmjhawuu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.dianchejie.cn/gtotufwsof.html

TS:   // 同 JS
来源：http://hz.fengsongda.top/gtwnhmqxta.html

Java: new Thread(() -> f()).start()
来源：http://hz.ywan-chungtsiang.top/gtrcltfxbi.html

Go:   go f()
来源：http://hz.cdnleiting.top/gtzyfofqdh.html

Ruby: Thread.new { f }
来源：http://hz.yvedp.cn/gtbnsdhebs.html

C#:   Task.Run(() => F());
来源：http://hz.jianghu66.top/gtdcgtxohy.html

[O02] 使用线程池
来源：http://hz.ydjk.org.cn/gtmyzitfqe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.birdmap.top/gtavsdjjfc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.meibo888.top/gtageuelsz.html

JS:   // worker_threads 线程池
来源：http://hz.jlsjyb.cn/gtgwtzuwbx.html

TS:   // worker_threads 线程池
来源：http://hz.cqqwz.cn/gtcvahltde.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cheryme.top/gtrwzzszga.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhixingplan.top/gtjilnfves.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.tianlin.xyz/gttnbilgmj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.chenjidiqi.icu/gtiyfthqyw.html

[O03] 加锁保护共享数据
来源：http://hz.jinghuilouyu.cn/gtclkyszlc.html

Py:   with lock: shared += 1
来源：http://hz.cashguo.top/gtopnxvgij.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yangfankeji.com/gtdpqsfknb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hnxiangtu.top/gtazqxqste.html

TS:   // 同 JS
来源：http://hz.shanyushiyangtech.top/gtokklvcag.html

Java: synchronized (this) { shared++; }
来源：http://hz.jianghu66.top/gtcikxhtdz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhengqikj.top/gtgutkrexi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.52xcode.cn/gtexjbxfxc.html

C#:   lock (gate) { shared++; }
来源：http://hz.gaohongyu789.top/gttyvrzjqh.html

[O04] 定义异步函数并等待
来源：http://hz.zhijiandao.cn/gtaqfizkwh.html

Py:   async def f():⏎    await g()
来源：http://hz.hnxiangtu.top/gtbgkswukw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.tian-w.cn/gtfhjvivud.html

JS:   async function f() { await g(); }
来源：http://hz.gotoacloud.top/gtxrihszho.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.wangshuangyany.cn/gtuimcpkgl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.svipenyu.cn/gtcthllmpo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhijiandao.cn/gtgacorgvr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.nanxinkj.top/gtdeqorkcs.html

C#:   async Task F() { await G(); }
来源：http://hz.cqqwz.cn/gtmjftverw.html

[O05] 并发执行并等待全部完成
来源：http://hz.aizwys.cn/gtvzmttafk.html

Py:   asyncio.gather(*tasks)
来源：http://hz.9152youxi.cn/gtinvdglsb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.aizwys.cn/gttltaexgr.html

JS:   await Promise.all(tasks)
来源：http://hz.xingfuxueyuan.xyz/gtenakmdcj.html

TS:   await Promise.all(tasks)
来源：http://hz.dianchejie.cn/gtljxpwydb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.andypj.xyz/gtejfcajza.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jyoumei.cn/gtcoevxeyi.html

Ruby: threads.map(&:join)
来源：http://hz.52xcode.cn/gtsmopxrln.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.fzhhl.top/gtbfmgvgzp.html

[O06] 使用进程池
来源：http://hz.daxiang520.top/gtewluwomb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.wangdashe.top/gtzcutsxhu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.c1oappe.top/gtnghuwimf.html

JS:   // child_process / cluster 模块
来源：http://hz.yueranfly.top/gtqrfvnkzg.html

TS:   // child_process / cluster 模块
来源：http://hz.yueranfly.top/gtfcpdiihm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xuanzx.com/gtwbothldu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.vqdsnc.cn/gtuwkuayai.html

Ruby: // fork 块
来源：http://hz.xinyue.icu/gtgzflknuj.html

C#:   Parallel.For
来源：http://hz.gzhubu.top/gtdoaheabu.html

================================================================================
来源：http://hz.nanxuanxn.top/gtgmxxcwkx.html

P. 常用工具函数
来源：http://hz.shzxlz.cn/gtyubfrrhs.html

================================================================================
来源：http://hz.tianlin.xyz/gtzltapuev.html

[P01] 生成 UUID
来源：http://hz.jinqigufen.top/gtodstaubz.html

Py:   str(uuid.uuid4())
来源：http://hz.yongpay.top/gtnyprbtuh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.tian-w.cn/gtfwrsiyst.html

JS:   crypto.randomUUID()
来源：http://hz.xinyue.icu/gtmxylpceq.html

TS:   crypto.randomUUID()
来源：http://hz.gotoacloud.top/gtfoytgbum.html

Java: UUID.randomUUID().toString()
来源：http://hz.yj20258.top/gtzbiqjyaf.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gzhubu.top/gtorawtkyu.html

Ruby: SecureRandom.uuid
来源：http://hz.quarkkingdee.top/gtfhzxmosa.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhiwuduotai.top/gtlrfhygem.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinqigufen.top/gtuzmtgsqo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.fengsongda.top/gthgxnqino.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hysaishi.cn/gtcyflcfyb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinqigufen.top/gtujmgtlss.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.mhx1999.top/gtlzksfmup.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jinghuilouyu.cn/gtveqybkcu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ydzc1.top/gtlmgzjuiu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xylfe.cn/gtyzcbfddj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yongpay.top/gtfcejdigj.html

[P03] 生成短随机字符串
来源：http://hz.svipenyu.cn/gtpjpvkhwj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.wangshuangyany.cn/gttizldvfh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shuidangran.top/gtjsblqzcd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yueranfly.top/gtjnillivn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhijiandao.cn/gtqwvqibna.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cqqwz.cn/gtlodtpbue.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.fengsongda.top/gtugkwkeeb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.iojbl.cn/gthsqwuhmu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.pengpengdd.cyou/gtchibrdxh.html

[P04] 求长度
来源：http://hz.pengpengdd.cyou/gtoteppkxr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shangyingyoupin.top/gttdwueesy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.daxiang520.top/gtowsqisbk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangdashe.top/gtmocetpaq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yvedp.cn/gtiqhcrzbp.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jinyuanbaomall.cn/gtcnzaxwys.html

Go:   len(arr);  len(m)
来源：http://hz.hfpthk.cn/gtcraesdcc.html

Ruby: x.length;  x.size
来源：http://hz.snrcjt.cn/gtliwewoiu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zdqjudy.top/gtuicqhgoa.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhengqikj.top/gtbbeaohcf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cqqwz.cn/gtqkvixmkm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.chenlongwang.top/gtsdaeapws.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hnqzz.top/gtbofzdwdr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.fzhhl.top/gtucbqlghn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shanyushiyangkeji.top/gteyibnclt.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hfpthk.cn/gthartfjqf.html

Ruby: a == b
来源：http://hz.zhaomingkeji.xyz/gtjcstkgem.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.daria6918.cn/gtuvdwhdts.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.dianchejie.cn/gtvgivgdgt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.smart0.xyz/gtuendaild.html

PHP:  if (empty($x)) {}
来源：http://hz.zycfv.cn/gthgutpbsv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.gaohongyu789.top/gturaqkihc.html

TS:   if (x == null) {}
来源：http://hz.shangyingyoupin.top/gtotsamhqt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhoulong.xyz/gtzlcobtgc.html

Go:   if x == nil {}
来源：http://hz.xinyue.icu/gtkyuhhwqa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cheryme.top/gtiisxbbto.html

C#:   if (x is null) {}
来源：http://hz.gaohongyu789.top/gtqilkhxxu.html

[P07] 防抖与节流
来源：http://hz.smart0.xyz/gtiixulkge.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hongshengwenyu.top/gtuisesdoc.html

PHP:  // 手写时间戳比较
来源：http://hz.quarkkingdee.top/gtwhaofcdn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xylfe.cn/gtdzuxyrzl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sxryk.cn/gtwzpvmabr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yanxiufei.cn/gtwcgshsfq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.kuanghao11.cn/gtuisfwufl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.vqdsnc.cn/gtgyfjries.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cqqwz.cn/gtkzazufff.html

[P08] 处理浮点精度问题
来源：http://hz.shanyushiyangkeji.top/gteagujnvz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.aizwys.cn/gttecsxiqd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.haohaochexian.top/gttkievxnl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jqgufenzy.top/gtusvhwhwz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yuanzhike.top/gtxtbfvfdj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shuidangran.top/gtsvilwjry.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.quarkkingdee.top/gtcvbzebsr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.nanxinkj.top/gtcagizpfs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shangyingyoupin.top/gtolxdmhud.html

================================================================================
来源：http://hz.sweek.top/gtawnqfjri.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.havefunace.top/gtxridoeud.html

================================================================================
来源：http://hz.dashuyun.cn/gtlszhrdfn.html

[Q01] 创建表
来源：http://hz.yuxming.cn/gtsfnikbjz.html

CREATE TABLE users (
来源：http://hz.jinyuanbaomall.cn/gtlvmjugzb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenjidiqi.icu/gtyrbndlqu.html

name VARCHAR(50) NOT NULL,
来源：http://hz.chenlongwang.top/gtrajtjmcm.html

email VARCHAR(100) UNIQUE,
来源：http://hz.chenjidiqi.icu/gtjzzmtcnl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.iojbl.cn/gtyzrpfwmm.html

);
来源：http://hz.zhongyouzk.top/gtuhrguboc.html

[Q02] 创建带外键的表
来源：http://hz.xuetiantiany.cn/gtumwhkefz.html

CREATE TABLE orders (
来源：http://hz.aibaodan.cn/gtxhgnvtbz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xziqi.cn/gtmmebawin.html

user_id INT NOT NULL,
来源：http://hz.jyoumei.cn/gtenmbvvlz.html

amount DECIMAL(10, 2),
来源：http://hz.bjfxy.top/gtudayaqks.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.c1oappe.top/gtqqkxylgt.html

);
来源：http://hz.sysykeji.top/gtpymvoynr.html

[Q03] 增加列
来源：http://hz.meibo888.top/gtplabpphq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.9152youxi.cn/gtfitthukw.html

[Q04] 修改列类型
来源：http://hz.zhengqikj.top/gtfgzpnryr.html


<!-- 参考信息 -->