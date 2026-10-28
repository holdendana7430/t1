代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://hz.aibaodan.cn/gtjigmtzfd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.iojbl.cn/gtyypbaowp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.svipenyu.cn/gtztqfaioc.html

JS:   resp.ok;  resp.status
来源：http://hz.0kj1m.cn/gtijyujssv.html

TS:   resp.ok;  resp.status
来源：http://hz.shuidangran.top/gtdtkdkhmm.html

Java: resp.statusCode()
来源：http://hz.ivvv.top/gtwdlqsxhs.html

Go:   resp.StatusCode
来源：http://hz.chenlongwang.top/gtuppaqvgc.html

Ruby: resp.code.to_i
来源：http://hz.sxryk.cn/gtiljylzvr.html

C#:   (int)resp.StatusCode
来源：http://hz.pengpengdd.cyou/gtuavpkuek.html

[L08] 并发请求多个地址
来源：http://hz.nwbrower.top/gtwuvfvtco.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinqigufen.top/gtmkorgypc.html

PHP:  curl_multi_init() 系列
来源：http://hz.ehwqpu.com/gtkzkmyndr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigufen.top/gthdhjmdxr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhaomingkeji.xyz/gtceqksyir.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.haohaochexian.top/gthynihcnw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhixingplan.top/gtxdqbsrgk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.guowangkeji.top/gtzxrmsrrx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yonumen.top/gtjshsmwku.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtxubmsqbc.html

M. 命令行 / 进程 / 环境
来源：http://hz.jlsjyb.cn/gtjnsghypo.html

================================================================================
来源：http://hz.chenlongwang.top/gtyfuztxlr.html

[M01] 读取命令行参数
来源：http://hz.52xcode.cn/gtznxwzoef.html

Py:   sys.argv[1:]
来源：http://hz.shanyushiyangkeji.top/gtsseabvft.html

PHP:  $argv;  $argc;
来源：http://hz.havefunace.top/gtqbgzjoqk.html

JS:   process.argv.slice(2)
来源：http://hz.chenlongwang.top/gttvtrgxqu.html

TS:   process.argv.slice(2)
来源：http://hz.hongshengwenyu.top/gtetdajcih.html

Java: args 数组（main 方法参数）
来源：http://hz.hammf.cn/gtjtdzhhlf.html

Go:   os.Args[1:]
来源：http://hz.ydjk.org.cn/gtdtgmupgr.html

Ruby: ARGV
来源：http://hz.yj20258888.top/gtqyxmpedi.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hnqzz.top/gtsdoeuukw.html

[M02] 读取环境变量
来源：http://hz.ppjwa.cn/gtpezkstue.html

Py:   os.environ.get("HOME")
来源：http://hz.tian-w.cn/gtagnxyock.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.guowangkeji.top/gtmsztjjnv.html

JS:   process.env.HOME
来源：http://hz.yj202588.top/gtztwahgdw.html

TS:   process.env.HOME
来源：http://hz.sufxvd.cn/gtnmypyenf.html

Java: System.getenv("HOME")
来源：http://hz.fzhhl.top/gtvirodqlt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.havefunace.top/gtirkgwfcw.html

Ruby: ENV["HOME"]
来源：http://hz.zhixingplan.top/gtifolxfil.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hfpthk.cn/gtqvndmomq.html

[M03] 执行外部命令
来源：http://hz.hongshengwenyu.top/gtptsrtrcu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ehwqpu.com/gtcwltqkls.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhixingplan.top/gtyofhgrlx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.smart0.xyz/gttemthmvw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhiwuduotai.top/gtyuefjgnj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xinyue.icu/gtwquqywzn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.chenlongwang.top/gtodysoqif.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinghuilouyu.cn/gtqsudytqw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yj20258888.top/gtqbwtousw.html

[M04] 获取当前工作目录
来源：http://hz.shzxlz.cn/gthcgzscxq.html

Py:   os.getcwd()
来源：http://hz.sweek.top/gtshwbhjvy.html

PHP:  getcwd();
来源：http://hz.cheryme.top/gtmbsfjfzr.html

JS:   process.cwd()
来源：http://hz.yuanzhike.top/gtvfdzxmxl.html

TS:   process.cwd()
来源：http://hz.vqdsnc.cn/gtxwobmnec.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.nwbrower.top/gtuadgemuu.html

