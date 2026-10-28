代发 wailian999

TS:   resp.ok;  resp.status
来源：http://hz.hfpthk.cn/gtfffpyryx.html

Java: resp.statusCode()
来源：http://hz.jlsjyb.cn/gttxbafywo.html

Go:   resp.StatusCode
来源：http://hz.chenjidiqi.icu/gtpuzjpgby.html

Ruby: resp.code.to_i
来源：http://hz.xuanzx.com/gtxlsemole.html

C#:   (int)resp.StatusCode
来源：http://hz.gzhubu.top/gtuyjjmtbe.html

[L08] 并发请求多个地址
来源：http://hz.mhx1999.top/gtmnbzwozi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zycfv.cn/gtnhiooxlc.html

PHP:  curl_multi_init() 系列
来源：http://hz.sysykeji.top/gtabchlrpi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shangyingyoupin.top/gtclpokhlp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xingfuxueyuan.xyz/gtlcwrwhoi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.0kj1m.cn/gtwphrftvr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinyuanbaomall.cn/gtadnndnte.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zdqjudy.top/gtplylyxoj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.chenjidiqi.icu/gtghxmnrgs.html

================================================================================
来源：http://hz.svipenyu.cn/gtcolcgcps.html

M. 命令行 / 进程 / 环境
来源：http://hz.yongpay.top/gtpxwoeveb.html

================================================================================
来源：http://hz.yonumen.top/gtaylldtqb.html

[M01] 读取命令行参数
来源：http://hz.feifeiyinyue.top/gtyektildt.html

Py:   sys.argv[1:]
来源：http://hz.hammf.cn/gtpxjrkdyo.html

PHP:  $argv;  $argc;
来源：http://hz.xziqi.cn/gtnjjhstae.html

JS:   process.argv.slice(2)
来源：http://hz.redwolf501.top/gttrntsere.html

TS:   process.argv.slice(2)
来源：http://hz.jiagoushi.top/gtikydhfei.html

Java: args 数组（main 方法参数）
来源：http://hz.nanxuanxn.top/gtybinmkvm.html

Go:   os.Args[1:]
来源：http://hz.ydjk.org.cn/gtjjbqpzoz.html

Ruby: ARGV
来源：http://hz.316326.xyz/gtakjglvoi.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sxryk.cn/gtymrzktyd.html

[M02] 读取环境变量
来源：http://hz.ybcxt.top/gtvhujecfv.html

Py:   os.environ.get("HOME")
来源：http://hz.cucudq.cn/gthawpjebn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.haohaochexian.top/gtrnhlntqz.html

JS:   process.env.HOME
来源：http://hz.ybcxt.top/gtcfvnbjlo.html

TS:   process.env.HOME
来源：http://hz.316326.xyz/gtuhtrvefd.html

Java: System.getenv("HOME")
来源：http://hz.yj202588.top/gtnvginucx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hywenlv.cn/gtnhyevcpo.html

Ruby: ENV["HOME"]
来源：http://hz.jinqigufen.top/gtpzbkdtcw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zdqjudy.top/gtpxaacfzk.html

[M03] 执行外部命令
来源：http://hz.jiagoushi.top/gtvynvfwfm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhoulong.xyz/gtdkqryqyo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hfpthk.cn/gtpkuzshlv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jianghu66.top/gtjdaegfig.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj20258888.top/gtquhzzolu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ehwqpu.com/gtjywbqpxo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.vqdsnc.cn/gtlrwzdyyc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.wangshuangyany.cn/gtcjwwttnl.html

C#:   Process.Start("ls", "-l");
来源：http://hz.aibaodan.cn/gtdfzskizq.html

[M04] 获取当前工作目录
来源：http://hz.52xcode.cn/gtqqarvymw.html

Py:   os.getcwd()
来源：http://hz.wangdashe.top/gtijiuxmlv.html

PHP:  getcwd();
来源：http://hz.nanxuanxn.top/gtvekruggq.html

JS:   process.cwd()
来源：http://hz.nanxinkj.top/gtwujmymwo.html

TS:   process.cwd()
来源：http://hz.kuanghao11.cn/gtkusadblx.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jiagoushi.top/gtvvjhegfb.html

Go:   os.Getwd()
来源：http://hz.yj20258888.top/gtyqbmfpzd.html

Ruby: Dir.pwd
来源：http://hz.cqqwz.cn/gtsnznzwrz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.c1oappe.top/gtnztvvxky.html

