代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxinkj.top/gtdlxzptdz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangdashe.top/gtdedzfxln.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.316326.xyz/gtuymyablx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhixingplan.top/gtvpqbztou.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hywenlv.cn/gtzlnaekhu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.chenlongwang.top/gtyowapdyr.html

================================================================================
来源：http://hz.aizwys.cn/gtwvxgymwc.html

M. 命令行 / 进程 / 环境
来源：http://hz.ydzc1.top/gtuwaqyggt.html

================================================================================
来源：http://hz.hongshengwenyu.top/gteisijkaa.html

[M01] 读取命令行参数
来源：http://hz.redwolf501.top/gtpdovpycz.html

Py:   sys.argv[1:]
来源：http://hz.zhengqikj.top/gtgaagozky.html

PHP:  $argv;  $argc;
来源：http://hz.ppjwa.cn/gtmxxjhywv.html

JS:   process.argv.slice(2)
来源：http://hz.jqgufenzy.top/gtpjqibmpy.html

TS:   process.argv.slice(2)
来源：http://hz.gogol.net.cn/gtbizbmqmm.html

Java: args 数组（main 方法参数）
来源：http://hz.jyoumei.cn/gtfpbbrtny.html

Go:   os.Args[1:]
来源：http://hz.daxiang520.top/gtbctxpzsk.html

Ruby: ARGV
来源：http://hz.zycfv.cn/gtgrdwhpef.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jiagoushi.top/gttmfxiuhi.html

[M02] 读取环境变量
来源：http://hz.pycfn.com/gtfqawzdfu.html

Py:   os.environ.get("HOME")
来源：http://hz.xingfuxueyuan.xyz/gtxnxvdzav.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.svipenyu.cn/gtzdvicuau.html

JS:   process.env.HOME
来源：http://hz.kuanghao11.cn/gtclhkonph.html

TS:   process.env.HOME
来源：http://hz.xziqi.cn/gtogehfpcm.html

Java: System.getenv("HOME")
来源：http://hz.jqgfzy.top/gtiakoawfd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhengqikj.top/gtbtcikdyr.html

Ruby: ENV["HOME"]
来源：http://hz.tian-w.cn/gtdajalhdb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jianghu66.top/gtocqvbtku.html

[M03] 执行外部命令
来源：http://hz.svipenyu.cn/gtttllajuv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.chenzaomai.com/gtdxozigab.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhoulong.xyz/gtewlvgncq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hongshengwenyu.top/gtgfhpvuey.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ybcxt.top/gtfgizpajo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinqigfzy.top/gtgehsgwvn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.svipenyu.cn/gtpubgmyra.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.nanxinkj.top/gtwkwyqxow.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shangyingyoupin.top/gtojtkciyr.html

[M04] 获取当前工作目录
来源：http://hz.zhoulong.xyz/gtdamagkhp.html

Py:   os.getcwd()
来源：http://hz.xuanzx.com/gtpkzqqari.html

PHP:  getcwd();
来源：http://hz.jianghu66.top/gttzjoempj.html

JS:   process.cwd()
来源：http://hz.9152youxi.cn/gtxdmyayxr.html

TS:   process.cwd()
来源：http://hz.c1oappe.top/gtmlczlpzf.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sysykeji.top/gtqwwfydgf.html

Go:   os.Getwd()
来源：http://hz.smart0.xyz/gtppmvbvli.html

Ruby: Dir.pwd
来源：http://hz.guowangkeji.top/gthdusuvsj.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cdnleiting.top/gtywfnuizf.html

[M05] 设置退出码
来源：http://hz.kuanghao11.cn/gtcxrylkak.html

Py:   sys.exit(1)
来源：http://hz.gotoacloud.top/gthlhtuqhx.html

PHP:  exit(1);
来源：http://hz.gaohongyu789.top/gtbfrmdayz.html

JS:   process.exit(1)
来源：http://hz.52xcode.cn/gtgeteejhl.html

TS:   process.exit(1)
来源：http://hz.chenlongwang.top/gtuoxydspn.html

Java: System.exit(1)
来源：http://hz.birdmap.top/gtwlwgdbkq.html

Go:   os.Exit(1)
来源：http://hz.wangdashe.top/gtbaxexerm.html

Ruby: exit 1
来源：http://hz.andypj.xyz/gtwsjecnul.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.quarkkingdee.top/gtgkssckgw.html

