代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.gaohongyu789.top/gtojzaibmq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xziqi.cn/gtpsvqnjyj.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtwwddxdze.html

M. 命令行 / 进程 / 环境
来源：http://hz.yongpay.top/gtymxatghx.html

================================================================================
来源：http://hz.tianlin.xyz/gtsstutlov.html

[M01] 读取命令行参数
来源：http://hz.pycfn.com/gtzpxknict.html

Py:   sys.argv[1:]
来源：http://hz.tian-w.cn/gtdtfixlhk.html

PHP:  $argv;  $argc;
来源：http://hz.vqdsnc.cn/gtudlyuurn.html

JS:   process.argv.slice(2)
来源：http://hz.dashuyun.cn/gtupbslera.html

TS:   process.argv.slice(2)
来源：http://hz.guowangkeji.top/gtslrghfxi.html

Java: args 数组（main 方法参数）
来源：http://hz.pycfn.com/gtlbjgxupm.html

Go:   os.Args[1:]
来源：http://hz.sufxvd.cn/gtaghcjsaz.html

Ruby: ARGV
来源：http://hz.quarkkingdee.top/gtrptvcaow.html

C#:   args 数组（Main 方法参数）
来源：http://hz.snrcjt.cn/gttwdfeoih.html

[M02] 读取环境变量
来源：http://hz.zhiwuduotai.top/gtfrjyfznu.html

Py:   os.environ.get("HOME")
来源：http://hz.mhx1999.top/gtkbwijynj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zdqjudy.top/gtsonndxjk.html

JS:   process.env.HOME
来源：http://hz.ivvv.top/gtyyrhycbf.html

TS:   process.env.HOME
来源：http://hz.bjfxy.top/gtiiybbbri.html

Java: System.getenv("HOME")
来源：http://hz.jyoumei.cn/gtduvhijgg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gogol.net.cn/gtrbcomlnw.html

Ruby: ENV["HOME"]
来源：http://hz.ivvv.top/gtjgzynvsh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.daxiang520.top/gtbxidgdvp.html

[M03] 执行外部命令
来源：http://hz.jinqigfzy.top/gtmreuvafl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.chenzaomai.com/gtxmcklzae.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.chenlongwang.top/gthqxgkugh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.mhx1999.top/gtozvqlrct.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cheryme.top/gtlfzlaciy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.birdmap.top/gtlktoocvv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shuidangran.top/gtupmfbwdv.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.fzhhl.top/gtynqypurb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinqigufen.top/gtwdtfrjcp.html

[M04] 获取当前工作目录
来源：http://hz.cdnleiting.top/gtwzlnqfpn.html

Py:   os.getcwd()
来源：http://hz.smart0.xyz/gtqrkhkqik.html

PHP:  getcwd();
来源：http://hz.wangshuangyany.cn/gthgtbnero.html

JS:   process.cwd()
来源：http://hz.smart0.xyz/gtpnowkprd.html

TS:   process.cwd()
来源：http://hz.jinghuilouyu.cn/gtjzdfxvld.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.kuanghao11.cn/gtdgwezxjz.html

Go:   os.Getwd()
来源：http://hz.yuanzhike.top/gtimpicaal.html

Ruby: Dir.pwd
来源：http://hz.meibo888.top/gtxcuweddc.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.haohaochexian.top/gtlblobcyi.html

[M05] 设置退出码
来源：http://hz.hywenlv.cn/gtiqyjrdrh.html

Py:   sys.exit(1)
来源：http://hz.jinqigufen.top/gtaikjvmin.html

PHP:  exit(1);
来源：http://hz.svipenyu.cn/gtdemzlgic.html

JS:   process.exit(1)
来源：http://hz.yanxiufei.cn/gtpwmcbhou.html

TS:   process.exit(1)
来源：http://hz.cdnleiting.top/gtbhypkosa.html

Java: System.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtyqevyiop.html

Go:   os.Exit(1)
来源：http://hz.xuanzx.com/gtltfydxul.html

Ruby: exit 1
来源：http://hz.zhengqikj.top/gtcglocxkb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sysykeji.top/gtjrboyxhs.html

[M06] 向标准错误输出
来源：http://hz.hywenlv.cn/gtzrkvycwl.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xziqi.cn/gtrvxsmlcc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhongyouzk.top/gtfcuaonzx.html

