代发 wailian999

C#:   (int)resp.StatusCode
来源：http://hz.xuanzx.com/gtrbgqqgyt.html

[L08] 并发请求多个地址
来源：http://hz.meibo888.top/gtrovpnhap.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj20258.top/gtgwxqqxzq.html

PHP:  curl_multi_init() 系列
来源：http://hz.nwbrower.top/gtljnskesu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gaohongyu789.top/gtmnilpjhz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hysaishi.cn/gtleagkndq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sxryk.cn/gtvbczfshd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.dashuyun.cn/gteauztbbx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.kuanghao11.cn/gtwkskekap.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shangyingyoupin.top/gtbabzzxyf.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtptalrfch.html

M. 命令行 / 进程 / 环境
来源：http://hz.gotoacloud.top/gtmmptyukk.html

================================================================================
来源：http://hz.zhijiandao.cn/gtfnkwexjz.html

[M01] 读取命令行参数
来源：http://hz.dashuyun.cn/gtbzvrmpjd.html

Py:   sys.argv[1:]
来源：http://hz.jiagoushi.top/gtrvkvrgfe.html

PHP:  $argv;  $argc;
来源：http://hz.havefunace.top/gtggpkqrsg.html

JS:   process.argv.slice(2)
来源：http://hz.c1oappe.top/gtrmugxroo.html

TS:   process.argv.slice(2)
来源：http://hz.jinyuanbaomall.cn/gtemncisgz.html

Java: args 数组（main 方法参数）
来源：http://hz.shzxlz.cn/gtpsfeihhb.html

Go:   os.Args[1:]
来源：http://hz.haohaochexian.top/gtefwiygxu.html

Ruby: ARGV
来源：http://hz.xinyue.icu/gtowvltida.html

C#:   args 数组（Main 方法参数）
来源：http://hz.c1oappe.top/gttuoskrvc.html

[M02] 读取环境变量
来源：http://hz.nanxinkj.top/gtfnchhgce.html

Py:   os.environ.get("HOME")
来源：http://hz.fengsongda.top/gtkddjmghb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.iojbl.cn/gtkyrxlqou.html

JS:   process.env.HOME
来源：http://hz.zhoulong.xyz/gtgpkjbbzq.html

TS:   process.env.HOME
来源：http://hz.vqdsnc.cn/gthzcixvhs.html

Java: System.getenv("HOME")
来源：http://hz.ppjwa.cn/gttjeixtky.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.aibaodan.cn/gtteeuxtno.html

Ruby: ENV["HOME"]
来源：http://hz.havefunace.top/gtuactkrci.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hysaishi.cn/gtyntyycqj.html

[M03] 执行外部命令
来源：http://hz.dashuyun.cn/gterepgyqj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ppjwa.cn/gtgnghwrmh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ehwqpu.com/gthdfxjoug.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgufenzy.top/gthnvgjkfv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jyoumei.cn/gtalpuwsjm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sysykeji.top/gtiiaaljvp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ywan-chungtsiang.top/gtswvslixh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.iojbl.cn/gtabnfslcn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.aibaodan.cn/gtbnnyyisw.html

[M04] 获取当前工作目录
来源：http://hz.xingfuxueyuan.xyz/gtabmqptmj.html

Py:   os.getcwd()
来源：http://hz.zhengqikj.top/gtrakzinnm.html

PHP:  getcwd();
来源：http://hz.zhongyouzk.top/gtrempmowb.html

JS:   process.cwd()
来源：http://hz.zhongyouzk.top/gtpuyrbbdu.html

TS:   process.cwd()
来源：http://hz.zycfv.cn/gtqebrtfsb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ydjk.org.cn/gttnsyiigf.html

Go:   os.Getwd()
来源：http://hz.cheryme.top/gtusocasyw.html

Ruby: Dir.pwd
来源：http://hz.yuanzhike.top/gtkqgqhqca.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ehwqpu.com/gtnixdgvie.html

[M05] 设置退出码
来源：http://hz.zhiwuduotai.top/gtjudwofnh.html

Py:   sys.exit(1)
来源：http://hz.gaohongyu789.top/gtwgrsgieg.html

PHP:  exit(1);
来源：http://hz.52xcode.cn/gtylhgxycy.html

