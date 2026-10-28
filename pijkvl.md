代发 wailian999

C#:   (int)resp.StatusCode
来源：http://hz.tian-w.cn/gtaxxapeld.html

[L08] 并发请求多个地址
来源：http://hz.yvedp.cn/gtdypaqokm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.havefunace.top/gthtqbepdl.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinqigfzy.top/gtdokhrvcb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.andypj.xyz/gttxkogevt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.haohaochexian.top/gtkpujxevp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yj20258.top/gtknmfenos.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zycfv.cn/gtxnyylrbd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.birdmap.top/gtlluedgvz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cheryme.top/gtqwdjyria.html

================================================================================
来源：http://hz.jqgfzy.top/gtmtabpceq.html

M. 命令行 / 进程 / 环境
来源：http://hz.wangdashe.top/gtoeebocmt.html

================================================================================
来源：http://hz.yvedp.cn/gtghyywuok.html

[M01] 读取命令行参数
来源：http://hz.quarkkingdee.top/gtebusvpnr.html

Py:   sys.argv[1:]
来源：http://hz.hnxiangtu.top/gtcmizpxsl.html

PHP:  $argv;  $argc;
来源：http://hz.fengsongda.top/gtvxbcjdag.html

JS:   process.argv.slice(2)
来源：http://hz.svipenyu.cn/gtefzglkzo.html

TS:   process.argv.slice(2)
来源：http://hz.ppjwa.cn/gtgvndlzlm.html

Java: args 数组（main 方法参数）
来源：http://hz.sxryk.cn/gtjmrjtvfx.html

Go:   os.Args[1:]
来源：http://hz.nwbrower.top/gttewimixo.html

Ruby: ARGV
来源：http://hz.tanke756.top/gtdccxbsmy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.havefunace.top/gthurhznjv.html

[M02] 读取环境变量
来源：http://hz.kuanghao11.cn/gtanbnlaad.html

Py:   os.environ.get("HOME")
来源：http://hz.hnqzz.top/gtvpfyfhsq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yonumen.top/gtsxmxeail.html

JS:   process.env.HOME
来源：http://hz.hfpthk.cn/gtvicejtfu.html

TS:   process.env.HOME
来源：http://hz.pengpengdd.cyou/gtalqmxfyj.html

Java: System.getenv("HOME")
来源：http://hz.cheryme.top/gtimuyjgwv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ydjk.org.cn/gthqbfonso.html

Ruby: ENV["HOME"]
来源：http://hz.shanyushiyangkeji.top/gtzvstecyu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ppjwa.cn/gtpxhedqfg.html

[M03] 执行外部命令
来源：http://hz.hysaishi.cn/gtfrcwmwze.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ywan-chungtsiang.top/gtxvfrdoal.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hnqzz.top/gtccnwdgnu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.svipenyu.cn/gtpbqwqlkn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.iojbl.cn/gtthtbzsrq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cashguo.top/gtbqiqdhbc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yongpay.top/gtiwtnmdbs.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jqgfzy.top/gtvucklqkz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jianghu66.top/gtntzoujyi.html

[M04] 获取当前工作目录
来源：http://hz.yangfankeji.com/gtccemyodv.html

Py:   os.getcwd()
来源：http://hz.jyoumei.cn/gtruigjtpk.html

PHP:  getcwd();
来源：http://hz.dashuyun.cn/gtjyekrmne.html

JS:   process.cwd()
来源：http://hz.jinqigufen.top/gtvtizcudx.html

TS:   process.cwd()
来源：http://hz.jinghuilouyu.cn/gtglmuvaqq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.quarkkingdee.top/gtvfvxiakr.html

Go:   os.Getwd()
来源：http://hz.fzhhl.top/gtaulpnmsl.html

Ruby: Dir.pwd
来源：http://hz.sxryk.cn/gtzktvuiwt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.kuanghao11.cn/gtkngfhxpu.html

[M05] 设置退出码
来源：http://hz.jyoumei.cn/gtyvxdeyib.html

Py:   sys.exit(1)
来源：http://hz.ydjk.org.cn/gtaivwfzyu.html

PHP:  exit(1);
来源：http://hz.xinyue.icu/gtbqtmzryy.html

JS:   process.exit(1)
来源：http://hz.kuanghao11.cn/gtimwfuztn.html

