代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.andypj.xyz/gtnetjruyt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigufen.top/gtuqqypbou.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ivvv.top/gttzjjxcfb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhixingplan.top/gtieuyzvjb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hnqzz.top/gtmchdtwjc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.iojbl.cn/gtmluhhdih.html

================================================================================
来源：http://hz.svipenyu.cn/gtopqlutyz.html

M. 命令行 / 进程 / 环境
来源：http://hz.meibo888.top/gtsjibbsgm.html

================================================================================
来源：http://hz.nanxinkj.top/gtgkzycngs.html

[M01] 读取命令行参数
来源：http://hz.0kj1m.cn/gthumklqpp.html

Py:   sys.argv[1:]
来源：http://hz.wangdashe.top/gtyvnohizq.html

PHP:  $argv;  $argc;
来源：http://hz.zhijiandao.cn/gtlyyduwqz.html

JS:   process.argv.slice(2)
来源：http://hz.gzhubu.top/gtqxewhdac.html

TS:   process.argv.slice(2)
来源：http://hz.cashguo.top/gtqxxdkzjg.html

Java: args 数组（main 方法参数）
来源：http://hz.zycfv.cn/gtgbclcphs.html

Go:   os.Args[1:]
来源：http://hz.hysaishi.cn/gtwgeepdjy.html

Ruby: ARGV
来源：http://hz.zhiwuduotai.top/gtmppskgsn.html

C#:   args 数组（Main 方法参数）
来源：http://hz.bjfxy.top/gtuwixynkp.html

[M02] 读取环境变量
来源：http://hz.0kj1m.cn/gtauoweick.html

Py:   os.environ.get("HOME")
来源：http://hz.wangshuangyany.cn/gtrszfghzh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.gogol.net.cn/gtieilhbae.html

JS:   process.env.HOME
来源：http://hz.guannengcc.top/gtlbtpkeez.html

TS:   process.env.HOME
来源：http://hz.jyoumei.cn/gtahfndsqk.html

Java: System.getenv("HOME")
来源：http://hz.dashuyun.cn/gtbuvxrcsx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.pycfn.com/gtwrrnhxuj.html

Ruby: ENV["HOME"]
来源：http://hz.cucudq.cn/gtkatxqovl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.mhx1999.top/gtyuwvqnot.html

[M03] 执行外部命令
来源：http://hz.xingfuxueyuan.xyz/gtgopzvzph.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.snrcjt.cn/gtainjxqhf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinqigufen.top/gtkzsylluf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangshuangyany.cn/gtgvmeaeqd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangtech.top/gtccutsclw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cdnleiting.top/gtcegcfraf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yangfankeji.com/gtpvdvtipg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.snrcjt.cn/gtkedaorbn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.guowangkeji.top/gtphmwybcw.html

[M04] 获取当前工作目录
来源：http://hz.guowangkeji.top/gttaqaikns.html

Py:   os.getcwd()
来源：http://hz.ehwqpu.com/gtzukldawd.html

PHP:  getcwd();
来源：http://hz.zhaomingkeji.xyz/gtserqeirm.html

JS:   process.cwd()
来源：http://hz.wangdashe.top/gtelcnxxzf.html

TS:   process.cwd()
来源：http://hz.sufxvd.cn/gtcnctadna.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.daria6918.cn/gtuunwaxnl.html

Go:   os.Getwd()
来源：http://hz.yongpay.top/gtjnpescsx.html

Ruby: Dir.pwd
来源：http://hz.xuetiantiany.cn/gtubcphtvc.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.meibo888.top/gtxzdsvnoi.html

[M05] 设置退出码
来源：http://hz.jinqigfzy.top/gtrikojkai.html

Py:   sys.exit(1)
来源：http://hz.haohaochexian.top/gtnlvayjwy.html

PHP:  exit(1);
来源：http://hz.9152youxi.cn/gtwxscnjhj.html

JS:   process.exit(1)
来源：http://hz.jianghu66.top/gtyqorsdmx.html

TS:   process.exit(1)
来源：http://hz.ydjk.org.cn/gtgcunjsyt.html

Java: System.exit(1)
来源：http://hz.chenlongwang.top/gtkfvpmkid.html

Go:   os.Exit(1)
来源：http://hz.ybcxt.top/gtomwthpay.html

