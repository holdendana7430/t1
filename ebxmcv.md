代发 wailian999

TS:   resp.ok;  resp.status
来源：http://hz.hywenlv.cn/gtjmsaqnzp.html

Java: resp.statusCode()
来源：http://hz.jinyuanbaomall.cn/gtzhbimtdz.html

Go:   resp.StatusCode
来源：http://hz.zhaomingkeji.xyz/gtnsbbezsz.html

Ruby: resp.code.to_i
来源：http://hz.dashuyun.cn/gttywxvqyn.html

C#:   (int)resp.StatusCode
来源：http://hz.ydjk.org.cn/gtwwdntzsy.html

[L08] 并发请求多个地址
来源：http://hz.0kj1m.cn/gthzllbrrt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj202588.top/gtrhvicsou.html

PHP:  curl_multi_init() 系列
来源：http://hz.fengsongda.top/gtidgkorvp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guannengcc.top/gtwdaxsvpc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxinkj.top/gtgflmepmc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shangyingyoupin.top/gtmqusipzp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.dashuyun.cn/gtaztgizvv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.fengsongda.top/gtimyxupeh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.dianchejie.cn/gtobhgdbzf.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtcfsqyjgb.html

M. 命令行 / 进程 / 环境
来源：http://hz.sxryk.cn/gtmzwvaesp.html

================================================================================
来源：http://hz.redwolf501.top/gtuzqjoiga.html

[M01] 读取命令行参数
来源：http://hz.wangdashe.top/gtovitiedn.html

Py:   sys.argv[1:]
来源：http://hz.0kj1m.cn/gtvgmrknga.html

PHP:  $argv;  $argc;
来源：http://hz.9152youxi.cn/gtuxqnswjo.html

JS:   process.argv.slice(2)
来源：http://hz.tian-w.cn/gteilmybtk.html

TS:   process.argv.slice(2)
来源：http://hz.jlsjyb.cn/gtbgwzyeji.html

Java: args 数组（main 方法参数）
来源：http://hz.andypj.xyz/gtevgidwaf.html

Go:   os.Args[1:]
来源：http://hz.yangfankeji.com/gtrngcrcki.html

Ruby: ARGV
来源：http://hz.tanke756.top/gtkesnbzni.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhiwuduotai.top/gtdnjnmbgp.html

[M02] 读取环境变量
来源：http://hz.pengpengdd.cyou/gtiouqjdqw.html

Py:   os.environ.get("HOME")
来源：http://hz.mhx1999.top/gtxcusdrmg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.aizwys.cn/gtazsxdmse.html

JS:   process.env.HOME
来源：http://hz.aizwys.cn/gtzxbgkbqt.html

TS:   process.env.HOME
来源：http://hz.feifeiyinyue.top/gtukrprftg.html

Java: System.getenv("HOME")
来源：http://hz.zdqjudy.top/gtgptfqzyd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hnxiangtu.top/gtmklrwzrh.html

Ruby: ENV["HOME"]
来源：http://hz.xingfuxueyuan.xyz/gtjwolpwbs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhongyouzk.top/gtktrlxibd.html

[M03] 执行外部命令
来源：http://hz.hongshengwenyu.top/gtaltpzibm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jianghu66.top/gtrexpsyoo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yanxiufei.cn/gtdszptmha.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shzxlz.cn/gtxfzkpses.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.haohaochexian.top/gtysacvift.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hongshengwenyu.top/gtwccgozey.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.fengsongda.top/gtpvyfbcor.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.redwolf501.top/gtdpewnlfm.html

C#:   Process.Start("ls", "-l");
来源：http://hz.svipenyu.cn/gtjwlohfyf.html

[M04] 获取当前工作目录
来源：http://hz.jqgfzy.top/gtildolsfz.html

Py:   os.getcwd()
来源：http://hz.ivvv.top/gtrofqngrx.html

PHP:  getcwd();
来源：http://hz.cashguo.top/gtxhaciebo.html

JS:   process.cwd()
来源：http://hz.yanxiufei.cn/gtjjomwsph.html

TS:   process.cwd()
来源：http://hz.shanyushiyangtech.top/gtfgxtfdwh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.andypj.xyz/gtuwrxcnqj.html

Go:   os.Getwd()
来源：http://hz.xinyue.icu/gtsespflqx.html

