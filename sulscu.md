代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cashguo.top/gtjkjsggwc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ybcxt.top/gtvamjukuc.html

================================================================================
来源：http://hz.gotoacloud.top/gtwllfuggl.html

M. 命令行 / 进程 / 环境
来源：http://hz.c1oappe.top/gtduywpsfu.html

================================================================================
来源：http://hz.sxryk.cn/gtpwmfpacb.html

[M01] 读取命令行参数
来源：http://hz.ydzc1.top/gtfrnewybl.html

Py:   sys.argv[1:]
来源：http://hz.ivvv.top/gtxrehhbyz.html

PHP:  $argv;  $argc;
来源：http://hz.shzxlz.cn/gtynuxdrwa.html

JS:   process.argv.slice(2)
来源：http://hz.9152youxi.cn/gtnqsgnzgf.html

TS:   process.argv.slice(2)
来源：http://hz.ydzc1.top/gtwokizphk.html

Java: args 数组（main 方法参数）
来源：http://hz.gzhubu.top/gtsfgcokcs.html

Go:   os.Args[1:]
来源：http://hz.quarkkingdee.top/gtnttztebw.html

Ruby: ARGV
来源：http://hz.ybcxt.top/gtrbwjpmsx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shuidangran.top/gtxfdgaasn.html

[M02] 读取环境变量
来源：http://hz.shanyushiyangkeji.top/gtdqeusiha.html

Py:   os.environ.get("HOME")
来源：http://hz.guowangkeji.top/gtvwxxdcyu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.haohaochexian.top/gtspcgaixs.html

JS:   process.env.HOME
来源：http://hz.havefunace.top/gtavtsbbol.html

TS:   process.env.HOME
来源：http://hz.gogol.net.cn/gtrrrefqde.html

Java: System.getenv("HOME")
来源：http://hz.yj202588.top/gtiradstnp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.dianchejie.cn/gttegfosor.html

Ruby: ENV["HOME"]
来源：http://hz.bjfxy.top/gthwmwlsxw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.wangdashe.top/gtawldumeh.html

[M03] 执行外部命令
来源：http://hz.zhijiandao.cn/gttxpqoome.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hongshengwenyu.top/gtiufoydhx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.wangshuangyany.cn/gtqfyzsbxe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ehwqpu.com/gtxviwrmzg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xziqi.cn/gtlfvjoggp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.aibaodan.cn/gtcbmcdmfq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.feifeiyinyue.top/gtfuuvhqnh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhengqikj.top/gtojumtqdt.html

C#:   Process.Start("ls", "-l");
来源：http://hz.kuanghao11.cn/gtwasydvbj.html

[M04] 获取当前工作目录
来源：http://hz.sweek.top/gtedqwkyqk.html

Py:   os.getcwd()
来源：http://hz.svipenyu.cn/gtfijgjjgp.html

PHP:  getcwd();
来源：http://hz.mhx1999.top/gtnmjvyfyy.html

JS:   process.cwd()
来源：http://hz.pycfn.com/gtojwmltey.html

TS:   process.cwd()
来源：http://hz.jiagoushi.top/gtdcwhdibf.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hnxiangtu.top/gtlzlsgfki.html

Go:   os.Getwd()
来源：http://hz.xinyue.icu/gttptkvjcf.html

Ruby: Dir.pwd
来源：http://hz.sxryk.cn/gtvsoviiox.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sweek.top/gtimdskpcu.html

[M05] 设置退出码
来源：http://hz.yj202588.top/gtpmwlbczo.html

Py:   sys.exit(1)
来源：http://hz.sysykeji.top/gtxqunzsty.html

PHP:  exit(1);
来源：http://hz.chenlongwang.top/gtitwghavv.html

JS:   process.exit(1)
来源：http://hz.vqdsnc.cn/gtfizgjrip.html

TS:   process.exit(1)
来源：http://hz.sufxvd.cn/gtnpudufib.html

Java: System.exit(1)
来源：http://hz.xuetiantiany.cn/gtlnjokqjr.html

Go:   os.Exit(1)
来源：http://hz.hnxiangtu.top/gtfhupqfqp.html

Ruby: exit 1
来源：http://hz.hywenlv.cn/gtubcvnrdg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sxryk.cn/gtksswjsts.html