[M06] 向标准错误输出
来源：http://hz.hfpthk.cn/gtyekkjhia.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sxryk.cn/gtqblnhmfw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.tanke756.top/gtnaystiju.html

JS:   console.error("err")
来源：http://hz.jlsjyb.cn/gtkvunhjpj.html

TS:   console.error("err")
来源：http://hz.cqqwz.cn/gtquhesmzb.html

Java: System.err.println("err")
来源：http://hz.andypj.xyz/gtojujseoh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xingfuxueyuan.xyz/gtfgvstfzg.html

Ruby: warn "err"
来源：http://hz.jinghuilouyu.cn/gtefpbokhv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xziqi.cn/gtgvlsqdjh.html

[M07] 判断是否为主入口
来源：http://hz.ehwqpu.com/gtacvfbxce.html

Py:   if __name__ == "__main__":
来源：http://hz.smart0.xyz/gtbylseqmz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.pengpengdd.cyou/gtsfpyjhvm.html

JS:   require.main === module
来源：http://hz.xylfe.cn/gtlcthikey.html

TS:   require.main === module
来源：http://hz.wangshuangyany.cn/gtdquwtnwu.html

Java: public static void main(String[] args)
来源：http://hz.jianghu66.top/gtzczkkzpb.html

Go:   func main()
来源：http://hz.yanxiufei.cn/gtigoztexl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.daxiang520.top/gtlocegdvb.html

C#:   static void Main(string[] args)
来源：http://hz.guowangkeji.top/gtywewttec.html

[M08] 获取系统与运行时信息
来源：http://hz.jlsjyb.cn/gtujvumgun.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xuanzx.com/gthamplpbi.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.daxiang520.top/gtqqwkpqdy.html

JS:   process.platform;  process.version
来源：http://hz.yongpay.top/gtwqsupjyk.html

TS:   process.platform;  process.version
来源：http://hz.ivvv.top/gtsuocdzpb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinqigfzy.top/gttztnawlx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yuxming.cn/gtzaeqctdo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gzhubu.top/gtiwddufbc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.pengpengdd.cyou/gtdxxccexz.html

================================================================================
来源：http://hz.birdmap.top/gtcsicvvyh.html

N. 数据结构与算法
来源：http://hz.pycfn.com/gtwaphlgxl.html

================================================================================
来源：http://hz.guannengcc.top/gtbyebxawj.html

[N01] 二分查找（有序数组）
来源：http://hz.jqgufenzy.top/gtwllnhnlu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.fengsongda.top/gthozntbgo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.haohaochexian.top/gtljbrksxo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cucudq.cn/gtacberhty.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gotoacloud.top/gtftepkurb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zycfv.cn/gttaeuzvcu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ivvv.top/gtdubtoxwa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.chenzaomai.com/gtdokkzlhg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shuidangran.top/gtjykmpxeq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhixingplan.top/gtcsockklc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhijiandao.cn/gtlpdxiwgm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.bjfxy.top/gtroilticv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinyuanbaomall.cn/gtaxlthfzz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.vqdsnc.cn/gtcaucdcll.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yuxming.cn/gtdzyaooyj.html

Go:   slices.Sort(arr)
来源：http://hz.xuetiantiany.cn/gtrypqxvfj.html

Ruby: arr.sort
来源：http://hz.ydjk.org.cn/gtkturizog.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhiwuduotai.top/gtrdlhcshp.html

[N03] 快速排序（分治示例）
来源：http://hz.sysykeji.top/gtuztcrees.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hnxiangtu.top/gtatnmnqjt.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhaomingkeji.xyz/gtoilbekyk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhongyouzk.top/gtxpdgisox.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.vqdsnc.cn/gtwcpezvhn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tanke756.top/gtxjvvvnpi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jqgfzy.top/gttswbuyas.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenjidiqi.icu/gtfnmklqyg.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhijiandao.cn/gtoumnkupu.html

[N04] 斐波那契数列
来源：http://hz.redwolf501.top/gtxlgibxzz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xuanzx.com/gtzwvjzume.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sufxvd.cn/gtpwyocuca.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pycfn.com/gtygzsykqx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuxming.cn/gtertokomh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.guannengcc.top/gtrnvsapjk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.dashuyun.cn/gtwpljssyr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj202588.top/gtniobegri.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xuanzx.com/gtfxrnlqbp.html

