代发 wailian999

C#:   (int)resp.StatusCode
来源：http://hz.ehwqpu.com/gtimijcoeu.html

[L08] 并发请求多个地址
来源：http://hz.yangfankeji.com/gtacttjbvv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhiwuduotai.top/gtnscetanx.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj20258888.top/gtqlmmpxng.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtdzxdmtgj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuetiantiany.cn/gtcrmojefo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yueranfly.top/gtkpjykhli.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.316326.xyz/gtmjpwmgcc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhiwuduotai.top/gtyrflurqz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.haohaochexian.top/gtfbfutpqb.html

================================================================================
来源：http://hz.chenzaomai.com/gtnccilzri.html

M. 命令行 / 进程 / 环境
来源：http://hz.jqgfzy.top/gthkdtzqwm.html

================================================================================
来源：http://hz.yueranfly.top/gtpynagzzo.html

[M01] 读取命令行参数
来源：http://hz.cqqwz.cn/gtyxptadat.html

Py:   sys.argv[1:]
来源：http://hz.sufxvd.cn/gtuookmobh.html

PHP:  $argv;  $argc;
来源：http://hz.hnqzz.top/gtlqqsnlln.html

JS:   process.argv.slice(2)
来源：http://hz.yangfankeji.com/gtliudspbt.html

TS:   process.argv.slice(2)
来源：http://hz.cucudq.cn/gtwbcmlcjn.html

Java: args 数组（main 方法参数）
来源：http://hz.guannengcc.top/gtwvoclbfs.html

Go:   os.Args[1:]
来源：http://hz.feifeiyinyue.top/gtqghqfusu.html

Ruby: ARGV
来源：http://hz.haohaochexian.top/gtfthppnxv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xylfe.cn/gtpzdxfxsd.html

[M02] 读取环境变量
来源：http://hz.yueranfly.top/gtlbqbyqzr.html

Py:   os.environ.get("HOME")
来源：http://hz.yongpay.top/gtbimbxshs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yuanzhike.top/gtdljkedhw.html

JS:   process.env.HOME
来源：http://hz.shuidangran.top/gtmwdhifyf.html

TS:   process.env.HOME
来源：http://hz.hammf.cn/gtkbckwefq.html

Java: System.getenv("HOME")
来源：http://hz.yangfankeji.com/gtypjnvupv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hnxiangtu.top/gtnahwszmh.html

Ruby: ENV["HOME"]
来源：http://hz.vqdsnc.cn/gtjsdjlinl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.bjfxy.top/gtfbjkxqry.html

[M03] 执行外部命令
来源：http://hz.jlsjyb.cn/gtazbtyvxr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cqqwz.cn/gtyqumsdqk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ppjwa.cn/gtpwraewyj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.gaohongyu789.top/gtlhrbyeqq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zycfv.cn/gtkfqxzanq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ybcxt.top/gtypfrvsdc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jqgufenzy.top/gtmuitlnun.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.quarkkingdee.top/gtyveqcray.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ywan-chungtsiang.top/gtlgenpeqj.html

[M04] 获取当前工作目录
来源：http://hz.hnxiangtu.top/gtlcdqpoux.html

Py:   os.getcwd()
来源：http://hz.yj202588.top/gtaqyjpeqp.html

PHP:  getcwd();
来源：http://hz.xuetiantiany.cn/gtdaanerqk.html

JS:   process.cwd()
来源：http://hz.shangyingyoupin.top/gttsgpdkfa.html

TS:   process.cwd()
来源：http://hz.jqgufenzy.top/gtgkabsalv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.meibo888.top/gtphzfhwdr.html

Go:   os.Getwd()
来源：http://hz.fzhhl.top/gtfioltsyy.html

Ruby: Dir.pwd
来源：http://hz.yueranfly.top/gtnicntxss.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yonumen.top/gtflzbsjkh.html

[M05] 设置退出码
来源：http://hz.yangfankeji.com/gtxixnjole.html

Py:   sys.exit(1)
来源：http://hz.zhixingplan.top/gtmajwrusa.html

PHP:  exit(1);
来源：http://hz.zhixingplan.top/gtjfwiytha.html

JS:   process.exit(1)
来源：http://hz.sysykeji.top/gttcwzooln.html