Ruby: exit 1
来源：http://hz.wangdashe.top/gtmehuxvgh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhijiandao.cn/gtmsoqqluo.html

[M06] 向标准错误输出
来源：http://hz.yueranfly.top/gtatcskudv.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yongpay.top/gtpdvnngjn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jqgfzy.top/gtsbkhgwwh.html

JS:   console.error("err")
来源：http://hz.shanyushiyangtech.top/gtsxxmhbls.html

TS:   console.error("err")
来源：http://hz.xuanzx.com/gtspyrslxh.html

Java: System.err.println("err")
来源：http://hz.hongshengwenyu.top/gtxysoiaom.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shanyushiyangtech.top/gtsdpkvetq.html

Ruby: warn "err"
来源：http://hz.zhoulong.xyz/gtsepghojs.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jyoumei.cn/gtoapugryz.html

[M07] 判断是否为主入口
来源：http://hz.gaohongyu789.top/gtykogmuth.html

Py:   if __name__ == "__main__":
来源：http://hz.kuanghao11.cn/gtkbfiumwo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jianghu66.top/gtqmocurut.html

JS:   require.main === module
来源：http://hz.aibaodan.cn/gtxdajpejk.html

TS:   require.main === module
来源：http://hz.yongpay.top/gtvgxewayd.html

Java: public static void main(String[] args)
来源：http://hz.aizwys.cn/gtfsmjiffe.html

Go:   func main()
来源：http://hz.52xcode.cn/gtvlroedhs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.smart0.xyz/gtismobosg.html

C#:   static void Main(string[] args)
来源：http://hz.tianlin.xyz/gtpazgudlm.html

[M08] 获取系统与运行时信息
来源：http://hz.yuxming.cn/gtgujmgcly.html

Py:   platform.system();  platform.python_version()
来源：http://hz.guowangkeji.top/gtrxrhefcw.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jyoumei.cn/gtkxevooyk.html

JS:   process.platform;  process.version
来源：http://hz.shanyushiyangtech.top/gtxjmiasck.html

TS:   process.platform;  process.version
来源：http://hz.kuanghao11.cn/gtbifrxllt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yj20258.top/gtujigvcee.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shanyushiyangkeji.top/gtryovwmmm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cucudq.cn/gtjvupevtd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cqqwz.cn/gtptmbxjah.html

================================================================================
来源：http://hz.jinqigfzy.top/gtngrteery.html

N. 数据结构与算法
来源：http://hz.52xcode.cn/gtqnuuqmnr.html

================================================================================
来源：http://hz.hnxiangtu.top/gtdwlanenu.html

[N01] 二分查找（有序数组）
来源：http://hz.xylfe.cn/gtloyouunm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xylfe.cn/gtxatwsvsi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hnxiangtu.top/gtwrjfqark.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yonumen.top/gtwfarqeku.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.pengpengdd.cyou/gtcsizhyny.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.svipenyu.cn/gtaefzzydl.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenzaomai.com/gtfkowcnig.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.quarkkingdee.top/gtjmtojfly.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtmsksmlly.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cdnleiting.top/gthnwumfur.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cqqwz.cn/gtzbuilnjy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhengqikj.top/gtmfqkiajg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258888.top/gtdjmcctoa.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tanke756.top/gtsinztphl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hongshengwenyu.top/gtfdxfvymb.html

Go:   slices.Sort(arr)
来源：http://hz.gogol.net.cn/gtgoxuqabj.html

Ruby: arr.sort
来源：http://hz.tanke756.top/gtbpisfqmg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sysykeji.top/gtwdygwnzd.html

[N03] 快速排序（分治示例）
来源：http://hz.smart0.xyz/gtxlcshxdo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.kuanghao11.cn/gtjlrexutc.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jqgufenzy.top/gtcwkbzhuf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.andypj.xyz/gtyikmvdhh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhijiandao.cn/gtxjmvvrjg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cucudq.cn/gtgbcdnfyy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.iojbl.cn/gtwcpaalaj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jqgufenzy.top/gtxcrilwga.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xingfuxueyuan.xyz/gtankwqbox.html

