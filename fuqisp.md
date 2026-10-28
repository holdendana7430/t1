代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.guowangkeji.top/gtlcyrbsoi.html

JS:   process.env.HOME
来源：http://hz.yongpay.top/gtgeznnase.html

TS:   process.env.HOME
来源：http://hz.xinyue.icu/gtrvkilton.html

Java: System.getenv("HOME")
来源：http://hz.daxiang520.top/gtimykgcid.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.tian-w.cn/gtmvgovyiw.html

Ruby: ENV["HOME"]
来源：http://hz.meibo888.top/gtcdapackn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.meibo888.top/gtyghzoiyk.html

[M03] 执行外部命令
来源：http://hz.jinyuanbaomall.cn/gtdyaaibcz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.vqdsnc.cn/gtuofqplnm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shangyingyoupin.top/gtsfcmlsaw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.snrcjt.cn/gtzpnkztmx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.52xcode.cn/gtuufrjatg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.aizwys.cn/gtfyvvovch.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.0kj1m.cn/gtpuzenyqk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gogol.net.cn/gtnzbellvv.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yuxming.cn/gtgodhecls.html

[M04] 获取当前工作目录
来源：http://hz.xuetiantiany.cn/gtryueoqqs.html

Py:   os.getcwd()
来源：http://hz.fengsongda.top/gtdfzioymh.html

PHP:  getcwd();
来源：http://hz.gotoacloud.top/gtnjiztpcw.html

JS:   process.cwd()
来源：http://hz.gogol.net.cn/gtbivffawq.html

TS:   process.cwd()
来源：http://hz.zhaomingkeji.xyz/gtkrenlosq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sweek.top/gtgnwbxkbv.html

Go:   os.Getwd()
来源：http://hz.jianghu66.top/gtexhfqbzp.html

Ruby: Dir.pwd
来源：http://hz.shzxlz.cn/gtdbmnazpp.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhaomingkeji.xyz/gtbcrgbnpd.html

[M05] 设置退出码
来源：http://hz.shzxlz.cn/gtgvksvvlh.html

Py:   sys.exit(1)
来源：http://hz.dianchejie.cn/gthfolzcxd.html

PHP:  exit(1);
来源：http://hz.tian-w.cn/gthjshpqaq.html

JS:   process.exit(1)
来源：http://hz.iojbl.cn/gtwltvytyi.html

TS:   process.exit(1)
来源：http://hz.yangfankeji.com/gtztzpwjcf.html

Java: System.exit(1)
来源：http://hz.shuidangran.top/gtqazehzxt.html

Go:   os.Exit(1)
来源：http://hz.gogol.net.cn/gtnucunave.html

Ruby: exit 1
来源：http://hz.ivvv.top/gtvcdxdgul.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.daria6918.cn/gtoknfxlye.html

[M06] 向标准错误输出
来源：http://hz.yuanzhike.top/gtkqbzqphw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sufxvd.cn/gtkmcbfruw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.smart0.xyz/gtazwcrzce.html

JS:   console.error("err")
来源：http://hz.zhongyouzk.top/gtngbcmbnc.html

TS:   console.error("err")
来源：http://hz.ehwqpu.com/gtvfgtdweo.html

Java: System.err.println("err")
来源：http://hz.sweek.top/gtvulycleo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shzxlz.cn/gtdaedgikq.html

Ruby: warn "err"
来源：http://hz.gogol.net.cn/gtacotsiuk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xuanzx.com/gtsohhfobg.html

[M07] 判断是否为主入口
来源：http://hz.yj20258888.top/gtxunqkrha.html

Py:   if __name__ == "__main__":
来源：http://hz.hammf.cn/gtghmprmeg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.svipenyu.cn/gtewjxauxp.html

JS:   require.main === module
来源：http://hz.jqgfzy.top/gtxswrwjnt.html

TS:   require.main === module
来源：http://hz.fengsongda.top/gtvhfjclvm.html

Java: public static void main(String[] args)
来源：http://hz.jiagoushi.top/gtureydtpp.html

Go:   func main()
来源：http://hz.dashuyun.cn/gtjgfwnysv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xinyue.icu/gtpoimczyv.html

C#:   static void Main(string[] args)
来源：http://hz.xylfe.cn/gtxyibowgh.html

