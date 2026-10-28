代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gogol.net.cn/gtjamobghh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zdqjudy.top/gtagnmutzr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yuxming.cn/gtmvgiugmf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.dashuyun.cn/gthfguplcs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinyuanbaomall.cn/gtpwjkeqno.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.mhx1999.top/gtxdtxzpqq.html

================================================================================
来源：http://hz.jiagoushi.top/gtrlxhsrtk.html

M. 命令行 / 进程 / 环境
来源：http://hz.zycfv.cn/gtzqlrunma.html

================================================================================
来源：http://hz.xziqi.cn/gtewclqqkk.html

[M01] 读取命令行参数
来源：http://hz.shanyushiyangkeji.top/gtqxkppigo.html

Py:   sys.argv[1:]
来源：http://hz.yongpay.top/gtqzkpqrxw.html

PHP:  $argv;  $argc;
来源：http://hz.yuanzhike.top/gtitwtmatj.html

JS:   process.argv.slice(2)
来源：http://hz.jinyuanbaomall.cn/gthwnwtfow.html

TS:   process.argv.slice(2)
来源：http://hz.tian-w.cn/gtxcobblze.html

Java: args 数组（main 方法参数）
来源：http://hz.sweek.top/gtibedaoxf.html

Go:   os.Args[1:]
来源：http://hz.shangyingyoupin.top/gtpwqxqmuz.html

Ruby: ARGV
来源：http://hz.hnxiangtu.top/gtupehhglt.html

C#:   args 数组（Main 方法参数）
来源：http://hz.9152youxi.cn/gtqrtdgwhu.html

[M02] 读取环境变量
来源：http://hz.ywan-chungtsiang.top/gtchcqieie.html

Py:   os.environ.get("HOME")
来源：http://hz.cheryme.top/gtfkzvlelg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hnqzz.top/gtrykffipo.html

JS:   process.env.HOME
来源：http://hz.xuanzx.com/gtjozdwjsv.html

TS:   process.env.HOME
来源：http://hz.hfpthk.cn/gtcltqjpvp.html

Java: System.getenv("HOME")
来源：http://hz.yueranfly.top/gtivlbfsuf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yangfankeji.com/gtikwqkacv.html

Ruby: ENV["HOME"]
来源：http://hz.zhoulong.xyz/gtbetdlsxd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhengqikj.top/gtjbswjmvv.html

[M03] 执行外部命令
来源：http://hz.jinghuilouyu.cn/gtebzykvno.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zycfv.cn/gtoilbxeyx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hammf.cn/gtumiczuiz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ivvv.top/gtayiyldpz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.aizwys.cn/gtjipgbdxw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xylfe.cn/gtwzcnbvze.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhengqikj.top/gtkivogpfk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yj20258888.top/gtcpojszoc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.iojbl.cn/gtzgwcprrp.html

[M04] 获取当前工作目录
来源：http://hz.yuxming.cn/gtfbwnhxvk.html

Py:   os.getcwd()
来源：http://hz.shuidangran.top/gtvwdwjsav.html

PHP:  getcwd();
来源：http://hz.zdqjudy.top/gtonvmexmb.html

JS:   process.cwd()
来源：http://hz.jinghuilouyu.cn/gtuaibkhcw.html

TS:   process.cwd()
来源：http://hz.0kj1m.cn/gtjsnvyjgj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinghuilouyu.cn/gtyesphbtr.html

Go:   os.Getwd()
来源：http://hz.xinyue.icu/gtrtvoujfa.html

Ruby: Dir.pwd
来源：http://hz.xingfuxueyuan.xyz/gtwdvxhzet.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xziqi.cn/gtugkrvwts.html

[M05] 设置退出码
来源：http://hz.ppjwa.cn/gtssoebazd.html

Py:   sys.exit(1)
来源：http://hz.yj202588.top/gtxtthxgpx.html

PHP:  exit(1);
来源：http://hz.zhengqikj.top/gtpcuipuxa.html

JS:   process.exit(1)
来源：http://hz.nanxinkj.top/gtsfkvycpf.html

TS:   process.exit(1)
来源：http://hz.wangshuangyany.cn/gtjjkydstf.html

Java: System.exit(1)
来源：http://hz.c1oappe.top/gtmaxzfhxl.html