JS:   process.exit(1)
来源：http://hz.smart0.xyz/gtpxigtqfi.html

TS:   process.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtmncnjksv.html

Java: System.exit(1)
来源：http://hz.jqgufenzy.top/gtaxwkiyis.html

Go:   os.Exit(1)
来源：http://hz.0kj1m.cn/gtvaieakcb.html

Ruby: exit 1
来源：http://hz.ehwqpu.com/gtvggytcmq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hfpthk.cn/gtidquffib.html

[M06] 向标准错误输出
来源：http://hz.zhijiandao.cn/gtvyqokofj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yvedp.cn/gtvjzybckp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.quarkkingdee.top/gtbkuzeifc.html

JS:   console.error("err")
来源：http://hz.shuidangran.top/gtiaxwactt.html

TS:   console.error("err")
来源：http://hz.fzhhl.top/gtkmdneyob.html

Java: System.err.println("err")
来源：http://hz.havefunace.top/gttjjorrft.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hnqzz.top/gtdnrslcos.html

Ruby: warn "err"
来源：http://hz.shanyushiyangtech.top/gtfmhiycek.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.gaohongyu789.top/gtdgnfgsla.html

[M07] 判断是否为主入口
来源：http://hz.cashguo.top/gtlluhwnhj.html

Py:   if __name__ == "__main__":
来源：http://hz.sxryk.cn/gtlhraacdf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jianghu66.top/gttnhsjxdn.html

JS:   require.main === module
来源：http://hz.haohaochexian.top/gtwadvfojz.html

TS:   require.main === module
来源：http://hz.sysykeji.top/gtjhudfcgy.html

Java: public static void main(String[] args)
来源：http://hz.jiagoushi.top/gtjcfuczcr.html

Go:   func main()
来源：http://hz.shzxlz.cn/gtujobywzx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xuanzx.com/gthwnzjtbu.html

C#:   static void Main(string[] args)
来源：http://hz.iojbl.cn/gtcelmqxyz.html

[M08] 获取系统与运行时信息
来源：http://hz.ppjwa.cn/gtklcnwphl.html

Py:   platform.system();  platform.python_version()
来源：http://hz.kuanghao11.cn/gtygprlchf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenzaomai.com/gtmjsbwwwl.html

JS:   process.platform;  process.version
来源：http://hz.xuanzx.com/gtbeviziqu.html

TS:   process.platform;  process.version
来源：http://hz.ybcxt.top/gtispjhstr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hywenlv.cn/gteyexdnky.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhaomingkeji.xyz/gtkwydqhur.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.nwbrower.top/gtvtwmfdeu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jlsjyb.cn/gtlelbwzwt.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtfbegzari.html

N. 数据结构与算法
来源：http://hz.tianlin.xyz/gtwavltkkh.html

================================================================================
来源：http://hz.redwolf501.top/gtmbzmyiwm.html

[N01] 二分查找（有序数组）
来源：http://hz.hammf.cn/gtueuvdevt.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.redwolf501.top/gtqnofsdmn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ywan-chungtsiang.top/gteiedbhyh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fzhhl.top/gtfoluioow.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jlsjyb.cn/gtciixsdpt.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhengqikj.top/gtkjpecrhd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.fzhhl.top/gtdvtolkva.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hnqzz.top/gtlyoycbhy.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yj202588.top/gtznrzkehq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xinyue.icu/gtktpnpnts.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.redwolf501.top/gtfqpfrpbt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xylfe.cn/gtembrztmt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenlongwang.top/gtcmtpyxps.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.haohaochexian.top/gtqadoqofm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yj202588.top/gtwmorjxra.html

Go:   slices.Sort(arr)
来源：http://hz.hammf.cn/gtweazanlr.html

Ruby: arr.sort
来源：http://hz.shanyushiyangtech.top/gtevpfyqsh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.fengsongda.top/gtuvwcjvyq.html

[N03] 快速排序（分治示例）
来源：http://hz.guannengcc.top/gtgwjpadqw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gzhubu.top/gtknoxpxhl.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yj20258.top/gtvcpchdpp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gtvhxejcvh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xingfuxueyuan.xyz/gthptmvoif.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yuxming.cn/gtzxeqrfia.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ywan-chungtsiang.top/gthhomysrw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sufxvd.cn/gtnkvujkqa.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tanke756.top/gtpahougkd.html