TS:   process.exit(1)
来源：http://hz.zhixingplan.top/gtyjigcppm.html

Java: System.exit(1)
来源：http://hz.ydzc1.top/gtangqjdfv.html

Go:   os.Exit(1)
来源：http://hz.316326.xyz/gtgnmcbwyh.html

Ruby: exit 1
来源：http://hz.hfpthk.cn/gtksfmhjjb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ywan-chungtsiang.top/gtafqpvbup.html

[M06] 向标准错误输出
来源：http://hz.xinyue.icu/gtvxcixyzp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xziqi.cn/gtzkiygpai.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.kuanghao11.cn/gtbltdewqb.html

JS:   console.error("err")
来源：http://hz.hnxiangtu.top/gtttxhzpfz.html

TS:   console.error("err")
来源：http://hz.yj202588.top/gtgacuoxou.html

Java: System.err.println("err")
来源：http://hz.tanke756.top/gtqpojgrrc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jlsjyb.cn/gtfkdxstqm.html

Ruby: warn "err"
来源：http://hz.hnqzz.top/gtmrwpwfld.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yanxiufei.cn/gthbgvihvw.html

[M07] 判断是否为主入口
来源：http://hz.havefunace.top/gtidhljiqd.html

Py:   if __name__ == "__main__":
来源：http://hz.yangfankeji.com/gtbjiwqbrb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.haohaochexian.top/gtnxzzopyd.html

JS:   require.main === module
来源：http://hz.jqgufenzy.top/gtciywlgqt.html

TS:   require.main === module
来源：http://hz.zdqjudy.top/gtnfzlfvnc.html

Java: public static void main(String[] args)
来源：http://hz.aizwys.cn/gtawvrerwa.html

Go:   func main()
来源：http://hz.jyoumei.cn/gtyecgymzx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yongpay.top/gtcivuoysp.html

C#:   static void Main(string[] args)
来源：http://hz.xziqi.cn/gtvaqelklr.html

[M08] 获取系统与运行时信息
来源：http://hz.yj20258888.top/gtafyzmmqg.html

Py:   platform.system();  platform.python_version()
来源：http://hz.pycfn.com/gtxidupwkj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.snrcjt.cn/gtpctdnipf.html

JS:   process.platform;  process.version
来源：http://hz.xingfuxueyuan.xyz/gtsluifhip.html

TS:   process.platform;  process.version
来源：http://hz.ydzc1.top/gtahdewlgi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shzxlz.cn/gttjnmqdij.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.feifeiyinyue.top/gttcjkipja.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hywenlv.cn/gtbbtvzzuf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ppjwa.cn/gtvmekvmvw.html

================================================================================
来源：http://hz.zhoulong.xyz/gtsnmhicrg.html

N. 数据结构与算法
来源：http://hz.cdnleiting.top/gtqkebdfvh.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtqetxwsen.html

[N01] 二分查找（有序数组）
来源：http://hz.nwbrower.top/gtcoijsdnh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ivvv.top/gtglkjrfdw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.nanxuanxn.top/gtmxppghgb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhengqikj.top/gtgzvbymyd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhixingplan.top/gtlhppkpsq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.snrcjt.cn/gtlppbpntg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinghuilouyu.cn/gtabtpvwwl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xingfuxueyuan.xyz/gtezwjioqr.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sufxvd.cn/gtsgfxjwmo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.tianlin.xyz/gtqxfjsoic.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.guowangkeji.top/gtobkiaumz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.dashuyun.cn/gtnnmkofms.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gogol.net.cn/gtlagssnrw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sysykeji.top/gtbqjhlnmd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.andypj.xyz/gtdodxfyue.html

Go:   slices.Sort(arr)
来源：http://hz.gzhubu.top/gtdowdzldl.html

Ruby: arr.sort
来源：http://hz.gzhubu.top/gtfstrchet.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ybcxt.top/gtsupghofj.html

[N03] 快速排序（分治示例）
来源：http://hz.sysykeji.top/gttdzayalm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhongyouzk.top/gtrvhfgfjd.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gotoacloud.top/gtoubydgrt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.feifeiyinyue.top/gtabujwzec.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hammf.cn/gtdsadnlyu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.nanxuanxn.top/gtimcnuukz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shanyushiyangkeji.top/gtvefdanra.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sxryk.cn/gtynsjvfaa.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhoulong.xyz/gtmmrmcwsy.html