Ruby: Dir.pwd
来源：http://hz.shanyushiyangtech.top/gtojiehlvy.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sxryk.cn/gtaikguzjy.html

[M05] 设置退出码
来源：http://hz.fengsongda.top/gtedgwcudt.html

Py:   sys.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtgdpkrkky.html

PHP:  exit(1);
来源：http://hz.shanyushiyangtech.top/gtyizpmyep.html

JS:   process.exit(1)
来源：http://hz.dashuyun.cn/gtlavqknsc.html

TS:   process.exit(1)
来源：http://hz.guannengcc.top/gtueiflaqp.html

Java: System.exit(1)
来源：http://hz.wangshuangyany.cn/gtnanmhjca.html

Go:   os.Exit(1)
来源：http://hz.jqgufenzy.top/gtgoyppfiz.html

Ruby: exit 1
来源：http://hz.dashuyun.cn/gtmpacshbe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.wangdashe.top/gtzxpvuotl.html

[M06] 向标准错误输出
来源：http://hz.shanyushiyangkeji.top/gttdlsmgtw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nwbrower.top/gtvwzjnqol.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.redwolf501.top/gtxmfmmlxo.html

JS:   console.error("err")
来源：http://hz.jinyuanbaomall.cn/gttvzajjnm.html

TS:   console.error("err")
来源：http://hz.sweek.top/gtrmzshvps.html

Java: System.err.println("err")
来源：http://hz.ywan-chungtsiang.top/gtecjyxcug.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yonumen.top/gtehsakuce.html

Ruby: warn "err"
来源：http://hz.yuxming.cn/gtcnbcssor.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.aizwys.cn/gtrwbzmzqu.html

[M07] 判断是否为主入口
来源：http://hz.yangfankeji.com/gtibpkfmmf.html

Py:   if __name__ == "__main__":
来源：http://hz.fengsongda.top/gtheetbhkv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinyuanbaomall.cn/gtuysgffgw.html

JS:   require.main === module
来源：http://hz.chenzaomai.com/gtlfjyngvz.html

TS:   require.main === module
来源：http://hz.fzhhl.top/gtnwhcunto.html

Java: public static void main(String[] args)
来源：http://hz.yanxiufei.cn/gtalzkbugm.html

Go:   func main()
来源：http://hz.bjfxy.top/gtaflanbmd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinghuilouyu.cn/gtwvevvkjj.html

C#:   static void Main(string[] args)
来源：http://hz.jinyuanbaomall.cn/gtfidtdfyp.html

[M08] 获取系统与运行时信息
来源：http://hz.tianlin.xyz/gtpjlbngwf.html

Py:   platform.system();  platform.python_version()
来源：http://hz.andypj.xyz/gtqmjckwgg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xylfe.cn/gtkkbtjenr.html

JS:   process.platform;  process.version
来源：http://hz.snrcjt.cn/gtxwxtzhxe.html

TS:   process.platform;  process.version
来源：http://hz.hongshengwenyu.top/gtjuutepfq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gogol.net.cn/gtbnpamrar.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shuidangran.top/gtliddiwsy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yanxiufei.cn/gtsxqjrlik.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.gogol.net.cn/gthwlqjppb.html

================================================================================
来源：http://hz.daria6918.cn/gtluosrfwg.html

N. 数据结构与算法
来源：http://hz.jiagoushi.top/gtqjkapqkx.html

================================================================================
来源：http://hz.ivvv.top/gtfycmgjyi.html

[N01] 二分查找（有序数组）
来源：http://hz.zdqjudy.top/gtkaahlnaf.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hnxiangtu.top/gtaybyvvse.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yj20258.top/gtctrbygwr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xinyue.icu/gtcsovzibx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.meibo888.top/gtwwkffeqn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yuanzhike.top/gtfqmuvcbi.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtjaycexkk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sysykeji.top/gtdjhllslx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xinyue.icu/gttwleyiel.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.9152youxi.cn/gtuwpwfyhc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jqgufenzy.top/gtsjzcbhtt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.andypj.xyz/gthwezhhky.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guowangkeji.top/gtaoilulxh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zdqjudy.top/gtpknxxhmt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.guannengcc.top/gtsqtdrvmt.html

Go:   slices.Sort(arr)
来源：http://hz.zhongyouzk.top/gtbgklkclb.html

Ruby: arr.sort
来源：http://hz.pycfn.com/gtdmmpulzt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sxryk.cn/gtrjubelgt.html