JS:   console.error("err")
来源：http://hz.yj20258.top/gtcegbublt.html

TS:   console.error("err")
来源：http://hz.shanyushiyangtech.top/gttpnztimj.html

Java: System.err.println("err")
来源：http://hz.hnqzz.top/gtdpjwjpmb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xinyue.icu/gteturwtkb.html

Ruby: warn "err"
来源：http://hz.aizwys.cn/gtohcwemsl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.snrcjt.cn/gthykrvvnj.html

[M07] 判断是否为主入口
来源：http://hz.hywenlv.cn/gtrjjovltc.html

Py:   if __name__ == "__main__":
来源：http://hz.ydjk.org.cn/gtqeshthog.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.wangshuangyany.cn/gtdsmjlhby.html

JS:   require.main === module
来源：http://hz.chenjidiqi.icu/gtcwpjngcr.html

TS:   require.main === module
来源：http://hz.cheryme.top/gthxfyepru.html

Java: public static void main(String[] args)
来源：http://hz.316326.xyz/gtrklkpyvu.html

Go:   func main()
来源：http://hz.hysaishi.cn/gttehviggb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.chenzaomai.com/gtzhylpihm.html

C#:   static void Main(string[] args)
来源：http://hz.gaohongyu789.top/gtaltluptq.html

[M08] 获取系统与运行时信息
来源：http://hz.quarkkingdee.top/gtajdyhqsv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ehwqpu.com/gtvdrjngmn.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.9152youxi.cn/gtlwhhsnxe.html

JS:   process.platform;  process.version
来源：http://hz.dianchejie.cn/gtyncpagua.html

TS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtpwcpjhzx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinghuilouyu.cn/gtarhpaxaf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gzhubu.top/gtvcgynjxe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jqgufenzy.top/gtiyqbihpc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.gotoacloud.top/gtlhnezzqx.html

================================================================================
来源：http://hz.haohaochexian.top/gtwblxxrvf.html

N. 数据结构与算法
来源：http://hz.gogol.net.cn/gtuduheovc.html

================================================================================
来源：http://hz.jianghu66.top/gtjezmzsot.html

[N01] 二分查找（有序数组）
来源：http://hz.xuanzx.com/gtuppjowdx.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ppjwa.cn/gtgmhvkwfv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hongshengwenyu.top/gtjsttynwb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigfzy.top/gtxyjyvulr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnxiangtu.top/gtwkqneymh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.svipenyu.cn/gthvzfqlqg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.wangshuangyany.cn/gtxigmkbas.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhongyouzk.top/gtvhzbjalw.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinghuilouyu.cn/gtweizdfvt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ybcxt.top/gtyzciudzl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.haohaochexian.top/gtehstmooz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nanxuanxn.top/gtprhddyze.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aibaodan.cn/gtsyuqzkju.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cheryme.top/gtydhumzgw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hongshengwenyu.top/gtfhclctor.html

Go:   slices.Sort(arr)
来源：http://hz.c1oappe.top/gtqemqjixo.html

Ruby: arr.sort
来源：http://hz.0kj1m.cn/gtdfgunetb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.smart0.xyz/gtopchoxmr.html

[N03] 快速排序（分治示例）
来源：http://hz.yueranfly.top/gtescrwhbx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jianghu66.top/gttqezdefa.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yj20258888.top/gtyffjajpu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.52xcode.cn/gtcrakddlb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.0kj1m.cn/gtuwifcdqo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhijiandao.cn/gtdrtnzffr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.snrcjt.cn/gtubuoekem.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.iojbl.cn/gtzuxehwlj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xingfuxueyuan.xyz/gtzichicky.html

[N04] 斐波那契数列
来源：http://hz.c1oappe.top/gtserhfans.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tian-w.cn/gtvfbouwlk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shanyushiyangkeji.top/gtwzoxcmlj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pycfn.com/gtwatlmrae.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gotoacloud.top/gtmeptqauv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zdqjudy.top/gtivfstxmp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.daria6918.cn/gtobvrmfgb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhiwuduotai.top/gtelkrkfaf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ppjwa.cn/gtqtklpjxv.html

[N05] 最大公约数
来源：http://hz.shuidangran.top/gtuveebhxa.html

