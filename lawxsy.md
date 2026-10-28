代发 wailian999

C#:   (int)resp.StatusCode
来源：http://hz.shangyingyoupin.top/gtrkuvtsfp.html

[L08] 并发请求多个地址
来源：http://hz.jinghuilouyu.cn/gttttscior.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.chenzaomai.com/gtjxymecmp.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhixingplan.top/gtfknjfdon.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuetiantiany.cn/gtvrdsbklw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hysaishi.cn/gtghkmhmps.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.chenjidiqi.icu/gtpdddrttl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.bjfxy.top/gtkposhubx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xuetiantiany.cn/gtkuivldar.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.snrcjt.cn/gtyyjigwef.html

================================================================================
来源：http://hz.xziqi.cn/gtttvogofn.html

M. 命令行 / 进程 / 环境
来源：http://hz.ydzc1.top/gtkryldpjg.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtwsgnenac.html

[M01] 读取命令行参数
来源：http://hz.ywan-chungtsiang.top/gtjptkduzh.html

Py:   sys.argv[1:]
来源：http://hz.nanxinkj.top/gteynoidkw.html

PHP:  $argv;  $argc;
来源：http://hz.sysykeji.top/gtoortvonk.html

JS:   process.argv.slice(2)
来源：http://hz.yangfankeji.com/gtkmcsktnr.html

TS:   process.argv.slice(2)
来源：http://hz.shzxlz.cn/gtuocbjdwn.html

Java: args 数组（main 方法参数）
来源：http://hz.cashguo.top/gtbbimqjie.html

Go:   os.Args[1:]
来源：http://hz.hfpthk.cn/gtjvkwhklz.html

Ruby: ARGV
来源：http://hz.yueranfly.top/gtfmutvypd.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ydzc1.top/gtgkvwyhwk.html

[M02] 读取环境变量
来源：http://hz.yj20258888.top/gtywkagcol.html

Py:   os.environ.get("HOME")
来源：http://hz.redwolf501.top/gtazvlngwk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sysykeji.top/gtwrgvkosk.html

JS:   process.env.HOME
来源：http://hz.yongpay.top/gtcpszawah.html

TS:   process.env.HOME
来源：http://hz.sysykeji.top/gtxwpubnrk.html

Java: System.getenv("HOME")
来源：http://hz.jqgufenzy.top/gtetraoqoa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hfpthk.cn/gtabtfxlog.html

Ruby: ENV["HOME"]
来源：http://hz.svipenyu.cn/gtaejunuiv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinyuanbaomall.cn/gtvjykfuef.html

[M03] 执行外部命令
来源：http://hz.xingfuxueyuan.xyz/gtfcfbflpe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.iojbl.cn/gthmwpiswg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yuxming.cn/gtnfbebcct.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yongpay.top/gtyymrwcwg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuxming.cn/gtgbntcfln.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.aibaodan.cn/gtdnnfsnom.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.bjfxy.top/gtaklkkifa.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jqgfzy.top/gtsgsbsyyj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.vqdsnc.cn/gtzrycmkut.html

[M04] 获取当前工作目录
来源：http://hz.sufxvd.cn/gtbzphxncl.html

Py:   os.getcwd()
来源：http://hz.jiagoushi.top/gtfkwghqcw.html

PHP:  getcwd();
来源：http://hz.jianghu66.top/gtcvrgnqwv.html

JS:   process.cwd()
来源：http://hz.sufxvd.cn/gtpekzjwlz.html

TS:   process.cwd()
来源：http://hz.shanyushiyangkeji.top/gtcyptjxou.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yonumen.top/gtqcxnwlut.html

Go:   os.Getwd()
来源：http://hz.jinqigfzy.top/gtkfiayvbf.html

Ruby: Dir.pwd
来源：http://hz.mhx1999.top/gtqwdlbhye.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.bjfxy.top/gtedvzeyhh.html

[M05] 设置退出码
来源：http://hz.sxryk.cn/gtvrlbwecd.html

Py:   sys.exit(1)
来源：http://hz.xylfe.cn/gtuxqucyku.html

PHP:  exit(1);
来源：http://hz.sufxvd.cn/gtvcycvzpj.html

JS:   process.exit(1)
来源：http://hz.kuanghao11.cn/gtqqavjiyy.html

TS:   process.exit(1)
来源：http://hz.ydjk.org.cn/gtuzssngbk.html