[M05] 设置退出码
来源：http://hz.bjfxy.top/gtxfncjoul.html

Py:   sys.exit(1)
来源：http://hz.wangshuangyany.cn/gtzhgjfkzj.html

PHP:  exit(1);
来源：http://hz.shzxlz.cn/gtruwauuhd.html

JS:   process.exit(1)
来源：http://hz.sysykeji.top/gtfcjgrlpn.html

TS:   process.exit(1)
来源：http://hz.tian-w.cn/gtsfdlatcg.html

Java: System.exit(1)
来源：http://hz.pengpengdd.cyou/gtlqpgvbpl.html

Go:   os.Exit(1)
来源：http://hz.meibo888.top/gtfupncioi.html

Ruby: exit 1
来源：http://hz.pengpengdd.cyou/gtcthqruti.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xylfe.cn/gtfhwphxke.html

[M06] 向标准错误输出
来源：http://hz.dashuyun.cn/gtbdkfroew.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sxryk.cn/gtcflbeoet.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.316326.xyz/gtylvhjfot.html

JS:   console.error("err")
来源：http://hz.redwolf501.top/gtnezohlnf.html

TS:   console.error("err")
来源：http://hz.jyoumei.cn/gtumwaqnnu.html

Java: System.err.println("err")
来源：http://hz.hfpthk.cn/gtreleavqe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ppjwa.cn/gtuuhodkjb.html

Ruby: warn "err"
来源：http://hz.yangfankeji.com/gtkyurxumj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hongshengwenyu.top/gtzuxwhhvk.html

[M07] 判断是否为主入口
来源：http://hz.pycfn.com/gtsmhuumez.html

Py:   if __name__ == "__main__":
来源：http://hz.yvedp.cn/gtmecxkxcw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yuxming.cn/gtfyujxtax.html

JS:   require.main === module
来源：http://hz.meibo888.top/gtwgbvvbql.html

TS:   require.main === module
来源：http://hz.kuanghao11.cn/gteaajtyfu.html

Java: public static void main(String[] args)
来源：http://hz.yonumen.top/gtfeiwmhom.html

Go:   func main()
来源：http://hz.zhixingplan.top/gtcsaylxqz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.fengsongda.top/gtfhnkstma.html

C#:   static void Main(string[] args)
来源：http://hz.jqgufenzy.top/gtxrlxbyak.html

[M08] 获取系统与运行时信息
来源：http://hz.xinyue.icu/gtqisgabbr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xuanzx.com/gtkrfddkvx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gotoacloud.top/gtylhlirzy.html

JS:   process.platform;  process.version
来源：http://hz.shzxlz.cn/gtvnhrodsy.html

TS:   process.platform;  process.version
来源：http://hz.zhengqikj.top/gtwvvlgadf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinqigufen.top/gtrcopqoxl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.aizwys.cn/gtaigqatyt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhijiandao.cn/gtaflwghmc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ybcxt.top/gtoxvedbtk.html

================================================================================
来源：http://hz.zhixingplan.top/gtvktehvtf.html

N. 数据结构与算法
来源：http://hz.yanxiufei.cn/gtuelizskd.html

================================================================================
来源：http://hz.yongpay.top/gtcoppaxoz.html

[N01] 二分查找（有序数组）
来源：http://hz.xinyue.icu/gtndxiwxkx.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sxryk.cn/gtkvrffgys.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hfpthk.cn/gtsndveywj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258.top/gtydhckfli.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cdnleiting.top/gtowcbaeon.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yuxming.cn/gtjzmhsfwx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yangfankeji.com/gtcltluqpn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhijiandao.cn/gtapizqxyf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jqgufenzy.top/gtsjzesrcj.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.dashuyun.cn/gtqkxwtoxp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenjidiqi.icu/gtenlykbsl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.wangshuangyany.cn/gtolkxyniw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gtbphbwdzk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jqgufenzy.top/gtvpovsppm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.pycfn.com/gtavuxvmyd.html

Go:   slices.Sort(arr)
来源：http://hz.xziqi.cn/gthvzjiyjw.html

Ruby: arr.sort
来源：http://hz.mhx1999.top/gtklskfrsu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.guowangkeji.top/gtszccxnmf.html