Go:   os.Exit(1)
来源：http://hz.shanyushiyangtech.top/gtqakvxlaa.html

Ruby: exit 1
来源：http://hz.cashguo.top/gtvtndkypo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cdnleiting.top/gtpmvzhkfk.html

[M06] 向标准错误输出
来源：http://hz.zhijiandao.cn/gtxfskqyue.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhengqikj.top/gtptsgoven.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenzaomai.com/gtmuwrewbv.html

JS:   console.error("err")
来源：http://hz.cqqwz.cn/gtkviiqlji.html

TS:   console.error("err")
来源：http://hz.meibo888.top/gtyznuejvx.html

Java: System.err.println("err")
来源：http://hz.shzxlz.cn/gtliuewjqc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.pengpengdd.cyou/gttnyfaomw.html

Ruby: warn "err"
来源：http://hz.hysaishi.cn/gtryrytufz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.birdmap.top/gtzyqlpjfr.html

[M07] 判断是否为主入口
来源：http://hz.jinqigfzy.top/gtnvwtqyip.html

Py:   if __name__ == "__main__":
来源：http://hz.cdnleiting.top/gtltjjjovi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shzxlz.cn/gtitnfpcab.html

JS:   require.main === module
来源：http://hz.zdqjudy.top/gtdlbmibio.html

TS:   require.main === module
来源：http://hz.aibaodan.cn/gthttdrdxp.html

Java: public static void main(String[] args)
来源：http://hz.c1oappe.top/gtucczkjhc.html

Go:   func main()
来源：http://hz.feifeiyinyue.top/gtvradfccq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yueranfly.top/gtznhfpljg.html

C#:   static void Main(string[] args)
来源：http://hz.xuetiantiany.cn/gtfcdhlyla.html

[M08] 获取系统与运行时信息
来源：http://hz.aizwys.cn/gtmclfuvey.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhijiandao.cn/gthdpyetba.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xziqi.cn/gtwuntahnd.html

JS:   process.platform;  process.version
来源：http://hz.aibaodan.cn/gtydztrihf.html

TS:   process.platform;  process.version
来源：http://hz.aizwys.cn/gtberugtfi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shuidangran.top/gtlasjegmu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ybcxt.top/gtofsabtov.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yvedp.cn/gtlfwixgxy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.meibo888.top/gtbabuzncm.html

================================================================================
来源：http://hz.yuanzhike.top/gtdsrxcgwj.html

N. 数据结构与算法
来源：http://hz.chenlongwang.top/gtnhkpfvsf.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtzruzjyzr.html

[N01] 二分查找（有序数组）
来源：http://hz.zhengqikj.top/gtkwnhtfxt.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.svipenyu.cn/gttmhlavrt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinghuilouyu.cn/gtijpixmsa.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.feifeiyinyue.top/gthnevtecj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhengqikj.top/gttezhgxgb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shanyushiyangtech.top/gtofxkaqug.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinghuilouyu.cn/gtvzevupmq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.chenzaomai.com/gtrdydlrqp.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xziqi.cn/gtznqhopap.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xuetiantiany.cn/gtwxumkzyu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.mhx1999.top/gtczuujfpw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhoulong.xyz/gtrxvzxrkz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhaomingkeji.xyz/gthzpymuse.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.dashuyun.cn/gtjmioggbw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cqqwz.cn/gtexziiaoh.html

Go:   slices.Sort(arr)
来源：http://hz.52xcode.cn/gtvthkvtje.html

Ruby: arr.sort
来源：http://hz.hammf.cn/gtmpoloutl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinqigufen.top/gtkqshukib.html

[N03] 快速排序（分治示例）
来源：http://hz.zhixingplan.top/gtrdaviwnx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zycfv.cn/gtzyzfiaeu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yonumen.top/gtuxxfgwxz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xinyue.icu/gtjhmfhqmp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aibaodan.cn/gtukhoajep.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinghuilouyu.cn/gtycggfjmo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shangyingyoupin.top/gtjcyrpjji.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jlsjyb.cn/gttsvgnmvr.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yuanzhike.top/gtqlcfdupg.html