[N04] 斐波那契数列
来源：http://hz.iojbl.cn/gtwlzkvmmg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.iojbl.cn/gtaawweoyq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yvedp.cn/gtclrdpehe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnqzz.top/gtdsmmiqkj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gtsatdlujo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.quarkkingdee.top/gtnfvxeoyl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sxryk.cn/gtztwtxxzq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shangyingyoupin.top/gtsonsocoo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yonumen.top/gtdazrzruw.html

[N05] 最大公约数
来源：http://hz.chenjidiqi.icu/gtpjbkzhct.html

Py:   math.gcd(a, b)
来源：http://hz.c1oappe.top/gtopehnkgn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jianghu66.top/gtycgjdbut.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.bjfxy.top/gtuzcsbjvw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nanxinkj.top/gtfrakvzwg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yongpay.top/gtaiganmjl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.wangshuangyany.cn/gtbcopqmnl.html

Ruby: a.gcd(b)
来源：http://hz.shuidangran.top/gtgpppnfgd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yj20258888.top/gtinoqdvug.html

[N06] 判断回文字符串
来源：http://hz.hnxiangtu.top/gtxqhbjyvn.html

Py:   s == s[::-1]
来源：http://hz.andypj.xyz/gtoiujtvpm.html

PHP:  $s === strrev($s);
来源：http://hz.chenlongwang.top/gtebkqknou.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xuanzx.com/gtocovlmfd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sweek.top/gtixjazgjw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.aibaodan.cn/gtwpdxhrwx.html

Go:   // 双指针从两端比较
来源：http://hz.daxiang520.top/gtkvwzgvmx.html

Ruby: s == s.reverse
来源：http://hz.ehwqpu.com/gtpvdcpbsm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.daxiang520.top/gtvrzfuqku.html

[N07] 两数之和（返回下标）
来源：http://hz.dianchejie.cn/gtremnizoc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.c1oappe.top/gtrifpsqim.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xziqi.cn/gtdxkcunun.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.pengpengdd.cyou/gtiurgofws.html

TS:   // 手写 Map<string, number>
来源：http://hz.pycfn.com/gtljdlfktz.html

Java: // 手写 HashMap
来源：http://hz.9152youxi.cn/gtlhakkqcb.html

Go:   // 手写 map[int]int
来源：http://hz.yj20258.top/gtfkpgdhsq.html

Ruby: // 手写 Hash
来源：http://hz.yj20258.top/gtigbtgivr.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.guowangkeji.top/gthcsldulj.html

[N08] 生成全排列
来源：http://hz.daria6918.cn/gtzpaknyft.html

Py:   itertools.permutations(arr)
来源：http://hz.jinghuilouyu.cn/gtxixdfosr.html

PHP:  // 手写递归交换
来源：http://hz.chenlongwang.top/gtoxaftygm.html

JS:   // 手写回溯递归
来源：http://hz.zycfv.cn/gtbrsaaaiu.html

TS:   // 手写回溯递归
来源：http://hz.aizwys.cn/gttpqrimth.html

Java: // 手写回溯递归
来源：http://hz.9152youxi.cn/gthosmgeen.html

Go:   // 手写回溯递归
来源：http://hz.quarkkingdee.top/gtwpcsmuue.html

Ruby: arr.permutation.to_a
来源：http://hz.yuanzhike.top/gtajpknqmk.html

C#:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtkfsetbsg.html

[N09] 栈与队列
来源：http://hz.hongshengwenyu.top/gtrsahkkkn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.tian-w.cn/gtfrfqdgcb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhoulong.xyz/gteyjuktsc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.shuidangran.top/gtfndaalzo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ywan-chungtsiang.top/gtenalxjhu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.svipenyu.cn/gtatyybicu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.vqdsnc.cn/gtatxwxuuh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yonumen.top/gtehmetcxa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.pycfn.com/gttjgwvsmw.html

[N10] 链表节点定义
来源：http://hz.redwolf501.top/gtwhdvilmp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yonumen.top/gttgxkkhga.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.haohaochexian.top/gtpxkztwrg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jianghu66.top/gttoocmxhc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shuidangran.top/gtmyouvbrj.html