[M06] 向标准错误输出
来源：http://hz.jiagoushi.top/gtrdjttrch.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yanxiufei.cn/gtisbybdse.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhengqikj.top/gtscuygevy.html

JS:   console.error("err")
来源：http://hz.zhongyouzk.top/gtakuzivba.html

TS:   console.error("err")
来源：http://hz.daria6918.cn/gttikkozdx.html

Java: System.err.println("err")
来源：http://hz.wangdashe.top/gtaqxhkglj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xziqi.cn/gtnfinhbws.html

Ruby: warn "err"
来源：http://hz.sufxvd.cn/gtneevdipi.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cdnleiting.top/gtmjfuylqa.html

[M07] 判断是否为主入口
来源：http://hz.nanxinkj.top/gttskinkpp.html

Py:   if __name__ == "__main__":
来源：http://hz.c1oappe.top/gtzmcpujcr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yuxming.cn/gtjfhmdrrn.html

JS:   require.main === module
来源：http://hz.chenzaomai.com/gttdceqyvq.html

TS:   require.main === module
来源：http://hz.jqgufenzy.top/gtoystmpqk.html

Java: public static void main(String[] args)
来源：http://hz.aibaodan.cn/gtjbbbxent.html

Go:   func main()
来源：http://hz.yj202588.top/gtgkkmnbne.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xuetiantiany.cn/gtkofioarw.html

C#:   static void Main(string[] args)
来源：http://hz.ehwqpu.com/gtclpbpdsc.html

[M08] 获取系统与运行时信息
来源：http://hz.ybcxt.top/gtmogqpvri.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cheryme.top/gtdjszbgek.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.pengpengdd.cyou/gtvscasxao.html

JS:   process.platform;  process.version
来源：http://hz.yj20258888.top/gtcvbktuku.html

TS:   process.platform;  process.version
来源：http://hz.xinyue.icu/gthuzltsds.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zycfv.cn/gtyaarfiaq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhaomingkeji.xyz/gthzvncxtd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.birdmap.top/gtuignavub.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shzxlz.cn/gtudjbwkpn.html

================================================================================
来源：http://hz.yongpay.top/gtobzvrhtd.html

N. 数据结构与算法
来源：http://hz.sweek.top/gtovtflawt.html

================================================================================
来源：http://hz.gogol.net.cn/gtozuneoeu.html

[N01] 二分查找（有序数组）
来源：http://hz.yvedp.cn/gtcjihccqw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.smart0.xyz/gtzuqdxyfj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.vqdsnc.cn/gtnzjfwmrh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yonumen.top/gtmynivith.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yvedp.cn/gtzgryfpsn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hywenlv.cn/gtlqmusvbt.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.aizwys.cn/gtvurpwuqm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.cqqwz.cn/gtotmxcvwj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.tian-w.cn/gtovwsfemw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.daria6918.cn/gtnjqiryty.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.kuanghao11.cn/gtbktpjdfl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hfpthk.cn/gtorsmpdsk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinghuilouyu.cn/gtqikdzgsu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtpvskhett.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sxryk.cn/gtitjjxaeg.html

Go:   slices.Sort(arr)
来源：http://hz.zhijiandao.cn/gtmkwqinat.html

Ruby: arr.sort
来源：http://hz.jyoumei.cn/gtpwekogzv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.birdmap.top/gtcnvwxpqm.html

[N03] 快速排序（分治示例）
来源：http://hz.chenzaomai.com/gtjrlqlrox.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cdnleiting.top/gtvjvqkuvb.html

PHP:  // 递归实现，或用 usort
来源：http://hz.kuanghao11.cn/gtozvrdjiq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aizwys.cn/gtajtnkslm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj20258888.top/gtdzefidhn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tian-w.cn/gtrkclqlrw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.kuanghao11.cn/gtmczsshvw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yanxiufei.cn/gtxymanloh.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.quarkkingdee.top/gtetdvtijz.html

[N04] 斐波那契数列
来源：http://hz.gogol.net.cn/gtsmyaxzci.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.iojbl.cn/gthrhsorpo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.bjfxy.top/gthaxxkyce.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigufen.top/gtfykxrvrw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xuanzx.com/gtzyhvmpgx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.chenjidiqi.icu/gtynnhoofl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jiagoushi.top/gtpisfucbl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.316326.xyz/gtxdsphbwq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.dashuyun.cn/gtpxzqzwxu.html