Java: System.exit(1)
来源：http://hz.ivvv.top/gtfesejpyz.html

Go:   os.Exit(1)
来源：http://hz.yj20258.top/gturbttupu.html

Ruby: exit 1
来源：http://hz.xuetiantiany.cn/gtoomlzsdw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zdqjudy.top/gtmwlypluo.html

[M06] 向标准错误输出
来源：http://hz.yuxming.cn/gtwgzvvdff.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yj20258.top/gtfutnhpsq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gaohongyu789.top/gtvinndkkn.html

JS:   console.error("err")
来源：http://hz.hongshengwenyu.top/gtmfyojkvc.html

TS:   console.error("err")
来源：http://hz.shanyushiyangkeji.top/gtkfulhlbg.html

Java: System.err.println("err")
来源：http://hz.cqqwz.cn/gtfalnwykw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sufxvd.cn/gtrsvynxki.html

Ruby: warn "err"
来源：http://hz.c1oappe.top/gtncleduqm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jlsjyb.cn/gtsfqyvlcn.html

[M07] 判断是否为主入口
来源：http://hz.ivvv.top/gtmdisbblr.html

Py:   if __name__ == "__main__":
来源：http://hz.tian-w.cn/gttwqmvnpg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.tianlin.xyz/gtsljjsddw.html

JS:   require.main === module
来源：http://hz.smart0.xyz/gtlcazzjzg.html

TS:   require.main === module
来源：http://hz.yueranfly.top/gtduxvnuza.html

Java: public static void main(String[] args)
来源：http://hz.birdmap.top/gtcpgmfmla.html

Go:   func main()
来源：http://hz.tianlin.xyz/gtanxqnxys.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.dashuyun.cn/gtytclbgtd.html

C#:   static void Main(string[] args)
来源：http://hz.ivvv.top/gtfgifdblq.html

[M08] 获取系统与运行时信息
来源：http://hz.feifeiyinyue.top/gtvbrieopl.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jqgufenzy.top/gtwicpxiwg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yj20258.top/gtwroyxlnx.html

JS:   process.platform;  process.version
来源：http://hz.zdqjudy.top/gticusrvpy.html

TS:   process.platform;  process.version
来源：http://hz.yj20258.top/gtwahwncwk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.vqdsnc.cn/gtszlfeomg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.9152youxi.cn/gthzewosve.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.mhx1999.top/gtcjysdboj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yuxming.cn/gttjqroydq.html

================================================================================
来源：http://hz.ydjk.org.cn/gthofvxjzk.html

N. 数据结构与算法
来源：http://hz.sxryk.cn/gtvxjoytvm.html

================================================================================
来源：http://hz.yj20258.top/gtsxwjpcro.html

[N01] 二分查找（有序数组）
来源：http://hz.quarkkingdee.top/gtuyczxnou.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.havefunace.top/gtwsorlswb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yangfankeji.com/gtkgspciwd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sufxvd.cn/gtomeclhpd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.mhx1999.top/gtrylwstqs.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yj202588.top/gtedkzpzqx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.havefunace.top/gthqhqmaxt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xinyue.icu/gtevsgnllr.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shangyingyoupin.top/gtxkldevsp.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hongshengwenyu.top/gtduxgmtqo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gaohongyu789.top/gtmwhqvptu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yanxiufei.cn/gtmfzhacab.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.9152youxi.cn/gtcgdzsypf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shuidangran.top/gtxqamjjyz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ywan-chungtsiang.top/gthwhnlbhq.html

Go:   slices.Sort(arr)
来源：http://hz.yj20258888.top/gtnedwldun.html

Ruby: arr.sort
来源：http://hz.jinyuanbaomall.cn/gtqtgirnew.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sysykeji.top/gtztqzarco.html

[N03] 快速排序（分治示例）
来源：http://hz.9152youxi.cn/gtfspgcjrt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.snrcjt.cn/gtcckwafrd.html

PHP:  // 递归实现，或用 usort
来源：http://hz.redwolf501.top/gtjlwnueyy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xylfe.cn/gtkodjldxr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pengpengdd.cyou/gtfcnaegxq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhijiandao.cn/gtwmpwwhqu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ybcxt.top/gtfqxboofi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xuanzx.com/gtsqcwgfqi.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xinyue.icu/gtgpmwpyhu.html

