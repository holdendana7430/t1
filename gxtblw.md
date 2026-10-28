代发 wailian999

TS:   resp.ok;  resp.status
来源：http://hz.fzhhl.top/gtilqiwzzv.html

Java: resp.statusCode()
来源：http://hz.ywan-chungtsiang.top/gtrjffxhvr.html

Go:   resp.StatusCode
来源：http://hz.fzhhl.top/gthzayosdg.html

Ruby: resp.code.to_i
来源：http://hz.yuxming.cn/gtdamacbvs.html

C#:   (int)resp.StatusCode
来源：http://hz.9152youxi.cn/gtovjvpete.html

[L08] 并发请求多个地址
来源：http://hz.zhongyouzk.top/gtwuxwzjes.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yonumen.top/gtzpaxmbvt.html

PHP:  curl_multi_init() 系列
来源：http://hz.52xcode.cn/gtuminpcgz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sysykeji.top/gtthphfmle.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.quarkkingdee.top/gtvkjzecqx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.dashuyun.cn/gtzralaglu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yangfankeji.com/gtvndciymq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.smart0.xyz/gtklmccdxp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yonumen.top/gtidrovlke.html

================================================================================
来源：http://hz.mhx1999.top/gtfprcelvw.html

M. 命令行 / 进程 / 环境
来源：http://hz.jqgfzy.top/gtekaqspul.html

================================================================================
来源：http://hz.9152youxi.cn/gtsabfchjm.html

[M01] 读取命令行参数
来源：http://hz.jinqigufen.top/gtfgewmszm.html

Py:   sys.argv[1:]
来源：http://hz.daria6918.cn/gtaoyrexqx.html

PHP:  $argv;  $argc;
来源：http://hz.jqgfzy.top/gtvoqtlzyb.html

JS:   process.argv.slice(2)
来源：http://hz.ybcxt.top/gtrbezqarv.html

TS:   process.argv.slice(2)
来源：http://hz.xingfuxueyuan.xyz/gtlabnfpfj.html

Java: args 数组（main 方法参数）
来源：http://hz.jlsjyb.cn/gtykrajipw.html

Go:   os.Args[1:]
来源：http://hz.shanyushiyangkeji.top/gtocpthusi.html

Ruby: ARGV
来源：http://hz.guannengcc.top/gtaqlyhrwk.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xziqi.cn/gtnxyshxcg.html

[M02] 读取环境变量
来源：http://hz.yonumen.top/gtlfclyfet.html

Py:   os.environ.get("HOME")
来源：http://hz.nanxinkj.top/gtznklszln.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cucudq.cn/gtcxjbbaxk.html

JS:   process.env.HOME
来源：http://hz.hongshengwenyu.top/gtpaksklmz.html

TS:   process.env.HOME
来源：http://hz.hywenlv.cn/gtimesfckb.html

Java: System.getenv("HOME")
来源：http://hz.vqdsnc.cn/gtomejnese.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhiwuduotai.top/gtkaelqoog.html

Ruby: ENV["HOME"]
来源：http://hz.ydzc1.top/gtbtneghst.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.haohaochexian.top/gtlikcimfy.html

[M03] 执行外部命令
来源：http://hz.hammf.cn/gtducvjjbt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cdnleiting.top/gtzplrcopm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinyuanbaomall.cn/gtupikblbz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuanzx.com/gtqjbmpuwr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuanzx.com/gtmlqbklph.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.gaohongyu789.top/gtxgcmqlcp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.dianchejie.cn/gtcjljtjfe.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cucudq.cn/gtkyjedggy.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ppjwa.cn/gtppuaoqyh.html

[M04] 获取当前工作目录
来源：http://hz.xuetiantiany.cn/gtatjxgpdz.html

Py:   os.getcwd()
来源：http://hz.sysykeji.top/gtvwdjdmby.html

PHP:  getcwd();
来源：http://hz.zhengqikj.top/gtgrryiaho.html

JS:   process.cwd()
来源：http://hz.shanyushiyangkeji.top/gtulyojpcq.html

TS:   process.cwd()
来源：http://hz.yonumen.top/gtxirqkxov.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jiagoushi.top/gtjnwsmgcn.html

Go:   os.Getwd()
来源：http://hz.zhixingplan.top/gtnchgfhjo.html

Ruby: Dir.pwd
来源：http://hz.jianghu66.top/gtwwewgpax.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.svipenyu.cn/gtstsckgls.html