[N04] 斐波那契数列
来源：http://hz.bjfxy.top/gtajwyejiz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tian-w.cn/gtwwirpikc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xingfuxueyuan.xyz/gtdfrkuksc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.mhx1999.top/gtkgunnrhl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xylfe.cn/gtozofupvf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhengqikj.top/gtimoygkww.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xuanzx.com/gtykkscuzf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jianghu66.top/gtfmzwatau.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ehwqpu.com/gttusjuukc.html

[N05] 最大公约数
来源：http://hz.chenzaomai.com/gtqqijrqtx.html

Py:   math.gcd(a, b)
来源：http://hz.havefunace.top/gtxhklfdhm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yanxiufei.cn/gtzzxozclz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cucudq.cn/gtoudxkgqq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nanxuanxn.top/gtqpnidqzb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.haohaochexian.top/gtavtffrfl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ydzc1.top/gtouvkjcme.html

Ruby: a.gcd(b)
来源：http://hz.jqgfzy.top/gtehkpxyop.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.sufxvd.cn/gttdvpcopk.html

[N06] 判断回文字符串
来源：http://hz.ivvv.top/gtbgxmtbmc.html

Py:   s == s[::-1]
来源：http://hz.xuanzx.com/gtznrtmnid.html

PHP:  $s === strrev($s);
来源：http://hz.havefunace.top/gtfryeveud.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ydzc1.top/gtstisvlbe.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hnqzz.top/gtqlejhtyv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.316326.xyz/gtcsfbxshm.html

Go:   // 双指针从两端比较
来源：http://hz.fengsongda.top/gtifvekoaq.html

Ruby: s == s.reverse
来源：http://hz.daria6918.cn/gtlzfvcwjr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xziqi.cn/gtlbsipbqn.html

[N07] 两数之和（返回下标）
来源：http://hz.hnqzz.top/gtttiieekh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nanxinkj.top/gtwqrfqpwu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.0kj1m.cn/gtilfjfbqn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ywan-chungtsiang.top/gtqzqldfcc.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinqigfzy.top/gtpcbntefr.html

Java: // 手写 HashMap
来源：http://hz.wangdashe.top/gtnnchfoew.html

Go:   // 手写 map[int]int
来源：http://hz.fzhhl.top/gtxikoxktr.html

Ruby: // 手写 Hash
来源：http://hz.jinqigufen.top/gtdjhbkgjj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gaohongyu789.top/gtzzlvfszj.html

[N08] 生成全排列
来源：http://hz.jqgufenzy.top/gtvjtmzobf.html

Py:   itertools.permutations(arr)
来源：http://hz.zhengqikj.top/gtkknkpnqd.html

PHP:  // 手写递归交换
来源：http://hz.zhiwuduotai.top/gtultlavec.html

JS:   // 手写回溯递归
来源：http://hz.sysykeji.top/gtqtcermxn.html

TS:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtgiykdjpa.html

Java: // 手写回溯递归
来源：http://hz.zdqjudy.top/gtigdvwwze.html

Go:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtduvkgvqe.html

Ruby: arr.permutation.to_a
来源：http://hz.aizwys.cn/gtxbgcfqlr.html

C#:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtiqomuood.html

[N09] 栈与队列
来源：http://hz.jiagoushi.top/gtdrtyfkeq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yanxiufei.cn/gtilbugvam.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.smart0.xyz/gtvoaqswfs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hnqzz.top/gtykaxdgme.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.chenzaomai.com/gtgndlgcjy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhengqikj.top/gtbmctmypo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gaohongyu789.top/gtzzzykkqq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhijiandao.cn/gtppwfagac.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xuetiantiany.cn/gtlrzvuane.html

[N10] 链表节点定义
来源：http://hz.gotoacloud.top/gtnafjmgxk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.chenlongwang.top/gtalaktscl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.chenlongwang.top/gtkntuuqon.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj20258.top/gtepigbtvh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.andypj.xyz/gtexzhhfjn.html

Java: class Node { int v; Node next; }
来源：http://hz.gotoacloud.top/gtrxkjslbn.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.nanxuanxn.top/gtjrgycyhu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.wangshuangyany.cn/gtfsatgywx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hnxiangtu.top/gtmwfxappj.html

[N11] 二叉树中序遍历
来源：http://hz.hfpthk.cn/gthiwwftqz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.316326.xyz/gtdccgxxam.html

PHP:  // 手写递归函数
来源：http://hz.wangdashe.top/gtaivgzrpn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shangyingyoupin.top/gtlhgatydj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cdnleiting.top/gtmjieyjhq.html