Py:   math.gcd(a, b)
来源：http://hz.ywan-chungtsiang.top/gthkbjqkun.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.aibaodan.cn/gtelynlmeb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cucudq.cn/gtfftwmdae.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangshuangyany.cn/gtnkitbynv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hnqzz.top/gtrrybtsqa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yj20258.top/gtubamkete.html

Ruby: a.gcd(b)
来源：http://hz.svipenyu.cn/gtqpmdwlut.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gotoacloud.top/gtwbcoatfn.html

[N06] 判断回文字符串
来源：http://hz.yuanzhike.top/gtplabcaql.html

Py:   s == s[::-1]
来源：http://hz.yanxiufei.cn/gtspaemtkx.html

PHP:  $s === strrev($s);
来源：http://hz.daxiang520.top/gtjrdgjcuk.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sysykeji.top/gttyvnmkie.html

TS:   s === [...s].reverse().join("")
来源：http://hz.52xcode.cn/gtdzzpjuba.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.gzhubu.top/gtdgbreiqi.html

Go:   // 双指针从两端比较
来源：http://hz.gogol.net.cn/gtulghqwng.html

Ruby: s == s.reverse
来源：http://hz.fengsongda.top/gtqsbxzjgw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hysaishi.cn/gtuoaymrza.html

[N07] 两数之和（返回下标）
来源：http://hz.tanke756.top/gtykdnrxrw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gotoacloud.top/gtlfodiqzp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhongyouzk.top/gtfkjxxtvn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.pengpengdd.cyou/gttlrkiysv.html

TS:   // 手写 Map<string, number>
来源：http://hz.shanyushiyangkeji.top/gthgnxyabr.html

Java: // 手写 HashMap
来源：http://hz.aizwys.cn/gtnuyxrxjk.html

Go:   // 手写 map[int]int
来源：http://hz.daxiang520.top/gtieomlcjq.html

Ruby: // 手写 Hash
来源：http://hz.hongshengwenyu.top/gtjnkfzwoj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.bjfxy.top/gtkbszkytx.html

[N08] 生成全排列
来源：http://hz.hywenlv.cn/gtgffmaafq.html

Py:   itertools.permutations(arr)
来源：http://hz.aibaodan.cn/gttrvcjpaw.html

PHP:  // 手写递归交换
来源：http://hz.zhengqikj.top/gtiosbxqpc.html

JS:   // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtsxjvhbty.html

TS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtkmuxfenv.html

Java: // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtjhnlfanb.html

Go:   // 手写回溯递归
来源：http://hz.sxryk.cn/gtiadpmfsd.html

Ruby: arr.permutation.to_a
来源：http://hz.zhongyouzk.top/gtohuigffn.html

C#:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtajzqzsnp.html

[N09] 栈与队列
来源：http://hz.zhongyouzk.top/gtjzkdocma.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zycfv.cn/gtwjaeumwd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hammf.cn/gtjiosftuu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.52xcode.cn/gtnotfqdcu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hysaishi.cn/gthmtoemtq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.birdmap.top/gtdaetvvyd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hnxiangtu.top/gtuvxqdhjs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.guowangkeji.top/gtuhuhpudb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.sxryk.cn/gtxienmztq.html

[N10] 链表节点定义
来源：http://hz.zhiwuduotai.top/gtzibypbhe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yuanzhike.top/gtxdwlisfa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.bjfxy.top/gtykfqezey.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yangfankeji.com/gtfjovuixt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shanyushiyangkeji.top/gtmafwihcf.html

Java: class Node { int v; Node next; }
来源：http://hz.jinyuanbaomall.cn/gtyxvjkecm.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.kuanghao11.cn/gtbkkmxkwj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.mhx1999.top/gtxwkexudd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shanyushiyangtech.top/gtizmaihjd.html

[N11] 二叉树中序遍历
来源：http://hz.jinghuilouyu.cn/gtmsencjmr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xingfuxueyuan.xyz/gtvyfahafp.html

PHP:  // 手写递归函数
来源：http://hz.nanxinkj.top/gtlbxbmkyj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.haohaochexian.top/gtpnpwgpkk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhoulong.xyz/gtfzcpvfog.html

Java: // 手写递归
来源：http://hz.jlsjyb.cn/gtormqbvaa.html

Go:   // 手写递归
来源：http://hz.chenzaomai.com/gtupyprtyz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yangfankeji.com/gtujvigbyg.html