Go:   os.Getwd()
来源：http://hz.shuidangran.top/gtiuqpmfgl.html

Ruby: Dir.pwd
来源：http://hz.zdqjudy.top/gtkqyiwknt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.feifeiyinyue.top/gtptvrelmj.html

[M05] 设置退出码
来源：http://hz.yj20258888.top/gtuxynczxh.html

Py:   sys.exit(1)
来源：http://hz.c1oappe.top/gtjjyjooss.html

PHP:  exit(1);
来源：http://hz.jiagoushi.top/gtnsnflkik.html

JS:   process.exit(1)
来源：http://hz.dashuyun.cn/gtbtqfiwrb.html

TS:   process.exit(1)
来源：http://hz.yanxiufei.cn/gtohzxtcdi.html

Java: System.exit(1)
来源：http://hz.andypj.xyz/gtbdwppber.html

Go:   os.Exit(1)
来源：http://hz.guowangkeji.top/gtiqrexinm.html

Ruby: exit 1
来源：http://hz.aibaodan.cn/gtgekupbtt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gaohongyu789.top/gtoyjdfcfl.html

[M06] 向标准错误输出
来源：http://hz.yj202588.top/gtcqulomso.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shanyushiyangkeji.top/gtgynvtopv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jlsjyb.cn/gtibamnyld.html

JS:   console.error("err")
来源：http://hz.hnqzz.top/gtrwwizbjn.html

TS:   console.error("err")
来源：http://hz.smart0.xyz/gtstzmpial.html

Java: System.err.println("err")
来源：http://hz.aizwys.cn/gtcbxndoem.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xziqi.cn/gtcpzuxgvg.html

Ruby: warn "err"
来源：http://hz.havefunace.top/gtexhzsvlg.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.nanxinkj.top/gtaksmrlcy.html

[M07] 判断是否为主入口
来源：http://hz.guannengcc.top/gtzzmxfhxv.html

Py:   if __name__ == "__main__":
来源：http://hz.haohaochexian.top/gttectjcmy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cucudq.cn/gttedapunz.html

JS:   require.main === module
来源：http://hz.feifeiyinyue.top/gtdjbhlkns.html

TS:   require.main === module
来源：http://hz.yonumen.top/gtjyqpvomv.html

Java: public static void main(String[] args)
来源：http://hz.gaohongyu789.top/gtrsnddjth.html

Go:   func main()
来源：http://hz.wangdashe.top/gtcbrpzpbg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.daxiang520.top/gtlnamojug.html

C#:   static void Main(string[] args)
来源：http://hz.zhengqikj.top/gtdgzynwtn.html

[M08] 获取系统与运行时信息
来源：http://hz.gogol.net.cn/gtqauewyrr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hfpthk.cn/gtuysuozse.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shzxlz.cn/gtoajskqzi.html

JS:   process.platform;  process.version
来源：http://hz.9152youxi.cn/gtcllzwlkm.html

TS:   process.platform;  process.version
来源：http://hz.pycfn.com/gtsmqfoccn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.guannengcc.top/gttdjlnnaf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinqigfzy.top/gtzkacirse.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.kuanghao11.cn/gtpfqxkatf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj20258.top/gtiwxoecow.html

================================================================================
来源：http://hz.jyoumei.cn/gtieqvpmhh.html

N. 数据结构与算法
来源：http://hz.redwolf501.top/gtofjorlas.html

================================================================================
来源：http://hz.jinqigufen.top/gtipmabwtc.html

[N01] 二分查找（有序数组）
来源：http://hz.shzxlz.cn/gtjpxmqhoe.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.birdmap.top/gtxydxobta.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gotoacloud.top/gtlbnmaihb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.iojbl.cn/gtjklrulnt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sxryk.cn/gtwmyqtvak.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ppjwa.cn/gtjvqpsjwf.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shuidangran.top/gtzxudpexk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zdqjudy.top/gtfgkfawxb.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ydzc1.top/gtdcggolcr.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.316326.xyz/gtkcxbdkat.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.daxiang520.top/gttshcaoyk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinqigufen.top/gtluulxipx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yonumen.top/gtljvqbnai.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinqigufen.top/gtrcwzogmk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.kuanghao11.cn/gtwxchxbzn.html

Go:   slices.Sort(arr)
来源：http://hz.yvedp.cn/gttbegxoir.html