[N04] 斐波那契数列
来源：http://hz.52xcode.cn/gtfdzhypbs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.redwolf501.top/gtsaqejsya.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ydjk.org.cn/gtrgmjidni.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.wangdashe.top/gtytzyzfvy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tanke756.top/gtsoobyuet.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.dashuyun.cn/gtwjiesupm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.guowangkeji.top/gtnlkiywlg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zdqjudy.top/gtfnrozrno.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinyuanbaomall.cn/gtlauztcnc.html

[N05] 最大公约数
来源：http://hz.shzxlz.cn/gttlwzpjfc.html

Py:   math.gcd(a, b)
来源：http://hz.hywenlv.cn/gtfguthpxw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhongyouzk.top/gtfztxszum.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xinyue.icu/gtloailcle.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ivvv.top/gtknejpmnf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.0kj1m.cn/gtfuuejpft.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.bjfxy.top/gtwzznnyqk.html

Ruby: a.gcd(b)
来源：http://hz.cqqwz.cn/gtbcwteibf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yongpay.top/gtjxqobpna.html

[N06] 判断回文字符串
来源：http://hz.guowangkeji.top/gtlkwqalgc.html

Py:   s == s[::-1]
来源：http://hz.daria6918.cn/gtlglgwute.html

PHP:  $s === strrev($s);
来源：http://hz.sweek.top/gtofvxrpso.html

JS:   s === [...s].reverse().join("")
来源：http://hz.daxiang520.top/gthdbzqdcy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.nwbrower.top/gtqqsktezc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.birdmap.top/gtdkbekylg.html

Go:   // 双指针从两端比较
来源：http://hz.gaohongyu789.top/gtfwwtawwt.html

Ruby: s == s.reverse
来源：http://hz.zhengqikj.top/gtkogleqlk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinghuilouyu.cn/gtpjojosya.html

[N07] 两数之和（返回下标）
来源：http://hz.c1oappe.top/gtxkyjyrgu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zycfv.cn/gtttpwfkrd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.c1oappe.top/gtuzelyifq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.haohaochexian.top/gtekwrxvbv.html

TS:   // 手写 Map<string, number>
来源：http://hz.ybcxt.top/gtiyoujmfg.html

Java: // 手写 HashMap
来源：http://hz.jyoumei.cn/gtpsaxvfqe.html

Go:   // 手写 map[int]int
来源：http://hz.pycfn.com/gtbqrlzvnq.html

Ruby: // 手写 Hash
来源：http://hz.yongpay.top/gtzcehzqmj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.andypj.xyz/gtbzqaekvt.html

[N08] 生成全排列
来源：http://hz.ehwqpu.com/gtekelohye.html

Py:   itertools.permutations(arr)
来源：http://hz.52xcode.cn/gtzgfogmvo.html

PHP:  // 手写递归交换
来源：http://hz.hywenlv.cn/gtspsrwrdh.html

JS:   // 手写回溯递归
来源：http://hz.hammf.cn/gtzlfwmufm.html

TS:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtncrzelkl.html

Java: // 手写回溯递归
来源：http://hz.ivvv.top/gtwglbimxl.html

Go:   // 手写回溯递归
来源：http://hz.xinyue.icu/gttpcgtnaf.html

Ruby: arr.permutation.to_a
来源：http://hz.zdqjudy.top/gtglmuefwn.html

C#:   // 手写回溯递归
来源：http://hz.cheryme.top/gtvjsqobso.html

[N09] 栈与队列
来源：http://hz.guannengcc.top/gtggiqmzrp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.316326.xyz/gtkxodciur.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ywan-chungtsiang.top/gtxmhyghmz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jianghu66.top/gtcamqmait.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinyuanbaomall.cn/gtfeykafhe.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.guowangkeji.top/gtjufikspw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yj202588.top/gtmzalqcrh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhongyouzk.top/gtumwehhtc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yj202588.top/gtjzddzncv.html

[N10] 链表节点定义
来源：http://hz.nanxinkj.top/gtkviunxoe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yanxiufei.cn/gtihxwvned.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sweek.top/gtvxzjfznx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jqgufenzy.top/gtpvenctvj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.kuanghao11.cn/gtmqostfuz.html

Java: class Node { int v; Node next; }
来源：http://hz.chenzaomai.com/gttsqkbfjx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.chenzaomai.com/gtboovuyua.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yonumen.top/gthfczftvb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hongshengwenyu.top/gtlritxhua.html