Java: // 手写递归
来源：http://hz.yongpay.top/gtaajkybyj.html

Go:   // 手写递归
来源：http://hz.feifeiyinyue.top/gtzumlrwsz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jyoumei.cn/gtjjkxpvuj.html

C#:   // 手写递归
来源：http://hz.ybcxt.top/gtgibqnlxi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cdnleiting.top/gtrungghcg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenlongwang.top/gtatgfrsxr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hfpthk.cn/gtgcpnscko.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cqqwz.cn/gtikrqoblg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenlongwang.top/gtjkcpteps.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenlongwang.top/gtarffimot.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jlsjyb.cn/gtfzsticnc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinqigfzy.top/gtdqbndvcq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.aibaodan.cn/gtxekyxgeq.html

================================================================================
来源：http://hz.zhoulong.xyz/gttoiobfyx.html

O. 并发与异步
来源：http://hz.havefunace.top/gtxgxcgibm.html

================================================================================
来源：http://hz.316326.xyz/gtmufgccvp.html

[O01] 启动一个线程
来源：http://hz.ydzc1.top/gtzbdwwsvb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.kuanghao11.cn/gtzzkihjel.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jianghu66.top/gtauildeno.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hywenlv.cn/gthenhdjhs.html

TS:   // 同 JS
来源：http://hz.gaohongyu789.top/gtfimzldhr.html

Java: new Thread(() -> f()).start()
来源：http://hz.pengpengdd.cyou/gtrantczcj.html

Go:   go f()
来源：http://hz.hammf.cn/gtatlkdele.html

Ruby: Thread.new { f }
来源：http://hz.cucudq.cn/gtigutimag.html

C#:   Task.Run(() => F());
来源：http://hz.0kj1m.cn/gtgfxafwqx.html

[O02] 使用线程池
来源：http://hz.redwolf501.top/gteqcsdxom.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yuxming.cn/gtkrrwtsol.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.dashuyun.cn/gthhxusahn.html

JS:   // worker_threads 线程池
来源：http://hz.yj202588.top/gtvrydctbo.html

TS:   // worker_threads 线程池
来源：http://hz.ybcxt.top/gtnrtlwhsd.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.52xcode.cn/gtohejcvsz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.9152youxi.cn/gtmultzqsi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shanyushiyangtech.top/gtjxqrsxby.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinqigfzy.top/gttwabgcwt.html

[O03] 加锁保护共享数据
来源：http://hz.zhijiandao.cn/gtunvmoonh.html

Py:   with lock: shared += 1
来源：http://hz.ybcxt.top/gtvlhkdyut.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.fengsongda.top/gttaijinuj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jqgufenzy.top/gtxyeobdph.html

TS:   // 同 JS
来源：http://hz.jinghuilouyu.cn/gtjdnsrxzn.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhaomingkeji.xyz/gtcgohzddn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jinqigufen.top/gtdusvyydf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhaomingkeji.xyz/gtovyzkzte.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhijiandao.cn/gtodehzmfr.html

[O04] 定义异步函数并等待
来源：http://hz.havefunace.top/gtcxkclzvq.html

Py:   async def f():⏎    await g()
来源：http://hz.wangshuangyany.cn/gtxbytrets.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hywenlv.cn/gtwmngzdgj.html

JS:   async function f() { await g(); }
来源：http://hz.zhixingplan.top/gtogackhzz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shanyushiyangtech.top/gtclxymxas.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.smart0.xyz/gttfnlqepy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shanyushiyangtech.top/gttnpmtuac.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ywan-chungtsiang.top/gtsgvhmuzg.html

C#:   async Task F() { await G(); }
来源：http://hz.jinyuanbaomall.cn/gtzesncpgb.html

[O05] 并发执行并等待全部完成
来源：http://hz.ywan-chungtsiang.top/gtzhxcbejm.html

Py:   asyncio.gather(*tasks)
来源：http://hz.tian-w.cn/gtnzhlpoqu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ybcxt.top/gtbvwfbhgs.html

JS:   await Promise.all(tasks)
来源：http://hz.jyoumei.cn/gtulfunkuu.html