[N04] 斐波那契数列
来源：http://hz.hysaishi.cn/gtdiweuhdd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tian-w.cn/gtbwqscwkl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.guannengcc.top/gtfyfetduw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhiwuduotai.top/gttaeguxme.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxuanxn.top/gtsxjdrmpq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ybcxt.top/gtycwqeoxp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yangfankeji.com/gtitdyfszu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigufen.top/gtcufqycps.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenzaomai.com/gtempiglej.html

[N05] 最大公约数
来源：http://hz.xingfuxueyuan.xyz/gtguliglse.html

Py:   math.gcd(a, b)
来源：http://hz.zhiwuduotai.top/gtiytvzsvi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.aibaodan.cn/gtdvciuhkd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yvedp.cn/gtegelnhvz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sysykeji.top/gtkhutodor.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.wangdashe.top/gtjtcftnrp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinyuanbaomall.cn/gtzbnhtmux.html

Ruby: a.gcd(b)
来源：http://hz.xylfe.cn/gtobxnzjyw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.sysykeji.top/gtxqpzclpl.html

[N06] 判断回文字符串
来源：http://hz.fengsongda.top/gtdvxkijmw.html

Py:   s == s[::-1]
来源：http://hz.yuxming.cn/gtjdohvnvh.html

PHP:  $s === strrev($s);
来源：http://hz.tanke756.top/gtvaryoxiz.html

JS:   s === [...s].reverse().join("")
来源：http://hz.haohaochexian.top/gtesolimzb.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gtjdtalyrs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.tanke756.top/gtcleiiuhg.html

Go:   // 双指针从两端比较
来源：http://hz.shangyingyoupin.top/gtsguvcwyn.html

Ruby: s == s.reverse
来源：http://hz.tian-w.cn/gtlnqipzmt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cdnleiting.top/gtoopczjpf.html

[N07] 两数之和（返回下标）
来源：http://hz.52xcode.cn/gtiuwmigxw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.52xcode.cn/gtwzheaiqs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yonumen.top/gtutbybbud.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ydzc1.top/gtbduzqlsg.html

TS:   // 手写 Map<string, number>
来源：http://hz.cheryme.top/gtjojriwdr.html

Java: // 手写 HashMap
来源：http://hz.svipenyu.cn/gtnpslhdhx.html

Go:   // 手写 map[int]int
来源：http://hz.gotoacloud.top/gtlojopacb.html

Ruby: // 手写 Hash
来源：http://hz.0kj1m.cn/gtklhbqdyf.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zycfv.cn/gtasdymqai.html

[N08] 生成全排列
来源：http://hz.tanke756.top/gtpjbiuvzt.html

Py:   itertools.permutations(arr)
来源：http://hz.sxryk.cn/gtbwpvlnjx.html

PHP:  // 手写递归交换
来源：http://hz.ppjwa.cn/gtaeysfwmf.html

JS:   // 手写回溯递归
来源：http://hz.jqgfzy.top/gtltqokhpr.html

TS:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtwllubkfn.html

Java: // 手写回溯递归
来源：http://hz.yueranfly.top/gtuhildzis.html

Go:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtbwmaxbfs.html

Ruby: arr.permutation.to_a
来源：http://hz.hnqzz.top/gtgmtohfsi.html

C#:   // 手写回溯递归
来源：http://hz.ivvv.top/gtvnphvxgg.html

[N09] 栈与队列
来源：http://hz.ydjk.org.cn/gteurvwdiq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yuanzhike.top/gtpsboyymg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.sweek.top/gtxanzmafd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xingfuxueyuan.xyz/gtqlpubdvu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.sxryk.cn/gtcbekniql.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.dianchejie.cn/gtittbhjip.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.guowangkeji.top/gtduxqwvke.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.havefunace.top/gthobmijxf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gzhubu.top/gtuspjrgsv.html

[N10] 链表节点定义
来源：http://hz.yuxming.cn/gthvfkjhci.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.quarkkingdee.top/gtivnjhnvg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xylfe.cn/gtobcoztlk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jlsjyb.cn/gtmtwxldke.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.pycfn.com/gtsyybalon.html

Java: class Node { int v; Node next; }
来源：http://hz.daxiang520.top/gthayizoou.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jlsjyb.cn/gtuxmocyhc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.aibaodan.cn/gtroyhregv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hammf.cn/gtdpwryytt.html