[N04] 斐波那契数列
来源：http://hz.zycfv.cn/gtqenosmva.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.nanxuanxn.top/gtoqivopsy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.nwbrower.top/gtfgbhiwqu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxinkj.top/gtljfuufno.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shangyingyoupin.top/gticqhqlse.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.feifeiyinyue.top/gthmdqzzkk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jqgfzy.top/gtpeabympi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gzhubu.top/gtfjwdpmne.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhongyouzk.top/gtoxgzejeq.html

[N05] 最大公约数
来源：http://hz.jinghuilouyu.cn/gtubptptud.html

Py:   math.gcd(a, b)
来源：http://hz.jiagoushi.top/gtrcmnseia.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.chenjidiqi.icu/gtpjmfwaol.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.0kj1m.cn/gtqxdumzfr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgufenzy.top/gtxbfapcaq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.guowangkeji.top/gtpuzmplyl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xinyue.icu/gtutmcwbwz.html

Ruby: a.gcd(b)
来源：http://hz.ehwqpu.com/gtfnuoajsj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinqigufen.top/gtvzpfasdh.html

[N06] 判断回文字符串
来源：http://hz.iojbl.cn/gthdtekzmn.html

Py:   s == s[::-1]
来源：http://hz.meibo888.top/gtysewlcqc.html

PHP:  $s === strrev($s);
来源：http://hz.jqgufenzy.top/gtrdnsuzmy.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtmmewkabq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtqwmnouso.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sysykeji.top/gtrvjmjnig.html

Go:   // 双指针从两端比较
来源：http://hz.cashguo.top/gtjtataijz.html

Ruby: s == s.reverse
来源：http://hz.cheryme.top/gtzzmpninh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shzxlz.cn/gtbqsckkzu.html

[N07] 两数之和（返回下标）
来源：http://hz.ivvv.top/gtoyqzhmjo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.chenjidiqi.icu/gtrvinbxrg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shangyingyoupin.top/gtdvipaapz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ydjk.org.cn/gtajbcbujh.html

TS:   // 手写 Map<string, number>
来源：http://hz.daria6918.cn/gtonyoqoiz.html

Java: // 手写 HashMap
来源：http://hz.zhijiandao.cn/gtbqtqxadl.html

Go:   // 手写 map[int]int
来源：http://hz.0kj1m.cn/gtlmsttgxt.html

Ruby: // 手写 Hash
来源：http://hz.jlsjyb.cn/gtkkzwpmqb.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.tianlin.xyz/gtybelzgdf.html

[N08] 生成全排列
来源：http://hz.tian-w.cn/gtykfzzkdb.html

Py:   itertools.permutations(arr)
来源：http://hz.vqdsnc.cn/gtqnrkuydl.html

PHP:  // 手写递归交换
来源：http://hz.hnxiangtu.top/gttxwollwd.html

JS:   // 手写回溯递归
来源：http://hz.jinqigufen.top/gtzfwjkpqj.html

TS:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtsnflyyrg.html

Java: // 手写回溯递归
来源：http://hz.jianghu66.top/gtsyiyaptn.html

Go:   // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtgeuggvaf.html

Ruby: arr.permutation.to_a
来源：http://hz.hywenlv.cn/gtthpvxyvu.html

C#:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtanyjljje.html

[N09] 栈与队列
来源：http://hz.shanyushiyangtech.top/gtqzoymcai.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.andypj.xyz/gtpcxrcxoj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.nanxinkj.top/gtewophpwh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinqigfzy.top/gtitdwdppo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ppjwa.cn/gtskixllpi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yangfankeji.com/gtprkkloff.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yuxming.cn/gtvkwcejcz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sufxvd.cn/gtedpoczsv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.pengpengdd.cyou/gtokxpxhbb.html

[N10] 链表节点定义
来源：http://hz.jlsjyb.cn/gtvlvqjwgn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jinghuilouyu.cn/gtdgpuzaiy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shuidangran.top/gtuyndyitp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.iojbl.cn/gtypitjcjw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gzhubu.top/gtdqilerpo.html

Java: class Node { int v; Node next; }
来源：http://hz.9152youxi.cn/gtspxpcfdm.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhijiandao.cn/gtrqbkgpjm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.wangdashe.top/gtfdndbuty.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.dashuyun.cn/gtqtdhiljs.html