Ruby: arr.sort
来源：http://hz.shuidangran.top/gtgsgibszq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinqigfzy.top/gtjrfxgcqr.html

[N03] 快速排序（分治示例）
来源：http://hz.ydzc1.top/gtpnibjivm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.aizwys.cn/gtnppihkcm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cashguo.top/gtkarvvroy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dashuyun.cn/gtdilpwbop.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shzxlz.cn/gtbopukati.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shanyushiyangkeji.top/gtmwpzhuat.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ppjwa.cn/gtmoagtdsf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ivvv.top/gtjzotwnfw.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ppjwa.cn/gtatguewoy.html

[N04] 斐波那契数列
来源：http://hz.nanxuanxn.top/gtuishiaqf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yongpay.top/gtfupkbjwp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xziqi.cn/gtzvstosvf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jianghu66.top/gteigqhlwj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.redwolf501.top/gtxeddagnv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ppjwa.cn/gtvtdexxqz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jlsjyb.cn/gtzungtdav.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sysykeji.top/gttvscscui.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj202588.top/gtaadjkbbg.html

[N05] 最大公约数
来源：http://hz.yj20258888.top/gturyertlq.html

Py:   math.gcd(a, b)
来源：http://hz.zhoulong.xyz/gtfufzsfrw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hnxiangtu.top/gtuxkaopmn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gogol.net.cn/gtftoclunu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.haohaochexian.top/gtfvnovqsu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.iojbl.cn/gtszcsyvpv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.snrcjt.cn/gtbettalkp.html

Ruby: a.gcd(b)
来源：http://hz.shanyushiyangkeji.top/gtfhvmzuih.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xuetiantiany.cn/gtefsuicbj.html

[N06] 判断回文字符串
来源：http://hz.sxryk.cn/gtczaobkhj.html

Py:   s == s[::-1]
来源：http://hz.jyoumei.cn/gtdkiwthub.html

PHP:  $s === strrev($s);
来源：http://hz.fzhhl.top/gtlaixcqvg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtnhqthpfw.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cqqwz.cn/gtdvpfpysv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sweek.top/gtmvwzhemt.html

Go:   // 双指针从两端比较
来源：http://hz.fengsongda.top/gtgnhqfoxp.html

Ruby: s == s.reverse
来源：http://hz.shzxlz.cn/gtkkzwtakh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhijiandao.cn/gtgtfsrusu.html

[N07] 两数之和（返回下标）
来源：http://hz.cheryme.top/gtiztdkbrt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.andypj.xyz/gtmxvqdkhe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jqgfzy.top/gtvykofdkh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sweek.top/gtgufiojqq.html

TS:   // 手写 Map<string, number>
来源：http://hz.xuanzx.com/gthgnrfdco.html

Java: // 手写 HashMap
来源：http://hz.0kj1m.cn/gtjkebfwtw.html

Go:   // 手写 map[int]int
来源：http://hz.smart0.xyz/gtclevdile.html

Ruby: // 手写 Hash
来源：http://hz.vqdsnc.cn/gtepadumxx.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cdnleiting.top/gtwkaqjuhd.html

[N08] 生成全排列
来源：http://hz.gotoacloud.top/gthbjgrjwy.html

Py:   itertools.permutations(arr)
来源：http://hz.quarkkingdee.top/gtvaeiakkt.html

PHP:  // 手写递归交换
来源：http://hz.yongpay.top/gtguailnfw.html

JS:   // 手写回溯递归
来源：http://hz.tanke756.top/gtzsyfzubw.html

TS:   // 手写回溯递归
来源：http://hz.wangdashe.top/gtzjtktsum.html

Java: // 手写回溯递归
来源：http://hz.snrcjt.cn/gtiaefpjtt.html

Go:   // 手写回溯递归
来源：http://hz.aibaodan.cn/gtpyzlzsrb.html

Ruby: arr.permutation.to_a
来源：http://hz.shanyushiyangkeji.top/gtenskikgp.html

C#:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtuzvhqwgo.html

[N09] 栈与队列
来源：http://hz.gogol.net.cn/gtofrfjxhv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yuanzhike.top/gtitsmbfdk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.chenjidiqi.icu/gtuslpgmfn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yj20258888.top/gtqmvklrsf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.316326.xyz/gtunnlndzq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.andypj.xyz/gttiqbfhdc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shzxlz.cn/gtelhppbll.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.dianchejie.cn/gttzbrrywz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.haohaochexian.top/gtmlcfmatv.html