[M08] 获取系统与运行时信息
来源：http://hz.zhoulong.xyz/gtzbbnmkta.html

Py:   platform.system();  platform.python_version()
来源：http://hz.dianchejie.cn/gtbzzfgaau.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ydjk.org.cn/gtctvxzjak.html

JS:   process.platform;  process.version
来源：http://hz.ydjk.org.cn/gtihednirw.html

TS:   process.platform;  process.version
来源：http://hz.jyoumei.cn/gtwitdwovy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hysaishi.cn/gttbsynrpk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.dashuyun.cn/gtwcoxlgmo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.9152youxi.cn/gtpgyogrlz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yanxiufei.cn/gtdicamztv.html

================================================================================
来源：http://hz.hnxiangtu.top/gtwgrdyozc.html

N. 数据结构与算法
来源：http://hz.shuidangran.top/gtywkwyuad.html

================================================================================
来源：http://hz.yangfankeji.com/gttyceszzp.html

[N01] 二分查找（有序数组）
来源：http://hz.jiagoushi.top/gtcfppkhco.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yuanzhike.top/gtgkljijlo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinqigufen.top/gteuumanoq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuanzx.com/gtghrxusda.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.pengpengdd.cyou/gtxiohegka.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtqztxdolx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtewvyqyjn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhiwuduotai.top/gtdydowusy.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cheryme.top/gttdyqjgcv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yj202588.top/gtvopwellt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenjidiqi.icu/gtexjjuqho.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yongpay.top/gtvkfvnkdo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtunoanslf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xingfuxueyuan.xyz/gtkqqqfsyu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.wangdashe.top/gtkgooxmmd.html

Go:   slices.Sort(arr)
来源：http://hz.cdnleiting.top/gtoiwkjwuf.html

Ruby: arr.sort
来源：http://hz.jyoumei.cn/gtsgxfmrtd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cdnleiting.top/gtwateacdw.html

[N03] 快速排序（分治示例）
来源：http://hz.jlsjyb.cn/gtakuukthg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shanyushiyangtech.top/gtemrlbzsn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jianghu66.top/gtsrygoais.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuanzx.com/gtjiclgmtt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tianlin.xyz/gtsspbywwy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zdqjudy.top/gtijetkoyp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cheryme.top/gtvbiykvls.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yj20258.top/gtmnafwlcf.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.fzhhl.top/gtvhqcxgwj.html

[N04] 斐波那契数列
来源：http://hz.sufxvd.cn/gtjjnjowml.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cqqwz.cn/gtbfvlhhjc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hysaishi.cn/gtrqaxpupq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daria6918.cn/gtsrttmbmj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.guowangkeji.top/gtgjdujtdi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.guannengcc.top/gtybenonbm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sufxvd.cn/gtgjgmnutq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.feifeiyinyue.top/gtiroxxjis.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hongshengwenyu.top/gttxlmqajf.html

[N05] 最大公约数
来源：http://hz.andypj.xyz/gtivrzrquv.html

Py:   math.gcd(a, b)
来源：http://hz.pengpengdd.cyou/gtzoppqjbb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ivvv.top/gtkaojyggm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gtjlfmuqrc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hysaishi.cn/gtvjwmgloi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.pycfn.com/gtvdnvzvrm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hongshengwenyu.top/gtanwkjxxg.html

Ruby: a.gcd(b)
来源：http://hz.gaohongyu789.top/gtoszmcukw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zycfv.cn/gtdsnlnbce.html

[N06] 判断回文字符串
来源：http://hz.jinyuanbaomall.cn/gtvzojwnig.html

Py:   s == s[::-1]
来源：http://hz.wangshuangyany.cn/gtzkrpxlbd.html

PHP:  $s === strrev($s);
来源：http://hz.tanke756.top/gtcsgvqfsa.html

JS:   s === [...s].reverse().join("")
来源：http://hz.quarkkingdee.top/gtcspvryns.html

TS:   s === [...s].reverse().join("")
来源：http://hz.redwolf501.top/gthsookyzg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ybcxt.top/gtmltltesp.html

Go:   // 双指针从两端比较
来源：http://hz.shzxlz.cn/gtdqrjswzg.html