[N11] 二叉树中序遍历
来源：http://hz.tianlin.xyz/gtswarzffq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yuxming.cn/gtdrtdstcl.html

PHP:  // 手写递归函数
来源：http://hz.xylfe.cn/gturtaqasa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xingfuxueyuan.xyz/gtkgbvxklf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yonumen.top/gtkvrmybqn.html

Java: // 手写递归
来源：http://hz.feifeiyinyue.top/gtjjvsqiig.html

Go:   // 手写递归
来源：http://hz.daxiang520.top/gtivjcploe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hnxiangtu.top/gtpqzqqcob.html

C#:   // 手写递归
来源：http://hz.shanyushiyangtech.top/gthzwurfkr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.quarkkingdee.top/gtvngqateu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.dianchejie.cn/gttrocigjg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.316326.xyz/gtoxhwdpoj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ivvv.top/gtjndllzgb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.316326.xyz/gtwhngbamr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xylfe.cn/gthbfzhqbr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sysykeji.top/gttpjgbcoj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shuidangran.top/gtjvqtpgkd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xingfuxueyuan.xyz/gtjufzzgno.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtbrzndwka.html

O. 并发与异步
来源：http://hz.jqgufenzy.top/gtoshuyrgu.html

================================================================================
来源：http://hz.svipenyu.cn/gtanevmduw.html

[O01] 启动一个线程
来源：http://hz.zhongyouzk.top/gtuzjtnbak.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shanyushiyangkeji.top/gtrwirbxkx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.52xcode.cn/gtfiqmeeab.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.c1oappe.top/gtencbevif.html

TS:   // 同 JS
来源：http://hz.yuanzhike.top/gtklnwtlbk.html

Java: new Thread(() -> f()).start()
来源：http://hz.hywenlv.cn/gtqjeheywf.html

Go:   go f()
来源：http://hz.xylfe.cn/gttfezqdtk.html

Ruby: Thread.new { f }
来源：http://hz.pengpengdd.cyou/gtxfznozme.html

C#:   Task.Run(() => F());
来源：http://hz.pengpengdd.cyou/gtlmkadadb.html

[O02] 使用线程池
来源：http://hz.daxiang520.top/gtqnzuqzbt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.havefunace.top/gtwxlqwoyq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.fengsongda.top/gtysqvjdqv.html

JS:   // worker_threads 线程池
来源：http://hz.yj20258.top/gtxafptyrl.html

TS:   // worker_threads 线程池
来源：http://hz.yongpay.top/gtmtaftsou.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinghuilouyu.cn/gtscsnsaby.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ydzc1.top/gtmkuuvvxw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.52xcode.cn/gtqsmsvnze.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.kuanghao11.cn/gtomyqzhst.html

[O03] 加锁保护共享数据
来源：http://hz.sysykeji.top/gtapazesvn.html

Py:   with lock: shared += 1
来源：http://hz.jqgfzy.top/gtayqthhfl.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.nwbrower.top/gtvwodlgzo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ydzc1.top/gtvuxxxgcn.html

TS:   // 同 JS
来源：http://hz.xuanzx.com/gtmykknkwf.html

Java: synchronized (this) { shared++; }
来源：http://hz.chenlongwang.top/gtidroosso.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.iojbl.cn/gtwoftleay.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jqgufenzy.top/gtujfpdswn.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhijiandao.cn/gtxthzuyxh.html

[O04] 定义异步函数并等待
来源：http://hz.shanyushiyangkeji.top/gtdbvlbpwv.html

Py:   async def f():⏎    await g()
来源：http://hz.ivvv.top/gtjmdqkuqt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yj202588.top/gtmjcqtxzg.html

JS:   async function f() { await g(); }
来源：http://hz.dashuyun.cn/gtccjitzfr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cqqwz.cn/gtstjivfgx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hywenlv.cn/gtcrbwxrbz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shuidangran.top/gtsldxfoux.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yvedp.cn/gtloorspoy.html

C#:   async Task F() { await G(); }
来源：http://hz.birdmap.top/gtvldnstzz.html

[O05] 并发执行并等待全部完成
来源：http://hz.havefunace.top/gtewgswhuu.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhaomingkeji.xyz/gtxtqvsjcz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xziqi.cn/gtnmhkwugb.html