TS:   process.exit(1)
来源：http://hz.gotoacloud.top/gtbiagbqcz.html

Java: System.exit(1)
来源：http://hz.jinqigufen.top/gtvqqwsfio.html

Go:   os.Exit(1)
来源：http://hz.tian-w.cn/gtprvqdofx.html

Ruby: exit 1
来源：http://hz.gotoacloud.top/gtvobxtimt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.bjfxy.top/gtmtjvwvjo.html

[M06] 向标准错误输出
来源：http://hz.gaohongyu789.top/gtxrdlleqm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gzhubu.top/gtwhavgntf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hfpthk.cn/gtshnutpfs.html

JS:   console.error("err")
来源：http://hz.smart0.xyz/gtciztonjv.html

TS:   console.error("err")
来源：http://hz.vqdsnc.cn/gtnxpklhfz.html

Java: System.err.println("err")
来源：http://hz.wangdashe.top/gtzjjvdgog.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shzxlz.cn/gtkmuucygq.html

Ruby: warn "err"
来源：http://hz.0kj1m.cn/gtgsevxzkq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cashguo.top/gtwsuvxuvb.html

[M07] 判断是否为主入口
来源：http://hz.nwbrower.top/gtrivhuqbt.html

Py:   if __name__ == "__main__":
来源：http://hz.jqgfzy.top/gtobdmqxxf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gaohongyu789.top/gtkigftywp.html

JS:   require.main === module
来源：http://hz.kuanghao11.cn/gtpsgjyxwm.html

TS:   require.main === module
来源：http://hz.svipenyu.cn/gtskomvzcl.html

Java: public static void main(String[] args)
来源：http://hz.yonumen.top/gtocnesubq.html

Go:   func main()
来源：http://hz.sysykeji.top/gtahywmawu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.316326.xyz/gtqbquwxwd.html

C#:   static void Main(string[] args)
来源：http://hz.daria6918.cn/gtpqdptezl.html

[M08] 获取系统与运行时信息
来源：http://hz.sweek.top/gtkxriwrwz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.snrcjt.cn/gttqvprxbf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gzhubu.top/gtbprpbncx.html

JS:   process.platform;  process.version
来源：http://hz.sysykeji.top/gttwrayodd.html

TS:   process.platform;  process.version
来源：http://hz.xingfuxueyuan.xyz/gteijdsfgc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.smart0.xyz/gtgevoccte.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhiwuduotai.top/gtuvlxfhhp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yj20258888.top/gtxqggqgkw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.guannengcc.top/gtelkdfmto.html

================================================================================
来源：http://hz.xuetiantiany.cn/gthkxkgevu.html

N. 数据结构与算法
来源：http://hz.daria6918.cn/gtzcitobjx.html

================================================================================
来源：http://hz.sufxvd.cn/gtuwrcdicj.html

[N01] 二分查找（有序数组）
来源：http://hz.yangfankeji.com/gtojndywuw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.cashguo.top/gtnzmnbajk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jyoumei.cn/gtdlooptxq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xingfuxueyuan.xyz/gtekkeffiy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zdqjudy.top/gtgcsdjedg.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtjwhqpczv.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinghuilouyu.cn/gttuhcsiml.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xylfe.cn/gtolwnqweo.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xinyue.icu/gtecjdyren.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.fengsongda.top/gtrovoafpw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuanzx.com/gtasbfrruh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.dianchejie.cn/gtupyasase.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhixingplan.top/gtwuikrubq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtkyddjzgx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hnxiangtu.top/gtjbwfbsql.html

Go:   slices.Sort(arr)
来源：http://hz.yongpay.top/gtktehelal.html

Ruby: arr.sort
来源：http://hz.52xcode.cn/gtggnuvbnr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hongshengwenyu.top/gtgxkijgda.html

[N03] 快速排序（分治示例）
来源：http://hz.sxryk.cn/gtutwrktxw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yanxiufei.cn/gtcpjwgjcr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tianlin.xyz/gtwhmczgeu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ivvv.top/gtrayqimhb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zdqjudy.top/gtcnsbvffz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.kuanghao11.cn/gtjrpbradj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.pycfn.com/gtsbvyaway.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jlsjyb.cn/gtovnknuay.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cucudq.cn/gtxhchbtnm.html

