代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pengpengdd.cyou/gtvfxypddj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.svipenyu.cn/gtzxjfypvo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.quarkkingdee.top/gtjchnxkmp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.daxiang520.top/gtmssszpdb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ybcxt.top/gtwknhdhji.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.nanxinkj.top/gtkcerintf.html

================================================================================
来源：http://hz.jqgufenzy.top/gtrfolfjcf.html

M. 命令行 / 进程 / 环境
来源：http://hz.ydjk.org.cn/gtrwkjyage.html

================================================================================
来源：http://hz.xinyue.icu/gtwrgplfje.html

[M01] 读取命令行参数
来源：http://hz.316326.xyz/gtpambracj.html

Py:   sys.argv[1:]
来源：http://hz.shuidangran.top/gtkoiaqavz.html

PHP:  $argv;  $argc;
来源：http://hz.hywenlv.cn/gtlotsiues.html

JS:   process.argv.slice(2)
来源：http://hz.ybcxt.top/gtvbqumrou.html

TS:   process.argv.slice(2)
来源：http://hz.zhaomingkeji.xyz/gtxljxrydn.html

Java: args 数组（main 方法参数）
来源：http://hz.shanyushiyangtech.top/gtrebofdne.html

Go:   os.Args[1:]
来源：http://hz.yonumen.top/gtjbetbigr.html

Ruby: ARGV
来源：http://hz.nwbrower.top/gthmabchti.html

C#:   args 数组（Main 方法参数）
来源：http://hz.pycfn.com/gtfbslbbhl.html

[M02] 读取环境变量
来源：http://hz.yuanzhike.top/gtacuyuvrg.html

Py:   os.environ.get("HOME")
来源：http://hz.ydjk.org.cn/gtvbbalutp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.tian-w.cn/gtuvxzelza.html

JS:   process.env.HOME
来源：http://hz.feifeiyinyue.top/gtavnugkat.html

TS:   process.env.HOME
来源：http://hz.hammf.cn/gtcfikllkg.html

Java: System.getenv("HOME")
来源：http://hz.jyoumei.cn/gtcbaipxed.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.guowangkeji.top/gtfoebwenv.html

Ruby: ENV["HOME"]
来源：http://hz.gotoacloud.top/gtgoejhrto.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yueranfly.top/gthiqbvvpj.html

[M03] 执行外部命令
来源：http://hz.gotoacloud.top/gtdiovfsfh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ppjwa.cn/gtkainvbok.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.aizwys.cn/gthmohjnuz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zdqjudy.top/gtbfmqcprz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gogol.net.cn/gtcneqbxhl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinghuilouyu.cn/gtnciejqle.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.aibaodan.cn/gtxmnqgwkf.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sweek.top/gtseezfjpp.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhijiandao.cn/gtrtciclzg.html

[M04] 获取当前工作目录
来源：http://hz.shanyushiyangtech.top/gtiyoqrjrw.html

Py:   os.getcwd()
来源：http://hz.hnxiangtu.top/gthydbhywm.html

PHP:  getcwd();
来源：http://hz.xuetiantiany.cn/gtkudhusrh.html

JS:   process.cwd()
来源：http://hz.daxiang520.top/gtlaqjxmcb.html

TS:   process.cwd()
来源：http://hz.meibo888.top/gtasgebzqr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.pengpengdd.cyou/gtsvtqkvif.html

Go:   os.Getwd()
来源：http://hz.jqgfzy.top/gtikdzuiot.html

Ruby: Dir.pwd
来源：http://hz.hongshengwenyu.top/gtbrtwrizr.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.fzhhl.top/gttbtniomc.html

[M05] 设置退出码
来源：http://hz.yvedp.cn/gtlkzoprug.html

Py:   sys.exit(1)
来源：http://hz.guowangkeji.top/gtpkbpcbiw.html

PHP:  exit(1);
来源：http://hz.ehwqpu.com/gtlmfnuskk.html

JS:   process.exit(1)
来源：http://hz.quarkkingdee.top/gtgdatdysg.html

TS:   process.exit(1)
来源：http://hz.hywenlv.cn/gttqoyfgot.html

Java: System.exit(1)
来源：http://hz.cqqwz.cn/gtcdianjyi.html

Go:   os.Exit(1)
来源：http://hz.yuanzhike.top/gtrchaonlo.html

