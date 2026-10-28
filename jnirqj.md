代发 wailian999

[M04] 获取当前工作目录
来源：http://hz.feifeiyinyue.top/gtftfnlqnz.html

Py:   os.getcwd()
来源：http://hz.c1oappe.top/gthhglfwoy.html

PHP:  getcwd();
来源：http://hz.xylfe.cn/gteuftftsu.html

JS:   process.cwd()
来源：http://hz.gotoacloud.top/gtnmtvxwza.html

TS:   process.cwd()
来源：http://hz.hammf.cn/gtwufcpfvt.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shanyushiyangtech.top/gtgefbjyvv.html

Go:   os.Getwd()
来源：http://hz.meibo888.top/gtbuvpgdal.html

Ruby: Dir.pwd
来源：http://hz.iojbl.cn/gtsqsxctso.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jinqigufen.top/gtkvygnhcp.html

[M05] 设置退出码
来源：http://hz.redwolf501.top/gtvcmumnlj.html

Py:   sys.exit(1)
来源：http://hz.zhengqikj.top/gthcgymimk.html

PHP:  exit(1);
来源：http://hz.c1oappe.top/gtexbuacze.html

JS:   process.exit(1)
来源：http://hz.hongshengwenyu.top/gtcivultqu.html

TS:   process.exit(1)
来源：http://hz.yuxming.cn/gtpmbttqhg.html

Java: System.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtiffobvro.html

Go:   os.Exit(1)
来源：http://hz.chenzaomai.com/gtferdcagu.html

Ruby: exit 1
来源：http://hz.yuanzhike.top/gtwxrxixpn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.tian-w.cn/gtlllgxdch.html

[M06] 向标准错误输出
来源：http://hz.jinqigfzy.top/gtuerbisoy.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cucudq.cn/gtbazwfyvz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinghuilouyu.cn/gtkqnplcxg.html

JS:   console.error("err")
来源：http://hz.nwbrower.top/gtpejioqgg.html

TS:   console.error("err")
来源：http://hz.yueranfly.top/gtmbywnzlx.html

Java: System.err.println("err")
来源：http://hz.xylfe.cn/gtoghwkxbh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cheryme.top/gtcajyxvmc.html

Ruby: warn "err"
来源：http://hz.bjfxy.top/gtsglcruor.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.smart0.xyz/gtyxvkkwil.html

[M07] 判断是否为主入口
来源：http://hz.xinyue.icu/gtxfunajbp.html

Py:   if __name__ == "__main__":
来源：http://hz.xuetiantiany.cn/gtseqktrmc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.svipenyu.cn/gtqoobxtdr.html

JS:   require.main === module
来源：http://hz.svipenyu.cn/gtamvpdvsw.html

TS:   require.main === module
来源：http://hz.smart0.xyz/gtqmaynpop.html

Java: public static void main(String[] args)
来源：http://hz.zycfv.cn/gtmkqtyjgp.html

Go:   func main()
来源：http://hz.daxiang520.top/gtinesbwhy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.tianlin.xyz/gtmkogbkle.html

C#:   static void Main(string[] args)
来源：http://hz.jqgfzy.top/gtiikdfzkz.html

[M08] 获取系统与运行时信息
来源：http://hz.daria6918.cn/gtxegsyjbe.html

Py:   platform.system();  platform.python_version()
来源：http://hz.aibaodan.cn/gtoipdwmqa.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.daxiang520.top/gtalknrdrp.html

JS:   process.platform;  process.version
来源：http://hz.snrcjt.cn/gtgzmbgvdt.html

TS:   process.platform;  process.version
来源：http://hz.pycfn.com/gtrlurvkev.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jqgfzy.top/gtzszazeau.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.smart0.xyz/gtcfivxcvm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.fengsongda.top/gtixjpsfpz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sysykeji.top/gtzwhbluga.html

================================================================================
来源：http://hz.aibaodan.cn/gtyawjpjgc.html

N. 数据结构与算法
来源：http://hz.shzxlz.cn/gtfcjshlme.html

================================================================================
来源：http://hz.chenlongwang.top/gtwhjksapk.html

