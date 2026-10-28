代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guowangkeji.top/gtkkugahtb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cheryme.top/gtslzscskx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.redwolf501.top/gtybijjxbp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shanyushiyangtech.top/gtcxcfiwkp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhijiandao.cn/gtuzvljedg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sxryk.cn/gtyjamuaam.html

================================================================================
来源：http://hz.ydzc1.top/gtrhdukulu.html

M. 命令行 / 进程 / 环境
来源：http://hz.hammf.cn/gtzmzibcqf.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtljapeebg.html

[M01] 读取命令行参数
来源：http://hz.yangfankeji.com/gtbvkzlahp.html

Py:   sys.argv[1:]
来源：http://hz.mhx1999.top/gtmyxvsxkb.html

PHP:  $argv;  $argc;
来源：http://hz.cdnleiting.top/gtksljceze.html

JS:   process.argv.slice(2)
来源：http://hz.pengpengdd.cyou/gtilhircxc.html

TS:   process.argv.slice(2)
来源：http://hz.cucudq.cn/gtjzslthwv.html

Java: args 数组（main 方法参数）
来源：http://hz.xziqi.cn/gtdwzkrlnb.html

Go:   os.Args[1:]
来源：http://hz.yj202588.top/gtwsrakvfk.html

Ruby: ARGV
来源：http://hz.mhx1999.top/gttmlowfba.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nwbrower.top/gtymlqjnwm.html

[M02] 读取环境变量
来源：http://hz.shzxlz.cn/gtsppgjgml.html

Py:   os.environ.get("HOME")
来源：http://hz.yangfankeji.com/gtuhymelgq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yj20258888.top/gtshspdzzf.html

JS:   process.env.HOME
来源：http://hz.hfpthk.cn/gtzeljcqet.html

TS:   process.env.HOME
来源：http://hz.jlsjyb.cn/gthxarprdm.html

Java: System.getenv("HOME")
来源：http://hz.pycfn.com/gtkllyizav.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yj20258.top/gtfirkmgum.html

Ruby: ENV["HOME"]
来源：http://hz.feifeiyinyue.top/gtzoycltng.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.bjfxy.top/gtwornuvcv.html

[M03] 执行外部命令
来源：http://hz.sufxvd.cn/gttdzludud.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hfpthk.cn/gtlbpekgzo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.dianchejie.cn/gtfgmptxrd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhaomingkeji.xyz/gtkafxcgpl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj20258888.top/gtifjrgejy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhoulong.xyz/gtrppavwjg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.snrcjt.cn/gtjfyhuftv.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sweek.top/gtasagwlcn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.kuanghao11.cn/gtaqqhpxdt.html

[M04] 获取当前工作目录
来源：http://hz.yueranfly.top/gtiplofmgs.html

Py:   os.getcwd()
来源：http://hz.cqqwz.cn/gttymbfbkh.html

PHP:  getcwd();
来源：http://hz.316326.xyz/gtoyfobpyc.html

JS:   process.cwd()
来源：http://hz.jqgfzy.top/gttkxxketw.html

TS:   process.cwd()
来源：http://hz.wangshuangyany.cn/gtknkkhfbo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.guannengcc.top/gtyflplvqq.html

Go:   os.Getwd()
来源：http://hz.mhx1999.top/gtpftuqrer.html

Ruby: Dir.pwd
来源：http://hz.fengsongda.top/gtzuexkxvv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.kuanghao11.cn/gtceloxctq.html

[M05] 设置退出码
来源：http://hz.52xcode.cn/gtlbivfsqi.html

Py:   sys.exit(1)
来源：http://hz.nanxuanxn.top/gthmuotbgn.html

PHP:  exit(1);
来源：http://hz.dashuyun.cn/gtqiemclgy.html

JS:   process.exit(1)
来源：http://hz.snrcjt.cn/gtouhxmpsc.html

TS:   process.exit(1)
来源：http://hz.ivvv.top/gtyfcdzbga.html

Java: System.exit(1)
来源：http://hz.pengpengdd.cyou/gtaornzlqd.html

Go:   os.Exit(1)
来源：http://hz.xziqi.cn/gtjyzsbbjf.html

Ruby: exit 1
来源：http://hz.gogol.net.cn/gtazscrkad.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shangyingyoupin.top/gtdorwbjqe.html

