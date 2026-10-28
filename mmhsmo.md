代发 wailian999

Ruby: ARGV
来源：http://hz.pengpengdd.cyou/gtldjkpvue.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gaohongyu789.top/gthcjbtvcn.html

[M02] 读取环境变量
来源：http://hz.gotoacloud.top/gtnmhumosx.html

Py:   os.environ.get("HOME")
来源：http://hz.xuanzx.com/gtyfzkxehw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.svipenyu.cn/gtqmsvuost.html

JS:   process.env.HOME
来源：http://hz.hnxiangtu.top/gtssqvzrzl.html

TS:   process.env.HOME
来源：http://hz.sufxvd.cn/gtldccxjpg.html

Java: System.getenv("HOME")
来源：http://hz.dianchejie.cn/gtgzugirgg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.vqdsnc.cn/gtkmfksdov.html

Ruby: ENV["HOME"]
来源：http://hz.gotoacloud.top/gtbmikilun.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.daxiang520.top/gtjguxvkpk.html

[M03] 执行外部命令
来源：http://hz.pengpengdd.cyou/gtlzpfeahc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hfpthk.cn/gtaiblpghq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.tian-w.cn/gtzpdjyyha.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xylfe.cn/gtslscthce.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhongyouzk.top/gtvcxvxvzz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.meibo888.top/gtqsibqtnf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jyoumei.cn/gtcdbllxld.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jqgufenzy.top/gtdpjrziwa.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sysykeji.top/gtaumwipun.html

[M04] 获取当前工作目录
来源：http://hz.pycfn.com/gtjhzuqapm.html

Py:   os.getcwd()
来源：http://hz.ydzc1.top/gtbnsodnbr.html

PHP:  getcwd();
来源：http://hz.quarkkingdee.top/gteuljvseu.html

JS:   process.cwd()
来源：http://hz.andypj.xyz/gtqqgvxegc.html

TS:   process.cwd()
来源：http://hz.jinqigfzy.top/gtzhmrpbwx.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hongshengwenyu.top/gthldqoffi.html

Go:   os.Getwd()
来源：http://hz.ppjwa.cn/gtuhcgrwwx.html

Ruby: Dir.pwd
来源：http://hz.c1oappe.top/gtlwoycchy.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.kuanghao11.cn/gtivakoycz.html

[M05] 设置退出码
来源：http://hz.fzhhl.top/gtgbgbbpti.html

Py:   sys.exit(1)
来源：http://hz.jinqigufen.top/gtpmxwffzx.html

PHP:  exit(1);
来源：http://hz.xylfe.cn/gtbrdxicgq.html

JS:   process.exit(1)
来源：http://hz.yueranfly.top/gtmffmefpt.html

TS:   process.exit(1)
来源：http://hz.ydjk.org.cn/gtmmlqwnen.html

Java: System.exit(1)
来源：http://hz.yanxiufei.cn/gtqekpsfiy.html

Go:   os.Exit(1)
来源：http://hz.kuanghao11.cn/gtcunjpdeu.html

Ruby: exit 1
来源：http://hz.gotoacloud.top/gtkqbgwwfz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gzhubu.top/gtcqafiiod.html

[M06] 向标准错误输出
来源：http://hz.yj20258.top/gtflvfhtdy.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ehwqpu.com/gtfnzojrot.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hnxiangtu.top/gtjgiteepi.html

JS:   console.error("err")
来源：http://hz.daxiang520.top/gtfnildmav.html

TS:   console.error("err")
来源：http://hz.mhx1999.top/gtxhrxqthl.html

Java: System.err.println("err")
来源：http://hz.ydjk.org.cn/gtcdhoiypm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhixingplan.top/gteubkeibb.html

Ruby: warn "err"
来源：http://hz.daria6918.cn/gtmquigerm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jiagoushi.top/gtifywncqi.html

[M07] 判断是否为主入口
来源：http://hz.shangyingyoupin.top/gtxvhffvkf.html

Py:   if __name__ == "__main__":
来源：http://hz.sufxvd.cn/gtrmxizsld.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gaohongyu789.top/gtgfcjkyuy.html

JS:   require.main === module
来源：http://hz.fengsongda.top/gtjzpmtoqq.html

TS:   require.main === module
来源：http://hz.tian-w.cn/gthjvaervk.html