[N01] 二分查找（有序数组）
来源：http://hz.fzhhl.top/gtijmlhcxp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shangyingyoupin.top/gtkqplmlkg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yangfankeji.com/gtnhzkekyd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yueranfly.top/gtstxsicia.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258888.top/gtlmyikfyt.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.0kj1m.cn/gtkjypfnyy.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jqgfzy.top/gtpdoawhbg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.dashuyun.cn/gtkrrfjtwm.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.dashuyun.cn/gtjdxscgsz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhengqikj.top/gtntbhmkex.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cheryme.top/gtevkzaqlm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.iojbl.cn/gtkxsqngvy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.bjfxy.top/gtzyxegenh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gtinngbilk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cashguo.top/gtzstjkvkb.html

Go:   slices.Sort(arr)
来源：http://hz.ywan-chungtsiang.top/gtsagvmruo.html

Ruby: arr.sort
来源：http://hz.shuidangran.top/gtzanzmjdr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhaomingkeji.xyz/gttxmbmajm.html

[N03] 快速排序（分治示例）
来源：http://hz.0kj1m.cn/gtvhbmzzqy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.fzhhl.top/gtipydbhfy.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shangyingyoupin.top/gtswhcfpwd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.birdmap.top/gtqwkypwnm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cdnleiting.top/gtrtrrdsio.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.kuanghao11.cn/gtrxzrvejb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shzxlz.cn/gtyziucxxl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cdnleiting.top/gtjwsreurv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.quarkkingdee.top/gtxuzigwix.html

[N04] 斐波那契数列
来源：http://hz.tian-w.cn/gtwiaehlhk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jlsjyb.cn/gthkelvwjo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zycfv.cn/gtnbghsrqa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fengsongda.top/gtkojwntab.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj202588.top/gtpdvxyuja.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ppjwa.cn/gtsihhzzkv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.dashuyun.cn/gtglfvejlv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.snrcjt.cn/gtissnsogf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.mhx1999.top/gtcwvbjmgk.html

[N05] 最大公约数
来源：http://hz.zhoulong.xyz/gtsrztuhee.html

Py:   math.gcd(a, b)
来源：http://hz.cdnleiting.top/gtbfcwnbnh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jiagoushi.top/gtkiibvicl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zycfv.cn/gtwvhyjbru.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fzhhl.top/gtvokpdkcr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.nanxuanxn.top/gtesswfydp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zdqjudy.top/gtbozdnlcq.html

Ruby: a.gcd(b)
来源：http://hz.xingfuxueyuan.xyz/gtatgtqagg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.chenjidiqi.icu/gtaiqrksuo.html

[N06] 判断回文字符串
来源：http://hz.smart0.xyz/gtujduitil.html

Py:   s == s[::-1]
来源：http://hz.sufxvd.cn/gtkgkvqrhv.html

PHP:  $s === strrev($s);
来源：http://hz.zhixingplan.top/gtpihpppbb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yanxiufei.cn/gtiguuqnlj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gtomdpfzfv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.dashuyun.cn/gtluosqlya.html

Go:   // 双指针从两端比较
来源：http://hz.cucudq.cn/gthgslamso.html

Ruby: s == s.reverse
来源：http://hz.9152youxi.cn/gtnpfhqxkf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ywan-chungtsiang.top/gtzihbezio.html

[N07] 两数之和（返回下标）
来源：http://hz.dianchejie.cn/gtkvocekdl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nanxinkj.top/gtcipcltcf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.chenzaomai.com/gtsisfzrsz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.cashguo.top/gtursjidau.html

TS:   // 手写 Map<string, number>
来源：http://hz.cashguo.top/gtfyfapbxu.html

Java: // 手写 HashMap
来源：http://hz.ydzc1.top/gtsgfmbemd.html

Go:   // 手写 map[int]int
来源：http://hz.quarkkingdee.top/gtlumknekg.html

Ruby: // 手写 Hash
来源：http://hz.chenlongwang.top/gtznspltfy.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yonumen.top/gtetrfeouk.html

[N08] 生成全排列
来源：http://hz.ywan-chungtsiang.top/gtkjetvnuc.html

Py:   itertools.permutations(arr)
来源：http://hz.hnqzz.top/gtskbsumia.html

PHP:  // 手写递归交换
来源：http://hz.xuetiantiany.cn/gtoxyukmfy.html