Java: class Node { int v; Node next; }
来源：http://hz.ydzc1.top/gtymfszwqy.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yuxming.cn/gthzafebeu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhijiandao.cn/gtamtzrtra.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.tianlin.xyz/gtyfaisoaw.html

[N11] 二叉树中序遍历
来源：http://hz.xylfe.cn/gtvyyosxak.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ydjk.org.cn/gttbmmowno.html

PHP:  // 手写递归函数
来源：http://hz.shzxlz.cn/gtnwydisqk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hywenlv.cn/gtelrdwwda.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhengqikj.top/gtrhqrcmys.html

Java: // 手写递归
来源：http://hz.dianchejie.cn/gtgecnngvd.html

Go:   // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtmetrxshp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yonumen.top/gtwawuijcw.html

C#:   // 手写递归
来源：http://hz.0kj1m.cn/gtfimlxdqg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yuxming.cn/gtkooponxm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.haohaochexian.top/gtxgsljejr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.mhx1999.top/gttojligwv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxuanxn.top/gteprligpa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydzc1.top/gtycxmebhk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hnxiangtu.top/gtzlxmddwe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ywan-chungtsiang.top/gtigcexflu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shanyushiyangtech.top/gtyznnufwi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.meibo888.top/gttnvmijwy.html

================================================================================
来源：http://hz.chenlongwang.top/gtjjpjfoqa.html

O. 并发与异步
来源：http://hz.zhaomingkeji.xyz/gtysnulxfa.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtdlpoqmkz.html

[O01] 启动一个线程
来源：http://hz.vqdsnc.cn/gtkjvajxwf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cashguo.top/gtklsvmich.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jqgfzy.top/gthcyicaky.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ppjwa.cn/gtzmfgnnum.html

TS:   // 同 JS
来源：http://hz.hnxiangtu.top/gtkqnqncuz.html

Java: new Thread(() -> f()).start()
来源：http://hz.tian-w.cn/gtiwalhvvt.html

Go:   go f()
来源：http://hz.wangshuangyany.cn/gtxxdfahgq.html

Ruby: Thread.new { f }
来源：http://hz.dianchejie.cn/gtdksblxuv.html

C#:   Task.Run(() => F());
来源：http://hz.jqgufenzy.top/gtprpojksh.html

[O02] 使用线程池
来源：http://hz.ppjwa.cn/gtoztzssxq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.redwolf501.top/gtwpnumzzc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.c1oappe.top/gtedfpcqyn.html

JS:   // worker_threads 线程池
来源：http://hz.kuanghao11.cn/gthnntkzgy.html

TS:   // worker_threads 线程池
来源：http://hz.hfpthk.cn/gtykvehpzn.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xziqi.cn/gtnivrxzmb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ywan-chungtsiang.top/gtucpzapfh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gogol.net.cn/gtplhkwrfe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.snrcjt.cn/gtwyqpnmvg.html

[O03] 加锁保护共享数据
来源：http://hz.mhx1999.top/gtqupkqcdv.html

Py:   with lock: shared += 1
来源：http://hz.yanxiufei.cn/gtyhzgyuxn.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.52xcode.cn/gtwxyiajbn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.sysykeji.top/gtfpaxcogd.html

TS:   // 同 JS
来源：http://hz.bjfxy.top/gtxzrtmivb.html

Java: synchronized (this) { shared++; }
来源：http://hz.nanxuanxn.top/gtzbzwhsoz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.snrcjt.cn/gtprxmzwbj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.gaohongyu789.top/gtcdwqfkvw.html

C#:   lock (gate) { shared++; }
来源：http://hz.tian-w.cn/gtybvzeuss.html

[O04] 定义异步函数并等待
来源：http://hz.jqgufenzy.top/gtrbpdjowc.html

Py:   async def f():⏎    await g()
来源：http://hz.hywenlv.cn/gtuhixsazz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.pycfn.com/gtkjntkjxx.html

JS:   async function f() { await g(); }
来源：http://hz.cashguo.top/gtbxjwdpvv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hysaishi.cn/gtvuxjghbk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ppjwa.cn/gttffvuuro.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sweek.top/gtvjyogwbm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shangyingyoupin.top/gthvpnwjzi.html

C#:   async Task F() { await G(); }
来源：http://hz.hammf.cn/gtiwbefdtg.html