[N05] 最大公约数
来源：http://hz.zhijiandao.cn/gtjfovzmvg.html

Py:   math.gcd(a, b)
来源：http://hz.dashuyun.cn/gtwzdvvwgo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.316326.xyz/gtxwszvrdf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jiagoushi.top/gthprrakko.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tanke756.top/gtzlmqlcsw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xziqi.cn/gtyyumjhdi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.tian-w.cn/gtajhljyxq.html

Ruby: a.gcd(b)
来源：http://hz.vqdsnc.cn/gtsfmoysyz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zdqjudy.top/gtudabyfiq.html

[N06] 判断回文字符串
来源：http://hz.chenzaomai.com/gtpxoggurq.html

Py:   s == s[::-1]
来源：http://hz.pycfn.com/gtxmewjlma.html

PHP:  $s === strrev($s);
来源：http://hz.ydjk.org.cn/gtoicdawkg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yvedp.cn/gtvohkmtsu.html

TS:   s === [...s].reverse().join("")
来源：http://hz.iojbl.cn/gtvjmtuqst.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinyuanbaomall.cn/gtpskbbkzh.html

Go:   // 双指针从两端比较
来源：http://hz.zhixingplan.top/gtgzrlarmk.html

Ruby: s == s.reverse
来源：http://hz.tian-w.cn/gtguxznjgl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tanke756.top/gthdguozfp.html

[N07] 两数之和（返回下标）
来源：http://hz.sweek.top/gtxmhgoxqx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.quarkkingdee.top/gtuamwskkv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sweek.top/gtdwvoksko.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hnqzz.top/gtahnztest.html

TS:   // 手写 Map<string, number>
来源：http://hz.xuanzx.com/gtltcawlew.html

Java: // 手写 HashMap
来源：http://hz.mhx1999.top/gtfmrmzuoq.html

Go:   // 手写 map[int]int
来源：http://hz.shanyushiyangkeji.top/gtpieykxby.html

Ruby: // 手写 Hash
来源：http://hz.yuanzhike.top/gtetnwouom.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yj20258888.top/gturqtclkf.html

[N08] 生成全排列
来源：http://hz.pengpengdd.cyou/gtmwuzqvzf.html

Py:   itertools.permutations(arr)
来源：http://hz.jinghuilouyu.cn/gtqhgmlxrr.html

PHP:  // 手写递归交换
来源：http://hz.yongpay.top/gtuqofigjq.html

JS:   // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtqgriuqck.html

TS:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtuzdxojco.html

Java: // 手写回溯递归
来源：http://hz.xuanzx.com/gtsfycvzes.html

Go:   // 手写回溯递归
来源：http://hz.ppjwa.cn/gticsfkxst.html

Ruby: arr.permutation.to_a
来源：http://hz.sweek.top/gthkmsyjru.html

C#:   // 手写回溯递归
来源：http://hz.ehwqpu.com/gtekvjobpo.html

[N09] 栈与队列
来源：http://hz.ydzc1.top/gtfebwyhlw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hfpthk.cn/gtgfhiegww.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hnxiangtu.top/gteioicyki.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hfpthk.cn/gtssumkltd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.sxryk.cn/gtbwzzwtnf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.quarkkingdee.top/gtxbqxvtpl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hysaishi.cn/gtppcbmtyt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.nanxinkj.top/gtlbvjlymp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ybcxt.top/gtcyrajbcs.html

[N10] 链表节点定义
来源：http://hz.hammf.cn/gtoqjmcqgd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yuxming.cn/gtpshlfene.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhixingplan.top/gthgazrpeh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cdnleiting.top/gtvjkofdrx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhoulong.xyz/gtldtqqfeo.html

Java: class Node { int v; Node next; }
来源：http://hz.52xcode.cn/gtyfvkczqj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhongyouzk.top/gtryaavlty.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.havefunace.top/gtjthyonff.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zycfv.cn/gtfbqefyal.html

[N11] 二叉树中序遍历
来源：http://hz.jinqigfzy.top/gtqmwcqflx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shanyushiyangkeji.top/gtqnjtairj.html

PHP:  // 手写递归函数
来源：http://hz.cqqwz.cn/gtcnrswjcp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yonumen.top/gtkaewzzhn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ybcxt.top/gtmrpqjvzp.html

