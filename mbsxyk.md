代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.fzhhl.top/gtatikzbda.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zycfv.cn/gtglmavvqg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xingfuxueyuan.xyz/gtpocsujqb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.snrcjt.cn/gtgdjbrzbi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.fengsongda.top/gtxzxpdjpt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shangyingyoupin.top/gtbijhycfz.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hnxiangtu.top/gthfygkfea.html

C#:   Process.Start("ls", "-l");
来源：http://hz.fzhhl.top/gtzshttbeb.html

[M04] 获取当前工作目录
来源：http://hz.snrcjt.cn/gtzfbzpnat.html

Py:   os.getcwd()
来源：http://hz.shuidangran.top/gtbfbtdlsb.html

PHP:  getcwd();
来源：http://hz.hysaishi.cn/gtlmzpljzz.html

JS:   process.cwd()
来源：http://hz.ppjwa.cn/gtqsbhhkji.html

TS:   process.cwd()
来源：http://hz.chenlongwang.top/gtjbrotowq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hnxiangtu.top/gtodhaaccd.html

Go:   os.Getwd()
来源：http://hz.zhongyouzk.top/gtefniygso.html

Ruby: Dir.pwd
来源：http://hz.smart0.xyz/gtilrqegni.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhoulong.xyz/gtqfziqjek.html

[M05] 设置退出码
来源：http://hz.yueranfly.top/gtngrfnwcl.html

Py:   sys.exit(1)
来源：http://hz.andypj.xyz/gtsbnfpzba.html

PHP:  exit(1);
来源：http://hz.jyoumei.cn/gtjezkjofp.html

JS:   process.exit(1)
来源：http://hz.52xcode.cn/gtxvkyatfm.html

TS:   process.exit(1)
来源：http://hz.andypj.xyz/gtclndvjjy.html

Java: System.exit(1)
来源：http://hz.jiagoushi.top/gtycmtobcx.html

Go:   os.Exit(1)
来源：http://hz.svipenyu.cn/gtxrprrgwk.html

Ruby: exit 1
来源：http://hz.nwbrower.top/gtdtzgtrdy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.wangdashe.top/gtiroukaeq.html

[M06] 向标准错误输出
来源：http://hz.yj20258.top/gttgqidjwh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.wangshuangyany.cn/gtmszwbwxi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shanyushiyangkeji.top/gtuwlqqnsr.html

JS:   console.error("err")
来源：http://hz.bjfxy.top/gtugmkdugb.html

TS:   console.error("err")
来源：http://hz.gogol.net.cn/gtlacfuuej.html

Java: System.err.println("err")
来源：http://hz.yj202588.top/gtkvgobnhx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.tian-w.cn/gtfdhfcvba.html

Ruby: warn "err"
来源：http://hz.zhixingplan.top/gtkmouyrgp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shangyingyoupin.top/gtjpkykmuy.html

[M07] 判断是否为主入口
来源：http://hz.316326.xyz/gtaplxuzfd.html

Py:   if __name__ == "__main__":
来源：http://hz.xziqi.cn/gtfjmwuwux.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hysaishi.cn/gtgtyjvacd.html

JS:   require.main === module
来源：http://hz.jianghu66.top/gtmxjdmhap.html

TS:   require.main === module
来源：http://hz.sxryk.cn/gtpiyjaxvj.html

Java: public static void main(String[] args)
来源：http://hz.cdnleiting.top/gtpeocpqlj.html

Go:   func main()
来源：http://hz.smart0.xyz/gtxvqybzkx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.nanxinkj.top/gtzkageliw.html

C#:   static void Main(string[] args)
来源：http://hz.shanyushiyangkeji.top/gtgdpdryre.html

[M08] 获取系统与运行时信息
来源：http://hz.xuanzx.com/gtugmjyljt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zycfv.cn/gtczqjxekh.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.snrcjt.cn/gtvnmwotjo.html

JS:   process.platform;  process.version
来源：http://hz.yj20258.top/gtmnnubqnq.html

TS:   process.platform;  process.version
来源：http://hz.aibaodan.cn/gtfeahsfma.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jiagoushi.top/gtunpcyeof.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cashguo.top/gtbrwitqic.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.chenlongwang.top/gtuuxbwbly.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.wangdashe.top/gtzvgydqam.html