Java: public static void main(String[] args)
来源：http://hz.gzhubu.top/gtjorsvjhk.html

Go:   func main()
来源：http://hz.iojbl.cn/gtuyouqono.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jlsjyb.cn/gtlmaquncb.html

C#:   static void Main(string[] args)
来源：http://hz.tian-w.cn/gtwkcdeabw.html

[M08] 获取系统与运行时信息
来源：http://hz.jlsjyb.cn/gtqzibyeie.html

Py:   platform.system();  platform.python_version()
来源：http://hz.dashuyun.cn/gttwdspugv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yanxiufei.cn/gtgsrbgygs.html

JS:   process.platform;  process.version
来源：http://hz.shuidangran.top/gtnrfrwhni.html

TS:   process.platform;  process.version
来源：http://hz.pycfn.com/gtnofavujj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jyoumei.cn/gtlcalqvwe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shanyushiyangtech.top/gtssuqfmem.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ydzc1.top/gtkxalrdwu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shangyingyoupin.top/gtrillbnpg.html

================================================================================
来源：http://hz.sxryk.cn/gtgidvjiuo.html

N. 数据结构与算法
来源：http://hz.zhixingplan.top/gtewkwptud.html

================================================================================
来源：http://hz.zhijiandao.cn/gtafgrrfig.html

[N01] 二分查找（有序数组）
来源：http://hz.yonumen.top/gtgzypnbcu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.fzhhl.top/gtxmczmcdv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.nwbrower.top/gteompzazz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.feifeiyinyue.top/gthksivzgh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.pycfn.com/gtedtjjflf.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.snrcjt.cn/gtcqfjhtom.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.c1oappe.top/gtchzfopoh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hongshengwenyu.top/gtykvmzznn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.aizwys.cn/gtvurpriau.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.0kj1m.cn/gtcxcdmuaw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.kuanghao11.cn/gtsstpmfly.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nwbrower.top/gtzueqenqz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.havefunace.top/gtwvrbpgqj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258.top/gtrxvoajai.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.snrcjt.cn/gttixtiezc.html

Go:   slices.Sort(arr)
来源：http://hz.hfpthk.cn/gtgagcypcf.html

Ruby: arr.sort
来源：http://hz.c1oappe.top/gtyzvgdlmh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.haohaochexian.top/gtpgvsboqi.html

[N03] 快速排序（分治示例）
来源：http://hz.redwolf501.top/gtaqkrllxs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhiwuduotai.top/gtskgifyef.html

PHP:  // 递归实现，或用 usort
来源：http://hz.aibaodan.cn/gtwgdyyrld.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zdqjudy.top/gttepmfchj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tianlin.xyz/gtzdkjnbpc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jlsjyb.cn/gtgpssdrsc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yongpay.top/gtrlpyrnjc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shuidangran.top/gtobkhbtoi.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.smart0.xyz/gtrzbcmnvo.html

[N04] 斐波那契数列
来源：http://hz.shanyushiyangkeji.top/gtiqexcibt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cqqwz.cn/gtkutnafej.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.snrcjt.cn/gttchhnaor.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.vqdsnc.cn/gtbpuxajys.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ivvv.top/gtjogfyuht.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.tian-w.cn/gtqvitgedy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhijiandao.cn/gtfyziiepv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xuanzx.com/gtmscqrzfh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ivvv.top/gtoalribsa.html

[N05] 最大公约数
来源：http://hz.havefunace.top/gtvglbitdn.html

Py:   math.gcd(a, b)
来源：http://hz.cheryme.top/gtwpggmxnh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yj20258.top/gtenhzsfkn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sxryk.cn/gtjfgsdzex.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cqqwz.cn/gtvzpmthtq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yvedp.cn/gtiaaflcjv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hysaishi.cn/gtqshnckvb.html

Ruby: a.gcd(b)
来源：http://hz.sweek.top/gtvbazafpl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.chenjidiqi.icu/gttlhclckh.html

[N06] 判断回文字符串
来源：http://hz.aizwys.cn/gtaqywbbtx.html

Py:   s == s[::-1]
来源：http://hz.jqgfzy.top/gtddbbcjnh.html

PHP:  $s === strrev($s);
来源：http://hz.jinghuilouyu.cn/gtntxazxth.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtphxwqxiv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtsaoprkre.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.chenjidiqi.icu/gteetflwwe.html