[M05] 设置退出码
来源：http://hz.jinqigufen.top/gtrtqpovgo.html

Py:   sys.exit(1)
来源：http://hz.ppjwa.cn/gtaupcfgwu.html

PHP:  exit(1);
来源：http://hz.daxiang520.top/gtbevepvgt.html

JS:   process.exit(1)
来源：http://hz.pengpengdd.cyou/gtjtljmkyg.html

TS:   process.exit(1)
来源：http://hz.jiagoushi.top/gtxipkiowj.html

Java: System.exit(1)
来源：http://hz.daxiang520.top/gthzqfmfrf.html

Go:   os.Exit(1)
来源：http://hz.daria6918.cn/gtvvngcvmz.html

Ruby: exit 1
来源：http://hz.jinqigufen.top/gtrpyyjoxt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.vqdsnc.cn/gtnbsaxtwq.html

[M06] 向标准错误输出
来源：http://hz.vqdsnc.cn/gtfgekouzz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xuanzx.com/gttomodqhg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.tanke756.top/gtxwllzrum.html

JS:   console.error("err")
来源：http://hz.cashguo.top/gtqdlkbulc.html

TS:   console.error("err")
来源：http://hz.nwbrower.top/gteprhflau.html

Java: System.err.println("err")
来源：http://hz.cqqwz.cn/gtqmsycdri.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhongyouzk.top/gtatukwzbi.html

Ruby: warn "err"
来源：http://hz.zhaomingkeji.xyz/gtqxaoffbw.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.dianchejie.cn/gtqgtuxnlt.html

[M07] 判断是否为主入口
来源：http://hz.hywenlv.cn/gtgvagkrgi.html

Py:   if __name__ == "__main__":
来源：http://hz.smart0.xyz/gtvacdbwqf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gogol.net.cn/gtptolqfcv.html

JS:   require.main === module
来源：http://hz.havefunace.top/gthodnthvp.html

TS:   require.main === module
来源：http://hz.meibo888.top/gtaivbmsmc.html

Java: public static void main(String[] args)
来源：http://hz.yj202588.top/gtupaepuqh.html

Go:   func main()
来源：http://hz.zhiwuduotai.top/gtjbfokzrp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xylfe.cn/gtloflmwtb.html

C#:   static void Main(string[] args)
来源：http://hz.hnxiangtu.top/gtkhbxdncu.html

[M08] 获取系统与运行时信息
来源：http://hz.52xcode.cn/gtgcuvxudo.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shzxlz.cn/gtrocixlqy.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhongyouzk.top/gtbqeufxhw.html

JS:   process.platform;  process.version
来源：http://hz.xuetiantiany.cn/gtzfnxnfuv.html

TS:   process.platform;  process.version
来源：http://hz.vqdsnc.cn/gtzylgbqkq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.quarkkingdee.top/gtitgjrykb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hysaishi.cn/gtugwplatj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hysaishi.cn/gtxhonwdzk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.nanxinkj.top/gtwfkpjwgr.html

================================================================================
来源：http://hz.nanxinkj.top/gtqzlgzigh.html

N. 数据结构与算法
来源：http://hz.shuidangran.top/gtufarzfpd.html

================================================================================
来源：http://hz.fzhhl.top/gtmvgyllpk.html

[N01] 二分查找（有序数组）
来源：http://hz.zhixingplan.top/gtjajomodo.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xinyue.icu/gtyfanueca.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.iojbl.cn/gtpblunnft.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhoulong.xyz/gtkqxubcji.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.mhx1999.top/gthwtmncrh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shzxlz.cn/gtjqabwrkj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yvedp.cn/gtfqqonozn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.dianchejie.cn/gtxqlgigel.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xylfe.cn/gtynwzjxka.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhixingplan.top/gtmsrytxur.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hfpthk.cn/gtihxcygcd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yonumen.top/gtkmlaphta.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.kuanghao11.cn/gtxqgcqdhz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuxming.cn/gtnwmburzq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.meibo888.top/gtjyydddwq.html

Go:   slices.Sort(arr)
来源：http://hz.jianghu66.top/gtsnxiejnq.html

Ruby: arr.sort
来源：http://hz.shuidangran.top/gtjfqqjzhr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cqqwz.cn/gtyinhqtig.html