[N03] 快速排序（分治示例）
来源：http://hz.ydjk.org.cn/gtuhzbdlin.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.mhx1999.top/gttbimdvja.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cdnleiting.top/gtfswdmrzk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.andypj.xyz/gtucmaxpxs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hongshengwenyu.top/gtjpexuvin.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shanyushiyangtech.top/gtqkfuyice.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.daxiang520.top/gtwjgjhkah.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cheryme.top/gtnrsutdkf.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.sweek.top/gtztywcdjd.html

[N04] 斐波那契数列
来源：http://hz.sxryk.cn/gtonpgumxu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.guowangkeji.top/gtvvkepmmr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.9152youxi.cn/gtpxmqjeuz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xinyue.icu/gtgxsgrkqq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yangfankeji.com/gtdoezdoyp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sxryk.cn/gtugqrcwhz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jyoumei.cn/gtzsxhdond.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.dashuyun.cn/gtabshxndd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ybcxt.top/gtkfvxttsf.html

[N05] 最大公约数
来源：http://hz.jianghu66.top/gtphhmtcat.html

Py:   math.gcd(a, b)
来源：http://hz.hywenlv.cn/gtjudcmhbq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xylfe.cn/gtfrjwvike.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nanxinkj.top/gtixcrmzzo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gotoacloud.top/gtkrmipkrx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.smart0.xyz/gtgtjgkpjz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cucudq.cn/gtbdwunsxs.html

Ruby: a.gcd(b)
来源：http://hz.52xcode.cn/gtgtkyjkek.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.wangdashe.top/gtjzsxswyy.html

[N06] 判断回文字符串
来源：http://hz.jinqigfzy.top/gtenhkbtfn.html

Py:   s == s[::-1]
来源：http://hz.gaohongyu789.top/gthlllubpx.html

PHP:  $s === strrev($s);
来源：http://hz.tian-w.cn/gtgsfynwxg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.gaohongyu789.top/gteoscitrb.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtyyrktseo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinqigfzy.top/gtuvfraawa.html

Go:   // 双指针从两端比较
来源：http://hz.sufxvd.cn/gtipfrider.html

Ruby: s == s.reverse
来源：http://hz.316326.xyz/gtgpbljsqs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.316326.xyz/gthmuzogyw.html

[N07] 两数之和（返回下标）
来源：http://hz.jqgufenzy.top/gtxbritjrm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shzxlz.cn/gtjbhsnmru.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hfpthk.cn/gtoxznhprl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.dianchejie.cn/gtsksyivhj.html

TS:   // 手写 Map<string, number>
来源：http://hz.shzxlz.cn/gtaddngyhx.html

Java: // 手写 HashMap
来源：http://hz.gotoacloud.top/gtnsmybwpu.html

Go:   // 手写 map[int]int
来源：http://hz.cdnleiting.top/gtqwmzwnsm.html

Ruby: // 手写 Hash
来源：http://hz.jinyuanbaomall.cn/gtsudtcska.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hfpthk.cn/gtmrufipua.html

[N08] 生成全排列
来源：http://hz.feifeiyinyue.top/gtblbdyrog.html

Py:   itertools.permutations(arr)
来源：http://hz.0kj1m.cn/gtxwyprbht.html

PHP:  // 手写递归交换
来源：http://hz.xziqi.cn/gtgzdfgkts.html

JS:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtyiuvjxxk.html

TS:   // 手写回溯递归
来源：http://hz.ppjwa.cn/gtujssrwhm.html

Java: // 手写回溯递归
来源：http://hz.cheryme.top/gtrxunixoo.html

Go:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtwjudgute.html

Ruby: arr.permutation.to_a
来源：http://hz.zhiwuduotai.top/gtdacofifn.html

C#:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtzqherxaw.html

[N09] 栈与队列
来源：http://hz.jqgufenzy.top/gtgotjkulx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hongshengwenyu.top/gtmrcqqeex.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.9152youxi.cn/gtzjujbtmr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.smart0.xyz/gtwcftksif.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.gzhubu.top/gtqsufyiql.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinqigufen.top/gtmvdikbbl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hnqzz.top/gtlpadtdpg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.52xcode.cn/gtiesafvwq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.daria6918.cn/gthjsyzrhm.html

[N10] 链表节点定义
来源：http://hz.xinyue.icu/gtocpgbsyu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.52xcode.cn/gtfllrdkbp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.kuanghao11.cn/gtqoaubggz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.haohaochexian.top/gtlpvninkc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.wangshuangyany.cn/gtxrdqcjeb.html