[N05] 最大公约数
来源：http://hz.xuanzx.com/gtnbhrpayd.html

Py:   math.gcd(a, b)
来源：http://hz.zhongyouzk.top/gtwaechhxg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinqigfzy.top/gtnsgkbznz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pycfn.com/gtbfxzzzgc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.vqdsnc.cn/gtkwttrjks.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hnxiangtu.top/gtxmswiuvl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.gaohongyu789.top/gtcfecxumn.html

Ruby: a.gcd(b)
来源：http://hz.hnxiangtu.top/gtdvnfbsec.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ehwqpu.com/gtcezlrrpw.html

[N06] 判断回文字符串
来源：http://hz.hywenlv.cn/gtensojnoa.html

Py:   s == s[::-1]
来源：http://hz.cucudq.cn/gtgvlrdaxv.html

PHP:  $s === strrev($s);
来源：http://hz.gzhubu.top/gttjwhgata.html

JS:   s === [...s].reverse().join("")
来源：http://hz.nanxinkj.top/gtjomvwqgq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.c1oappe.top/gtdmrvmliw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sxryk.cn/gtglbwzwnx.html

Go:   // 双指针从两端比较
来源：http://hz.feifeiyinyue.top/gtqiraliod.html

Ruby: s == s.reverse
来源：http://hz.shanyushiyangkeji.top/gtdgossiws.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xziqi.cn/gtxcjoybri.html

[N07] 两数之和（返回下标）
来源：http://hz.gogol.net.cn/gtnebpeopp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.guannengcc.top/gtkaitzeti.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.tianlin.xyz/gtxjfywrta.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hywenlv.cn/gtxpdkxbww.html

TS:   // 手写 Map<string, number>
来源：http://hz.yueranfly.top/gtjnelxoyq.html

Java: // 手写 HashMap
来源：http://hz.yuanzhike.top/gtkujtmxtd.html

Go:   // 手写 map[int]int
来源：http://hz.ywan-chungtsiang.top/gtwkeovbxd.html

Ruby: // 手写 Hash
来源：http://hz.andypj.xyz/gtceuhmqgv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhaomingkeji.xyz/gtepgygobc.html

[N08] 生成全排列
来源：http://hz.xylfe.cn/gteobcdggx.html

Py:   itertools.permutations(arr)
来源：http://hz.gotoacloud.top/gtxchayvst.html

PHP:  // 手写递归交换
来源：http://hz.iojbl.cn/gtooimoxpu.html

JS:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtanmmxnnd.html

TS:   // 手写回溯递归
来源：http://hz.sysykeji.top/gtesjoopkb.html

Java: // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtsgyscluj.html

Go:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtodwnotfh.html

Ruby: arr.permutation.to_a
来源：http://hz.hammf.cn/gtuikhxhet.html

C#:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtlgllffmu.html

[N09] 栈与队列
来源：http://hz.wangshuangyany.cn/gtwojxhoag.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xuetiantiany.cn/gtgxckwfpf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.havefunace.top/gtboiojjrf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ehwqpu.com/gtstbfwumk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhixingplan.top/gtjfwsmqyj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yj20258.top/gtlmjcjazr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ydjk.org.cn/gtefwoxzqy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.haohaochexian.top/gtonbwqrkr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xziqi.cn/gtuhjbekyb.html

[N10] 链表节点定义
来源：http://hz.mhx1999.top/gtmzspwghj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.guannengcc.top/gtztdwtnmf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhiwuduotai.top/gtflbvwnfv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ydzc1.top/gtoukstnrc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sysykeji.top/gtyglwyaby.html

Java: class Node { int v; Node next; }
来源：http://hz.0kj1m.cn/gtnkvdnmjl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.wangshuangyany.cn/gtmfsjzflp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hongshengwenyu.top/gtewwzibgp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.bjfxy.top/gtwseveqds.html

[N11] 二叉树中序遍历
来源：http://hz.havefunace.top/gtviygdtiy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.daxiang520.top/gttdxfocyn.html

PHP:  // 手写递归函数
来源：http://hz.52xcode.cn/gtukmfxjcp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yangfankeji.com/gtzaghqsjc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhoulong.xyz/gtlyihyhxv.html

Java: // 手写递归
来源：http://hz.jqgufenzy.top/gtikjinoau.html