Java: // 手写递归
来源：http://hz.nanxuanxn.top/gtrxexfhzq.html

Go:   // 手写递归
来源：http://hz.cashguo.top/gtjesubsuo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yuanzhike.top/gtvymmvzdt.html

C#:   // 手写递归
来源：http://hz.yuxming.cn/gtclnrkloo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hnqzz.top/gtrglssalw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.vqdsnc.cn/gtlcvknuuo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.kuanghao11.cn/gthwubxldz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenzaomai.com/gtpzgfxhjs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cqqwz.cn/gtqgazjsem.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xylfe.cn/gtuloswjdw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.smart0.xyz/gtoryxyrtc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.wangshuangyany.cn/gtkhfzjxcf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cashguo.top/gtjuhgofae.html

================================================================================
来源：http://hz.zhengqikj.top/gtbmapvhcy.html

O. 并发与异步
来源：http://hz.birdmap.top/gtqlptbpxe.html

================================================================================
来源：http://hz.daxiang520.top/gtkxstmbef.html

[O01] 启动一个线程
来源：http://hz.andypj.xyz/gtorqlpiwe.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cqqwz.cn/gtokcbpicm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinqigufen.top/gtbyrdyukk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yuanzhike.top/gthhegomwm.html

TS:   // 同 JS
来源：http://hz.gogol.net.cn/gtczcmlkpi.html

Java: new Thread(() -> f()).start()
来源：http://hz.ybcxt.top/gtbctvkowr.html

Go:   go f()
来源：http://hz.316326.xyz/gtlwzfvvcb.html

Ruby: Thread.new { f }
来源：http://hz.mhx1999.top/gtuchjerip.html

C#:   Task.Run(() => F());
来源：http://hz.nanxuanxn.top/gtjegcvqui.html

[O02] 使用线程池
来源：http://hz.hfpthk.cn/gtampexbqc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cashguo.top/gtgikpybsi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.316326.xyz/gtwzduxqsx.html

JS:   // worker_threads 线程池
来源：http://hz.ppjwa.cn/gtmlqgjxcu.html

TS:   // worker_threads 线程池
来源：http://hz.tianlin.xyz/gtgaxhzbei.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hfpthk.cn/gtozxddssb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yangfankeji.com/gthyquyncp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.chenzaomai.com/gtwibmwmwb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.andypj.xyz/gtmblphitv.html

[O03] 加锁保护共享数据
来源：http://hz.0kj1m.cn/gtrwuswwls.html

Py:   with lock: shared += 1
来源：http://hz.yanxiufei.cn/gthytxlmkh.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cdnleiting.top/gteksqdmbr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.316326.xyz/gtmrepflib.html

TS:   // 同 JS
来源：http://hz.andypj.xyz/gtvyxpmywv.html

Java: synchronized (this) { shared++; }
来源：http://hz.xinyue.icu/gtfndsyamn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.havefunace.top/gtnronxrws.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yj20258888.top/gtsvtiyvik.html

C#:   lock (gate) { shared++; }
来源：http://hz.nwbrower.top/gtwgcipalr.html

[O04] 定义异步函数并等待
来源：http://hz.yangfankeji.com/gttuziyeyd.html

Py:   async def f():⏎    await g()
来源：http://hz.316326.xyz/gtyznkqjgk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.redwolf501.top/gteuyaovdl.html

JS:   async function f() { await g(); }
来源：http://hz.gogol.net.cn/gtxqukjwmv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hnxiangtu.top/gtszsrfxab.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zdqjudy.top/gtnuzhxwms.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.gogol.net.cn/gtafeggmyr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gogol.net.cn/gtfzervkow.html

C#:   async Task F() { await G(); }
来源：http://hz.cashguo.top/gtjdqqangd.html

[O05] 并发执行并等待全部完成
来源：http://hz.sxryk.cn/gtmriyqybe.html

Py:   asyncio.gather(*tasks)
来源：http://hz.0kj1m.cn/gtkdhdipfy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xingfuxueyuan.xyz/gtcgapdqho.html

JS:   await Promise.all(tasks)
来源：http://hz.kuanghao11.cn/gtnoblpzfo.html