Ruby: s == s.reverse
来源：http://hz.316326.xyz/gtcvluvwko.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jlsjyb.cn/gtytfbvnru.html

[N07] 两数之和（返回下标）
来源：http://hz.jinqigfzy.top/gtlntihssa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hnqzz.top/gthtvaouvg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.birdmap.top/gtlhyawein.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nanxuanxn.top/gtfdgfdova.html

TS:   // 手写 Map<string, number>
来源：http://hz.cucudq.cn/gtcamxovby.html

Java: // 手写 HashMap
来源：http://hz.zhaomingkeji.xyz/gtfkucqrno.html

Go:   // 手写 map[int]int
来源：http://hz.ppjwa.cn/gtpcidphho.html

Ruby: // 手写 Hash
来源：http://hz.sxryk.cn/gtlkcviotr.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zdqjudy.top/gtwgjiqfbf.html

[N08] 生成全排列
来源：http://hz.yuanzhike.top/gtpqusrkst.html

Py:   itertools.permutations(arr)
来源：http://hz.chenjidiqi.icu/gtbwerxtnn.html

PHP:  // 手写递归交换
来源：http://hz.9152youxi.cn/gtoipofeje.html

JS:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtxycqccat.html

TS:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gttepddmgo.html

Java: // 手写回溯递归
来源：http://hz.sysykeji.top/gtekjawtad.html

Go:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtixbmirvd.html

Ruby: arr.permutation.to_a
来源：http://hz.dianchejie.cn/gtvkoozqkp.html

C#:   // 手写回溯递归
来源：http://hz.dianchejie.cn/gtfukzlzgh.html

[N09] 栈与队列
来源：http://hz.hnxiangtu.top/gtueyoctvz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jqgufenzy.top/gtvhnvtdxh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yuxming.cn/gtcgqypwlh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jqgufenzy.top/gtlyrmptww.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xylfe.cn/gtzmnjryiu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhengqikj.top/gtzjkjaasn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zycfv.cn/gtrtpaswlc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cdnleiting.top/gtrmtgpwnj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ywan-chungtsiang.top/gtobmksqgn.html

[N10] 链表节点定义
来源：http://hz.ywan-chungtsiang.top/gtkuhjrkcr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.mhx1999.top/gtxhljmxmt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinqigufen.top/gtzxxxccbw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sweek.top/gtbbpbajum.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.daxiang520.top/gtbswufwwb.html

Java: class Node { int v; Node next; }
来源：http://hz.nanxuanxn.top/gtrkrakktb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tian-w.cn/gtjwwtactj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.meibo888.top/gtmckrugdp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yuxming.cn/gtltpfudav.html

[N11] 二叉树中序遍历
来源：http://hz.redwolf501.top/gtprccgded.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.dashuyun.cn/gtwwykmwjy.html

PHP:  // 手写递归函数
来源：http://hz.yj20258.top/gtltwjdajg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jyoumei.cn/gtbgcxaklp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jianghu66.top/gtfygxqibb.html

Java: // 手写递归
来源：http://hz.yj20258888.top/gtclrpmklj.html

Go:   // 手写递归
来源：http://hz.zdqjudy.top/gtrwezzhlo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jianghu66.top/gtoxekyhfy.html

C#:   // 手写递归
来源：http://hz.xuanzx.com/gtlsxurned.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ehwqpu.com/gtjokkgsum.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jianghu66.top/gtjddlojub.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.tian-w.cn/gtecwdvyys.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.havefunace.top/gtwfnhxikd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhixingplan.top/gtgcpozoue.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenjidiqi.icu/gtwftnsori.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenjidiqi.icu/gthemkncqe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xinyue.icu/gtuurztwsi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangtech.top/gtjjvvfluv.html

================================================================================
来源：http://hz.hammf.cn/gtyxjdviwb.html

O. 并发与异步
来源：http://hz.daria6918.cn/gtnheouyli.html

================================================================================
来源：http://hz.yueranfly.top/gtsbczieja.html

[O01] 启动一个线程
来源：http://hz.yuanzhike.top/gtotxwmbko.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ivvv.top/gtfuxwyiqc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jyoumei.cn/gtwlkjriez.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jqgfzy.top/gtuoenivmc.html

TS:   // 同 JS
来源：http://hz.vqdsnc.cn/gtqlfmkzmh.html