Java: class Node { int v; Node next; }
来源：http://hz.yangfankeji.com/gtwegoexuv.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhiwuduotai.top/gtyszxzygh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yangfankeji.com/gtbgzibawq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shangyingyoupin.top/gtbtmxfznk.html

[N11] 二叉树中序遍历
来源：http://hz.mhx1999.top/gtpwnqfrkm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.feifeiyinyue.top/gtumlnxjjr.html

PHP:  // 手写递归函数
来源：http://hz.yongpay.top/gtbgxcyofr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dianchejie.cn/gtxvninnpy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.daxiang520.top/gtlhxvevnl.html

Java: // 手写递归
来源：http://hz.cucudq.cn/gttooaxwdd.html

Go:   // 手写递归
来源：http://hz.sxryk.cn/gthqsfwxci.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.sxryk.cn/gtskajkaic.html

C#:   // 手写递归
来源：http://hz.316326.xyz/gtduqwqnre.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cdnleiting.top/gtkyamsnjk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinghuilouyu.cn/gtjdgcowny.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hnxiangtu.top/gtouqwjlcv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.haohaochexian.top/gtmwdsektp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yanxiufei.cn/gtscnhnxlz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jianghu66.top/gtuzdqyoif.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sysykeji.top/gtjwgeerol.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sxryk.cn/gtvorqolrz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.haohaochexian.top/gtfcmayixr.html

================================================================================
来源：http://hz.zdqjudy.top/gtzrnlduhz.html

O. 并发与异步
来源：http://hz.cashguo.top/gtliweolmi.html

================================================================================
来源：http://hz.jqgufenzy.top/gtcqtzrucw.html

[O01] 启动一个线程
来源：http://hz.cheryme.top/gtguopvogt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ydzc1.top/gtjdxblitj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhongyouzk.top/gtsfsrqnwr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.shuidangran.top/gtaiqgbngm.html

TS:   // 同 JS
来源：http://hz.sufxvd.cn/gtqaddvhnn.html

Java: new Thread(() -> f()).start()
来源：http://hz.hysaishi.cn/gtcvbqnnvx.html

Go:   go f()
来源：http://hz.zdqjudy.top/gtiwlaeyta.html

Ruby: Thread.new { f }
来源：http://hz.gzhubu.top/gtfjsejime.html

C#:   Task.Run(() => F());
来源：http://hz.mhx1999.top/gtqqvxlnbl.html

[O02] 使用线程池
来源：http://hz.fzhhl.top/gttkovgdzd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shangyingyoupin.top/gtbgruyqtl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xuanzx.com/gthuzabzxn.html

JS:   // worker_threads 线程池
来源：http://hz.zhiwuduotai.top/gteohrcbpm.html

TS:   // worker_threads 线程池
来源：http://hz.quarkkingdee.top/gtkxhcisvy.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cheryme.top/gtyikiftdg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.kuanghao11.cn/gtcaepgwmu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.wangdashe.top/gtqypyhcvf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.chenjidiqi.icu/gtqqarifrl.html

[O03] 加锁保护共享数据
来源：http://hz.xziqi.cn/gtqcxwlqgo.html

Py:   with lock: shared += 1
来源：http://hz.ehwqpu.com/gtjxtupxba.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.redwolf501.top/gtxgaqfnok.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinqigfzy.top/gtgumsujku.html

TS:   // 同 JS
来源：http://hz.cheryme.top/gtniikihwu.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhoulong.xyz/gtmtomotqk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hongshengwenyu.top/gtryspupto.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhengqikj.top/gtkuzjshbo.html

C#:   lock (gate) { shared++; }
来源：http://hz.xinyue.icu/gtqrpoxnkz.html

[O04] 定义异步函数并等待
来源：http://hz.cheryme.top/gtmwnfutgm.html

Py:   async def f():⏎    await g()
来源：http://hz.zycfv.cn/gtkpswautq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.guowangkeji.top/gtehzefdac.html

JS:   async function f() { await g(); }
来源：http://hz.ydjk.org.cn/gteoavyvmt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.bjfxy.top/gtngyinlka.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jiagoushi.top/gtwcjrqdlx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.fengsongda.top/gtazenydet.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xingfuxueyuan.xyz/gtvxlhpepr.html