C#:   // 手写递归
来源：http://hz.jqgfzy.top/gtdaggpadg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.daxiang520.top/gtypxfktgp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.9152youxi.cn/gtomjefftb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cqqwz.cn/gtaddpairh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ppjwa.cn/gtgajlxrwy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yanxiufei.cn/gtrkdafatr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guowangkeji.top/gttpkvbdyh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xziqi.cn/gtqiyxfemp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.havefunace.top/gttulvxwnp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yvedp.cn/gtlsbzdgje.html

================================================================================
来源：http://hz.mhx1999.top/gtsnwsojft.html

O. 并发与异步
来源：http://hz.snrcjt.cn/gtbdmqdfqh.html

================================================================================
来源：http://hz.jqgufenzy.top/gtteogaxhn.html

[O01] 启动一个线程
来源：http://hz.jinqigfzy.top/gtitihfyri.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.guowangkeji.top/gtmvecmxgt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jyoumei.cn/gtdyhbculj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenjidiqi.icu/gtteosjjjq.html

TS:   // 同 JS
来源：http://hz.hammf.cn/gtekgwrstr.html

Java: new Thread(() -> f()).start()
来源：http://hz.tian-w.cn/gtwhpltjcx.html

Go:   go f()
来源：http://hz.gogol.net.cn/gtnybaymou.html

Ruby: Thread.new { f }
来源：http://hz.feifeiyinyue.top/gtstulhunw.html

C#:   Task.Run(() => F());
来源：http://hz.jinghuilouyu.cn/gtqtqcrmbn.html

[O02] 使用线程池
来源：http://hz.feifeiyinyue.top/gtjldbdsza.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yonumen.top/gtaehdgxfj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nanxinkj.top/gtmcuwgnfq.html

JS:   // worker_threads 线程池
来源：http://hz.smart0.xyz/gtthgvmqxv.html

TS:   // worker_threads 线程池
来源：http://hz.fengsongda.top/gtrejrqdfi.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhoulong.xyz/gtmtnevdsy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shanyushiyangkeji.top/gthiryjiqm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zycfv.cn/gtsaybsscg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yj20258.top/gtpusizeeo.html

[O03] 加锁保护共享数据
来源：http://hz.xuetiantiany.cn/gtnpttcqvg.html

Py:   with lock: shared += 1
来源：http://hz.shuidangran.top/gtwoakqprb.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zdqjudy.top/gtrdpfawcq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.aizwys.cn/gtwbgqvffo.html

TS:   // 同 JS
来源：http://hz.tian-w.cn/gtskrdrpyt.html

Java: synchronized (this) { shared++; }
来源：http://hz.zdqjudy.top/gtpdmistwc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.chenlongwang.top/gtvszndobr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zdqjudy.top/gtvgbwcvgt.html

C#:   lock (gate) { shared++; }
来源：http://hz.nwbrower.top/gtzcxhppxi.html

[O04] 定义异步函数并等待
来源：http://hz.quarkkingdee.top/gtppqkzlss.html

Py:   async def f():⏎    await g()
来源：http://hz.yonumen.top/gtpgxmmdqm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jyoumei.cn/gtfwvwhodc.html

JS:   async function f() { await g(); }
来源：http://hz.yj202588.top/gtzpwomrsy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xuetiantiany.cn/gtlbfmzuzy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cqqwz.cn/gtgtiddvxb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.kuanghao11.cn/gtjegaxtqa.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.tanke756.top/gtcmzzvlrm.html

C#:   async Task F() { await G(); }
来源：http://hz.nanxuanxn.top/gtaixrenru.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhaomingkeji.xyz/gtcmbwhhjx.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gzhubu.top/gthqbatykp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hnqzz.top/gtigoeognt.html

JS:   await Promise.all(tasks)
来源：http://hz.zycfv.cn/gtdyoovfgd.html

TS:   await Promise.all(tasks)
来源：http://hz.smart0.xyz/gtujksmvvi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ybcxt.top/gtdgusmofj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shanyushiyangtech.top/gtttdmoman.html

Ruby: threads.map(&:join)
来源：http://hz.zhijiandao.cn/gtlwknzrmd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ppjwa.cn/gtsdotrlpv.html