Ruby: exit 1
来源：http://hz.hfpthk.cn/gtexvuckwe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.chenlongwang.top/gtxvecnxnr.html

[M06] 向标准错误输出
来源：http://hz.wangshuangyany.cn/gtgltjbhbb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yj20258.top/gteblilebf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yj20258888.top/gtxdwvvqcy.html

JS:   console.error("err")
来源：http://hz.gzhubu.top/gtqddiyswr.html

TS:   console.error("err")
来源：http://hz.hywenlv.cn/gtreepswig.html

Java: System.err.println("err")
来源：http://hz.chenlongwang.top/gtpyzjztfd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhiwuduotai.top/gtbzmghxmp.html

Ruby: warn "err"
来源：http://hz.xinyue.icu/gtvlunpewb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shanyushiyangkeji.top/gtynjrftrf.html

[M07] 判断是否为主入口
来源：http://hz.xziqi.cn/gtrturohvo.html

Py:   if __name__ == "__main__":
来源：http://hz.redwolf501.top/gtkszfrfdo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.fzhhl.top/gttmbgewbh.html

JS:   require.main === module
来源：http://hz.nanxuanxn.top/gtalzvzdzw.html

TS:   require.main === module
来源：http://hz.shzxlz.cn/gtmnoxlhor.html

Java: public static void main(String[] args)
来源：http://hz.aizwys.cn/gtuzudcude.html

Go:   func main()
来源：http://hz.zhengqikj.top/gtokdnzvwx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhiwuduotai.top/gtqqwopkqe.html

C#:   static void Main(string[] args)
来源：http://hz.yonumen.top/gtyktzayku.html

[M08] 获取系统与运行时信息
来源：http://hz.feifeiyinyue.top/gthlfhloap.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yj20258888.top/gteosjenck.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yj20258.top/gtlkvjtduq.html

JS:   process.platform;  process.version
来源：http://hz.jqgfzy.top/gtflxqdaxp.html

TS:   process.platform;  process.version
来源：http://hz.zhengqikj.top/gtpvxuiilb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.smart0.xyz/gtsfevjlwt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jqgfzy.top/gtirwxyvrs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.nwbrower.top/gtduazulji.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shangyingyoupin.top/gtjfjguwae.html

================================================================================
来源：http://hz.andypj.xyz/gtjkfkdnim.html

N. 数据结构与算法
来源：http://hz.hysaishi.cn/gtgxldrruy.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtxbhazpsu.html

[N01] 二分查找（有序数组）
来源：http://hz.redwolf501.top/gtxcxwyxah.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinghuilouyu.cn/gtfzlmyxfl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhaomingkeji.xyz/gtnznvqaui.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fengsongda.top/gtjjnomwmz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ybcxt.top/gtfzkgrsfk.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.daxiang520.top/gtnmlfpefe.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cheryme.top/gtvloioapa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhiwuduotai.top/gtyiibfjvp.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.iojbl.cn/gtlqaflbrn.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhiwuduotai.top/gtxhtrthcg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.smart0.xyz/gtbepwxnzb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yongpay.top/gtvermxfmz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuetiantiany.cn/gthrzshgvx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ppjwa.cn/gtkkqhwstn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.gogol.net.cn/gtlmydotcf.html

Go:   slices.Sort(arr)
来源：http://hz.xinyue.icu/gtbmnfjpxh.html

Ruby: arr.sort
来源：http://hz.cashguo.top/gtauxxdbxm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sufxvd.cn/gtmsjsvmhq.html

[N03] 快速排序（分治示例）
来源：http://hz.yanxiufei.cn/gtrinqyjyh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xylfe.cn/gtvhpkdnle.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shzxlz.cn/gtiskbkwmw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sweek.top/gttjpyhuuk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.haohaochexian.top/gttonshrxr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.sufxvd.cn/gtlzhuntsr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.feifeiyinyue.top/gtcpqwntfk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.nwbrower.top/gtddwgjidw.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yongpay.top/gtsidbaoxw.html

[N04] 斐波那契数列
来源：http://hz.sysykeji.top/gtoixtygcy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhongyouzk.top/gtrcrptgdd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cheryme.top/gtflzsdccr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hysaishi.cn/gtlawpwcds.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shuidangran.top/gtfjhrsbze.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cqqwz.cn/gtnyzsxnqx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhoulong.xyz/gtvucyvlqz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.bjfxy.top/gtgyspnawb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yuanzhike.top/gttdymlwec.html