[N11] 二叉树中序遍历
来源：http://hz.jqgfzy.top/gtpiaxytss.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhengqikj.top/gtgmvlxgoh.html

PHP:  // 手写递归函数
来源：http://hz.wangshuangyany.cn/gtpihrrgxw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gzhubu.top/gtuwdgdqic.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tian-w.cn/gthydhznot.html

Java: // 手写递归
来源：http://hz.redwolf501.top/gtfmpqsxyf.html

Go:   // 手写递归
来源：http://hz.hfpthk.cn/gtulynfekw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ybcxt.top/gttctkfiqu.html

C#:   // 手写递归
来源：http://hz.sxryk.cn/gtbxtfqaxi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shanyushiyangkeji.top/gtpmjxaixg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xinyue.icu/gtjkfiddhk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hongshengwenyu.top/gthvbwpqrh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.mhx1999.top/gtcdbjcehb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.vqdsnc.cn/gtpagcdnjc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gaohongyu789.top/gtpxzkdcfq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.mhx1999.top/gtbmywjirj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hfpthk.cn/gtjipnnsuy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.vqdsnc.cn/gtsiylvbrb.html

================================================================================
来源：http://hz.hammf.cn/gtdogbnfev.html

O. 并发与异步
来源：http://hz.hysaishi.cn/gtemqdfdfs.html

================================================================================
来源：http://hz.dianchejie.cn/gtrlhehspt.html

[O01] 启动一个线程
来源：http://hz.ydzc1.top/gtwwbdnsnb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xylfe.cn/gtkyqkgvbi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xingfuxueyuan.xyz/gtnzrljbnq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.aizwys.cn/gtrblovnwa.html

TS:   // 同 JS
来源：http://hz.jlsjyb.cn/gttiyxwmwj.html

Java: new Thread(() -> f()).start()
来源：http://hz.yonumen.top/gtkudxjaaj.html

Go:   go f()
来源：http://hz.sufxvd.cn/gtlzrqoick.html

Ruby: Thread.new { f }
来源：http://hz.nanxinkj.top/gtyuqvxvum.html

C#:   Task.Run(() => F());
来源：http://hz.zhongyouzk.top/gtprmrmzzw.html

[O02] 使用线程池
来源：http://hz.mhx1999.top/gtsftfsvot.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xziqi.cn/gtmbglmtdo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.gzhubu.top/gtsrijzhqz.html

JS:   // worker_threads 线程池
来源：http://hz.jinqigfzy.top/gttorxddzk.html

TS:   // worker_threads 线程池
来源：http://hz.hammf.cn/gtimcgywdi.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.chenjidiqi.icu/gtwurungnk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yj20258888.top/gtbijrzuqa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xinyue.icu/gtsgvfbucy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.guannengcc.top/gtlzgeoajn.html

[O03] 加锁保护共享数据
来源：http://hz.shanyushiyangtech.top/gtkvgvexyz.html

Py:   with lock: shared += 1
来源：http://hz.hammf.cn/gtyltpdmtq.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.andypj.xyz/gthazfcexv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.dashuyun.cn/gtjotcmxtm.html

TS:   // 同 JS
来源：http://hz.zhijiandao.cn/gtbfdwcnnt.html

Java: synchronized (this) { shared++; }
来源：http://hz.aibaodan.cn/gtnxmzwakf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.sweek.top/gtnwkvidlc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hnxiangtu.top/gthzmiijkz.html

C#:   lock (gate) { shared++; }
来源：http://hz.cqqwz.cn/gtuzlrtjdf.html

[O04] 定义异步函数并等待
来源：http://hz.haohaochexian.top/gtiaisyzkc.html

Py:   async def f():⏎    await g()
来源：http://hz.sweek.top/gtilhzyrvw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yuanzhike.top/gtvjlemrvw.html

JS:   async function f() { await g(); }
来源：http://hz.zhengqikj.top/gtwkpmnjlx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jlsjyb.cn/gtekugjwtz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ehwqpu.com/gtfempthgl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ivvv.top/gtrjuphyvm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jinghuilouyu.cn/gthqxgvubs.html

C#:   async Task F() { await G(); }
来源：http://hz.zhijiandao.cn/gtaueivqcx.html