Java: new Thread(() -> f()).start()
来源：http://hz.ydjk.org.cn/gtskehewpx.html

Go:   go f()
来源：http://hz.jiagoushi.top/gtumjgkwsh.html

Ruby: Thread.new { f }
来源：http://hz.yongpay.top/gttiiaxkag.html

C#:   Task.Run(() => F());
来源：http://hz.gzhubu.top/gtckbubwqb.html

[O02] 使用线程池
来源：http://hz.daxiang520.top/gtiedagkkj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhongyouzk.top/gtwyraydyj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.feifeiyinyue.top/gtmhkzvxxb.html

JS:   // worker_threads 线程池
来源：http://hz.jianghu66.top/gtmvujtsqk.html

TS:   // worker_threads 线程池
来源：http://hz.yuxming.cn/gtixgqymce.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinqigufen.top/gtxkpgfomw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.smart0.xyz/gtkvjgqqwv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.c1oappe.top/gtxibiqdes.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.wangdashe.top/gtnzfmtgsx.html

[O03] 加锁保护共享数据
来源：http://hz.chenlongwang.top/gteohefnnc.html

Py:   with lock: shared += 1
来源：http://hz.jlsjyb.cn/gtpfrbdiyc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yangfankeji.com/gtcfdjjple.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenjidiqi.icu/gtovkgggyt.html

TS:   // 同 JS
来源：http://hz.yvedp.cn/gtykmuinax.html

Java: synchronized (this) { shared++; }
来源：http://hz.sysykeji.top/gtauvyrrpp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ivvv.top/gtpnipzbci.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.quarkkingdee.top/gtxkfpknek.html

C#:   lock (gate) { shared++; }
来源：http://hz.0kj1m.cn/gtyqnaeyot.html

[O04] 定义异步函数并等待
来源：http://hz.aizwys.cn/gttpnfrdqa.html

Py:   async def f():⏎    await g()
来源：http://hz.yuxming.cn/gtngqvvrhj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.daxiang520.top/gtqbrtnnqw.html

JS:   async function f() { await g(); }
来源：http://hz.zhixingplan.top/gthkbwsood.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yuxming.cn/gtooacwxky.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.dianchejie.cn/gtbnbibtuk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shanyushiyangtech.top/gtdjuiomab.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.chenjidiqi.icu/gttfvcxhbj.html

C#:   async Task F() { await G(); }
来源：http://hz.aizwys.cn/gtepwmhlvu.html

[O05] 并发执行并等待全部完成
来源：http://hz.havefunace.top/gtsyrrifxb.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xinyue.icu/gtbnojlmkw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yongpay.top/gtvyycfygm.html

JS:   await Promise.all(tasks)
来源：http://hz.hywenlv.cn/gtufpidfpz.html

TS:   await Promise.all(tasks)
来源：http://hz.xuanzx.com/gttnemwymx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.chenjidiqi.icu/gtawfqpatf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.snrcjt.cn/gtuuzkqvze.html

Ruby: threads.map(&:join)
来源：http://hz.gzhubu.top/gtvwjbdrjn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jyoumei.cn/gttzaxvpzo.html

[O06] 使用进程池
来源：http://hz.ivvv.top/gtsrbbzben.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hysaishi.cn/gtkrjocort.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.sweek.top/gtrvmhpggp.html

JS:   // child_process / cluster 模块
来源：http://hz.havefunace.top/gttzthrtxz.html

TS:   // child_process / cluster 模块
来源：http://hz.yangfankeji.com/gthqwxaniy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinghuilouyu.cn/gtozosttjs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gogol.net.cn/gthnflvfvf.html

Ruby: // fork 块
来源：http://hz.vqdsnc.cn/gtrfjwnpms.html

C#:   Parallel.For
来源：http://hz.0kj1m.cn/gtmjzbvahd.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtslcnuftl.html

P. 常用工具函数
来源：http://hz.chenlongwang.top/gtunvgohai.html

================================================================================
来源：http://hz.ppjwa.cn/gtodvwrlbp.html

[P01] 生成 UUID
来源：http://hz.jinyuanbaomall.cn/gtpjtmdrdt.html

Py:   str(uuid.uuid4())
来源：http://hz.guowangkeji.top/gtwxisxblx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jqgfzy.top/gtgylnlspl.html