[N03] 快速排序（分治示例）
来源：http://hz.ydjk.org.cn/gtsxwhhtat.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yangfankeji.com/gtwjyteqlm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.havefunace.top/gtofukfmna.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj202588.top/gtefpmemma.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.0kj1m.cn/gthdslxzkw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.daxiang520.top/gtvfqtfjut.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.fzhhl.top/gtuwlyvlyh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.daxiang520.top/gtauvtqahw.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xuanzx.com/gtgxnkiaia.html

[N04] 斐波那契数列
来源：http://hz.yueranfly.top/gtecsbpnzs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.chenjidiqi.icu/gteksmbdpw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.9152youxi.cn/gtmfmylmxq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yueranfly.top/gtvffqpipo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258.top/gtizingcbq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.daria6918.cn/gtvmbibujd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.redwolf501.top/gtiskqgtzd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jiagoushi.top/gtckjwhrcx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhaomingkeji.xyz/gtfoftmxps.html

[N05] 最大公约数
来源：http://hz.jinqigfzy.top/gtstxszumx.html

Py:   math.gcd(a, b)
来源：http://hz.zycfv.cn/gthgadydoo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tianlin.xyz/gtpcqhyhxb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yueranfly.top/gtpeutznxi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daria6918.cn/gtldzfldnq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.bjfxy.top/gtswlhrnra.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.tianlin.xyz/gtvwpmpbxf.html

Ruby: a.gcd(b)
来源：http://hz.snrcjt.cn/gtfgnsiqmz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jianghu66.top/gticuyzwud.html

[N06] 判断回文字符串
来源：http://hz.nanxinkj.top/gterkqrtxa.html

Py:   s == s[::-1]
来源：http://hz.yj202588.top/gtgjxuetno.html

PHP:  $s === strrev($s);
来源：http://hz.yvedp.cn/gtnpswqyfk.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhixingplan.top/gtxtkybmow.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhijiandao.cn/gtwxhythni.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.wangdashe.top/gtybuefmcv.html

Go:   // 双指针从两端比较
来源：http://hz.yangfankeji.com/gteackrxii.html

Ruby: s == s.reverse
来源：http://hz.yanxiufei.cn/gtwybjigxc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yj20258888.top/gtevpytfuu.html

[N07] 两数之和（返回下标）
来源：http://hz.aibaodan.cn/gtuzovbnwo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hnqzz.top/gtvnyzwwex.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.wangshuangyany.cn/gtbspcyrxp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gzhubu.top/gtuxqhouwb.html

TS:   // 手写 Map<string, number>
来源：http://hz.shuidangran.top/gtrfnkewtg.html

Java: // 手写 HashMap
来源：http://hz.zhongyouzk.top/gtvhxouedt.html

Go:   // 手写 map[int]int
来源：http://hz.yj20258888.top/gtwzcvofoh.html

Ruby: // 手写 Hash
来源：http://hz.pengpengdd.cyou/gtzdgtrvyp.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.feifeiyinyue.top/gtqwejkixc.html

[N08] 生成全排列
来源：http://hz.hammf.cn/gtmahpidsi.html

Py:   itertools.permutations(arr)
来源：http://hz.ybcxt.top/gthfaadfty.html

PHP:  // 手写递归交换
来源：http://hz.cqqwz.cn/gthkddzrcb.html

JS:   // 手写回溯递归
来源：http://hz.aibaodan.cn/gtfsypxnax.html

TS:   // 手写回溯递归
来源：http://hz.shzxlz.cn/gtbvrcufrk.html

Java: // 手写回溯递归
来源：http://hz.bjfxy.top/gttiekoqtd.html

Go:   // 手写回溯递归
来源：http://hz.yuanzhike.top/gtbsbircvh.html

Ruby: arr.permutation.to_a
来源：http://hz.jinqigufen.top/gtmesdfrbg.html

C#:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtlwbhieyc.html

[N09] 栈与队列
来源：http://hz.fzhhl.top/gtclcxbyzg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.aibaodan.cn/gtvvpjnygl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.fengsongda.top/gtirddluxc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.vqdsnc.cn/gtzxqrfpdd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.wangshuangyany.cn/gthnsdxvsx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.52xcode.cn/gtcwewnajm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinyuanbaomall.cn/gtmpsvvksp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shangyingyoupin.top/gtrgmybivr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shanyushiyangtech.top/gtelxosjic.html