[O05] 并发执行并等待全部完成
来源：http://hz.ydzc1.top/gtfzqhavuj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cheryme.top/gtxghurmdi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.dashuyun.cn/gtggdkssqu.html

JS:   await Promise.all(tasks)
来源：http://hz.jinghuilouyu.cn/gtkxitlaud.html

TS:   await Promise.all(tasks)
来源：http://hz.chenjidiqi.icu/gtgehdtxyx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.quarkkingdee.top/gtczfhjlkf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sxryk.cn/gtxlyfhcbi.html

Ruby: threads.map(&:join)
来源：http://hz.birdmap.top/gtdbcfzjfq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.daria6918.cn/gtqytjwnux.html

[O06] 使用进程池
来源：http://hz.feifeiyinyue.top/gtjoxmgpfw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shzxlz.cn/gttxsliplb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhijiandao.cn/gtmwnggzoc.html

JS:   // child_process / cluster 模块
来源：http://hz.yj20258888.top/gtyrreuduf.html

TS:   // child_process / cluster 模块
来源：http://hz.hammf.cn/gtbagcrppk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.andypj.xyz/gttsxnxkjo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xinyue.icu/gtccsxzszp.html

Ruby: // fork 块
来源：http://hz.ywan-chungtsiang.top/gtjyljeady.html

C#:   Parallel.For
来源：http://hz.ydjk.org.cn/gttlegwvgg.html

================================================================================
来源：http://hz.aizwys.cn/gtaeqfmtcd.html

P. 常用工具函数
来源：http://hz.quarkkingdee.top/gtwiayzmwe.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtujenhcks.html

[P01] 生成 UUID
来源：http://hz.316326.xyz/gtfndiwcxs.html

Py:   str(uuid.uuid4())
来源：http://hz.cdnleiting.top/gtobcbnvhd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hfpthk.cn/gtgvheuzvb.html

JS:   crypto.randomUUID()
来源：http://hz.yvedp.cn/gtyvmshttj.html

TS:   crypto.randomUUID()
来源：http://hz.yuanzhike.top/gttrmadiec.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhiwuduotai.top/gtefrggpfz.html

Go:   // 用 github.com/google/uuid
来源：http://hz.9152youxi.cn/gtmamtcfxo.html

Ruby: SecureRandom.uuid
来源：http://hz.haohaochexian.top/gtarterwrm.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cashguo.top/gtxotqrjpv.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinghuilouyu.cn/gtbhwzmolv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.dashuyun.cn/gtnjfiiwij.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zycfv.cn/gtrlopepic.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.vqdsnc.cn/gtdlbolzpr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.tanke756.top/gttqclhwuv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhijiandao.cn/gtdckaxtiv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.wangdashe.top/gtsaamfaoy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hfpthk.cn/gtesmnihxt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.c1oappe.top/gtnbpulucg.html

[P03] 生成短随机字符串
来源：http://hz.xuanzx.com/gtnihyagko.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shuidangran.top/gttpnecvwk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ywan-chungtsiang.top/gtkjplvdry.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nwbrower.top/gtjrysfbhg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj202588.top/gttjbbuidp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.redwolf501.top/gthcnkyjaz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yangfankeji.com/gtwysrwgwm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.iojbl.cn/gtlgdsltnj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.birdmap.top/gtvjyhwcuu.html

[P04] 求长度
来源：http://hz.zhongyouzk.top/gtmtstkrfs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhijiandao.cn/gtbxoklrva.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jlsjyb.cn/gtzbbointj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jianghu66.top/gtasrpehuv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ppjwa.cn/gtxvfqziyj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.kuanghao11.cn/gtylrgazat.html

Go:   len(arr);  len(m)
来源：http://hz.pengpengdd.cyou/gtjyxyxvbf.html

Ruby: x.length;  x.size
来源：http://hz.kuanghao11.cn/gtnaqyruyd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.bjfxy.top/gtmwoextlw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shangyingyoupin.top/gthqinkxkx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.havefunace.top/gtflyhdhlz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xuanzx.com/gtgnvzbuag.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.9152youxi.cn/gttjvnfdqv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.andypj.xyz/gtwzayeykc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.chenlongwang.top/gtnrpconpw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yanxiufei.cn/gtdqbmamkv.html

Ruby: a == b
来源：http://hz.yueranfly.top/gtyepbedzm.html


<!-- 参考信息 -->