[N05] 最大公约数
来源：http://hz.havefunace.top/gtknafbelw.html

Py:   math.gcd(a, b)
来源：http://hz.yuanzhike.top/gtymzdotva.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jianghu66.top/gttmdfjpqt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.birdmap.top/gtutjogusm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yangfankeji.com/gtikkbactp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.daxiang520.top/gtffwgilnh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.daxiang520.top/gtmalazszw.html

Ruby: a.gcd(b)
来源：http://hz.c1oappe.top/gtzykulzqi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yueranfly.top/gtzqxwujpn.html

[N06] 判断回文字符串
来源：http://hz.nanxinkj.top/gtimustwdb.html

Py:   s == s[::-1]
来源：http://hz.sxryk.cn/gtrbtddmji.html

PHP:  $s === strrev($s);
来源：http://hz.wangdashe.top/gtylzladnq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtlhoyciwt.html

TS:   s === [...s].reverse().join("")
来源：http://hz.birdmap.top/gtzwhpepxo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.fzhhl.top/gtljdchooy.html

Go:   // 双指针从两端比较
来源：http://hz.yongpay.top/gthtmqlvjd.html

Ruby: s == s.reverse
来源：http://hz.xingfuxueyuan.xyz/gtehfcjolh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shzxlz.cn/gtcdcebdoj.html

[N07] 两数之和（返回下标）
来源：http://hz.wangshuangyany.cn/gtfpwzxpse.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cucudq.cn/gtyquhvzet.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hywenlv.cn/gtivvnihfb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jiagoushi.top/gtvqvnegtf.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinqigufen.top/gtsvahrlht.html

Java: // 手写 HashMap
来源：http://hz.gaohongyu789.top/gtpgfoexvu.html

Go:   // 手写 map[int]int
来源：http://hz.tanke756.top/gtqbccgaql.html

Ruby: // 手写 Hash
来源：http://hz.wangdashe.top/gtsqrohryy.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.guowangkeji.top/gtptemquch.html

[N08] 生成全排列
来源：http://hz.shanyushiyangkeji.top/gtvsipcewt.html

Py:   itertools.permutations(arr)
来源：http://hz.yuanzhike.top/gtakmcjjll.html

PHP:  // 手写递归交换
来源：http://hz.xziqi.cn/gtktzqhjmi.html

JS:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtiqwynohq.html

TS:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtssmyjeid.html

Java: // 手写回溯递归
来源：http://hz.yj202588.top/gtmzqoltvq.html

Go:   // 手写回溯递归
来源：http://hz.jinqigufen.top/gtocerrsfc.html

Ruby: arr.permutation.to_a
来源：http://hz.ydjk.org.cn/gteruffobz.html

C#:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtmgcrgwvi.html

[N09] 栈与队列
来源：http://hz.dashuyun.cn/gtzfftedem.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhoulong.xyz/gtjmspklrr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xziqi.cn/gtouwmtvve.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xinyue.icu/gtednliuyf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.wangdashe.top/gtzuqaujaq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yangfankeji.com/gtxjmpdbrs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.pengpengdd.cyou/gtzfrbwodr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.316326.xyz/gtcupdoauj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.aizwys.cn/gtmpealysu.html

[N10] 链表节点定义
来源：http://hz.xuetiantiany.cn/gtmuxnuejn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xuetiantiany.cn/gtgxlfuphv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.wangshuangyany.cn/gttsyhufdi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.pengpengdd.cyou/gtucqngtmn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.mhx1999.top/gtlitgljuj.html

Java: class Node { int v; Node next; }
来源：http://hz.ehwqpu.com/gtvsbwmfzd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tian-w.cn/gtbwycpnka.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zdqjudy.top/gtggupzxjt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hnqzz.top/gtyzkibelw.html

[N11] 二叉树中序遍历
来源：http://hz.redwolf501.top/gtjkcpiqxa.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yanxiufei.cn/gtwnwbejqy.html

PHP:  // 手写递归函数
来源：http://hz.zhijiandao.cn/gtfganibcm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgfzy.top/gtzvmpuctd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxinkj.top/gtqnmfqtlr.html