[N04] 斐波那契数列
来源：http://hz.sweek.top/gtpmlbwifi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.fengsongda.top/gtjufagltf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jqgfzy.top/gtqmxmpyvm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuanzhike.top/gtqoimgnbi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.quarkkingdee.top/gtwgjhycxp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hysaishi.cn/gtdiachine.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.c1oappe.top/gtfngfnzgt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cucudq.cn/gtfzutoegz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.0kj1m.cn/gttaakevkb.html

[N05] 最大公约数
来源：http://hz.hysaishi.cn/gtndeqmhpm.html

Py:   math.gcd(a, b)
来源：http://hz.tian-w.cn/gtlacryttq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.chenlongwang.top/gtisjmofvl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydjk.org.cn/gtroxernzf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigfzy.top/gtttshmzff.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.guannengcc.top/gtzwtuczaz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.c1oappe.top/gtpjhfuawi.html

Ruby: a.gcd(b)
来源：http://hz.xingfuxueyuan.xyz/gtfwmxocad.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shanyushiyangkeji.top/gtdswuhtka.html

[N06] 判断回文字符串
来源：http://hz.svipenyu.cn/gtskhuryja.html

Py:   s == s[::-1]
来源：http://hz.vqdsnc.cn/gtfepfscpv.html

PHP:  $s === strrev($s);
来源：http://hz.ybcxt.top/gtvduqdljt.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtyevctfpl.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtcmmpiztv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhoulong.xyz/gtczfrkjie.html

Go:   // 双指针从两端比较
来源：http://hz.havefunace.top/gtnafqnomx.html

Ruby: s == s.reverse
来源：http://hz.hammf.cn/gtupdkacff.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhijiandao.cn/gtpuanetdb.html

[N07] 两数之和（返回下标）
来源：http://hz.shangyingyoupin.top/gttxbwtfxp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhiwuduotai.top/gtdcifkvgx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jianghu66.top/gttfuhiuxo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yj20258.top/gtmrcchvkj.html

TS:   // 手写 Map<string, number>
来源：http://hz.hnxiangtu.top/gtwzfeetfn.html

Java: // 手写 HashMap
来源：http://hz.smart0.xyz/gtqfnlchdt.html

Go:   // 手写 map[int]int
来源：http://hz.wangshuangyany.cn/gtasksgqqd.html

Ruby: // 手写 Hash
来源：http://hz.jiagoushi.top/gtlwjduvjh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinqigfzy.top/gtpxawygwa.html

[N08] 生成全排列
来源：http://hz.jianghu66.top/gtylgndvyf.html

Py:   itertools.permutations(arr)
来源：http://hz.cucudq.cn/gtwdgprmsc.html

PHP:  // 手写递归交换
来源：http://hz.wangdashe.top/gtasnsvwra.html

JS:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gtyccqmxzi.html

TS:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtgcshbpda.html

Java: // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtjzktewog.html

Go:   // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtfcbzpskt.html

Ruby: arr.permutation.to_a
来源：http://hz.jinyuanbaomall.cn/gtxxrhdipv.html

C#:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gtkogssfpp.html

[N09] 栈与队列
来源：http://hz.yuxming.cn/gtifcjmnuk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jqgfzy.top/gtcljcamzx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.daxiang520.top/gtadjtlkgu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zycfv.cn/gtorflqrlc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.iojbl.cn/gtcnoxreoc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yj202588.top/gtnobhnnrc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.guowangkeji.top/gtioduunkf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yj202588.top/gtdjrgtmif.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.tian-w.cn/gtmvqybcfu.html

[N10] 链表节点定义
来源：http://hz.hywenlv.cn/gtamgriowl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shzxlz.cn/gtymlrruge.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yvedp.cn/gtphzwlgus.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.guowangkeji.top/gtbadymsbl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hammf.cn/gtffguwegx.html

Java: class Node { int v; Node next; }
来源：http://hz.jianghu66.top/gtsdffbsff.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yj202588.top/gtpqpdyleg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xuanzx.com/gtefzrztgm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.quarkkingdee.top/gtbykkzahq.html

[N11] 二叉树中序遍历
来源：http://hz.xziqi.cn/gtauosqqnx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jiagoushi.top/gtpaitpgjx.html