JS:   // 手写回溯递归
来源：http://hz.tanke756.top/gtcavvdhvf.html

TS:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtenhadhij.html

Java: // 手写回溯递归
来源：http://hz.cucudq.cn/gtubnfhwpl.html

Go:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtwjbxuypy.html

Ruby: arr.permutation.to_a
来源：http://hz.aibaodan.cn/gtzyvbmcpw.html

C#:   // 手写回溯递归
来源：http://hz.jyoumei.cn/gtoajkfvfa.html

[N09] 栈与队列
来源：http://hz.52xcode.cn/gtiesbnpjl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.9152youxi.cn/gtxtihmhuu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.chenlongwang.top/gtunbfpdaz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.andypj.xyz/gtpptdbyja.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.nanxuanxn.top/gtwuxgzsff.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.9152youxi.cn/gtxblihlwa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhaomingkeji.xyz/gtghcgwiyz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xuetiantiany.cn/gtwcwqtgcj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gzhubu.top/gtpkoirugg.html

[N10] 链表节点定义
来源：http://hz.jqgufenzy.top/gtjhupombg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ehwqpu.com/gtgoaelyee.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinyuanbaomall.cn/gtatayunan.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xziqi.cn/gtjgkimxge.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.nanxinkj.top/gttjtemyff.html

Java: class Node { int v; Node next; }
来源：http://hz.nanxinkj.top/gtzrjwuvag.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.smart0.xyz/gtwcbtappw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shanyushiyangkeji.top/gtlqwcytox.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zdqjudy.top/gtioyyaahz.html

[N11] 二叉树中序遍历
来源：http://hz.aibaodan.cn/gtgliixsgf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yonumen.top/gtukispmso.html

PHP:  // 手写递归函数
来源：http://hz.gzhubu.top/gthndfqdtn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnxiangtu.top/gtfisuhkli.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zycfv.cn/gtspydbcmw.html

Java: // 手写递归
来源：http://hz.zhengqikj.top/gtfskeydos.html

Go:   // 手写递归
来源：http://hz.nanxinkj.top/gtnttvntdu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tianlin.xyz/gtnhsrysem.html

C#:   // 手写递归
来源：http://hz.nwbrower.top/gtpvmjvtkp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xingfuxueyuan.xyz/gtnrguskin.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jqgfzy.top/gtctftunbl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hywenlv.cn/gtmzgdaprs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuetiantiany.cn/gtehusmmwb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinqigufen.top/gtylhxrvry.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cashguo.top/gtytquqwnh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yanxiufei.cn/gtmpxlkorc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jiagoushi.top/gtyeuotleb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cheryme.top/gtlwnnqjtw.html

================================================================================
来源：http://hz.ydjk.org.cn/gtlycjiwdr.html

O. 并发与异步
来源：http://hz.haohaochexian.top/gtidimyhor.html

================================================================================
来源：http://hz.zhengqikj.top/gtqejrkbby.html

[O01] 启动一个线程
来源：http://hz.hfpthk.cn/gteubczikd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xziqi.cn/gtddbdnmcb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.chenlongwang.top/gtlhxlruuo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xuanzx.com/gtohvypmkr.html

TS:   // 同 JS
来源：http://hz.daxiang520.top/gtkgajmqla.html

Java: new Thread(() -> f()).start()
来源：http://hz.gzhubu.top/gtpipjgybq.html

Go:   go f()
来源：http://hz.snrcjt.cn/gtcjezhuzd.html

Ruby: Thread.new { f }
来源：http://hz.quarkkingdee.top/gtkumfznjh.html

C#:   Task.Run(() => F());
来源：http://hz.yj202588.top/gtiwraxbza.html

[O02] 使用线程池
来源：http://hz.jlsjyb.cn/gtrgkzjikf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.316326.xyz/gtgflwostk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sysykeji.top/gtnuvenqlg.html

JS:   // worker_threads 线程池
来源：http://hz.0kj1m.cn/gteqvxtdwg.html

TS:   // worker_threads 线程池
来源：http://hz.andypj.xyz/gtbjcncxgi.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.0kj1m.cn/gtxnygxcpz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.guannengcc.top/gtvjqkiboq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yonumen.top/gtjtlsegjc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.kuanghao11.cn/gtgrbbtvqq.html