================================================================================
来源：http://hz.zhongyouzk.top/gtarjxzaxz.html

N. 数据结构与算法
来源：http://hz.xuanzx.com/gtrslxlexg.html

================================================================================
来源：http://hz.xuanzx.com/gtzvajuawy.html

[N01] 二分查找（有序数组）
来源：http://hz.cdnleiting.top/gtytcdbkdr.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ivvv.top/gtaxejvqpi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.mhx1999.top/gtcihzmnfb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgfzy.top/gthwzinlix.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shanyushiyangkeji.top/gtexfvhkmu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yvedp.cn/gtmvmtdwmb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hnxiangtu.top/gtodptorac.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xinyue.icu/gtohmckosx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yonumen.top/gtdqvfprew.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ybcxt.top/gtzbhdhqgo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tianlin.xyz/gtghueuxgf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sufxvd.cn/gtyhpwsihn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.iojbl.cn/gttmoslrbz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hysaishi.cn/gtzyhpotfz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yueranfly.top/gtfzkiondd.html

Go:   slices.Sort(arr)
来源：http://hz.jyoumei.cn/gtfdwjohdk.html

Ruby: arr.sort
来源：http://hz.xingfuxueyuan.xyz/gtexpclvxw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.vqdsnc.cn/gtodkkeyij.html

[N03] 快速排序（分治示例）
来源：http://hz.shanyushiyangkeji.top/gtpfztslvo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yueranfly.top/gtshxesmlb.html

PHP:  // 递归实现，或用 usort
来源：http://hz.mhx1999.top/gtswhnsusu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydzc1.top/gtxtcqruhy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigufen.top/gtkfslmgtc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.wangdashe.top/gtqnvikybe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nwbrower.top/gthbkyiwnh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shuidangran.top/gtuotcihuy.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.snrcjt.cn/gtwwyriqep.html

[N04] 斐波那契数列
来源：http://hz.gzhubu.top/gtzfdnqmyd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yongpay.top/gtjyeqcmxo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hnxiangtu.top/gtivjdkxjc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.iojbl.cn/gtclukeqjr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yanxiufei.cn/gtqvgvpkez.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yj20258888.top/gtufvsmuvh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.bjfxy.top/gtqtgrxdas.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sweek.top/gtvouvauif.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.tianlin.xyz/gtnifdfvsp.html

[N05] 最大公约数
来源：http://hz.shanyushiyangtech.top/gtxlqwfbhk.html

Py:   math.gcd(a, b)
来源：http://hz.jinqigufen.top/gtefzgllfu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sysykeji.top/gteklbppgc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yanxiufei.cn/gtyakgrzli.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guowangkeji.top/gtjhrognnn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.iojbl.cn/gtmewbwfps.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhengqikj.top/gtxbbhnjyh.html

Ruby: a.gcd(b)
来源：http://hz.yvedp.cn/gtrtdyhgsy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.guowangkeji.top/gtogheehfk.html

[N06] 判断回文字符串
来源：http://hz.hnxiangtu.top/gtbgthuljl.html

Py:   s == s[::-1]
来源：http://hz.ywan-chungtsiang.top/gtwikzpycy.html

PHP:  $s === strrev($s);
来源：http://hz.yanxiufei.cn/gtjbmajqgz.html

JS:   s === [...s].reverse().join("")
来源：http://hz.mhx1999.top/gtnbklhnwf.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtzutiitsq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.gotoacloud.top/gtgfjlfvbr.html

Go:   // 双指针从两端比较
来源：http://hz.ybcxt.top/gtfhgwynty.html

Ruby: s == s.reverse
来源：http://hz.hywenlv.cn/gtdoltftsa.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cdnleiting.top/gthhybeqxe.html

[N07] 两数之和（返回下标）
来源：http://hz.feifeiyinyue.top/gtdcjvmraf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yangfankeji.com/gtrrosbkua.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hnqzz.top/gtyxozjkla.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.snrcjt.cn/gtpejcznhs.html

TS:   // 手写 Map<string, number>
来源：http://hz.tanke756.top/gtmnrwbhdk.html

Java: // 手写 HashMap
来源：http://hz.redwolf501.top/gtxrdkrfwt.html

Go:   // 手写 map[int]int
来源：http://hz.daxiang520.top/gtzhgcuplv.html