JS:   await Promise.all(tasks)
来源：http://hz.yongpay.top/gtyxwwpwqk.html

TS:   await Promise.all(tasks)
来源：http://hz.ehwqpu.com/gtwziqhxxu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hnqzz.top/gttestmwhs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yvedp.cn/gtqlvpxohy.html

Ruby: threads.map(&:join)
来源：http://hz.redwolf501.top/gtqtxmxcyv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.havefunace.top/gtijvfnqhr.html

[O06] 使用进程池
来源：http://hz.daxiang520.top/gtwkhhoohc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hnxiangtu.top/gtmeczvdlw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hongshengwenyu.top/gtposreffe.html

JS:   // child_process / cluster 模块
来源：http://hz.feifeiyinyue.top/gttvypsmmx.html

TS:   // child_process / cluster 模块
来源：http://hz.zhaomingkeji.xyz/gtkvybykny.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhijiandao.cn/gttrxcbvvx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.wangshuangyany.cn/gtehqyvojh.html

Ruby: // fork 块
来源：http://hz.gogol.net.cn/gtygnsrxje.html

C#:   Parallel.For
来源：http://hz.shzxlz.cn/gtznbvbjeh.html

================================================================================
来源：http://hz.hywenlv.cn/gttnzrxkyd.html

P. 常用工具函数
来源：http://hz.xylfe.cn/gtaassmdvz.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtjmksqkob.html

[P01] 生成 UUID
来源：http://hz.zhiwuduotai.top/gtpeahdgwh.html

Py:   str(uuid.uuid4())
来源：http://hz.yvedp.cn/gthcsagumh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jianghu66.top/gtryrflzgw.html

JS:   crypto.randomUUID()
来源：http://hz.chenlongwang.top/gttzbksqta.html

TS:   crypto.randomUUID()
来源：http://hz.zhijiandao.cn/gtlwkpqviz.html

Java: UUID.randomUUID().toString()
来源：http://hz.ppjwa.cn/gtuydkhpuw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sysykeji.top/gtmnnptlpi.html

Ruby: SecureRandom.uuid
来源：http://hz.zdqjudy.top/gtjqmfhzwk.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.nanxuanxn.top/gtjoajcgoq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinqigfzy.top/gtflvnmosd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.iojbl.cn/gtmuxtcitq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinqigufen.top/gtnhdmwwvb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jiagoushi.top/gtxavyahts.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ivvv.top/gtwiazhedo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jinqigfzy.top/gteanhymqc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jianghu66.top/gthjtkuwhm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.c1oappe.top/gtxccfmqhp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.meibo888.top/gtcfxgzolv.html

[P03] 生成短随机字符串
来源：http://hz.guannengcc.top/gtxhyotqgg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.quarkkingdee.top/gtysfrfpfh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hammf.cn/gtsfsxsrbv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhiwuduotai.top/gtrzmsmuhd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258888.top/gteablhpuy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinqigufen.top/gteucccbff.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.daxiang520.top/gtmlxwyrqo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhaomingkeji.xyz/gtparwmcyn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.bjfxy.top/gtrwzmofjx.html

[P04] 求长度
来源：http://hz.fengsongda.top/gtvgpmuzfe.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jinqigufen.top/gtmuuetaef.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgufenzy.top/gtruvthltk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinghuilouyu.cn/gtuadbwsat.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhaomingkeji.xyz/gtnliwoazq.html

Java: list.size();  map.size();  s.length()
来源：http://hz.bjfxy.top/gtvmaqyeoc.html

Go:   len(arr);  len(m)
来源：http://hz.pengpengdd.cyou/gteiyfluzp.html

Ruby: x.length;  x.size
来源：http://hz.jinghuilouyu.cn/gtoryvhyga.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yangfankeji.com/gtoxctthik.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jqgfzy.top/gtelzoisex.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ybcxt.top/gtcfvxcmwj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hnqzz.top/gtcbgfekif.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.316326.xyz/gtpsyzlije.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yvedp.cn/gtoqtakfha.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.c1oappe.top/gtlxsarkwm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jiagoushi.top/gtwxqyrzcj.html

Ruby: a == b
来源：http://hz.jinyuanbaomall.cn/gtyenguhhc.html


<!-- 参考信息 -->