TS:   await Promise.all(tasks)
来源：http://hz.gaohongyu789.top/gtwmiugsay.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.tanke756.top/gtzcgajtxh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.tanke756.top/gtrrnwgslt.html

Ruby: threads.map(&:join)
来源：http://hz.aibaodan.cn/gtcmladnxm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.chenjidiqi.icu/gtdqdtqbvc.html

[O06] 使用进程池
来源：http://hz.yuanzhike.top/gtljimkueu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yonumen.top/gthiqfpzqz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.snrcjt.cn/gtpkugdxor.html

JS:   // child_process / cluster 模块
来源：http://hz.fzhhl.top/gtczrvmjoq.html

TS:   // child_process / cluster 模块
来源：http://hz.shanyushiyangtech.top/gtkbmljmkh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.fzhhl.top/gtyznfhnwf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.vqdsnc.cn/gtyidfunkx.html

Ruby: // fork 块
来源：http://hz.cheryme.top/gtgcjjfjzl.html

C#:   Parallel.For
来源：http://hz.sysykeji.top/gtdfvwuema.html

================================================================================
来源：http://hz.dianchejie.cn/gtnvlgmoir.html

P. 常用工具函数
来源：http://hz.xuetiantiany.cn/gttiwshrqw.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtgjktopfn.html

[P01] 生成 UUID
来源：http://hz.guowangkeji.top/gtuigtgfts.html

Py:   str(uuid.uuid4())
来源：http://hz.andypj.xyz/gtevssxqsx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hywenlv.cn/gtpvyirbqs.html

JS:   crypto.randomUUID()
来源：http://hz.jinqigfzy.top/gtdqnjqjjc.html

TS:   crypto.randomUUID()
来源：http://hz.sufxvd.cn/gtljirybga.html

Java: UUID.randomUUID().toString()
来源：http://hz.sufxvd.cn/gtsgfxbzbg.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhoulong.xyz/gtgiysduzl.html

Ruby: SecureRandom.uuid
来源：http://hz.hysaishi.cn/gtvehksyfw.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.c1oappe.top/gttrerhxbj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ydzc1.top/gtmvdofppf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yanxiufei.cn/gtcntvxjot.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.chenzaomai.com/gtfqshhvor.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.guowangkeji.top/gtzagksadh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.sysykeji.top/gtcvlzoylj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.quarkkingdee.top/gtuoqozrkd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.vqdsnc.cn/gttsssllwg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ywan-chungtsiang.top/gtcavtofqr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shangyingyoupin.top/gtuhygsfdk.html

[P03] 生成短随机字符串
来源：http://hz.jyoumei.cn/gtzraqsrhu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.haohaochexian.top/gtqkvyxhbw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yvedp.cn/gtzywbeclj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinghuilouyu.cn/gtdgzzgquc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dashuyun.cn/gtmyfgnqmv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.guannengcc.top/gtqaqbgfaz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jinghuilouyu.cn/gtltznmano.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhengqikj.top/gttraaffrw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yonumen.top/gtkmayvmvj.html

[P04] 求长度
来源：http://hz.gzhubu.top/gttdhasfpl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhaomingkeji.xyz/gtofpaukej.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tian-w.cn/gtmreulosp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.0kj1m.cn/gtkqdpemdr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hammf.cn/gtvgtnrglr.html

Java: list.size();  map.size();  s.length()
来源：http://hz.smart0.xyz/gtwfggppxh.html

Go:   len(arr);  len(m)
来源：http://hz.zhengqikj.top/gtxvdhgkcy.html

Ruby: x.length;  x.size
来源：http://hz.yuxming.cn/gtjfyzevci.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.nanxuanxn.top/gtdggqocpu.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xinyue.icu/gtlnjkgvlx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhoulong.xyz/gtfkuupvbq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhaomingkeji.xyz/gtawzvatms.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yongpay.top/gtuzriywui.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yongpay.top/gtxqvkzotu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jqgufenzy.top/gtdajngfbs.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhaomingkeji.xyz/gtznxqqoqu.html

Ruby: a == b
来源：http://hz.tian-w.cn/gtypstwvpi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.chenjidiqi.icu/gtqxdlgkfe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cdnleiting.top/gtiwzdprvg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ydzc1.top/gtqzyasncr.html

PHP:  if (empty($x)) {}
来源：http://hz.zhaomingkeji.xyz/gtmsohxvvq.html


<!-- 参考信息 -->