[N10] 链表节点定义
来源：http://hz.fzhhl.top/gtxbkyjlqx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.sufxvd.cn/gtrfrjibyf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.meibo888.top/gtumufbbvk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.fengsongda.top/gtrtsmmcyp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.daria6918.cn/gtwuijvlkb.html

Java: class Node { int v; Node next; }
来源：http://hz.hfpthk.cn/gttzmjqyed.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.nwbrower.top/gthsicshxt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.smart0.xyz/gthvqspaux.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.52xcode.cn/gtxvlkjzpi.html

[N11] 二叉树中序遍历
来源：http://hz.gogol.net.cn/gtjzwxhqij.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hnxiangtu.top/gtifvvzcyz.html

PHP:  // 手写递归函数
来源：http://hz.52xcode.cn/gtfaxcwpbl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinqigufen.top/gtubmerauu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ybcxt.top/gtfeupgxno.html

Java: // 手写递归
来源：http://hz.mhx1999.top/gtdxyhphop.html

Go:   // 手写递归
来源：http://hz.havefunace.top/gtpqmnaotd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hongshengwenyu.top/gtpnmjbmby.html

C#:   // 手写递归
来源：http://hz.jyoumei.cn/gteczbgnyy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ppjwa.cn/gtjpzcyrjy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.dianchejie.cn/gtlrqdnsyc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cdnleiting.top/gtvjynrlzh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jlsjyb.cn/gtptpbaskv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aizwys.cn/gtolfuukak.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangshuangyany.cn/gtvufxnxkg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shanyushiyangtech.top/gttmbthddg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jqgufenzy.top/gtckjougqf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tanke756.top/gtwgyyxgsh.html

================================================================================
来源：http://hz.birdmap.top/gtexyykrfj.html

O. 并发与异步
来源：http://hz.hfpthk.cn/gtqujkopts.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtgvcunitl.html

[O01] 启动一个线程
来源：http://hz.dianchejie.cn/gticfztsgg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xylfe.cn/gtppmhvtpa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.aibaodan.cn/gttwtrpwef.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.kuanghao11.cn/gttlnhaluc.html

TS:   // 同 JS
来源：http://hz.yuanzhike.top/gtnssrnpgw.html

Java: new Thread(() -> f()).start()
来源：http://hz.yueranfly.top/gtrktgvixt.html

Go:   go f()
来源：http://hz.pycfn.com/gthyzprlfw.html

Ruby: Thread.new { f }
来源：http://hz.0kj1m.cn/gtztgrlias.html

C#:   Task.Run(() => F());
来源：http://hz.nwbrower.top/gtfmuuhrug.html

[O02] 使用线程池
来源：http://hz.nwbrower.top/gtntjtnkyd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.guannengcc.top/gtwpeftvuf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sysykeji.top/gtqplzvydg.html

JS:   // worker_threads 线程池
来源：http://hz.sxryk.cn/gtcuvvnind.html

TS:   // worker_threads 线程池
来源：http://hz.zhijiandao.cn/gtldmrabhj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.dianchejie.cn/gtbcpziank.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.daria6918.cn/gtjdyglhil.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jqgfzy.top/gtiijjnegx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.andypj.xyz/gtncxjdzuz.html

[O03] 加锁保护共享数据
来源：http://hz.cheryme.top/gtgplaetvk.html

Py:   with lock: shared += 1
来源：http://hz.ivvv.top/gtaqjyemun.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xuetiantiany.cn/gtcblnmicg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.iojbl.cn/gtvhcasrbh.html

TS:   // 同 JS
来源：http://hz.gzhubu.top/gtvkfomfbw.html

Java: synchronized (this) { shared++; }
来源：http://hz.ydzc1.top/gtifpvxwqy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.bjfxy.top/gteeqiejmy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ydjk.org.cn/gtowitlzkv.html

C#:   lock (gate) { shared++; }
来源：http://hz.0kj1m.cn/gtgsabozme.html

[O04] 定义异步函数并等待
来源：http://hz.52xcode.cn/gtubyrprbz.html

Py:   async def f():⏎    await g()
来源：http://hz.9152youxi.cn/gtlakacfci.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nwbrower.top/gtjdrzdrie.html