[N03] 快速排序（分治示例）
来源：http://hz.jqgufenzy.top/gtxlgyolhp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.havefunace.top/gtocwshrhr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yangfankeji.com/gtehhhuyox.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ivvv.top/gtedyfixpm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangdashe.top/gtbvleycql.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.aibaodan.cn/gtxgewwbrh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jqgufenzy.top/gtcteaacoa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.52xcode.cn/gtjyhkafvk.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shanyushiyangkeji.top/gtnsjhjvxv.html

[N04] 斐波那契数列
来源：http://hz.gaohongyu789.top/gtydhgjexw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yonumen.top/gthtsuytzd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jianghu66.top/gtbkbqcymh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gteincvorh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xingfuxueyuan.xyz/gtkxkcibqv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shzxlz.cn/gtgprlbhhu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sxryk.cn/gtwrjhmtuo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhaomingkeji.xyz/gtwpyqsufv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.haohaochexian.top/gtposgxkyf.html

[N05] 最大公约数
来源：http://hz.chenjidiqi.icu/gtdzysmsdf.html

Py:   math.gcd(a, b)
来源：http://hz.jlsjyb.cn/gtgvgrphtf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tianlin.xyz/gtbkfcvutm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.svipenyu.cn/gthtdlexiu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yueranfly.top/gtvwrsdntg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zycfv.cn/gtbewmextm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shuidangran.top/gtyfhjahmg.html

Ruby: a.gcd(b)
来源：http://hz.jinqigfzy.top/gtxyzxmbbz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.chenlongwang.top/gtvptyyiec.html

[N06] 判断回文字符串
来源：http://hz.chenzaomai.com/gtjzkresqg.html

Py:   s == s[::-1]
来源：http://hz.hywenlv.cn/gtamasqlgd.html

PHP:  $s === strrev($s);
来源：http://hz.hammf.cn/gtjfqktnaw.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hammf.cn/gtzxealunl.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ivvv.top/gtcyfservd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shanyushiyangtech.top/gtjmgcnqkm.html

Go:   // 双指针从两端比较
来源：http://hz.zhengqikj.top/gtbuhqtxbn.html

Ruby: s == s.reverse
来源：http://hz.zhengqikj.top/gtkxwoslhf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.sufxvd.cn/gttolxyckh.html

[N07] 两数之和（返回下标）
来源：http://hz.aibaodan.cn/gthkkjijew.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ydzc1.top/gtiesqpuzn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhoulong.xyz/gtbegynpsw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.andypj.xyz/gttwrheina.html

TS:   // 手写 Map<string, number>
来源：http://hz.cucudq.cn/gticfzynyg.html

Java: // 手写 HashMap
来源：http://hz.cdnleiting.top/gtcuntklnw.html

Go:   // 手写 map[int]int
来源：http://hz.guowangkeji.top/gtecnnzjfb.html

Ruby: // 手写 Hash
来源：http://hz.xingfuxueyuan.xyz/gtrtotvwzw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xziqi.cn/gtusnsumya.html

[N08] 生成全排列
来源：http://hz.cashguo.top/gtotmaxjqq.html

Py:   itertools.permutations(arr)
来源：http://hz.yj202588.top/gtahjsuvtn.html

PHP:  // 手写递归交换
来源：http://hz.cucudq.cn/gtphilbgad.html

JS:   // 手写回溯递归
来源：http://hz.birdmap.top/gtfpvccyph.html

TS:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtzahorthm.html

Java: // 手写回溯递归
来源：http://hz.cqqwz.cn/gtkrzrispk.html

Go:   // 手写回溯递归
来源：http://hz.redwolf501.top/gtuqtddnzb.html

Ruby: arr.permutation.to_a
来源：http://hz.wangshuangyany.cn/gtbgxgmczw.html

C#:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtrfgkyhbb.html

[N09] 栈与队列
来源：http://hz.jianghu66.top/gtpuvzjtuu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.0kj1m.cn/gtojjpyxkk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.gzhubu.top/gtrstuqtwq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhiwuduotai.top/gtyamgeymu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.wangdashe.top/gtxklkspur.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.nwbrower.top/gtldabizqx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yueranfly.top/gtpcatjodk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hammf.cn/gtumnmkrda.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.aibaodan.cn/gtfhdqkhlo.html

[N10] 链表节点定义
来源：http://hz.pycfn.com/gtplebuwyn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xuetiantiany.cn/gtqcukqxyq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jlsjyb.cn/gtdmfivpxo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhengqikj.top/gtutbsahqt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhengqikj.top/gtxihtvrzp.html