[O03] 加锁保护共享数据
来源：http://hz.yj20258.top/gtrqnslhye.html

Py:   with lock: shared += 1
来源：http://hz.shangyingyoupin.top/gtyciskxik.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.meibo888.top/gtdxqyfrhq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.daxiang520.top/gtuuxkrpfo.html

TS:   // 同 JS
来源：http://hz.nwbrower.top/gtyahbfecr.html

Java: synchronized (this) { shared++; }
来源：http://hz.haohaochexian.top/gtgpnnigfe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ppjwa.cn/gtvuzvxspp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.wangdashe.top/gtwbeelmvf.html

C#:   lock (gate) { shared++; }
来源：http://hz.fzhhl.top/gtdwuwxgau.html

[O04] 定义异步函数并等待
来源：http://hz.zhixingplan.top/gtszirhpkl.html

Py:   async def f():⏎    await g()
来源：http://hz.guannengcc.top/gtprikjujv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.haohaochexian.top/gtzlpuuarb.html

JS:   async function f() { await g(); }
来源：http://hz.sxryk.cn/gttfnfsfek.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shuidangran.top/gtbwayfuud.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.redwolf501.top/gttscsmadm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhiwuduotai.top/gtoeamrswm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ivvv.top/gtqtjuxfze.html

C#:   async Task F() { await G(); }
来源：http://hz.gotoacloud.top/gtnagrnydl.html

[O05] 并发执行并等待全部完成
来源：http://hz.xingfuxueyuan.xyz/gtfceaejal.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gaohongyu789.top/gtzdjfzwxt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.mhx1999.top/gtxltulgmd.html

JS:   await Promise.all(tasks)
来源：http://hz.wangshuangyany.cn/gtvusbznhj.html

TS:   await Promise.all(tasks)
来源：http://hz.wangdashe.top/gtzknsakjb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.aizwys.cn/gtwhnnhdrj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhijiandao.cn/gtundpholb.html

Ruby: threads.map(&:join)
来源：http://hz.gaohongyu789.top/gtjgujgdyu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zycfv.cn/gtponzzgqy.html

[O06] 使用进程池
来源：http://hz.yj20258.top/gtvcrdxiek.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.pycfn.com/gtiasynijp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shangyingyoupin.top/gtaieqacmz.html

JS:   // child_process / cluster 模块
来源：http://hz.hnqzz.top/gtmsfaylcs.html

TS:   // child_process / cluster 模块
来源：http://hz.zhijiandao.cn/gtsvcyzhnd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hnqzz.top/gtupudxgey.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.quarkkingdee.top/gtkxirvult.html

Ruby: // fork 块
来源：http://hz.redwolf501.top/gtuaiwsxdv.html

C#:   Parallel.For
来源：http://hz.ehwqpu.com/gtrxonkymn.html

================================================================================
来源：http://hz.birdmap.top/gtbmknpedd.html

P. 常用工具函数
来源：http://hz.shangyingyoupin.top/gtqlzpmonc.html

================================================================================
来源：http://hz.gotoacloud.top/gtspumhrcd.html

[P01] 生成 UUID
来源：http://hz.chenlongwang.top/gtdrcpvyvz.html

Py:   str(uuid.uuid4())
来源：http://hz.sxryk.cn/gtpxhdwcjs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.tianlin.xyz/gtrkzjnkum.html

JS:   crypto.randomUUID()
来源：http://hz.hnxiangtu.top/gtgqdmamvf.html

TS:   crypto.randomUUID()
来源：http://hz.pycfn.com/gtdqkvehtr.html

Java: UUID.randomUUID().toString()
来源：http://hz.yvedp.cn/gtmnkxyhzh.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yuanzhike.top/gtbpzovzfd.html

Ruby: SecureRandom.uuid
来源：http://hz.hysaishi.cn/gthzditcvd.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.nanxuanxn.top/gtxyefpymt.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shanyushiyangtech.top/gtzvixpwvj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xinyue.icu/gtinrqixib.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.feifeiyinyue.top/gtefhhxanv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xuetiantiany.cn/gtduuobefx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ppjwa.cn/gteqgzpnrm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yonumen.top/gtrrbbgfle.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zdqjudy.top/gtfbqlhnsh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cucudq.cn/gtxykxzgyy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ehwqpu.com/gtfsutncdj.html