JS:   async function f() { await g(); }
来源：http://hz.sufxvd.cn/gtdytxxgvn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yanxiufei.cn/gttyqikalg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gogol.net.cn/gtzymbkxem.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sweek.top/gtusculred.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cheryme.top/gtnlvezbqg.html

C#:   async Task F() { await G(); }
来源：http://hz.shuidangran.top/gtnndcxxdy.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj20258888.top/gtwuphewpm.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yongpay.top/gthoecqzhj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.nanxinkj.top/gtsczvhneu.html

JS:   await Promise.all(tasks)
来源：http://hz.52xcode.cn/gtvzooacno.html

TS:   await Promise.all(tasks)
来源：http://hz.bjfxy.top/gtfbdfhyor.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ydjk.org.cn/gtknwzeyge.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.pycfn.com/gtystnzctn.html

Ruby: threads.map(&:join)
来源：http://hz.ehwqpu.com/gtirhuolsz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yj20258888.top/gtimlczsvy.html

[O06] 使用进程池
来源：http://hz.zhijiandao.cn/gtxydrlaof.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shuidangran.top/gtjfgpbldc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.snrcjt.cn/gtpafixlja.html

JS:   // child_process / cluster 模块
来源：http://hz.jiagoushi.top/gtvnudghvs.html

TS:   // child_process / cluster 模块
来源：http://hz.xuanzx.com/gtpsnobusm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.52xcode.cn/gtpvvswnfc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhiwuduotai.top/gtnmrhcukg.html

Ruby: // fork 块
来源：http://hz.ivvv.top/gtfhjmsgod.html

C#:   Parallel.For
来源：http://hz.zhixingplan.top/gtruaynjli.html

================================================================================
来源：http://hz.zhongyouzk.top/gtajsynszm.html

P. 常用工具函数
来源：http://hz.guowangkeji.top/gtvrobjyyi.html

================================================================================
来源：http://hz.xuanzx.com/gtxegzbbdc.html

[P01] 生成 UUID
来源：http://hz.tian-w.cn/gtvvvcidhq.html

Py:   str(uuid.uuid4())
来源：http://hz.yanxiufei.cn/gtnmiwhgko.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhiwuduotai.top/gtdtoaohbw.html

JS:   crypto.randomUUID()
来源：http://hz.birdmap.top/gtvlsbtybk.html

TS:   crypto.randomUUID()
来源：http://hz.zhiwuduotai.top/gtgbkzoqnp.html

Java: UUID.randomUUID().toString()
来源：http://hz.havefunace.top/gtxortmfit.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jqgufenzy.top/gtqyrsnlhf.html

Ruby: SecureRandom.uuid
来源：http://hz.gaohongyu789.top/gtcqmldjxp.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.wangdashe.top/gtkxbeafdh.html

[P02] MD5 / SHA256 摘要
来源：http://hz.havefunace.top/gttzwpuymu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xinyue.icu/gtipxrqxfs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.chenlongwang.top/gturujmicp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.haohaochexian.top/gtjsqxxgsh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.aizwys.cn/gtetalpjhq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jqgufenzy.top/gtyplybxho.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xuetiantiany.cn/gthawkxdqc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yuxming.cn/gtuvrhiulz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shzxlz.cn/gtldbinurk.html

[P03] 生成短随机字符串
来源：http://hz.yangfankeji.com/gtfpxtqmnd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sysykeji.top/gthocgwqbr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhengqikj.top/gtjwstfnpq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhengqikj.top/gtxyjpawso.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.meibo888.top/gtciloofdz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.feifeiyinyue.top/gtrpvfmise.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.dianchejie.cn/gtxmqkggnd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.9152youxi.cn/gtpnmnybab.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.iojbl.cn/gttroqfizf.html

[P04] 求长度
来源：http://hz.vqdsnc.cn/gtyewfzvcb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.0kj1m.cn/gtyywfsirs.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yonumen.top/gtvdbkbwbn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangshuangyany.cn/gtyguepjkh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pengpengdd.cyou/gtxhpehbxd.html

Java: list.size();  map.size();  s.length()
来源：http://hz.gotoacloud.top/gtyqqddkgc.html

Go:   len(arr);  len(m)
来源：http://hz.shangyingyoupin.top/gtzwvtayyd.html

Ruby: x.length;  x.size
来源：http://hz.yueranfly.top/gttvpyhexk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yuanzhike.top/gtkynbdfym.html


<!-- 参考信息 -->