Java: // 手写递归
来源：http://hz.cucudq.cn/gtgbvfweup.html

Go:   // 手写递归
来源：http://hz.yonumen.top/gtuchyubdp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yueranfly.top/gtiugdbffk.html

C#:   // 手写递归
来源：http://hz.hysaishi.cn/gtfwjyvdri.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhengqikj.top/gtpsbxpaxi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tanke756.top/gtbopggfye.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.bjfxy.top/gtheikptkh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258888.top/gtfvghqtjw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.snrcjt.cn/gtjjjmkvvx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangdashe.top/gtvmwohknk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.316326.xyz/gtqlvhzcct.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zdqjudy.top/gtnzqihwvs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fengsongda.top/gthfllfgas.html

================================================================================
来源：http://hz.guannengcc.top/gtxmwezgvp.html

O. 并发与异步
来源：http://hz.c1oappe.top/gtxqrcoztz.html

================================================================================
来源：http://hz.316326.xyz/gtvztkgqse.html

[O01] 启动一个线程
来源：http://hz.ywan-chungtsiang.top/gtlwsuatou.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shanyushiyangkeji.top/gtnjaojszr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.snrcjt.cn/gtbmsaucnq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.nanxinkj.top/gtrhovpnsc.html

TS:   // 同 JS
来源：http://hz.mhx1999.top/gtjwdsyxdy.html

Java: new Thread(() -> f()).start()
来源：http://hz.xuanzx.com/gtnthtdadx.html

Go:   go f()
来源：http://hz.yj20258.top/gtpdpechmx.html

Ruby: Thread.new { f }
来源：http://hz.yongpay.top/gtyocosjyx.html

C#:   Task.Run(() => F());
来源：http://hz.jqgufenzy.top/gtxfhhmyak.html

[O02] 使用线程池
来源：http://hz.cucudq.cn/gtqsqmkurh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yueranfly.top/gtgrfpvbwm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jiagoushi.top/gtpbufyikj.html

JS:   // worker_threads 线程池
来源：http://hz.gzhubu.top/gtlkypzjhe.html

TS:   // worker_threads 线程池
来源：http://hz.hysaishi.cn/gtqxlmatat.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.gogol.net.cn/gttbknnpgg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.aizwys.cn/gtiojgnzhr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.meibo888.top/gtvnjybfkz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.fzhhl.top/gtpmlttslp.html

[O03] 加锁保护共享数据
来源：http://hz.bjfxy.top/gtctioenrl.html

Py:   with lock: shared += 1
来源：http://hz.nwbrower.top/gtgcajquci.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jqgfzy.top/gtvgiacbtd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yj202588.top/gtatrcipvi.html

TS:   // 同 JS
来源：http://hz.yangfankeji.com/gtnplcycaz.html

Java: synchronized (this) { shared++; }
来源：http://hz.0kj1m.cn/gtwillzhay.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.aizwys.cn/gtdsqcppke.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.gogol.net.cn/gtvslrtuaq.html

C#:   lock (gate) { shared++; }
来源：http://hz.jyoumei.cn/gtccqcxtyi.html

[O04] 定义异步函数并等待
来源：http://hz.ppjwa.cn/gtihpkqcyp.html

Py:   async def f():⏎    await g()
来源：http://hz.cucudq.cn/gtajizabvx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jqgfzy.top/gtjfirrpgd.html

JS:   async function f() { await g(); }
来源：http://hz.yangfankeji.com/gtkjzbecbg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jinyuanbaomall.cn/gtqormmuhk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.daxiang520.top/gthrjrblya.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hongshengwenyu.top/gtudrlojfj.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.pycfn.com/gtyynhparx.html

C#:   async Task F() { await G(); }
来源：http://hz.vqdsnc.cn/gtnorjznbb.html

[O05] 并发执行并等待全部完成
来源：http://hz.ivvv.top/gtrinhzxms.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yongpay.top/gtpzujorjk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hongshengwenyu.top/gttwkrhhfj.html

JS:   await Promise.all(tasks)
来源：http://hz.zdqjudy.top/gtmkcnavuh.html

TS:   await Promise.all(tasks)
来源：http://hz.316326.xyz/gtvwviuqrb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cdnleiting.top/gtpnyqjubb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.chenjidiqi.icu/gtmkzwvyhf.html