[M06] 向标准错误输出
来源：http://hz.hnxiangtu.top/gtfbmvusfr.html

Py:   print("err", file=sys.stderr)
来源：http://hz.meibo888.top/gtulutvzxl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jqgfzy.top/gtrvqhbykx.html

JS:   console.error("err")
来源：http://hz.tianlin.xyz/gtsdcbdcio.html

TS:   console.error("err")
来源：http://hz.shuidangran.top/gtviypktaz.html

Java: System.err.println("err")
来源：http://hz.meibo888.top/gtwubnlebb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hysaishi.cn/gtntwunpjd.html

Ruby: warn "err"
来源：http://hz.jinqigfzy.top/gtlazbjmmk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.aibaodan.cn/gtfmxzfofu.html

[M07] 判断是否为主入口
来源：http://hz.daxiang520.top/gtqmmhqfam.html

Py:   if __name__ == "__main__":
来源：http://hz.hysaishi.cn/gtydzvvpuy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.fzhhl.top/gtdvpkdhzl.html

JS:   require.main === module
来源：http://hz.jinyuanbaomall.cn/gtkmhqblnk.html

TS:   require.main === module
来源：http://hz.zhoulong.xyz/gtodxczyns.html

Java: public static void main(String[] args)
来源：http://hz.yongpay.top/gtoljyzzsi.html

Go:   func main()
来源：http://hz.zhengqikj.top/gtxjjwreoj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shangyingyoupin.top/gtnjiwjrhd.html

C#:   static void Main(string[] args)
来源：http://hz.nanxuanxn.top/gtxbxxzfyd.html

[M08] 获取系统与运行时信息
来源：http://hz.wangshuangyany.cn/gttylnoual.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cdnleiting.top/gtunruijcl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ywan-chungtsiang.top/gtfgcukiac.html

JS:   process.platform;  process.version
来源：http://hz.yj202588.top/gtpwspdrtu.html

TS:   process.platform;  process.version
来源：http://hz.gzhubu.top/gtgbeurjdh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jianghu66.top/gtgjwbwuwe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jianghu66.top/gttsohrgvk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhiwuduotai.top/gtjixxfman.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jlsjyb.cn/gtlfunnpzu.html

================================================================================
来源：http://hz.pengpengdd.cyou/gthwrymewj.html

N. 数据结构与算法
来源：http://hz.cdnleiting.top/gtabajnxfc.html

================================================================================
来源：http://hz.zhengqikj.top/gtquhccwqg.html

[N01] 二分查找（有序数组）
来源：http://hz.sufxvd.cn/gtrycchevp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yangfankeji.com/gtowvrdxvd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.meibo888.top/gtkmintmof.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xziqi.cn/gtxqbngeou.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.birdmap.top/gtsepsnkna.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.guowangkeji.top/gtedanaavd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.wangdashe.top/gtjxdemila.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.daxiang520.top/gtyjvgiqxu.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtvvqlrwgg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xuetiantiany.cn/gtjijrjlzp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zdqjudy.top/gtangnttso.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shanyushiyangtech.top/gtmkvffinf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gtuklqtlsu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhixingplan.top/gtevttzqet.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shuidangran.top/gtwimgtzba.html

Go:   slices.Sort(arr)
来源：http://hz.316326.xyz/gtklmyxoof.html

Ruby: arr.sort
来源：http://hz.hnqzz.top/gtmhtffgnk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cdnleiting.top/gtycebluyb.html

[N03] 快速排序（分治示例）
来源：http://hz.feifeiyinyue.top/gtnqtaraew.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ydjk.org.cn/gtojpguprw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.meibo888.top/gtytgisxwp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydzc1.top/gtmqzmdtjq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj20258888.top/gtxwrmmsfs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yonumen.top/gtuvelxzbo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yj202588.top/gttaoiqocj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenjidiqi.icu/gtwjqzsizx.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.smart0.xyz/gtmzxmemlw.html

[N04] 斐波那契数列
来源：http://hz.cucudq.cn/gtvqdilrnh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.316326.xyz/gtfttokxqa.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.wangdashe.top/gtpakajbbd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxinkj.top/gticjotpas.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dashuyun.cn/gtjgmelvhi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gzhubu.top/gtfcnxcuuz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gzhubu.top/gtruuzrsdn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.mhx1999.top/gttwopzcqa.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.daxiang520.top/gtaioorlic.html