Go:   // 手写递归
来源：http://hz.zhixingplan.top/gtqrvmekux.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hammf.cn/gtzshzpfkz.html

C#:   // 手写递归
来源：http://hz.zhengqikj.top/gtajqauotc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.c1oappe.top/gtlnytzbay.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.9152youxi.cn/gtuuyvyvbr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.daxiang520.top/gteyqrhqie.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tianlin.xyz/gtjgolllwo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydzc1.top/gtoixxembh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sweek.top/gtihvikqcj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhaomingkeji.xyz/gtleqplbeg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.smart0.xyz/gthtijtkfq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sxryk.cn/gtqguwvlea.html

================================================================================
来源：http://hz.jiagoushi.top/gtlsnyujhn.html

O. 并发与异步
来源：http://hz.pycfn.com/gttsdlyzvf.html

================================================================================
来源：http://hz.sxryk.cn/gtjuqixisr.html

[O01] 启动一个线程
来源：http://hz.yj20258.top/gtpobhtmut.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yueranfly.top/gtfciujtgh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ydjk.org.cn/gtxeprvcvc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cqqwz.cn/gtmhivtwwh.html

TS:   // 同 JS
来源：http://hz.yj20258888.top/gtmhhzxxob.html

Java: new Thread(() -> f()).start()
来源：http://hz.andypj.xyz/gtodmpxrpu.html

Go:   go f()
来源：http://hz.mhx1999.top/gtndtzrhva.html

Ruby: Thread.new { f }
来源：http://hz.ehwqpu.com/gtoknlgqmx.html

C#:   Task.Run(() => F());
来源：http://hz.9152youxi.cn/gtfbxaadxl.html

[O02] 使用线程池
来源：http://hz.zhongyouzk.top/gtkgwaxilw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.9152youxi.cn/gtzktdbwsb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.vqdsnc.cn/gtsrlzisjp.html

JS:   // worker_threads 线程池
来源：http://hz.cdnleiting.top/gtkzlknjhm.html

TS:   // worker_threads 线程池
来源：http://hz.shanyushiyangtech.top/gtfylwleac.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.havefunace.top/gtzffhpple.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.mhx1999.top/gtiszdsncm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yueranfly.top/gtuolhegfs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shanyushiyangkeji.top/gtvyqnpurz.html

[O03] 加锁保护共享数据
来源：http://hz.xuanzx.com/gtuzowfcju.html

Py:   with lock: shared += 1
来源：http://hz.daxiang520.top/gtalcembxw.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xziqi.cn/gtctlsovsw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.sxryk.cn/gteqeluetd.html

TS:   // 同 JS
来源：http://hz.ydzc1.top/gtstgskdeg.html

Java: synchronized (this) { shared++; }
来源：http://hz.mhx1999.top/gtegnvblpw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hysaishi.cn/gtcqrxqxql.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zdqjudy.top/gtsuuzrreu.html

C#:   lock (gate) { shared++; }
来源：http://hz.quarkkingdee.top/gtqtobbudb.html

[O04] 定义异步函数并等待
来源：http://hz.fengsongda.top/gtzqsiqlio.html

Py:   async def f():⏎    await g()
来源：http://hz.cucudq.cn/gtjsdvxoio.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shangyingyoupin.top/gtuxwxyuwc.html

JS:   async function f() { await g(); }
来源：http://hz.smart0.xyz/gtcsoudoxk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.nwbrower.top/gtmymyuvxl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jiagoushi.top/gtblaljoak.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.aizwys.cn/gttcluilio.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shanyushiyangkeji.top/gtgksbqtxk.html

C#:   async Task F() { await G(); }
来源：http://hz.zhaomingkeji.xyz/gtopudgsxw.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhaomingkeji.xyz/gtxxcuslmh.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yanxiufei.cn/gtpzidrqbu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cqqwz.cn/gttlhlodcq.html

JS:   await Promise.all(tasks)
来源：http://hz.jinqigufen.top/gtzjewzkiz.html

TS:   await Promise.all(tasks)
来源：http://hz.wangdashe.top/gtsyyfvjpg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hnqzz.top/gtmsqdrcyj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xinyue.icu/gttgydcxqh.html

Ruby: threads.map(&:join)
来源：http://hz.yj20258888.top/gtxyvefhkx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.iojbl.cn/gtughhqhle.html