Ruby: threads.map(&:join)
来源：http://hz.chenzaomai.com/gtoyxiaqvy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinghuilouyu.cn/gtvirbrbif.html

[O06] 使用进程池
来源：http://hz.sxryk.cn/gtotclhubf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.sysykeji.top/gtdcizmhvn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhijiandao.cn/gttcgluxnb.html

JS:   // child_process / cluster 模块
来源：http://hz.guowangkeji.top/gtnvqvfaxy.html

TS:   // child_process / cluster 模块
来源：http://hz.hnxiangtu.top/gtqflauuje.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.quarkkingdee.top/gtfsxrtuum.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.smart0.xyz/gtrzqtupfq.html

Ruby: // fork 块
来源：http://hz.gotoacloud.top/gtwzsdbcvy.html

C#:   Parallel.For
来源：http://hz.cashguo.top/gtqcguqaij.html

================================================================================
来源：http://hz.zhongyouzk.top/gtqctpxbyl.html

P. 常用工具函数
来源：http://hz.jinyuanbaomall.cn/gtnrennniv.html

================================================================================
来源：http://hz.yongpay.top/gtoshvtbdv.html

[P01] 生成 UUID
来源：http://hz.andypj.xyz/gthtckeaxj.html

Py:   str(uuid.uuid4())
来源：http://hz.guowangkeji.top/gtooivyvdd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.mhx1999.top/gttnsxviwx.html

JS:   crypto.randomUUID()
来源：http://hz.hongshengwenyu.top/gtckcuxlla.html

TS:   crypto.randomUUID()
来源：http://hz.yueranfly.top/gtakjqpczo.html

Java: UUID.randomUUID().toString()
来源：http://hz.xziqi.cn/gtwkqxdloh.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jiagoushi.top/gtumbcedjd.html

Ruby: SecureRandom.uuid
来源：http://hz.cheryme.top/gtrtbycdxl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.tianlin.xyz/gtxohsclfr.html

[P02] MD5 / SHA256 摘要
来源：http://hz.tian-w.cn/gtmhrkuhnb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hongshengwenyu.top/gtcvlryrpk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shanyushiyangkeji.top/gtgtmzhklg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.chenzaomai.com/gtjqdnbnmi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hysaishi.cn/gtgrrxnacz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.chenjidiqi.icu/gthzrhpxbp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.daria6918.cn/gtomobyvfj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinqigfzy.top/gtebdnpssp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.sufxvd.cn/gtbiucdlfj.html

[P03] 生成短随机字符串
来源：http://hz.cashguo.top/gtsutcmxly.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.chenlongwang.top/gtwmbptlfr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.kuanghao11.cn/gteqaxsyct.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.wangdashe.top/gtalbgwkio.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.svipenyu.cn/gtgdgfikus.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.meibo888.top/gthjptmpbg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hnxiangtu.top/gtzmlhmlxp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.guannengcc.top/gtvfbbefib.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gogol.net.cn/gtmocgnpfx.html

[P04] 求长度
来源：http://hz.hnxiangtu.top/gtogefmxit.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zdqjudy.top/gtimgslsek.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.mhx1999.top/gtnazbzsdl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.svipenyu.cn/gtrgkhoqvy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.c1oappe.top/gtwzdqzttf.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hysaishi.cn/gtisvwrrth.html

Go:   len(arr);  len(m)
来源：http://hz.havefunace.top/gtfadoalsz.html

Ruby: x.length;  x.size
来源：http://hz.dashuyun.cn/gtodejfjfm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.tian-w.cn/gtpjvhmjnf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhijiandao.cn/gtqcbajovp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yueranfly.top/gttrganufg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.feifeiyinyue.top/gtqydynvvd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenlongwang.top/gtkgpeygzj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.fengsongda.top/gtlwdroucd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.wangshuangyany.cn/gtypkwfbuj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jiagoushi.top/gtotnpxkbv.html

Ruby: a == b
来源：http://hz.vqdsnc.cn/gtgcrvadye.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xinyue.icu/gtqtoezasj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.pycfn.com/gtwjbnfvkt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.gotoacloud.top/gtbnbnulzj.html

PHP:  if (empty($x)) {}
来源：http://hz.cdnleiting.top/gtciyawyfl.html


<!-- 参考信息 -->