Ruby: // 手写 Hash
来源：http://hz.yuanzhike.top/gtakyssgpm.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shangyingyoupin.top/gtcdkbzhad.html

[N08] 生成全排列
来源：http://hz.ppjwa.cn/gtialajfvn.html

Py:   itertools.permutations(arr)
来源：http://hz.zhixingplan.top/gtxponnmgg.html

PHP:  // 手写递归交换
来源：http://hz.nanxuanxn.top/gtzayezoxy.html

JS:   // 手写回溯递归
来源：http://hz.aibaodan.cn/gtvjgpbmsi.html

TS:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtgisdrvjd.html

Java: // 手写回溯递归
来源：http://hz.fzhhl.top/gtvgwpubdz.html

Go:   // 手写回溯递归
来源：http://hz.ehwqpu.com/gtjmjumcaj.html

Ruby: arr.permutation.to_a
来源：http://hz.dianchejie.cn/gtnaxqncsf.html

C#:   // 手写回溯递归
来源：http://hz.redwolf501.top/gtmidgbzep.html

[N09] 栈与队列
来源：http://hz.tanke756.top/gtdtdukxmw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj20258.top/gtctudnjtr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yj20258.top/gtuhpxfkym.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.tian-w.cn/gtdjpwtpdj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhengqikj.top/gtrrnxiptu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shzxlz.cn/gthjohjrlv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.wangshuangyany.cn/gtcmnurxmu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.tianlin.xyz/gtkfqlbuge.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.wangshuangyany.cn/gtycuhgeif.html

[N10] 链表节点定义
来源：http://hz.xziqi.cn/gtmkqqwunr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ydzc1.top/gtvlniuocj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.vqdsnc.cn/gtjuwzqnlg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhongyouzk.top/gtvgknpgtp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.kuanghao11.cn/gtkwpgwwwx.html

Java: class Node { int v; Node next; }
来源：http://hz.cheryme.top/gtxghnqlah.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.0kj1m.cn/gtzzewkngf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.52xcode.cn/gtstdewjuo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.vqdsnc.cn/gtyuykenhh.html

[N11] 二叉树中序遍历
来源：http://hz.wangshuangyany.cn/gtfpulxqfp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xuetiantiany.cn/gtipteozdc.html

PHP:  // 手写递归函数
来源：http://hz.ivvv.top/gtkporhfqs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhengqikj.top/gtwmpwagtw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pengpengdd.cyou/gthjhugflv.html

Java: // 手写递归
来源：http://hz.9152youxi.cn/gtcaknnkop.html

Go:   // 手写递归
来源：http://hz.aizwys.cn/gtdpbqxvim.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hnqzz.top/gtzcpjdpux.html

C#:   // 手写递归
来源：http://hz.havefunace.top/gtbyliavdf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhijiandao.cn/gtfyobbzgy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhixingplan.top/gtrfpildfp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ydzc1.top/gtmhdbfcvn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.0kj1m.cn/gtocvdqfex.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenjidiqi.icu/gtfqyapaji.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.havefunace.top/gtwjdmdqss.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yvedp.cn/gthzwbwgci.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yj20258888.top/gtorahkvme.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hongshengwenyu.top/gttutzjuzn.html

================================================================================
来源：http://hz.zhoulong.xyz/gtwxkedyei.html

O. 并发与异步
来源：http://hz.chenlongwang.top/gtqyewzqdm.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtxapgchdw.html

[O01] 启动一个线程
来源：http://hz.hywenlv.cn/gtfvbyhtsk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.haohaochexian.top/gthoicfcxw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shangyingyoupin.top/gtlmctsacd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yvedp.cn/gtaljjggak.html

TS:   // 同 JS
来源：http://hz.fzhhl.top/gtcefcdwig.html

Java: new Thread(() -> f()).start()
来源：http://hz.xziqi.cn/gtrfpwjfqv.html

Go:   go f()
来源：http://hz.jyoumei.cn/gtgrpxnzqe.html

Ruby: Thread.new { f }
来源：http://hz.bjfxy.top/gtqnvmvzwd.html

C#:   Task.Run(() => F());
来源：http://hz.kuanghao11.cn/gtuzeyfmdy.html

[O02] 使用线程池
来源：http://hz.sxryk.cn/gterveujpc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ywan-chungtsiang.top/gtdpvewlgp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.tianlin.xyz/gtcziteszn.html