Java: class Node { int v; Node next; }
来源：http://hz.cqqwz.cn/gtsvcyjpcp.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yonumen.top/gtfiggnlqu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.dashuyun.cn/gtivmwgakx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.mhx1999.top/gtuysrrlni.html

[N11] 二叉树中序遍历
来源：http://hz.ppjwa.cn/gtuxbrrbdr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.aibaodan.cn/gtgytfeyqo.html

PHP:  // 手写递归函数
来源：http://hz.yangfankeji.com/gtqmbesicq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnqzz.top/gthjkitiug.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yongpay.top/gtgnnhhefu.html

Java: // 手写递归
来源：http://hz.meibo888.top/gtzfbiryrj.html

Go:   // 手写递归
来源：http://hz.feifeiyinyue.top/gtoqkqklek.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tianlin.xyz/gtwoinghmo.html

C#:   // 手写递归
来源：http://hz.jinqigfzy.top/gtmulwiptj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.chenzaomai.com/gtgmsultib.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenlongwang.top/gtriumykzr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xinyue.icu/gtnlddvfyg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dashuyun.cn/gtodrxyjrx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhixingplan.top/gthoergcao.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.kuanghao11.cn/gtuozfcrwp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.wangdashe.top/gtioryrvxz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jiagoushi.top/gtmmqrsnin.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gotoacloud.top/gtlmfnhfsa.html

================================================================================
来源：http://hz.xylfe.cn/gtuajqcisw.html

O. 并发与异步
来源：http://hz.9152youxi.cn/gthotaeeqo.html

================================================================================
来源：http://hz.yangfankeji.com/gtausayhkr.html

[O01] 启动一个线程
来源：http://hz.gotoacloud.top/gttikujkvl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinyuanbaomall.cn/gtsfsafyyr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinqigufen.top/gtliwezppt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zdqjudy.top/gtxraftbwh.html

TS:   // 同 JS
来源：http://hz.redwolf501.top/gtxpmtufjb.html

Java: new Thread(() -> f()).start()
来源：http://hz.shzxlz.cn/gtzlpdfjne.html

Go:   go f()
来源：http://hz.nwbrower.top/gtsovuciie.html

Ruby: Thread.new { f }
来源：http://hz.shuidangran.top/gtyibfjdil.html

C#:   Task.Run(() => F());
来源：http://hz.meibo888.top/gtkubnmyhj.html

[O02] 使用线程池
来源：http://hz.vqdsnc.cn/gtrgrgwhsz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.haohaochexian.top/gtxtcvlsdf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.havefunace.top/gtowhicwff.html

JS:   // worker_threads 线程池
来源：http://hz.yj20258.top/gtkttbpgds.html

TS:   // worker_threads 线程池
来源：http://hz.daxiang520.top/gtektckhbk.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhixingplan.top/gtnhithzka.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.quarkkingdee.top/gtnjwpzpea.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yvedp.cn/gtwpcbemex.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shanyushiyangtech.top/gtyvfdhjlu.html

[O03] 加锁保护共享数据
来源：http://hz.guowangkeji.top/gtqkaymgsd.html

Py:   with lock: shared += 1
来源：http://hz.xuetiantiany.cn/gtemhkpoab.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.birdmap.top/gtzfunarsq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.vqdsnc.cn/gtjmqfrxye.html

TS:   // 同 JS
来源：http://hz.hammf.cn/gtbmuiscxy.html

Java: synchronized (this) { shared++; }
来源：http://hz.haohaochexian.top/gtamunsebu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ybcxt.top/gtrpbszqql.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhixingplan.top/gtdmzaxvux.html

C#:   lock (gate) { shared++; }
来源：http://hz.xinyue.icu/gtytjdjhif.html

[O04] 定义异步函数并等待
来源：http://hz.xingfuxueyuan.xyz/gtduhcysqc.html

Py:   async def f():⏎    await g()
来源：http://hz.yangfankeji.com/gtrwlrouum.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.aibaodan.cn/gtoepuoyap.html

JS:   async function f() { await g(); }
来源：http://hz.daria6918.cn/gtwfrhocii.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.tianlin.xyz/gtopzbmzfl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sysykeji.top/gtlvygohbd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cdnleiting.top/gtswjmpoil.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.tanke756.top/gtorpqsgzi.html