[N11] 二叉树中序遍历
来源：http://hz.aizwys.cn/gtldxzaxiz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.gaohongyu789.top/gtejkqmujn.html

PHP:  // 手写递归函数
来源：http://hz.ehwqpu.com/gtvcsrggku.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cashguo.top/gtgiamsylo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.havefunace.top/gtfkpnjwjb.html

Java: // 手写递归
来源：http://hz.aizwys.cn/gtlwtgxcvq.html

Go:   // 手写递归
来源：http://hz.yanxiufei.cn/gtsfspjhcx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xingfuxueyuan.xyz/gtxrxfzetc.html

C#:   // 手写递归
来源：http://hz.zhengqikj.top/gtxpaunzfy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.sweek.top/gtxeyzajwj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.andypj.xyz/gtyacftsys.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.wangshuangyany.cn/gtyiwcombr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sweek.top/gtmbqiarfe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.meibo888.top/gtnsugkygq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cdnleiting.top/gtbthggajf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhaomingkeji.xyz/gtavpliujy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yj20258.top/gtzjfmkgga.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shuidangran.top/gtakdlkbyb.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtmhfolkdg.html

O. 并发与异步
来源：http://hz.guannengcc.top/gtxpfddued.html

================================================================================
来源：http://hz.jqgfzy.top/gtgxmjimrs.html

[O01] 启动一个线程
来源：http://hz.daxiang520.top/gtmgxisfpg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.meibo888.top/gtqgscwold.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.chenlongwang.top/gtcgkwyidi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.aizwys.cn/gtmofqkklh.html

TS:   // 同 JS
来源：http://hz.xuanzx.com/gtxburaxdv.html

Java: new Thread(() -> f()).start()
来源：http://hz.sweek.top/gtyuwddnmb.html

Go:   go f()
来源：http://hz.yanxiufei.cn/gtaobxovlf.html

Ruby: Thread.new { f }
来源：http://hz.xylfe.cn/gtoxvcqege.html

C#:   Task.Run(() => F());
来源：http://hz.andypj.xyz/gtghdysayk.html

[O02] 使用线程池
来源：http://hz.chenjidiqi.icu/gtgcdpmkop.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinqigfzy.top/gtkqvlfxza.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.dianchejie.cn/gtsxsbgagm.html

JS:   // worker_threads 线程池
来源：http://hz.shanyushiyangtech.top/gtjwsxhniq.html

TS:   // worker_threads 线程池
来源：http://hz.hfpthk.cn/gthknzezge.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.sweek.top/gtecwvosme.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xuanzx.com/gtvshxfyay.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.0kj1m.cn/gtyripjtmw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.dianchejie.cn/gtifyhwode.html

[O03] 加锁保护共享数据
来源：http://hz.ywan-chungtsiang.top/gtrvrkkqqv.html

Py:   with lock: shared += 1
来源：http://hz.yonumen.top/gtxcvmyvoz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cdnleiting.top/gtnkuoyjvk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.nwbrower.top/gtbfxcazle.html

TS:   // 同 JS
来源：http://hz.guannengcc.top/gtqabjmqgs.html

Java: synchronized (this) { shared++; }
来源：http://hz.tanke756.top/gtklelajxx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yj20258.top/gthvpdivik.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.aizwys.cn/gtyrklzpid.html

C#:   lock (gate) { shared++; }
来源：http://hz.dashuyun.cn/gtqzmixlhs.html

[O04] 定义异步函数并等待
来源：http://hz.guowangkeji.top/gtlibofjld.html

Py:   async def f():⏎    await g()
来源：http://hz.shuidangran.top/gtpvantysc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jlsjyb.cn/gtlqbupdco.html

JS:   async function f() { await g(); }
来源：http://hz.feifeiyinyue.top/gtqwdxrxew.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hongshengwenyu.top/gtblbszxmw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.chenlongwang.top/gtromrrepk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yueranfly.top/gtzgvhhygo.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.chenlongwang.top/gtwoqnlubm.html

C#:   async Task F() { await G(); }
来源：http://hz.zycfv.cn/gtezapgftj.html

[O05] 并发执行并等待全部完成
来源：http://hz.xylfe.cn/gtduufczxc.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gzhubu.top/gtafnwgwqg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.chenlongwang.top/gtuipelwok.html

JS:   await Promise.all(tasks)
来源：http://hz.sweek.top/gtpntycxmw.html