[P03] 生成短随机字符串
来源：http://hz.jqgufenzy.top/gtlqtjjcvj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.nanxuanxn.top/gtupvzozjo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yj202588.top/gtlsbjjcod.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.snrcjt.cn/gtcsxcbqon.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shuidangran.top/gtmibgdjyu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.vqdsnc.cn/gtuhlirlar.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.guannengcc.top/gtsrmxxrbx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jqgufenzy.top/gtxcgazbue.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jqgufenzy.top/gtsvjwdclm.html

[P04] 求长度
来源：http://hz.nanxinkj.top/gtqffztezm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.52xcode.cn/gtzdyjachl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aizwys.cn/gtnhajvxiw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.52xcode.cn/gtrnxatilg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.havefunace.top/gtzllfptqh.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhaomingkeji.xyz/gtwbbtghmb.html

Go:   len(arr);  len(m)
来源：http://hz.vqdsnc.cn/gtdbqxiger.html

Ruby: x.length;  x.size
来源：http://hz.cucudq.cn/gtuleiumiz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.smart0.xyz/gtlzonqcfb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.tanke756.top/gtlpeetnje.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hywenlv.cn/gtdqypqoag.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.wangshuangyany.cn/gtczrzodmw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zycfv.cn/gthohrxapz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhixingplan.top/gtcctytset.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shanyushiyangtech.top/gtnjxbsoof.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jqgufenzy.top/gtxocgbaxx.html

Ruby: a == b
来源：http://hz.jiagoushi.top/gtlobtogcn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shzxlz.cn/gtaosdfntq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhengqikj.top/gtbklgnrex.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jinghuilouyu.cn/gtnjuejmpz.html

PHP:  if (empty($x)) {}
来源：http://hz.hfpthk.cn/gtyajosumk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shzxlz.cn/gttqheqkqc.html

TS:   if (x == null) {}
来源：http://hz.hnxiangtu.top/gtdrdfqvio.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.daria6918.cn/gtsuhwixuq.html

Go:   if x == nil {}
来源：http://hz.316326.xyz/gtvfuivknw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yj20258888.top/gtiysujjdp.html

C#:   if (x is null) {}
来源：http://hz.ivvv.top/gtczrlnsxc.html

[P07] 防抖与节流
来源：http://hz.fengsongda.top/gtswqrulpj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yuanzhike.top/gtwsfsgqpt.html

PHP:  // 手写时间戳比较
来源：http://hz.snrcjt.cn/gtjtffiraz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hammf.cn/gthnxjtlgo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydjk.org.cn/gtvrxkznic.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.tanke756.top/gtegexpddx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.sweek.top/gtuaqaxgyk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.nanxinkj.top/gtyqptutdy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ppjwa.cn/gtxochyqqi.html

[P08] 处理浮点精度问题
来源：http://hz.ywan-chungtsiang.top/gtrshtnezh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shuidangran.top/gtrahhfaji.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yvedp.cn/gtqkokfwzu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zycfv.cn/gtirtchvem.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.andypj.xyz/gtarpjxdir.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shangyingyoupin.top/gteutasvil.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jiagoushi.top/gtunksuphq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cucudq.cn/gtrycxeqth.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenjidiqi.icu/gtzzqwzmje.html

================================================================================
来源：http://hz.jiagoushi.top/gtqiujwdak.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xuetiantiany.cn/gtfrmtnjhk.html

================================================================================
来源：http://hz.gotoacloud.top/gtvjadqugo.html

[Q01] 创建表
来源：http://hz.sxryk.cn/gtwgbkvdri.html

CREATE TABLE users (
来源：http://hz.fengsongda.top/gtuhioyrtz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yongpay.top/gtxxouskau.html

name VARCHAR(50) NOT NULL,
来源：http://hz.guannengcc.top/gtnkuhdrta.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jyoumei.cn/gthhtkishh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yj20258888.top/gtsqrivdzf.html

);
来源：http://hz.tian-w.cn/gtblgighsa.html

[Q02] 创建带外键的表
来源：http://hz.smart0.xyz/gttnuscjcp.html

CREATE TABLE orders (
来源：http://hz.xinyue.icu/gtkzlupvtv.html


<!-- 参考信息 -->