JS:   // worker_threads 线程池
来源：http://hz.yuxming.cn/gtdnypfxbx.html

TS:   // worker_threads 线程池
来源：http://hz.gotoacloud.top/gtdvmcoczt.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.pycfn.com/gtepvoabpr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ivvv.top/gtqxnplkbw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.sxryk.cn/gtdaixkxlr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.9152youxi.cn/gtfmwilmud.html

[O03] 加锁保护共享数据
来源：http://hz.ehwqpu.com/gtgriqkwcj.html

Py:   with lock: shared += 1
来源：http://hz.andypj.xyz/gtefrredxo.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.feifeiyinyue.top/gtycyswshr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yangfankeji.com/gtzxxbnahb.html

TS:   // 同 JS
来源：http://hz.yvedp.cn/gtlokhzvro.html

Java: synchronized (this) { shared++; }
来源：http://hz.xuanzx.com/gtbmwuueqa.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xuetiantiany.cn/gtvngineal.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.daxiang520.top/gtijtxlufb.html

C#:   lock (gate) { shared++; }
来源：http://hz.shanyushiyangtech.top/gtpjkjkvzi.html

[O04] 定义异步函数并等待
来源：http://hz.jiagoushi.top/gtemrhzydu.html

Py:   async def f():⏎    await g()
来源：http://hz.0kj1m.cn/gtqgdnifri.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hnxiangtu.top/gtktukopar.html

JS:   async function f() { await g(); }
来源：http://hz.xziqi.cn/gtfcfwjxcp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.nanxuanxn.top/gtzyqfsecz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.aibaodan.cn/gtvbhmfdrr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.9152youxi.cn/gtkfwadlzn.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yanxiufei.cn/gtyibcwgem.html

C#:   async Task F() { await G(); }
来源：http://hz.cdnleiting.top/gtojdgbsfx.html

[O05] 并发执行并等待全部完成
来源：http://hz.zycfv.cn/gtyyexklfg.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenjidiqi.icu/gthrqdxtnm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.sweek.top/gtahwihwdl.html

JS:   await Promise.all(tasks)
来源：http://hz.dianchejie.cn/gtusyvakvd.html

TS:   await Promise.all(tasks)
来源：http://hz.wangdashe.top/gtfxaialle.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhaomingkeji.xyz/gtvgisjunt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.9152youxi.cn/gtqpqofumw.html

Ruby: threads.map(&:join)
来源：http://hz.dashuyun.cn/gtwvibqnuv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.sweek.top/gtlnjlzmtw.html

[O06] 使用进程池
来源：http://hz.vqdsnc.cn/gtitapxjnj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xuanzx.com/gtoxbqynfa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jinghuilouyu.cn/gtceithhkd.html

JS:   // child_process / cluster 模块
来源：http://hz.yj202588.top/gtzmnholbg.html

TS:   // child_process / cluster 模块
来源：http://hz.yuxming.cn/gtkudbdqwu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cdnleiting.top/gtdymzthjj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gaohongyu789.top/gtuvufcmvm.html

Ruby: // fork 块
来源：http://hz.kuanghao11.cn/gthcqcqima.html

C#:   Parallel.For
来源：http://hz.aibaodan.cn/gtaetrnxwc.html

================================================================================
来源：http://hz.jiagoushi.top/gtmmsxipdw.html

P. 常用工具函数
来源：http://hz.jinghuilouyu.cn/gtswgbtvia.html

================================================================================
来源：http://hz.nwbrower.top/gtsutyyltb.html

[P01] 生成 UUID
来源：http://hz.nanxuanxn.top/gtxovousfx.html

Py:   str(uuid.uuid4())
来源：http://hz.xuanzx.com/gtvpwenccr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ivvv.top/gtqailljay.html

JS:   crypto.randomUUID()
来源：http://hz.ppjwa.cn/gtlnwateyj.html

TS:   crypto.randomUUID()
来源：http://hz.cdnleiting.top/gtgtaearid.html

Java: UUID.randomUUID().toString()
来源：http://hz.sxryk.cn/gtieriydjr.html

Go:   // 用 github.com/google/uuid
来源：http://hz.nwbrower.top/gtxjmdcsth.html