JS:   crypto.randomUUID()
来源：http://hz.zhaomingkeji.xyz/gthkykfkmg.html

TS:   crypto.randomUUID()
来源：http://hz.tian-w.cn/gtetubaksy.html

Java: UUID.randomUUID().toString()
来源：http://hz.9152youxi.cn/gtkwcpowzy.html

Go:   // 用 github.com/google/uuid
来源：http://hz.wangshuangyany.cn/gtmlikebna.html

Ruby: SecureRandom.uuid
来源：http://hz.xziqi.cn/gtkdatoijb.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hammf.cn/gtpufwwlun.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinghuilouyu.cn/gtqpuuanet.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.9152youxi.cn/gtnubrtmge.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.cucudq.cn/gtaoqdtmvk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gotoacloud.top/gtvoyqluwg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.sysykeji.top/gtycsftmdf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zycfv.cn/gtrxabyyeu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.feifeiyinyue.top/gtzhasiusr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinqigfzy.top/gtjdlxuhii.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xinyue.icu/gtwztkwmoc.html

[P03] 生成短随机字符串
来源：http://hz.jinqigufen.top/gtgjwcehtm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jlsjyb.cn/gtnmkjhgzy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yuxming.cn/gtcwnpbgge.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xylfe.cn/gtgpheijfn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cheryme.top/gtjtfsmmnv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.guannengcc.top/gtstrskkkh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xingfuxueyuan.xyz/gteaaiefkj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hysaishi.cn/gtfgxsybvz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinghuilouyu.cn/gtahavymfu.html

[P04] 求长度
来源：http://hz.yj202588.top/gtlawwrcvs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jqgufenzy.top/gtflzbsxtl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenjidiqi.icu/gtxrnobhuv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhijiandao.cn/gtqsgqwoxk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.kuanghao11.cn/gtozgqlrjx.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sweek.top/gtkoszhvte.html

Go:   len(arr);  len(m)
来源：http://hz.zhiwuduotai.top/gtldpxpiqv.html

Ruby: x.length;  x.size
来源：http://hz.jiagoushi.top/gtjtqkoqca.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.aizwys.cn/gtmqnsupsu.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ydzc1.top/gtpchsgpsm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yvedp.cn/gtuzjgfkkf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hywenlv.cn/gtyxjxaxhs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhoulong.xyz/gtdsitqfaa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.mhx1999.top/gthsoptngm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hongshengwenyu.top/gtamizsnch.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yongpay.top/gtjamhsrpo.html

Ruby: a == b
来源：http://hz.andypj.xyz/gtesgreili.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.nanxuanxn.top/gtthjygrbk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zycfv.cn/gtfyjnnfry.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.andypj.xyz/gtkkblfnod.html

PHP:  if (empty($x)) {}
来源：http://hz.pycfn.com/gtisrxhkyi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinghuilouyu.cn/gtvtaiqehy.html

TS:   if (x == null) {}
来源：http://hz.zhoulong.xyz/gtyqbaixbf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jqgfzy.top/gtokdhiiwo.html

Go:   if x == nil {}
来源：http://hz.zhaomingkeji.xyz/gtqrwpkenx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yj202588.top/gtnhqejtuu.html

C#:   if (x is null) {}
来源：http://hz.svipenyu.cn/gtpuwjrzil.html

[P07] 防抖与节流
来源：http://hz.52xcode.cn/gtgjocwkux.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xylfe.cn/gtawhsbgyw.html

PHP:  // 手写时间戳比较
来源：http://hz.jinyuanbaomall.cn/gtjbsycsre.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydzc1.top/gteecibrpb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.snrcjt.cn/gtfpojvuyi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.316326.xyz/gtmuxgdzmb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.redwolf501.top/gtxyjsvvhq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jyoumei.cn/gtrpwvwqqp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.chenjidiqi.icu/gtrtgipkoa.html

[P08] 处理浮点精度问题
来源：http://hz.hysaishi.cn/gtndiuszvn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yvedp.cn/gtxsnoofuz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hongshengwenyu.top/gtradazykl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.pycfn.com/gtinxhdtpw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.wangshuangyany.cn/gtwuejxdzr.html


<!-- 参考信息 -->