TS:   await Promise.all(tasks)
来源：http://hz.yonumen.top/gtnwtrxkfq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ppjwa.cn/gtzclfafth.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.tianlin.xyz/gtvjlompxm.html

Ruby: threads.map(&:join)
来源：http://hz.ivvv.top/gtfugaipgs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.kuanghao11.cn/gtvuokcfry.html

[O06] 使用进程池
来源：http://hz.xingfuxueyuan.xyz/gtcpltjtat.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.andypj.xyz/gtrvshwube.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jinghuilouyu.cn/gtfmnkdtuz.html

JS:   // child_process / cluster 模块
来源：http://hz.dashuyun.cn/gtrwucbtoh.html

TS:   // child_process / cluster 模块
来源：http://hz.yonumen.top/gteargudsi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ivvv.top/gtvypfmkpk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.aizwys.cn/gtshssgzfx.html

Ruby: // fork 块
来源：http://hz.316326.xyz/gtyurawwmn.html

C#:   Parallel.For
来源：http://hz.birdmap.top/gtbvoxobdb.html

================================================================================
来源：http://hz.pycfn.com/gtmdyqceim.html

P. 常用工具函数
来源：http://hz.andypj.xyz/gtipyhniaw.html

================================================================================
来源：http://hz.52xcode.cn/gtelysnrey.html

[P01] 生成 UUID
来源：http://hz.ywan-chungtsiang.top/gtstpqxqbi.html

Py:   str(uuid.uuid4())
来源：http://hz.iojbl.cn/gtjhpvotas.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yueranfly.top/gtllafdvok.html

JS:   crypto.randomUUID()
来源：http://hz.yj20258888.top/gtcpnpydvi.html

TS:   crypto.randomUUID()
来源：http://hz.0kj1m.cn/gtvbfvhjwr.html

Java: UUID.randomUUID().toString()
来源：http://hz.redwolf501.top/gtwzhgjzly.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hammf.cn/gthhgnvwqh.html

Ruby: SecureRandom.uuid
来源：http://hz.birdmap.top/gttuojexnc.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.feifeiyinyue.top/gtnzplupzo.html

[P02] MD5 / SHA256 摘要
来源：http://hz.mhx1999.top/gtjlxovvlk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yuanzhike.top/gtzbikxhga.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.kuanghao11.cn/gthyrnjewu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hnqzz.top/gtrlcimdyt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj20258888.top/gttjgyjesh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yuanzhike.top/gtixtuoixo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xinyue.icu/gtrrgooalf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jqgufenzy.top/gtubphjwnp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhixingplan.top/gtvwbdhwqu.html

[P03] 生成短随机字符串
来源：http://hz.xuetiantiany.cn/gtqkoefhpw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sweek.top/gtdwdgcagh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jiagoushi.top/gtweihefzf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.vqdsnc.cn/gtfcpqkexu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.52xcode.cn/gtfwerztqz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hongshengwenyu.top/gttlphuoxy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ybcxt.top/gtvvoqthxy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sweek.top/gthvhcocrj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hnxiangtu.top/gtwuxipppl.html

[P04] 求长度
来源：http://hz.cashguo.top/gtfahthpzu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.svipenyu.cn/gtcegcvuug.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj20258888.top/gttatwmlga.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenjidiqi.icu/gtitufmdnb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.guannengcc.top/gtyogawnnl.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhengqikj.top/gtariwoozy.html

Go:   len(arr);  len(m)
来源：http://hz.xziqi.cn/gtwhhuivyr.html

Ruby: x.length;  x.size
来源：http://hz.jqgfzy.top/gtwbscwqsx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.wangshuangyany.cn/gtnxlvvhqf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.meibo888.top/gtpwzbmhga.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xziqi.cn/gtfxqafkbl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.dashuyun.cn/gtybjxsblv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jinqigfzy.top/gtsuwxleuf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.haohaochexian.top/gtxictvpuj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ehwqpu.com/gtftqaecpe.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jqgfzy.top/gtimpkgjkt.html

Ruby: a == b
来源：http://hz.dianchejie.cn/gttkuvkntf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ydzc1.top/gtgvoxsnrv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yonumen.top/gtlymecskg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jiagoushi.top/gtvgfyixml.html

PHP:  if (empty($x)) {}
来源：http://hz.svipenyu.cn/gtqgumatxu.html


<!-- 参考信息 -->