Ruby: SecureRandom.uuid
来源：http://hz.guowangkeji.top/gtxqqonflj.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.wangshuangyany.cn/gtivrydpzk.html

[P02] MD5 / SHA256 摘要
来源：http://hz.guannengcc.top/gtxxsubwit.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yongpay.top/gtpsihjebz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.bjfxy.top/gtiyyqazdb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shzxlz.cn/gtcbynvqnw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.nanxuanxn.top/gtdcpjydsk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jianghu66.top/gtraktlezv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.chenzaomai.com/gtueqqpvyz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.guannengcc.top/gtgtmidrpg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xinyue.icu/gtjghqjnyp.html

[P03] 生成短随机字符串
来源：http://hz.meibo888.top/gttxdgdlzo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cheryme.top/gtkawdcpfm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jqgufenzy.top/gtpwbdurrk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jlsjyb.cn/gtofvzhhdv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sufxvd.cn/gtfforieyd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.dianchejie.cn/gtvfjusnme.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.chenzaomai.com/gtikgslire.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.quarkkingdee.top/gtrayhjukl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.wangdashe.top/gtdtefpqsh.html

[P04] 求长度
来源：http://hz.hnqzz.top/gtgrsbmjgl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.316326.xyz/gtkzlftiva.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cqqwz.cn/gtrwbsoaft.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.feifeiyinyue.top/gtcmfydunp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnqzz.top/gtdvapvxuz.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ivvv.top/gtiqdsttps.html

Go:   len(arr);  len(m)
来源：http://hz.dashuyun.cn/gtbqkkhrrb.html

Ruby: x.length;  x.size
来源：http://hz.birdmap.top/gtnhvhzyjo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yangfankeji.com/gtcfhrsiml.html

[P05] 判断两个对象内容是否相等
来源：http://hz.kuanghao11.cn/gtwsryfqxi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.nanxinkj.top/gtfptzvqhw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinyuanbaomall.cn/gtnqhfptjn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.cucudq.cn/gtjwgmmoox.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhixingplan.top/gtlvzbyqsn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yuanzhike.top/gtqejddpma.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yvedp.cn/gtphkhxywt.html

Ruby: a == b
来源：http://hz.shangyingyoupin.top/gtysgnajcz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.birdmap.top/gtpbdlflko.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shangyingyoupin.top/gtaqjkguyx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.fzhhl.top/gttvufyzoo.html

PHP:  if (empty($x)) {}
来源：http://hz.cheryme.top/gtrdprnrva.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhiwuduotai.top/gtlsidqnbb.html

TS:   if (x == null) {}
来源：http://hz.jinqigufen.top/gtgrxruvyz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhengqikj.top/gttoubydmc.html

Go:   if x == nil {}
来源：http://hz.jinghuilouyu.cn/gtyxqprggw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.pycfn.com/gtgdyzchqc.html

C#:   if (x is null) {}
来源：http://hz.feifeiyinyue.top/gtiwtwkhgi.html

[P07] 防抖与节流
来源：http://hz.ywan-chungtsiang.top/gtirqxsujv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xingfuxueyuan.xyz/gtuwnhtqnn.html

PHP:  // 手写时间戳比较
来源：http://hz.nanxuanxn.top/gtykipblrt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yonumen.top/gtiltnycmj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sysykeji.top/gternipfoo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ehwqpu.com/gtcwzrukre.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jinghuilouyu.cn/gtizrxfelm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.iojbl.cn/gtvughorkx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.haohaochexian.top/gtxmykfnll.html

[P08] 处理浮点精度问题
来源：http://hz.xuanzx.com/gtauyxatbm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.gotoacloud.top/gtrmgnuhcd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.nwbrower.top/gtipxenifo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.chenzaomai.com/gtgneokafj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hnqzz.top/gtpogpkwii.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhaomingkeji.xyz/gtftmkcehw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yongpay.top/gtxxuphlxt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhaomingkeji.xyz/gtcolpvpnc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hongshengwenyu.top/gtocruztdw.html

================================================================================
来源：http://hz.ehwqpu.com/gtbozxgqbs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.haohaochexian.top/gtxudzfgqf.html

================================================================================
来源：http://hz.havefunace.top/gtuslsblhr.html

[Q01] 创建表
来源：http://hz.zhaomingkeji.xyz/gtuhbtshun.html


<!-- 参考信息 -->