[O06] 使用进程池
来源：http://hz.yuxming.cn/gtxfhvbhes.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.iojbl.cn/gtmfgobmaa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yonumen.top/gtknekizsn.html

JS:   // child_process / cluster 模块
来源：http://hz.gogol.net.cn/gtfrduytim.html

TS:   // child_process / cluster 模块
来源：http://hz.fengsongda.top/gtkrdbbwbw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.svipenyu.cn/gtolvxqyov.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.smart0.xyz/gtuzflxlse.html

Ruby: // fork 块
来源：http://hz.iojbl.cn/gtjoescwaa.html

C#:   Parallel.For
来源：http://hz.smart0.xyz/gtjbrnhuuh.html

================================================================================
来源：http://hz.shzxlz.cn/gtugjtkexd.html

P. 常用工具函数
来源：http://hz.gogol.net.cn/gthwszpmkw.html

================================================================================
来源：http://hz.jyoumei.cn/gtfqerzwea.html

[P01] 生成 UUID
来源：http://hz.pycfn.com/gtsvbhsjxr.html

Py:   str(uuid.uuid4())
来源：http://hz.gzhubu.top/gtelsnwnxt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.iojbl.cn/gtbpkbeqlu.html

JS:   crypto.randomUUID()
来源：http://hz.xingfuxueyuan.xyz/gtxgoohpzi.html

TS:   crypto.randomUUID()
来源：http://hz.zhixingplan.top/gtyellnrbd.html

Java: UUID.randomUUID().toString()
来源：http://hz.hfpthk.cn/gtxhrhapcb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.pycfn.com/gtdqppmjsg.html

Ruby: SecureRandom.uuid
来源：http://hz.shanyushiyangtech.top/gteddrkfvb.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.daria6918.cn/gtdosllmin.html

[P02] MD5 / SHA256 摘要
来源：http://hz.andypj.xyz/gtcietxtsf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhengqikj.top/gteftofdhp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yonumen.top/gtavsncuch.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yueranfly.top/gtfzbtbhxb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shanyushiyangtech.top/gtklvriqcz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.nanxinkj.top/gtjlszdhxb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhaomingkeji.xyz/gtpvgltiac.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.daxiang520.top/gttgvnqdfk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.c1oappe.top/gtrpwxuanx.html

[P03] 生成短随机字符串
来源：http://hz.hammf.cn/gtgibkkzoi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.pengpengdd.cyou/gtajyzmjds.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.redwolf501.top/gtjcyonsle.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnqzz.top/gtzbaylvdl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhixingplan.top/gtupuknojp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.nwbrower.top/gthcrljdqv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.bjfxy.top/gtwsztmkkc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shzxlz.cn/gtefcwlsqr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xingfuxueyuan.xyz/gtqcjviwhs.html

[P04] 求长度
来源：http://hz.gotoacloud.top/gtjkhpueys.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shzxlz.cn/gtftnowhth.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gtmzmkdptz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.mhx1999.top/gtndvkwoll.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shzxlz.cn/gtecoojxdh.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jlsjyb.cn/gtmpjbidfx.html

Go:   len(arr);  len(m)
来源：http://hz.yvedp.cn/gtwgpzaxwr.html

Ruby: x.length;  x.size
来源：http://hz.jinghuilouyu.cn/gtsatfeusx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shuidangran.top/gtixzczivc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.dashuyun.cn/gtpfjghmbn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hnqzz.top/gtfnmoutoc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.quarkkingdee.top/gtnnkabykb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hammf.cn/gtytjvapsq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yuxming.cn/gtrcjggzxb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yueranfly.top/gtwnrnfvss.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.sufxvd.cn/gtuzmsilql.html

Ruby: a == b
来源：http://hz.tanke756.top/gtjpoxqxjm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cqqwz.cn/gtpfxrazaf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.pycfn.com/gthcxldslb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.sweek.top/gtfwhfwusa.html

PHP:  if (empty($x)) {}
来源：http://hz.ydjk.org.cn/gtjlsnqrmg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinyuanbaomall.cn/gtuojrgsda.html

TS:   if (x == null) {}
来源：http://hz.jiagoushi.top/gtotscgucq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jinqigfzy.top/gtbihhhypx.html

Go:   if x == nil {}
来源：http://hz.zhixingplan.top/gtwmhfkvsq.html


<!-- 参考信息 -->