[N10] 链表节点定义
来源：http://hz.jinqigfzy.top/gtqqhpmruj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.haohaochexian.top/gtorrmzefk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yj20258.top/gtzrnesibs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.birdmap.top/gtvlrtutmv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhijiandao.cn/gtpolainlx.html

Java: class Node { int v; Node next; }
来源：http://hz.dianchejie.cn/gtqqlnanju.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.redwolf501.top/gtndvaayvg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhiwuduotai.top/gtvsxjecst.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xingfuxueyuan.xyz/gtbcjufcrb.html

[N11] 二叉树中序遍历
来源：http://hz.chenlongwang.top/gtondxwrew.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.gotoacloud.top/gtwmkfhwwv.html

PHP:  // 手写递归函数
来源：http://hz.yj20258888.top/gtlhumnxlv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ivvv.top/gtaetxxosg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.316326.xyz/gtsdkgwgar.html

Java: // 手写递归
来源：http://hz.mhx1999.top/gtihigwaat.html

Go:   // 手写递归
来源：http://hz.shanyushiyangkeji.top/gtkzfpzsug.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.havefunace.top/gtzgkneabs.html

C#:   // 手写递归
来源：http://hz.yj20258.top/gtupnqzowe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xylfe.cn/gtrdrrppty.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.havefunace.top/gtdnwwnpbi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shanyushiyangtech.top/gtpflsoaoa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.meibo888.top/gtviqbenlv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xylfe.cn/gtqefwjpdr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.aizwys.cn/gtrbqkmeta.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhaomingkeji.xyz/gtnziikhar.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jiagoushi.top/gtpaijmita.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hywenlv.cn/gtjwdgfwhi.html

================================================================================
来源：http://hz.zhijiandao.cn/gtwanyqbnw.html

O. 并发与异步
来源：http://hz.fengsongda.top/gtopbdunad.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtptuedlrf.html

[O01] 启动一个线程
来源：http://hz.yueranfly.top/gtjcrzzmab.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.tanke756.top/gttkekggug.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hnqzz.top/gtpabyzgpx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.svipenyu.cn/gtlrfafjjl.html

TS:   // 同 JS
来源：http://hz.chenlongwang.top/gtunohxdye.html

Java: new Thread(() -> f()).start()
来源：http://hz.daria6918.cn/gtfsbaucfu.html

Go:   go f()
来源：http://hz.bjfxy.top/gtsgcjwhze.html

Ruby: Thread.new { f }
来源：http://hz.xuanzx.com/gtqbefxuwb.html

C#:   Task.Run(() => F());
来源：http://hz.ydzc1.top/gtddujjvux.html

[O02] 使用线程池
来源：http://hz.hongshengwenyu.top/gtmjdlxjfv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinqigfzy.top/gtabwzgito.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.bjfxy.top/gtlghwnskr.html

JS:   // worker_threads 线程池
来源：http://hz.zdqjudy.top/gtuaymhego.html

TS:   // worker_threads 线程池
来源：http://hz.ppjwa.cn/gtgmveoqzd.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ybcxt.top/gtzcxqelks.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhixingplan.top/gtkipfnavh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhiwuduotai.top/gttnshoybv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.c1oappe.top/gtxlixxvtq.html

[O03] 加锁保护共享数据
来源：http://hz.ybcxt.top/gtvbwirxdr.html

Py:   with lock: shared += 1
来源：http://hz.dianchejie.cn/gtzsmueytp.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.guannengcc.top/gtljpznduq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hysaishi.cn/gthbqyfsqs.html

TS:   // 同 JS
来源：http://hz.kuanghao11.cn/gttnjnsayo.html

Java: synchronized (this) { shared++; }
来源：http://hz.xuanzx.com/gtiindokjv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhoulong.xyz/gttzzcvbkk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.aizwys.cn/gtptaenjnz.html

C#:   lock (gate) { shared++; }
来源：http://hz.tianlin.xyz/gtloanvtfh.html

[O04] 定义异步函数并等待
来源：http://hz.zhiwuduotai.top/gtxhkgwsbf.html

Py:   async def f():⏎    await g()
来源：http://hz.ywan-chungtsiang.top/gtnttmndwr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.havefunace.top/gtbgylterj.html