[O05] 并发执行并等待全部完成
来源：http://hz.andypj.xyz/gtqfyorgnn.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhiwuduotai.top/gtjliailvt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zdqjudy.top/gtlrvbercq.html

JS:   await Promise.all(tasks)
来源：http://hz.316326.xyz/gtfroumdle.html

TS:   await Promise.all(tasks)
来源：http://hz.xinyue.icu/gthhcctqyd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hnxiangtu.top/gtqhotpavx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jqgufenzy.top/gtubxnfmrl.html

Ruby: threads.map(&:join)
来源：http://hz.chenlongwang.top/gtyhfzhbmq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.gogol.net.cn/gtplzrfrbt.html

[O06] 使用进程池
来源：http://hz.sysykeji.top/gtajfiskbs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ivvv.top/gtiblkcaue.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yangfankeji.com/gtosagfxlo.html

JS:   // child_process / cluster 模块
来源：http://hz.yuxming.cn/gthvidgsgx.html

TS:   // child_process / cluster 模块
来源：http://hz.gogol.net.cn/gtcdwxbjfc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.svipenyu.cn/gthvsyrztw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hammf.cn/gtnktsmavf.html

Ruby: // fork 块
来源：http://hz.guowangkeji.top/gtarewvydl.html

C#:   Parallel.For
来源：http://hz.c1oappe.top/gtamqdpomb.html

================================================================================
来源：http://hz.tianlin.xyz/gtgonpnpqy.html

P. 常用工具函数
来源：http://hz.cheryme.top/gtbhxoaxfd.html

================================================================================
来源：http://hz.jiagoushi.top/gtukyjsqbs.html

[P01] 生成 UUID
来源：http://hz.wangdashe.top/gtbzlczmpj.html

Py:   str(uuid.uuid4())
来源：http://hz.chenjidiqi.icu/gtkbetkslk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jqgufenzy.top/gtubyvwcxu.html

JS:   crypto.randomUUID()
来源：http://hz.svipenyu.cn/gtnnjjqnge.html

TS:   crypto.randomUUID()
来源：http://hz.sweek.top/gthppgzddp.html

Java: UUID.randomUUID().toString()
来源：http://hz.ydzc1.top/gtvztyhmcv.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sweek.top/gtebpqejjj.html

Ruby: SecureRandom.uuid
来源：http://hz.chenjidiqi.icu/gtslrgtjir.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.tianlin.xyz/gthmdckrib.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ydzc1.top/gtiyqgfqjd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yonumen.top/gtgwgiiddw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.pengpengdd.cyou/gtpyqhamhx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yangfankeji.com/gtuncnabyp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ydjk.org.cn/gtafmrlojq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jinqigfzy.top/gtlelqypxp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shanyushiyangkeji.top/gtopusvgsj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yangfankeji.com/gtcrewjxed.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yangfankeji.com/gtburexijg.html

[P03] 生成短随机字符串
来源：http://hz.hysaishi.cn/gtcgszkmpe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yj202588.top/gtddgimchn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.chenjidiqi.icu/gtzajwawje.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xingfuxueyuan.xyz/gtlxaqlors.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.bjfxy.top/gtebqyirpw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.52xcode.cn/gtpbxrxpdm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.snrcjt.cn/gtbgcfbpda.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinqigfzy.top/gtrvjqjmtt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.52xcode.cn/gtxotgwbfi.html

[P04] 求长度
来源：http://hz.vqdsnc.cn/gtiygdcqqy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.nwbrower.top/gthlloxpkc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtccsymmku.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yanxiufei.cn/gtvhzxtetc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenjidiqi.icu/gthfdhzicc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xuetiantiany.cn/gtfzctxqia.html

Go:   len(arr);  len(m)
来源：http://hz.hysaishi.cn/gtuxantvxp.html

Ruby: x.length;  x.size
来源：http://hz.zhoulong.xyz/gtyrcpdinz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jianghu66.top/gtmvdtrxsg.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hammf.cn/gtcrdwclys.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sxryk.cn/gtuwtexeqe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.dashuyun.cn/gtpperojub.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jianghu66.top/gtfcyxydoc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sufxvd.cn/gtijsgsmth.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.daxiang520.top/gtzbitqtsz.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.daria6918.cn/gtlxptujug.html

Ruby: a == b
来源：http://hz.daria6918.cn/gtftdntkpz.html


<!-- 参考信息 -->