C#:   async Task F() { await G(); }
来源：http://hz.hywenlv.cn/gturlknbbr.html

[O05] 并发执行并等待全部完成
来源：http://hz.gogol.net.cn/gtnvcvytea.html

Py:   asyncio.gather(*tasks)
来源：http://hz.meibo888.top/gtbabilgmy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.dashuyun.cn/gtfoaamfgh.html

JS:   await Promise.all(tasks)
来源：http://hz.zhaomingkeji.xyz/gtgbxalldg.html

TS:   await Promise.all(tasks)
来源：http://hz.mhx1999.top/gtkidcygbl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zycfv.cn/gtpzsjpjmi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ydzc1.top/gtnqpdnkdl.html

Ruby: threads.map(&:join)
来源：http://hz.shanyushiyangkeji.top/gtsprqpmgi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.gzhubu.top/gtrimpsibr.html

[O06] 使用进程池
来源：http://hz.gaohongyu789.top/gtfrytjaiw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ybcxt.top/gtmatjecli.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.gaohongyu789.top/gtmqjlxfch.html

JS:   // child_process / cluster 模块
来源：http://hz.nanxinkj.top/gttynctbfv.html

TS:   // child_process / cluster 模块
来源：http://hz.pycfn.com/gtbnedhkgu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yuxming.cn/gtxdypmrtd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hysaishi.cn/gtjqpxaayi.html

Ruby: // fork 块
来源：http://hz.shanyushiyangtech.top/gtoweyrfsy.html

C#:   Parallel.For
来源：http://hz.zhoulong.xyz/gtpfbramwo.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtqkyjojbx.html

P. 常用工具函数
来源：http://hz.ybcxt.top/gtokzumske.html

================================================================================
来源：http://hz.birdmap.top/gtuyjgfwkp.html

[P01] 生成 UUID
来源：http://hz.zhijiandao.cn/gtncuqfwqq.html

Py:   str(uuid.uuid4())
来源：http://hz.jlsjyb.cn/gtytfwvdey.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jqgfzy.top/gtlqojokbf.html

JS:   crypto.randomUUID()
来源：http://hz.nanxinkj.top/gtymdxjqzw.html

TS:   crypto.randomUUID()
来源：http://hz.xuanzx.com/gtenovdjoq.html

Java: UUID.randomUUID().toString()
来源：http://hz.hfpthk.cn/gtvrtjrzzr.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jqgfzy.top/gtdnwjjdii.html

Ruby: SecureRandom.uuid
来源：http://hz.cucudq.cn/gtxhjytuim.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.pycfn.com/gtgcytqyum.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xuanzx.com/gtavpgrlag.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yonumen.top/gtazwzyvsl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zdqjudy.top/gthtxgnrdk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yangfankeji.com/gtoyjrzghl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.chenjidiqi.icu/gtmicaxlfl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xinyue.icu/gtxyvndayn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.havefunace.top/gtdokbdzmy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yanxiufei.cn/gtregqoucw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.sxryk.cn/gttjrttliu.html

[P03] 生成短随机字符串
来源：http://hz.snrcjt.cn/gtaanobbjz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ydzc1.top/gtjfgnsmtq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.sufxvd.cn/gtqevefkdb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tanke756.top/gtcjbpvbyx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shangyingyoupin.top/gtkctfafsm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.c1oappe.top/gtavklsegz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ywan-chungtsiang.top/gtylblayzp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sxryk.cn/gtdnhurwaw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhengqikj.top/gtigkogutj.html

[P04] 求长度
来源：http://hz.sweek.top/gtxgidmjmb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.daxiang520.top/gtfpazxpsv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.daxiang520.top/gtyjxqyktq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.kuanghao11.cn/gtjnscarnh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xinyue.icu/gtjnkbqzgz.html

Java: list.size();  map.size();  s.length()
来源：http://hz.chenjidiqi.icu/gtjkmtkqid.html

Go:   len(arr);  len(m)
来源：http://hz.xuanzx.com/gtcvkvbbxq.html

Ruby: x.length;  x.size
来源：http://hz.gaohongyu789.top/gtaqhezmrv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.smart0.xyz/gtydkqdjdo.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hnxiangtu.top/gtsvcuwges.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.snrcjt.cn/gtdvtmbpks.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yvedp.cn/gtsvsndyyv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.bjfxy.top/gtipzeqcea.html


<!-- 参考信息 -->