[N05] 最大公约数
来源：http://hz.yuanzhike.top/gtrmsjykck.html

Py:   math.gcd(a, b)
来源：http://hz.havefunace.top/gtklyruygp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.iojbl.cn/gtbhpaxkqf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj20258888.top/gtzejxbsxk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ivvv.top/gtgqoueprv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.haohaochexian.top/gtpabdarys.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jiagoushi.top/gtvopmurum.html

Ruby: a.gcd(b)
来源：http://hz.jlsjyb.cn/gtzzdhfiqa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jiagoushi.top/gtnvkcqveb.html

[N06] 判断回文字符串
来源：http://hz.xuetiantiany.cn/gtyvdskbaz.html

Py:   s == s[::-1]
来源：http://hz.zdqjudy.top/gtvamdhira.html

PHP:  $s === strrev($s);
来源：http://hz.kuanghao11.cn/gtjeqdqhbu.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gtpcmerkxw.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtefmafytv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.havefunace.top/gtlskcpnoe.html

Go:   // 双指针从两端比较
来源：http://hz.jinqigfzy.top/gtualbmarq.html

Ruby: s == s.reverse
来源：http://hz.cdnleiting.top/gtohyrvynq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.sxryk.cn/gtnmujuekw.html

[N07] 两数之和（返回下标）
来源：http://hz.xuanzx.com/gttsrqztnc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.andypj.xyz/gtyuonitvi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hysaishi.cn/gtffdefstm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinyuanbaomall.cn/gtjxtekshd.html

TS:   // 手写 Map<string, number>
来源：http://hz.hammf.cn/gtadpcnqjp.html

Java: // 手写 HashMap
来源：http://hz.zhengqikj.top/gtnztlfwjx.html

Go:   // 手写 map[int]int
来源：http://hz.daxiang520.top/gteifopbwt.html

Ruby: // 手写 Hash
来源：http://hz.ydzc1.top/gtffzxiyng.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.svipenyu.cn/gtirexysmx.html

[N08] 生成全排列
来源：http://hz.ydzc1.top/gtbzvchzan.html

Py:   itertools.permutations(arr)
来源：http://hz.shanyushiyangkeji.top/gtdgvmyapj.html

PHP:  // 手写递归交换
来源：http://hz.jianghu66.top/gtejgnujqz.html

JS:   // 手写回溯递归
来源：http://hz.yongpay.top/gtfctqboeg.html

TS:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtwmfjawvh.html

Java: // 手写回溯递归
来源：http://hz.sufxvd.cn/gtkrbkyvrd.html

Go:   // 手写回溯递归
来源：http://hz.sweek.top/gtpjczmzvo.html

Ruby: arr.permutation.to_a
来源：http://hz.yj20258888.top/gtkyzgzkjg.html

C#:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtepawpudw.html

[N09] 栈与队列
来源：http://hz.zhoulong.xyz/gtrvogflcz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.gotoacloud.top/gtalzuakvn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xingfuxueyuan.xyz/gtftghjjpf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhoulong.xyz/gtisyspsih.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.nanxuanxn.top/gtxymbusbu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gzhubu.top/gtsagnfdcg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gzhubu.top/gtlnpomldp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.chenlongwang.top/gtwvnvgymd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhaomingkeji.xyz/gtretlfcic.html

[N10] 链表节点定义
来源：http://hz.hysaishi.cn/gtztifzcou.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhengqikj.top/gtuhfdywcr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xinyue.icu/gtxwsvadsw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.dashuyun.cn/gteutlkkab.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gotoacloud.top/gtdynjxmcg.html

Java: class Node { int v; Node next; }
来源：http://hz.iojbl.cn/gtzgzpzurb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ydzc1.top/gtyftnvbvt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.guowangkeji.top/gtjxeczdsi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hnqzz.top/gtnywvpenj.html

[N11] 二叉树中序遍历
来源：http://hz.gzhubu.top/gtpbveqwqo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sufxvd.cn/gtwgrdwtge.html