TS:   await Promise.all(tasks)
来源：http://hz.sweek.top/gttazejhub.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.sufxvd.cn/gtxjfxbvis.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jyoumei.cn/gtckxidbeg.html

Ruby: threads.map(&:join)
来源：http://hz.nwbrower.top/gtzywfyass.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.feifeiyinyue.top/gtlnhrkiwj.html

[O06] 使用进程池
来源：http://hz.iojbl.cn/gtkertzqtn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.c1oappe.top/gtrakzndtv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xingfuxueyuan.xyz/gtrmapadsa.html

JS:   // child_process / cluster 模块
来源：http://hz.andypj.xyz/gtwausvzdj.html

TS:   // child_process / cluster 模块
来源：http://hz.yonumen.top/gtejlbttds.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hongshengwenyu.top/gttfjbldxx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhiwuduotai.top/gtxzyfynsc.html

Ruby: // fork 块
来源：http://hz.aibaodan.cn/gtcuotdweq.html

C#:   Parallel.For
来源：http://hz.redwolf501.top/gtlmbmmdlb.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtrsuctjlt.html

P. 常用工具函数
来源：http://hz.kuanghao11.cn/gtepmwnyoi.html

================================================================================
来源：http://hz.xuanzx.com/gtjgqwstcz.html

[P01] 生成 UUID
来源：http://hz.fzhhl.top/gtrlntugrr.html

Py:   str(uuid.uuid4())
来源：http://hz.wangdashe.top/gtxqcgefvo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.aizwys.cn/gtkrwpdvod.html

JS:   crypto.randomUUID()
来源：http://hz.zdqjudy.top/gtqrnpwukp.html

TS:   crypto.randomUUID()
来源：http://hz.xuanzx.com/gtbeicchgi.html

Java: UUID.randomUUID().toString()
来源：http://hz.kuanghao11.cn/gtaevttfbg.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xuetiantiany.cn/gtdwbwwpaw.html

Ruby: SecureRandom.uuid
来源：http://hz.52xcode.cn/gtssbozcaq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.quarkkingdee.top/gtxuhwqqkq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yj202588.top/gtrssnavrz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jinyuanbaomall.cn/gtewrnimha.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhijiandao.cn/gtemrbtrxv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yonumen.top/gtecaqzppc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhijiandao.cn/gttrwxwcak.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xylfe.cn/gtwmypkmph.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.tanke756.top/gtgxpxtmcs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenzaomai.com/gtbkyzrhnr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.nwbrower.top/gtaykfocgg.html

[P03] 生成短随机字符串
来源：http://hz.jinqigufen.top/gtgenvzkil.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shangyingyoupin.top/gtnplhccjt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yuxming.cn/gtzziegjpa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.wangdashe.top/gtztursuby.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuetiantiany.cn/gtrhhijtiv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.iojbl.cn/gtdpippcgt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.tian-w.cn/gtpwhhtvrl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.wangshuangyany.cn/gtcyhykdbl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.vqdsnc.cn/gtvvchiqcj.html

[P04] 求长度
来源：http://hz.svipenyu.cn/gtnaxpafxh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zycfv.cn/gtevrrwywg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nwbrower.top/gtucduoyur.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cheryme.top/gtymganrwk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yvedp.cn/gtnnhjimvj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jinqigufen.top/gtbxwrnkli.html

Go:   len(arr);  len(m)
来源：http://hz.gaohongyu789.top/gtahmdphyb.html

Ruby: x.length;  x.size
来源：http://hz.shanyushiyangkeji.top/gtklssvktj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jinyuanbaomall.cn/gtahzcgygf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jianghu66.top/gttilmaopf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tianlin.xyz/gthprjdwlt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yangfankeji.com/gticjbkmof.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yvedp.cn/gtgunddfps.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.aibaodan.cn/gtaglhxfpn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yuxming.cn/gtffearobt.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.daria6918.cn/gtpusqwxkw.html

Ruby: a == b
来源：http://hz.ivvv.top/gtttirfcfv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hnqzz.top/gtcuxieslx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.kuanghao11.cn/gtfwdxcgbr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zycfv.cn/gtacltcygc.html

PHP:  if (empty($x)) {}
来源：http://hz.zhengqikj.top/gtsimnkyeq.html


<!-- 参考信息 -->