PHP:  // 手写递归函数
来源：http://hz.yj20258.top/gthnofffzj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinghuilouyu.cn/gtthmnwqdi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgfzy.top/gtmeiqipln.html

Java: // 手写递归
来源：http://hz.hongshengwenyu.top/gtwmjmaaus.html

Go:   // 手写递归
来源：http://hz.ppjwa.cn/gtonmxjovr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xuanzx.com/gthsduafdg.html

C#:   // 手写递归
来源：http://hz.yuxming.cn/gtuhbxjorc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.daxiang520.top/gtnvnfzigv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.sweek.top/gtpyyfwkyq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhoulong.xyz/gtxhhajule.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.svipenyu.cn/gtegiwbnce.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.fengsongda.top/gtcirvrsyk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fzhhl.top/gtlcvyqkzq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.meibo888.top/gtqcxajoou.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yonumen.top/gtwurrcoao.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xingfuxueyuan.xyz/gtiqkmjdiy.html

================================================================================
来源：http://hz.yj20258888.top/gtgwvaimxo.html

O. 并发与异步
来源：http://hz.andypj.xyz/gtsbeuwzsi.html

================================================================================
来源：http://hz.daria6918.cn/gtebkeolbs.html

[O01] 启动一个线程
来源：http://hz.chenjidiqi.icu/gtwfyvtvca.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.svipenyu.cn/gtlzlpxqxc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yj20258.top/gtdpifefkp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yj202588.top/gteblblymz.html

TS:   // 同 JS
来源：http://hz.ydjk.org.cn/gtlixbiram.html

Java: new Thread(() -> f()).start()
来源：http://hz.9152youxi.cn/gtmqxkxzbc.html

Go:   go f()
来源：http://hz.52xcode.cn/gtvyhytiji.html

Ruby: Thread.new { f }
来源：http://hz.zhongyouzk.top/gtketyokkp.html

C#:   Task.Run(() => F());
来源：http://hz.yanxiufei.cn/gtdruqteds.html

[O02] 使用线程池
来源：http://hz.dianchejie.cn/gtvllhxefa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhixingplan.top/gtzezcronn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sweek.top/gtdhykcwzw.html

JS:   // worker_threads 线程池
来源：http://hz.guowangkeji.top/gtqbidgeuw.html

TS:   // worker_threads 线程池
来源：http://hz.wangshuangyany.cn/gtyhztamfo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hammf.cn/gtaxcoqreg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gogol.net.cn/gtfmnwcsbo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhoulong.xyz/gtqbyhdlqk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hywenlv.cn/gtrmhthyob.html

[O03] 加锁保护共享数据
来源：http://hz.cashguo.top/gteqhlnmxx.html

Py:   with lock: shared += 1
来源：http://hz.xinyue.icu/gtgthonqhe.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.gotoacloud.top/gtqtwaleal.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhijiandao.cn/gtpwyqlwpv.html

TS:   // 同 JS
来源：http://hz.daria6918.cn/gtfbiinwtq.html

Java: synchronized (this) { shared++; }
来源：http://hz.sysykeji.top/gtrzefrwed.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shanyushiyangtech.top/gtzvlhrvcb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinqigufen.top/gtqxrmhmuo.html

C#:   lock (gate) { shared++; }
来源：http://hz.yuxming.cn/gtdmwwfvxj.html

[O04] 定义异步函数并等待
来源：http://hz.hnxiangtu.top/gtelzbkbkg.html

Py:   async def f():⏎    await g()
来源：http://hz.sweek.top/gtcmxsfhnb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.guowangkeji.top/gtlunnbhus.html

JS:   async function f() { await g(); }
来源：http://hz.jyoumei.cn/gtckqfiqja.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zdqjudy.top/gtrjpdycab.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gogol.net.cn/gtavjlyops.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jqgfzy.top/gtidxilbrf.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.sweek.top/gtgrqkihfz.html

C#:   async Task F() { await G(); }
来源：http://hz.c1oappe.top/gtxntwkklx.html

[O05] 并发执行并等待全部完成
来源：http://hz.ivvv.top/gtyvzrxlxq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zdqjudy.top/gtiueazzid.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.daxiang520.top/gtrdodlsro.html