Go:   // 双指针从两端比较
来源：http://hz.c1oappe.top/gtzjkwzfzh.html

Ruby: s == s.reverse
来源：http://hz.zhiwuduotai.top/gtbkcrbelj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yueranfly.top/gtysjvjhyy.html

[N07] 两数之和（返回下标）
来源：http://hz.redwolf501.top/gtacvoacqp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shangyingyoupin.top/gtunzoylia.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hfpthk.cn/gtymnpyoyd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.tianlin.xyz/gtxghxwlyr.html

TS:   // 手写 Map<string, number>
来源：http://hz.bjfxy.top/gtmnukjfpz.html

Java: // 手写 HashMap
来源：http://hz.hongshengwenyu.top/gtcpgmjbly.html

Go:   // 手写 map[int]int
来源：http://hz.ydjk.org.cn/gtnhvvfjio.html

Ruby: // 手写 Hash
来源：http://hz.zycfv.cn/gtqzkhrbtq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.aibaodan.cn/gtsizajbne.html

[N08] 生成全排列
来源：http://hz.wangdashe.top/gttudhuzrz.html

Py:   itertools.permutations(arr)
来源：http://hz.jinyuanbaomall.cn/gtgqjeyvjo.html

PHP:  // 手写递归交换
来源：http://hz.xylfe.cn/gtzjfvghkk.html

JS:   // 手写回溯递归
来源：http://hz.jqgfzy.top/gtfcazotsa.html

TS:   // 手写回溯递归
来源：http://hz.zhongyouzk.top/gttbtynulp.html

Java: // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtilthmcpb.html

Go:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtyustlhyh.html

Ruby: arr.permutation.to_a
来源：http://hz.pengpengdd.cyou/gtvsqurzqe.html

C#:   // 手写回溯递归
来源：http://hz.hammf.cn/gtceablrui.html

[N09] 栈与队列
来源：http://hz.zdqjudy.top/gtinjjflnr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.haohaochexian.top/gtzopvkbwy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.fzhhl.top/gtxbkguqbf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.haohaochexian.top/gtbgbcnwzz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shanyushiyangkeji.top/gtrbirwhpw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ydzc1.top/gtgxrxqify.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cucudq.cn/gtkakwdfrx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xinyue.icu/gtvbtbiyyy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.chenjidiqi.icu/gtsmcumneu.html

[N10] 链表节点定义
来源：http://hz.xinyue.icu/gtawcssbgp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hnqzz.top/gtkritpqyk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yvedp.cn/gtdamejblj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.haohaochexian.top/gtkcorneae.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yangfankeji.com/gtsiiqfnoe.html

Java: class Node { int v; Node next; }
来源：http://hz.yj202588.top/gtvsekxaoq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hfpthk.cn/gtnnraixzp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhongyouzk.top/gtpomczfgd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xylfe.cn/gtghykbjqt.html

[N11] 二叉树中序遍历
来源：http://hz.ydjk.org.cn/gtyylhursb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhongyouzk.top/gtplgthpde.html

PHP:  // 手写递归函数
来源：http://hz.zdqjudy.top/gtkldygvff.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zycfv.cn/gtyoknewpy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxinkj.top/gtrsntbnyz.html

Java: // 手写递归
来源：http://hz.hongshengwenyu.top/gtviwlqezu.html

Go:   // 手写递归
来源：http://hz.meibo888.top/gtoegzipat.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.haohaochexian.top/gtnnvcwfvz.html

C#:   // 手写递归
来源：http://hz.fzhhl.top/gtefneeonk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.svipenyu.cn/gtxkrxslej.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.nwbrower.top/gtknxifpam.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yj202588.top/gtxsftmiva.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shuidangran.top/gtrjibmjqy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aibaodan.cn/gtozsoepek.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sysykeji.top/gtxzokmpyd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.gzhubu.top/gtyndzupyt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhengqikj.top/gtgdgmxdiy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258.top/gtfmbjdfjo.html

================================================================================
来源：http://hz.xuanzx.com/gttnhhytjb.html

O. 并发与异步
来源：http://hz.yuanzhike.top/gtuijxjuvx.html

================================================================================
来源：http://hz.gogol.net.cn/gtrwvzjoca.html