PHP:  // 手写递归函数
来源：http://hz.hfpthk.cn/gtbiavyiri.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.daxiang520.top/gtusqbiqca.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yvedp.cn/gtajbonmvh.html

Java: // 手写递归
来源：http://hz.yuxming.cn/gtsvtvkegw.html

Go:   // 手写递归
来源：http://hz.jqgfzy.top/gtdcigjdaf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xinyue.icu/gtygkgruik.html

C#:   // 手写递归
来源：http://hz.hnqzz.top/gttrtvcpma.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.quarkkingdee.top/gtdsfrvtto.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenzaomai.com/gthguqdxav.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.mhx1999.top/gtjskdywvr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxuanxn.top/gtvjlzcggp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.haohaochexian.top/gttjogaazo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangshuangyany.cn/gtsaeztvxk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhaomingkeji.xyz/gtcxeofqwr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.gzhubu.top/gtenuljwxb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhiwuduotai.top/gtcgxexekq.html

================================================================================
来源：http://hz.yj20258888.top/gtdxwdccah.html

O. 并发与异步
来源：http://hz.tianlin.xyz/gtvnkzazwt.html

================================================================================
来源：http://hz.sysykeji.top/gtuiqviwrz.html

[O01] 启动一个线程
来源：http://hz.hysaishi.cn/gtchwobpiu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.quarkkingdee.top/gttodaifwh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cucudq.cn/gtfvcavdvi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.andypj.xyz/gtqlnewpdt.html

TS:   // 同 JS
来源：http://hz.daria6918.cn/gtdstrihwr.html

Java: new Thread(() -> f()).start()
来源：http://hz.pycfn.com/gtesqapjnp.html

Go:   go f()
来源：http://hz.xuetiantiany.cn/gtcxmmhnau.html

Ruby: Thread.new { f }
来源：http://hz.yuxming.cn/gtlgqkhjwn.html

C#:   Task.Run(() => F());
来源：http://hz.yuanzhike.top/gtkrqljktk.html

[O02] 使用线程池
来源：http://hz.sweek.top/gtaevsbtwa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.dashuyun.cn/gtmckmulnh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ivvv.top/gtwclpwdcb.html

JS:   // worker_threads 线程池
来源：http://hz.zhongyouzk.top/gtcwwkfzdi.html

TS:   // worker_threads 线程池
来源：http://hz.svipenyu.cn/gtbzdywrdu.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hysaishi.cn/gttxctkmqa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.pycfn.com/gtszptgvwb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.bjfxy.top/gtnapdepyx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yonumen.top/gtzdzibljk.html

[O03] 加锁保护共享数据
来源：http://hz.zhixingplan.top/gtwbdfmzoj.html

Py:   with lock: shared += 1
来源：http://hz.daxiang520.top/gtdillyjtk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jianghu66.top/gtptmgoivu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ybcxt.top/gtgwagalfk.html

TS:   // 同 JS
来源：http://hz.guannengcc.top/gtzqqudpee.html

Java: synchronized (this) { shared++; }
来源：http://hz.shanyushiyangkeji.top/gtzitljdoj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.c1oappe.top/gtuhwosfuf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yongpay.top/gttfqvnmmd.html

C#:   lock (gate) { shared++; }
来源：http://hz.cucudq.cn/gtuxvumuiv.html

[O04] 定义异步函数并等待
来源：http://hz.sufxvd.cn/gtucophjxi.html

Py:   async def f():⏎    await g()
来源：http://hz.chenzaomai.com/gtreilvbrl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.haohaochexian.top/gtjaluygjh.html

JS:   async function f() { await g(); }
来源：http://hz.andypj.xyz/gtbqevypvo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hfpthk.cn/gtjywsyjdz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ivvv.top/gttxtikzrm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhaomingkeji.xyz/gtbofdvoor.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yj20258888.top/gtquundbcy.html

C#:   async Task F() { await G(); }
来源：http://hz.xziqi.cn/gtzbpnkzim.html

[O05] 并发执行并等待全部完成
来源：http://hz.svipenyu.cn/gtndjijslj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.meibo888.top/gtayrqgssi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.tianlin.xyz/gtrsqkltwu.html

JS:   await Promise.all(tasks)
来源：http://hz.redwolf501.top/gtkdisdlkd.html