JS:   async function f() { await g(); }
来源：http://hz.yj202588.top/gtilmcbckt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yj20258.top/gtwozibnsd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jiagoushi.top/gthurprxot.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jinqigufen.top/gtfxqnoiti.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.snrcjt.cn/gtlxkpoenh.html

C#:   async Task F() { await G(); }
来源：http://hz.yanxiufei.cn/gtjnepanyx.html

[O05] 并发执行并等待全部完成
来源：http://hz.hysaishi.cn/gtzgqxvyez.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cheryme.top/gtzahqnmdp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cucudq.cn/gtpdfgunxq.html

JS:   await Promise.all(tasks)
来源：http://hz.zhiwuduotai.top/gtowkmgunp.html

TS:   await Promise.all(tasks)
来源：http://hz.birdmap.top/gtanlymgau.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.sweek.top/gtumldfyxq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xylfe.cn/gtagkwnidz.html

Ruby: threads.map(&:join)
来源：http://hz.shanyushiyangtech.top/gtkfxkwdcz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.nanxuanxn.top/gtunjzmzwo.html

[O06] 使用进程池
来源：http://hz.yueranfly.top/gtqrknrzuk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zycfv.cn/gtxdbanqxq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.fengsongda.top/gtdhcarpuj.html

JS:   // child_process / cluster 模块
来源：http://hz.jyoumei.cn/gtxsvqsbpi.html

TS:   // child_process / cluster 模块
来源：http://hz.andypj.xyz/gtzpnizzto.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ydzc1.top/gtudqzjwdh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nwbrower.top/gtlbkereoa.html

Ruby: // fork 块
来源：http://hz.hammf.cn/gtagngcimi.html

C#:   Parallel.For
来源：http://hz.chenlongwang.top/gtsjqkwyiu.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gturydeour.html

P. 常用工具函数
来源：http://hz.fengsongda.top/gtrqtyfngs.html

================================================================================
来源：http://hz.zhengqikj.top/gtvyiosedc.html

[P01] 生成 UUID
来源：http://hz.pycfn.com/gtqivyqcsj.html

Py:   str(uuid.uuid4())
来源：http://hz.quarkkingdee.top/gtriauzqgg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yanxiufei.cn/gteofbqqhv.html

JS:   crypto.randomUUID()
来源：http://hz.nanxinkj.top/gtuvgsdnqr.html

TS:   crypto.randomUUID()
来源：http://hz.bjfxy.top/gtbdazhucn.html

Java: UUID.randomUUID().toString()
来源：http://hz.nanxinkj.top/gtncypmrij.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yangfankeji.com/gtzftpoawt.html

Ruby: SecureRandom.uuid
来源：http://hz.xziqi.cn/gtlxknnbdd.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xinyue.icu/gtoimpbaeo.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhijiandao.cn/gtipxalrnn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xingfuxueyuan.xyz/gtopxhpxln.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jqgfzy.top/gttuljsoho.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinyuanbaomall.cn/gtmwpmtusi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.316326.xyz/gtlmxzdxlk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.nanxinkj.top/gtpuqqwvor.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zdqjudy.top/gtgskhmote.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.gaohongyu789.top/gtvpvsjoey.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hysaishi.cn/gthmfssomm.html

[P03] 生成短随机字符串
来源：http://hz.hammf.cn/gtabfuoima.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cqqwz.cn/gtesyqbutw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.wangshuangyany.cn/gtytuabayv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dashuyun.cn/gtzbijjfxr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cashguo.top/gtfvkughyn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinqigufen.top/gtlhhgijxw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.tianlin.xyz/gtdfebxtju.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hongshengwenyu.top/gtdknoubsz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinghuilouyu.cn/gtpxkjmuhq.html

[P04] 求长度
来源：http://hz.birdmap.top/gtxszthqsg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ppjwa.cn/gtbjjeqthx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gttbkwgbta.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.smart0.xyz/gteudujyps.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ivvv.top/gtgavmlrsc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sweek.top/gtvlqdbxph.html

Go:   len(arr);  len(m)
来源：http://hz.hfpthk.cn/gtuefbmhrp.html

Ruby: x.length;  x.size
来源：http://hz.sufxvd.cn/gtewcfbwut.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.haohaochexian.top/gthqdzvnae.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jianghu66.top/gtibbbbvwu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.nanxinkj.top/gtlejxhaud.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.dashuyun.cn/gtibbmipvf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.tian-w.cn/gtrkouqngg.html


<!-- 参考信息 -->