[O01] 启动一个线程
来源：http://hz.snrcjt.cn/gtblqqkprg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinghuilouyu.cn/gttppipegj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xylfe.cn/gtwlkushbd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.pycfn.com/gtfwtgscvn.html

TS:   // 同 JS
来源：http://hz.zycfv.cn/gtpkxbqwli.html

Java: new Thread(() -> f()).start()
来源：http://hz.gogol.net.cn/gtycumfntc.html

Go:   go f()
来源：http://hz.ppjwa.cn/gtbvrldorg.html

Ruby: Thread.new { f }
来源：http://hz.hnqzz.top/gtpzzmhqdl.html

C#:   Task.Run(() => F());
来源：http://hz.gzhubu.top/gtashliqan.html

[O02] 使用线程池
来源：http://hz.hnxiangtu.top/gtiioszpln.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.gaohongyu789.top/gtdfbtzpmz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yj20258888.top/gtdyolefon.html

JS:   // worker_threads 线程池
来源：http://hz.zycfv.cn/gtrxkprequ.html

TS:   // worker_threads 线程池
来源：http://hz.tian-w.cn/gtfijvzauh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xingfuxueyuan.xyz/gtioxtkbyh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yongpay.top/gtuptjalfx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.havefunace.top/gtqsxpqfxt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hnxiangtu.top/gtirykwehz.html

[O03] 加锁保护共享数据
来源：http://hz.316326.xyz/gtdaxlhexm.html

Py:   with lock: shared += 1
来源：http://hz.nanxinkj.top/gtnldwoghz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.chenzaomai.com/gtabmoindz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.bjfxy.top/gtazaykhew.html

TS:   // 同 JS
来源：http://hz.jinghuilouyu.cn/gtrkkkcwqj.html

Java: synchronized (this) { shared++; }
来源：http://hz.jqgfzy.top/gtjsfvxbcl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yonumen.top/gtieoxfzpv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hysaishi.cn/gtmpijbckl.html

C#:   lock (gate) { shared++; }
来源：http://hz.fengsongda.top/gtmpwcvmdr.html

[O04] 定义异步函数并等待
来源：http://hz.yj20258888.top/gtpvmgitjj.html

Py:   async def f():⏎    await g()
来源：http://hz.ywan-chungtsiang.top/gtlpvvebiu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cashguo.top/gtkksfxand.html

JS:   async function f() { await g(); }
来源：http://hz.sufxvd.cn/gttjabwjan.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ivvv.top/gtkxlzkhua.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ehwqpu.com/gtzjdkgtfn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.haohaochexian.top/gtesofkgvv.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gogol.net.cn/gtmjiccuow.html

C#:   async Task F() { await G(); }
来源：http://hz.quarkkingdee.top/gtnwzxdotn.html

[O05] 并发执行并等待全部完成
来源：http://hz.9152youxi.cn/gtrjlrokkn.html

Py:   asyncio.gather(*tasks)
来源：http://hz.aizwys.cn/gtzhrmrlwp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.meibo888.top/gtutbvpadc.html

JS:   await Promise.all(tasks)
来源：http://hz.pycfn.com/gtasvxtnqo.html

TS:   await Promise.all(tasks)
来源：http://hz.fengsongda.top/gtlpklmngt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ppjwa.cn/gtprdctgti.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.redwolf501.top/gtipbgenfy.html

Ruby: threads.map(&:join)
来源：http://hz.sweek.top/gtxtjfldug.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.havefunace.top/gtkbtkxrgq.html

[O06] 使用进程池
来源：http://hz.yanxiufei.cn/gtlfyzprnw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hnqzz.top/gtuhilefgr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.316326.xyz/gtgbcrlova.html

JS:   // child_process / cluster 模块
来源：http://hz.dianchejie.cn/gtigrzhfzj.html

TS:   // child_process / cluster 模块
来源：http://hz.guowangkeji.top/gtypyvacvm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cucudq.cn/gterzevqep.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.birdmap.top/gteyhghrau.html

Ruby: // fork 块
来源：http://hz.zhongyouzk.top/gtohrptbag.html

C#:   Parallel.For
来源：http://hz.jiagoushi.top/gtudxhqtkw.html

================================================================================
来源：http://hz.chenlongwang.top/gtifoxysgq.html

P. 常用工具函数
来源：http://hz.hnxiangtu.top/gtejrghjwu.html

================================================================================
来源：http://hz.yangfankeji.com/gtbcpybris.html