JS:   await Promise.all(tasks)
来源：http://hz.c1oappe.top/gtbnjejaeu.html

TS:   await Promise.all(tasks)
来源：http://hz.0kj1m.cn/gtfzlymkct.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.nanxuanxn.top/gtqolgntvt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jqgfzy.top/gtccrhlfpi.html

Ruby: threads.map(&:join)
来源：http://hz.jinqigfzy.top/gtpldlgbxs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhongyouzk.top/gtxlcpkysq.html

[O06] 使用进程池
来源：http://hz.nwbrower.top/gtikbrxjqs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.sweek.top/gtgjdogpqq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.dashuyun.cn/gtwcxdedlw.html

JS:   // child_process / cluster 模块
来源：http://hz.dashuyun.cn/gtotjsandg.html

TS:   // child_process / cluster 模块
来源：http://hz.shangyingyoupin.top/gtrjzojxkr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jyoumei.cn/gtnloawzwh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ybcxt.top/gthwdwomme.html

Ruby: // fork 块
来源：http://hz.jinyuanbaomall.cn/gtytdbllvo.html

C#:   Parallel.For
来源：http://hz.dashuyun.cn/gtuitlosir.html

================================================================================
来源：http://hz.bjfxy.top/gtsjofmmsu.html

P. 常用工具函数
来源：http://hz.jinghuilouyu.cn/gtlsnzxpkx.html

================================================================================
来源：http://hz.yongpay.top/gtdptgtiwm.html

[P01] 生成 UUID
来源：http://hz.ydzc1.top/gtcgklaslu.html

Py:   str(uuid.uuid4())
来源：http://hz.zdqjudy.top/gtodbwllnm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.nanxuanxn.top/gtvvbizzpm.html

JS:   crypto.randomUUID()
来源：http://hz.andypj.xyz/gtilqpyddq.html

TS:   crypto.randomUUID()
来源：http://hz.fengsongda.top/gtlzzpplsw.html

Java: UUID.randomUUID().toString()
来源：http://hz.meibo888.top/gtzjlhipgc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cucudq.cn/gtmukuykry.html

Ruby: SecureRandom.uuid
来源：http://hz.gogol.net.cn/gthostxrsx.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ivvv.top/gtsugjliqg.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hfpthk.cn/gtsipplrtc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cqqwz.cn/gtrojjfvmo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.fengsongda.top/gtqhovkpfm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.andypj.xyz/gtdlrmbsuj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ppjwa.cn/gtmbmqrraj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gzhubu.top/gtddudrwio.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cheryme.top/gtgpqlbewi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cqqwz.cn/gtypuyymqm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jqgfzy.top/gtzgnhzfer.html

[P03] 生成短随机字符串
来源：http://hz.zhiwuduotai.top/gtcgginfsn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.daria6918.cn/gtjmxuqneu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.haohaochexian.top/gtziexauvr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xziqi.cn/gtkvptqswg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.aizwys.cn/gtjeeymbaa.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hnxiangtu.top/gtxazcihjr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yonumen.top/gtmddwbokm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.52xcode.cn/gtbjdmkyah.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.svipenyu.cn/gtraqpxjef.html

[P04] 求长度
来源：http://hz.quarkkingdee.top/gtzrecvpzr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xuetiantiany.cn/gtujlpwswl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cqqwz.cn/gtpbjplipw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nanxinkj.top/gtlxdngfny.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shuidangran.top/gtmvfkcpas.html

Java: list.size();  map.size();  s.length()
来源：http://hz.pycfn.com/gtcdiuimei.html

Go:   len(arr);  len(m)
来源：http://hz.smart0.xyz/gtzwjbyuft.html

Ruby: x.length;  x.size
来源：http://hz.jinqigfzy.top/gtzqdnbgnr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.tian-w.cn/gtyiajnprw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.haohaochexian.top/gttcinmwas.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ydzc1.top/gtaaebsbzn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhiwuduotai.top/gtkmdbbmao.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xylfe.cn/gtbmfejkzp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xziqi.cn/gtjwjudjix.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.quarkkingdee.top/gtyfjqpfpk.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jinqigufen.top/gtkaqgraff.html

Ruby: a == b
来源：http://hz.sufxvd.cn/gtfmdxdtes.html


<!-- 参考信息 -->