TS:   await Promise.all(tasks)
来源：http://hz.zycfv.cn/gtaqvcrtdt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.wangshuangyany.cn/gtthcyrtqp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.52xcode.cn/gtmrzffuai.html

Ruby: threads.map(&:join)
来源：http://hz.redwolf501.top/gtqfcbfrgr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.nanxinkj.top/gtlasaxsji.html

[O06] 使用进程池
来源：http://hz.sysykeji.top/gtkcekmxkj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.chenlongwang.top/gttijkveih.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shanyushiyangkeji.top/gttxuherzl.html

JS:   // child_process / cluster 模块
来源：http://hz.shanyushiyangtech.top/gtbewzaoir.html

TS:   // child_process / cluster 模块
来源：http://hz.chenzaomai.com/gtoioitbsh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zycfv.cn/gtdlnsbflo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jianghu66.top/gtmadeqfxb.html

Ruby: // fork 块
来源：http://hz.jqgufenzy.top/gtmxfzdwln.html

C#:   Parallel.For
来源：http://hz.cashguo.top/gtxnlpxgth.html

================================================================================
来源：http://hz.bjfxy.top/gtissizcsl.html

P. 常用工具函数
来源：http://hz.yongpay.top/gtjnktrzqm.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gthnezyhis.html

[P01] 生成 UUID
来源：http://hz.snrcjt.cn/gtutcmeazr.html

Py:   str(uuid.uuid4())
来源：http://hz.cucudq.cn/gtabffpdae.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.aibaodan.cn/gtyttsyvvq.html

JS:   crypto.randomUUID()
来源：http://hz.haohaochexian.top/gtxnwtcpeh.html

TS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtennanant.html

Java: UUID.randomUUID().toString()
来源：http://hz.nanxuanxn.top/gtwuixysof.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ehwqpu.com/gtvngvwnec.html

Ruby: SecureRandom.uuid
来源：http://hz.tian-w.cn/gtbtgdmidr.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hongshengwenyu.top/gtvpxydiun.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hammf.cn/gtqbqihnez.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.svipenyu.cn/gtednmwnhj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.chenzaomai.com/gtmoaqsaup.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.birdmap.top/gtcftkorbz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.haohaochexian.top/gtpeycusnw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yuxming.cn/gthltnojaj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.aibaodan.cn/gtbtnrlyhe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.c1oappe.top/gtvmgnqygu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.gogol.net.cn/gtoheotkvi.html

[P03] 生成短随机字符串
来源：http://hz.aibaodan.cn/gtkffmolsz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gotoacloud.top/gtuypqfjnm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yuxming.cn/gtuzeysieh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.316326.xyz/gtjgtukaxh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nwbrower.top/gtfvunjjcy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shanyushiyangkeji.top/gtbngbvwny.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jiagoushi.top/gtnvulqkzi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ywan-chungtsiang.top/gtnemqppiu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yj20258888.top/gtnoggrldg.html

[P04] 求长度
来源：http://hz.nwbrower.top/gtzyvxvbgq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.andypj.xyz/gtmvtlzbqn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ppjwa.cn/gtnnhmjdkw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hammf.cn/gtglffscgl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daxiang520.top/gtfaokvjdq.html

Java: list.size();  map.size();  s.length()
来源：http://hz.vqdsnc.cn/gtlvdnrmhc.html

Go:   len(arr);  len(m)
来源：http://hz.yangfankeji.com/gtrlxtymbz.html

Ruby: x.length;  x.size
来源：http://hz.xinyue.icu/gtjrohoirb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yj20258.top/gtvnizgfwp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xinyue.icu/gtkrakbdrf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sweek.top/gtkjxodzyw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.dianchejie.cn/gtcdpwtodm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shanyushiyangkeji.top/gtimnaxeoa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.daria6918.cn/gtwmtczfgt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ppjwa.cn/gtgdmxfobp.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.daria6918.cn/gtnwcdaugz.html

Ruby: a == b
来源：http://hz.xziqi.cn/gtttsebrsf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xylfe.cn/gtwqsessco.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jqgufenzy.top/gthchvsdvt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ivvv.top/gtqonjbheg.html

PHP:  if (empty($x)) {}
来源：http://hz.tanke756.top/gtqxbyjwxv.html


<!-- 参考信息 -->