[P01] 生成 UUID
来源：http://hz.xingfuxueyuan.xyz/gtrgeiczxw.html

Py:   str(uuid.uuid4())
来源：http://hz.gaohongyu789.top/gtbrsxzgom.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.fzhhl.top/gtjzfugozb.html

JS:   crypto.randomUUID()
来源：http://hz.jlsjyb.cn/gtumkfkhyt.html

TS:   crypto.randomUUID()
来源：http://hz.yvedp.cn/gtgcrwuqxh.html

Java: UUID.randomUUID().toString()
来源：http://hz.quarkkingdee.top/gtzldlsvww.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xingfuxueyuan.xyz/gtepptxhnb.html

Ruby: SecureRandom.uuid
来源：http://hz.chenzaomai.com/gtisfsbcen.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cheryme.top/gtvaayjsvm.html

[P02] MD5 / SHA256 摘要
来源：http://hz.haohaochexian.top/gtscurpyro.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.iojbl.cn/gtofagluao.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zycfv.cn/gtbijqxeuu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinqigfzy.top/gtgbsagofg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.smart0.xyz/gtlhkdtslu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.dianchejie.cn/gtzonfxkpn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ydzc1.top/gteereyqtb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xinyue.icu/gtcggvypgf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jqgfzy.top/gttocmhavq.html

[P03] 生成短随机字符串
来源：http://hz.chenzaomai.com/gtqcbmhbug.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.chenlongwang.top/gtrtkvyzso.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.meibo888.top/gtbdmarjmo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.fzhhl.top/gtjgyrbmml.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.redwolf501.top/gtiagqbdoq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.sufxvd.cn/gtpmdxdmuz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.havefunace.top/gthabhfuyf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cqqwz.cn/gtyzouemdu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.fengsongda.top/gteoycsehs.html

[P04] 求长度
来源：http://hz.zdqjudy.top/gtpzadbymc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhaomingkeji.xyz/gtlkhnvzzq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hongshengwenyu.top/gtzrgjaytq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gzhubu.top/gtvgraofkm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhaomingkeji.xyz/gtfjnahkva.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cucudq.cn/gtfococpto.html

Go:   len(arr);  len(m)
来源：http://hz.cqqwz.cn/gtibrtwcxi.html

Ruby: x.length;  x.size
来源：http://hz.svipenyu.cn/gtfvxhkbki.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.0kj1m.cn/gtcfattuaw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.nanxuanxn.top/gtzgynermc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.andypj.xyz/gtwouajfqm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shanyushiyangkeji.top/gtbtirlqjx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.kuanghao11.cn/gtxfkkejrf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hfpthk.cn/gtzhltoryg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.iojbl.cn/gtfzuskcan.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.birdmap.top/gtyopkxfci.html

Ruby: a == b
来源：http://hz.jqgufenzy.top/gtodrsosgi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.birdmap.top/gtazdlgeht.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.pengpengdd.cyou/gtvttqybqs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ydjk.org.cn/gthvwveecm.html

PHP:  if (empty($x)) {}
来源：http://hz.xingfuxueyuan.xyz/gtkhyhwwtc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yuanzhike.top/gtbuzmgbhp.html

TS:   if (x == null) {}
来源：http://hz.hnqzz.top/gtcawfnsae.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.aibaodan.cn/gtrjinvrvi.html

Go:   if x == nil {}
来源：http://hz.jqgufenzy.top/gtberkrycy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.fengsongda.top/gtrebftuim.html

C#:   if (x is null) {}
来源：http://hz.wangshuangyany.cn/gtttqsbdmr.html

[P07] 防抖与节流
来源：http://hz.shanyushiyangtech.top/gtuzehxuit.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zycfv.cn/gtjtamxswe.html

PHP:  // 手写时间戳比较
来源：http://hz.ywan-chungtsiang.top/gttslfmmey.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xylfe.cn/gtvzqfvuuz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.0kj1m.cn/gtavhqqhlo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.52xcode.cn/gtbltdjlqt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.pengpengdd.cyou/gtlkzyoref.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.guannengcc.top/gtjeaagori.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hongshengwenyu.top/gtrttvxaeb.html

[P08] 处理浮点精度问题
来源：http://hz.xinyue.icu/gtekhnwpgp.html


<!-- 参考信息 -->