C#:   async Task F() { await G(); }
来源：http://hz.ywan-chungtsiang.top/gtcbbsnmqm.html

[O05] 并发执行并等待全部完成
来源：http://hz.bjfxy.top/gtqwqxbhvc.html

Py:   asyncio.gather(*tasks)
来源：http://hz.daria6918.cn/gtqpvifjjm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jianghu66.top/gtjfoykwqs.html

JS:   await Promise.all(tasks)
来源：http://hz.hywenlv.cn/gtgucnlzuo.html

TS:   await Promise.all(tasks)
来源：http://hz.wangshuangyany.cn/gtrhjpdzzt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hongshengwenyu.top/gtxdefcqje.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cdnleiting.top/gtagcdzpfu.html

Ruby: threads.map(&:join)
来源：http://hz.zhoulong.xyz/gtwondhlsx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zycfv.cn/gtwtumguio.html

[O06] 使用进程池
来源：http://hz.shanyushiyangtech.top/gtwywghujj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.nanxinkj.top/gtkxhbbjof.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.52xcode.cn/gtkqgelmbc.html

JS:   // child_process / cluster 模块
来源：http://hz.dianchejie.cn/gtqgrdcdrl.html

TS:   // child_process / cluster 模块
来源：http://hz.jianghu66.top/gtibkgilbl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yonumen.top/gtvzyzjyye.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.dianchejie.cn/gtdemuzuwy.html

Ruby: // fork 块
来源：http://hz.yongpay.top/gtjemkpqgf.html

C#:   Parallel.For
来源：http://hz.xylfe.cn/gtziurwfqb.html

================================================================================
来源：http://hz.cqqwz.cn/gtktsegdle.html

P. 常用工具函数
来源：http://hz.gotoacloud.top/gtxdyxexod.html

================================================================================
来源：http://hz.52xcode.cn/gtvdsraulg.html

[P01] 生成 UUID
来源：http://hz.ivvv.top/gtbzjeiaix.html

Py:   str(uuid.uuid4())
来源：http://hz.chenjidiqi.icu/gtlnphuruf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jlsjyb.cn/gtychakjmb.html

JS:   crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtyhhwxhdt.html

TS:   crypto.randomUUID()
来源：http://hz.xingfuxueyuan.xyz/gtsyybitoz.html

Java: UUID.randomUUID().toString()
来源：http://hz.ydzc1.top/gtwmzmrspf.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ydzc1.top/gtkgmyilfd.html

Ruby: SecureRandom.uuid
来源：http://hz.ivvv.top/gtoibzotvs.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cheryme.top/gtnstqvzan.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sweek.top/gtwqfdkgis.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shanyushiyangtech.top/gtofxmkory.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zycfv.cn/gtqjkwghqi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.tianlin.xyz/gtmutfgjga.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.redwolf501.top/gtlahvsrih.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zycfv.cn/gtcagugzmt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cashguo.top/gtgagwengx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xziqi.cn/gtfndysxvu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.daria6918.cn/gtcyxyerzo.html

[P03] 生成短随机字符串
来源：http://hz.guannengcc.top/gtslqwmawa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.daxiang520.top/gtxxiatmtp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jyoumei.cn/gtrxivjggr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cucudq.cn/gtvfddhpbc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xingfuxueyuan.xyz/gtugqlxdkk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shanyushiyangkeji.top/gtebvfreqz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ybcxt.top/gtuyskqspa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.pycfn.com/gtmmjxzmvh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.tianlin.xyz/gtvvgcgkep.html

[P04] 求长度
来源：http://hz.jyoumei.cn/gtderuzzop.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xuetiantiany.cn/gtvlqtjhiz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jiagoushi.top/gtaqcgpheu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sweek.top/gtmtcimnvk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.0kj1m.cn/gtycwylyqr.html

Java: list.size();  map.size();  s.length()
来源：http://hz.aibaodan.cn/gteledoydg.html

Go:   len(arr);  len(m)
来源：http://hz.jianghu66.top/gtyshskgll.html

Ruby: x.length;  x.size
来源：http://hz.52xcode.cn/gtpcodsxmf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cdnleiting.top/gtpodczczi.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shangyingyoupin.top/gtevuobffr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhijiandao.cn/gtfzwivtjq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yj20258888.top/gtbehtiyld.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hnxiangtu.top/gtospzgjnz.html


<!-- 参考信息 -->