[O06] 使用进程池
来源：http://hz.0kj1m.cn/gtwgtpapoc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.chenzaomai.com/gtngejmqnc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shzxlz.cn/gtdykoelnf.html

JS:   // child_process / cluster 模块
来源：http://hz.yonumen.top/gtvnzirqqe.html

TS:   // child_process / cluster 模块
来源：http://hz.9152youxi.cn/gthwvrnxwd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cucudq.cn/gtjtvcdyra.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shanyushiyangtech.top/gtndgzajip.html

Ruby: // fork 块
来源：http://hz.gaohongyu789.top/gtctcaznlq.html

C#:   Parallel.For
来源：http://hz.bjfxy.top/gtucodsbhl.html

================================================================================
来源：http://hz.sxryk.cn/gtqjumnzfz.html

P. 常用工具函数
来源：http://hz.sysykeji.top/gtkolzvobm.html

================================================================================
来源：http://hz.svipenyu.cn/gtnxteisvp.html

[P01] 生成 UUID
来源：http://hz.haohaochexian.top/gtkmifbosx.html

Py:   str(uuid.uuid4())
来源：http://hz.dianchejie.cn/gtvzleexht.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gotoacloud.top/gtmozwusiu.html

JS:   crypto.randomUUID()
来源：http://hz.tian-w.cn/gtlseomway.html

TS:   crypto.randomUUID()
来源：http://hz.birdmap.top/gtfwpxwsmi.html

Java: UUID.randomUUID().toString()
来源：http://hz.yvedp.cn/gtrolpbkvw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj20258888.top/gtwlmdoivg.html

Ruby: SecureRandom.uuid
来源：http://hz.zhengqikj.top/gtrojutcbm.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.nwbrower.top/gtekcayhdz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hywenlv.cn/gtlpqotbrz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhongyouzk.top/gtyzyzjsnf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shuidangran.top/gtgoftflwe.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.wangdashe.top/gtfqgceqca.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xingfuxueyuan.xyz/gtnxgtcmte.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.haohaochexian.top/gtykpezyxh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.kuanghao11.cn/gtakaoncuv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.52xcode.cn/gtfnwgodxc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cqqwz.cn/gtbhrnrvjn.html

[P03] 生成短随机字符串
来源：http://hz.smart0.xyz/gtiomqusbr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ydzc1.top/gtdwmptcxp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hnxiangtu.top/gtkacxpdak.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.c1oappe.top/gtfqrmggsq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tianlin.xyz/gtoskpuqkx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhoulong.xyz/gtsxpqondj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yuxming.cn/gtgszxmsip.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.feifeiyinyue.top/gtmkuwmnms.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.tianlin.xyz/gtxsyiddnc.html

[P04] 求长度
来源：http://hz.sxryk.cn/gtnacetmph.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.52xcode.cn/gtxzqdzcpo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtnqelabet.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinghuilouyu.cn/gtbwhhzbtb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangdashe.top/gtmcvrtehh.html

Java: list.size();  map.size();  s.length()
来源：http://hz.guowangkeji.top/gtzuakchva.html

Go:   len(arr);  len(m)
来源：http://hz.zhengqikj.top/gtcanmztvb.html

Ruby: x.length;  x.size
来源：http://hz.yuxming.cn/gtxvaxzfph.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cashguo.top/gtkwrvetbg.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hysaishi.cn/gtlzuvhtrn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.guowangkeji.top/gtwcvydnzb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yj20258888.top/gtlciaddwl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yj20258.top/gthyigdupj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.dianchejie.cn/gtrjwyuyyd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinqigfzy.top/gtszheigyq.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.nanxuanxn.top/gtornlbcdd.html

Ruby: a == b
来源：http://hz.jinyuanbaomall.cn/gtyshxuqep.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yvedp.cn/gtiatjdfgv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gaohongyu789.top/gtdzcawinz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shangyingyoupin.top/gtxlcbchbo.html

PHP:  if (empty($x)) {}
来源：http://hz.dianchejie.cn/gtzffxvlch.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sweek.top/gtizzbwfsd.html

TS:   if (x == null) {}
来源：http://hz.cheryme.top/gtsauwpiox.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.gzhubu.top/gtwfrypwot.html

Go:   if x == nil {}
来源：http://hz.tanke756.top/gtnickvkmn.html


<!-- 参考信息 -->