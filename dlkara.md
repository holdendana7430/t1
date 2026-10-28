代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.iojbl.cn/gthnigkkue.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yanxiufei.cn/gttfvbfpua.html

================================================================================
来源：http://hz.zhixingplan.top/gtreycszsb.html

M. 命令行 / 进程 / 环境
来源：http://hz.guannengcc.top/gtxqrazyta.html

================================================================================
来源：http://hz.ppjwa.cn/gtmdrlyjzg.html

[M01] 读取命令行参数
来源：http://hz.redwolf501.top/gtseidzyly.html

Py:   sys.argv[1:]
来源：http://hz.shanyushiyangkeji.top/gtexdsjfko.html

PHP:  $argv;  $argc;
来源：http://hz.yj202588.top/gtupjwxxus.html

JS:   process.argv.slice(2)
来源：http://hz.jiagoushi.top/gtfswgewan.html

TS:   process.argv.slice(2)
来源：http://hz.yuxming.cn/gtczajnlww.html

Java: args 数组（main 方法参数）
来源：http://hz.aizwys.cn/gtnltrwdnj.html

Go:   os.Args[1:]
来源：http://hz.c1oappe.top/gtoqciokmt.html

Ruby: ARGV
来源：http://hz.shzxlz.cn/gtbvngxkii.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinqigfzy.top/gtdwawjppb.html

[M02] 读取环境变量
来源：http://hz.shangyingyoupin.top/gtymipxotd.html

Py:   os.environ.get("HOME")
来源：http://hz.gogol.net.cn/gtyudgpjpk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jianghu66.top/gtngzcfobe.html

JS:   process.env.HOME
来源：http://hz.chenzaomai.com/gtmelrkbqg.html

TS:   process.env.HOME
来源：http://hz.nanxinkj.top/gtjxmfpbwy.html

Java: System.getenv("HOME")
来源：http://hz.yangfankeji.com/gthfrdibix.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhengqikj.top/gtiiataixw.html

Ruby: ENV["HOME"]
来源：http://hz.daria6918.cn/gtzagzukla.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yueranfly.top/gtrsxixewf.html

[M03] 执行外部命令
来源：http://hz.andypj.xyz/gtaegtgxrt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ywan-chungtsiang.top/gtcacivkrj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.aizwys.cn/gtxuupndna.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shangyingyoupin.top/gttdauuawn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.sxryk.cn/gtaljshuav.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jianghu66.top/gtrodyuytq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hnxiangtu.top/gtwowehmds.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.andypj.xyz/gtxgyfsgph.html

C#:   Process.Start("ls", "-l");
来源：http://hz.meibo888.top/gthmfjhxfc.html

[M04] 获取当前工作目录
来源：http://hz.jinyuanbaomall.cn/gtklwczmst.html

Py:   os.getcwd()
来源：http://hz.cucudq.cn/gtsokwuroa.html

PHP:  getcwd();
来源：http://hz.xuetiantiany.cn/gtfbqqtlyu.html

JS:   process.cwd()
来源：http://hz.hywenlv.cn/gtfppickxk.html

TS:   process.cwd()
来源：http://hz.haohaochexian.top/gtenptkuuk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hnqzz.top/gttrqloiwx.html

Go:   os.Getwd()
来源：http://hz.wangdashe.top/gthmomldlh.html

Ruby: Dir.pwd
来源：http://hz.yuxming.cn/gtbmbjkvwh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hongshengwenyu.top/gtdktitkag.html

[M05] 设置退出码
来源：http://hz.nanxinkj.top/gtwfxsxlfp.html

Py:   sys.exit(1)
来源：http://hz.shuidangran.top/gtvejfwppq.html

PHP:  exit(1);
来源：http://hz.yanxiufei.cn/gtocowmyln.html

JS:   process.exit(1)
来源：http://hz.sweek.top/gttyyimmbz.html

TS:   process.exit(1)
来源：http://hz.redwolf501.top/gtvzurnjiw.html

Java: System.exit(1)
来源：http://hz.hfpthk.cn/gtbzsawrfs.html

Go:   os.Exit(1)
来源：http://hz.andypj.xyz/gtocwfexgc.html

Ruby: exit 1
来源：http://hz.jqgufenzy.top/gtczggbsxa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gzhubu.top/gtzncidhtp.html

[M06] 向标准错误输出
来源：http://hz.fzhhl.top/gthpsbpaqz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.snrcjt.cn/gtynoylqie.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenzaomai.com/gtvbztnhgc.html

JS:   console.error("err")
来源：http://hz.xingfuxueyuan.xyz/gtygiqfcvq.html

TS:   console.error("err")
来源：http://hz.zhaomingkeji.xyz/gtexvqulic.html

Java: System.err.println("err")
来源：http://hz.aizwys.cn/gthxtbyena.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yvedp.cn/gtezlgscct.html

Ruby: warn "err"
来源：http://hz.hysaishi.cn/gtmgfwluyh.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhaomingkeji.xyz/gtoymuqkgi.html

[M07] 判断是否为主入口
来源：http://hz.shanyushiyangtech.top/gtrufaqgjd.html

Py:   if __name__ == "__main__":
来源：http://hz.wangdashe.top/gtbwlkgafu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.nwbrower.top/gtypzxqejv.html

JS:   require.main === module
来源：http://hz.sweek.top/gtgumoebam.html

TS:   require.main === module
来源：http://hz.haohaochexian.top/gtywxlzzos.html

Java: public static void main(String[] args)
来源：http://hz.zhongyouzk.top/gtsyfekjgo.html

Go:   func main()
来源：http://hz.tian-w.cn/gtbpvhpqbb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.tanke756.top/gtiqdaydet.html

C#:   static void Main(string[] args)
来源：http://hz.jinqigufen.top/gtofetumfg.html

[M08] 获取系统与运行时信息
来源：http://hz.zhiwuduotai.top/gtjkhkcwsr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jiagoushi.top/gtjnlovbdp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.pycfn.com/gtdzksuqti.html

JS:   process.platform;  process.version
来源：http://hz.birdmap.top/gtvusumybp.html

TS:   process.platform;  process.version
来源：http://hz.tian-w.cn/gtyouliked.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xuetiantiany.cn/gtrtbllopb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shanyushiyangtech.top/gtuzeqcknk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhixingplan.top/gtlzmxbeym.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhixingplan.top/gticbeqpvg.html

================================================================================
来源：http://hz.cdnleiting.top/gtvsdfcwgx.html

N. 数据结构与算法
来源：http://hz.zycfv.cn/gtdfkfhsbb.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtaikemlto.html

[N01] 二分查找（有序数组）
来源：http://hz.zhaomingkeji.xyz/gtfpsycclf.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jlsjyb.cn/gtesqhmecx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinqigufen.top/gtzznbozkl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinyuanbaomall.cn/gtefrpgouf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.meibo888.top/gtcgiywmlm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shanyushiyangtech.top/gtsachdbtp.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtbnhbtwnx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ehwqpu.com/gtzdbfjjtq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ydjk.org.cn/gtqwsmhcsn.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ywan-chungtsiang.top/gtcelpsiax.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jianghu66.top/gtckfbvvjk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sxryk.cn/gtrtwiagse.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.meibo888.top/gtqovnznvb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shzxlz.cn/gtrjxlpfso.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cashguo.top/gttcmjgqwx.html

Go:   slices.Sort(arr)
来源：http://hz.0kj1m.cn/gtteqqiqrq.html

Ruby: arr.sort
来源：http://hz.jlsjyb.cn/gtdqbepher.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.meibo888.top/gtalkofuha.html

[N03] 快速排序（分治示例）
来源：http://hz.ydjk.org.cn/gtobupczrg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yongpay.top/gtbxpyebym.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yj202588.top/gtjwfsuszf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhaomingkeji.xyz/gtvmxbtqas.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydjk.org.cn/gtjuiqagke.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ybcxt.top/gthaxszuwc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.tian-w.cn/gtcbdslowm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.wangdashe.top/gtkdibtfvo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhaomingkeji.xyz/gttqjbbwlb.html

[N04] 斐波那契数列
来源：http://hz.ehwqpu.com/gtnhsxptcm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xingfuxueyuan.xyz/gttdvovwju.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.dashuyun.cn/gttnevtles.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.feifeiyinyue.top/gtwfylziao.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuanzhike.top/gtddwamapd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ywan-chungtsiang.top/gtxydufknc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yangfankeji.com/gtttgkxdcg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinyuanbaomall.cn/gtplxevizz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj20258.top/gtjvypcmgd.html

[N05] 最大公约数
来源：http://hz.nanxinkj.top/gtitvcnmlv.html

Py:   math.gcd(a, b)
来源：http://hz.zycfv.cn/gtibuqtgse.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shuidangran.top/gtbcjhfiat.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.haohaochexian.top/gtnswczaeg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guannengcc.top/gtlhlmnunc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gaohongyu789.top/gtdbgaigqw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cheryme.top/gtkztpjrpt.html

Ruby: a.gcd(b)
来源：http://hz.ydzc1.top/gtezfislri.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xinyue.icu/gthkvnrxrt.html

[N06] 判断回文字符串
来源：http://hz.fzhhl.top/gtfaseuuxq.html

Py:   s == s[::-1]
来源：http://hz.0kj1m.cn/gtivhykyjq.html

PHP:  $s === strrev($s);
来源：http://hz.iojbl.cn/gtkcsyyvhq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangtech.top/gtzgvihvvu.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtisllgmgg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhengqikj.top/gtkpeotuhz.html

Go:   // 双指针从两端比较
来源：http://hz.fengsongda.top/gtzycrnlia.html

Ruby: s == s.reverse
来源：http://hz.zhongyouzk.top/gtfyyrwfbw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.chenjidiqi.icu/gtnplelmxk.html

[N07] 两数之和（返回下标）
来源：http://hz.tanke756.top/gtpfweycyt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.pengpengdd.cyou/gtjugyimfq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xinyue.icu/gtudfjbphx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ehwqpu.com/gtzfxhgopf.html

TS:   // 手写 Map<string, number>
来源：http://hz.fengsongda.top/gtxeurcglp.html

Java: // 手写 HashMap
来源：http://hz.shanyushiyangtech.top/gtbxcqywtf.html

Go:   // 手写 map[int]int
来源：http://hz.zhixingplan.top/gtvmjaunby.html

Ruby: // 手写 Hash
来源：http://hz.wangdashe.top/gtnsgpkwst.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.quarkkingdee.top/gtatwsnmpb.html

[N08] 生成全排列
来源：http://hz.daxiang520.top/gtlvoxhfeg.html

Py:   itertools.permutations(arr)
来源：http://hz.hywenlv.cn/gtsjaoniol.html

PHP:  // 手写递归交换
来源：http://hz.shanyushiyangkeji.top/gtggwqbwwk.html

JS:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtehinuxyi.html

TS:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtjscjcpbz.html

Java: // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtvmejjwfp.html

Go:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtrqynpxtr.html

Ruby: arr.permutation.to_a
来源：http://hz.sufxvd.cn/gtppuowlca.html

C#:   // 手写回溯递归
来源：http://hz.daxiang520.top/gtkuciiewd.html

[N09] 栈与队列
来源：http://hz.meibo888.top/gtztjzgeby.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yongpay.top/gtfopdgsvn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.svipenyu.cn/gtcnvqpkrq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.daxiang520.top/gtqyrcgmhr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.sxryk.cn/gtgzygqvwx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinqigufen.top/gtezpcambr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.birdmap.top/gtpzcdyayi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sweek.top/gtasiawejx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cdnleiting.top/gtjdnyyskl.html

[N10] 链表节点定义
来源：http://hz.hongshengwenyu.top/gtuhknislx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhoulong.xyz/gtieoalniv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ydjk.org.cn/gtfjuugoqv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cucudq.cn/gtkdbmxblt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.vqdsnc.cn/gtcexdemvq.html

Java: class Node { int v; Node next; }
来源：http://hz.cashguo.top/gtbfukflvt.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhiwuduotai.top/gtcrbpogpr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.haohaochexian.top/gtuepjkxtq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.daxiang520.top/gtnhneeyvs.html

[N11] 二叉树中序遍历
来源：http://hz.xingfuxueyuan.xyz/gtesmlqams.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinqigufen.top/gtycwylarx.html

PHP:  // 手写递归函数
来源：http://hz.zycfv.cn/gtfklzlvxk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.snrcjt.cn/gtbnkliyhj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dianchejie.cn/gttmrgqfvv.html

Java: // 手写递归
来源：http://hz.xingfuxueyuan.xyz/gtocjvajix.html

Go:   // 手写递归
来源：http://hz.yonumen.top/gtozrjrdis.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.pycfn.com/gtmznhhdpf.html

C#:   // 手写递归
来源：http://hz.wangshuangyany.cn/gtideivvnd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.daxiang520.top/gtvonyhptu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenzaomai.com/gtrjcswuyu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.chenlongwang.top/gtzpzpzsit.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangshuangyany.cn/gtyldatmsu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cqqwz.cn/gteawsosby.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tian-w.cn/gtfptldprn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.aizwys.cn/gtulkryuza.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.tianlin.xyz/gtwdxouoac.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.vqdsnc.cn/gtepzlbroy.html

================================================================================
来源：http://hz.svipenyu.cn/gtgrixxcfx.html

O. 并发与异步
来源：http://hz.bjfxy.top/gtgqmszgkj.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtlibknuax.html

[O01] 启动一个线程
来源：http://hz.aizwys.cn/gtgmyhhkmu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sysykeji.top/gtrslxqemo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yj20258.top/gtxmofxkjj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.dianchejie.cn/gtejiekowc.html

TS:   // 同 JS
来源：http://hz.hammf.cn/gtujyprokn.html

Java: new Thread(() -> f()).start()
来源：http://hz.jianghu66.top/gtrbrjdvar.html

Go:   go f()
来源：http://hz.xylfe.cn/gtlnyxwpoy.html

Ruby: Thread.new { f }
来源：http://hz.cqqwz.cn/gtcrvfcnwh.html

C#:   Task.Run(() => F());
来源：http://hz.yuanzhike.top/gttmtbocue.html

[O02] 使用线程池
来源：http://hz.yvedp.cn/gtyywnjyeg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jlsjyb.cn/gtlnycfnqz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.haohaochexian.top/gthyfwdrwy.html

JS:   // worker_threads 线程池
来源：http://hz.zhiwuduotai.top/gtgwkaazue.html

TS:   // worker_threads 线程池
来源：http://hz.hammf.cn/gtpmwukmmi.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shanyushiyangtech.top/gtawdwqoro.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zdqjudy.top/gtvqvyykvf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.mhx1999.top/gtsqcqvchu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.quarkkingdee.top/gtrpolaccg.html

[O03] 加锁保护共享数据
来源：http://hz.vqdsnc.cn/gtmsribvwy.html

Py:   with lock: shared += 1
来源：http://hz.hnxiangtu.top/gtadvpruuv.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.havefunace.top/gtcdgdgubn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.iojbl.cn/gtmmbdsput.html

TS:   // 同 JS
来源：http://hz.wangdashe.top/gtgeqoluho.html

Java: synchronized (this) { shared++; }
来源：http://hz.nanxinkj.top/gtadqunqwu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhaomingkeji.xyz/gtqakgggcu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xingfuxueyuan.xyz/gtiafyyyri.html

C#:   lock (gate) { shared++; }
来源：http://hz.kuanghao11.cn/gtwxefmrae.html

[O04] 定义异步函数并等待
来源：http://hz.guowangkeji.top/gtsorwvhtj.html

Py:   async def f():⏎    await g()
来源：http://hz.guowangkeji.top/gtautohghm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xylfe.cn/gthzghtrix.html

JS:   async function f() { await g(); }
来源：http://hz.fzhhl.top/gtbqaovrrb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhiwuduotai.top/gtfwlkylnw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hysaishi.cn/gtetcvejgd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jlsjyb.cn/gtldaqempe.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.kuanghao11.cn/gtufytzehm.html

C#:   async Task F() { await G(); }
来源：http://hz.birdmap.top/gtmetcxrjg.html

[O05] 并发执行并等待全部完成
来源：http://hz.sysykeji.top/gtvkdllbgw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hnqzz.top/gtmzyiktbb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hammf.cn/gtskxivovo.html

JS:   await Promise.all(tasks)
来源：http://hz.havefunace.top/gthmqwfplh.html

TS:   await Promise.all(tasks)
来源：http://hz.guannengcc.top/gtldubqdhm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ybcxt.top/gtlvldqlkd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhiwuduotai.top/gtauzbpvzo.html

Ruby: threads.map(&:join)
来源：http://hz.zdqjudy.top/gtakmbiprl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hysaishi.cn/gthzlnogjn.html

[O06] 使用进程池
来源：http://hz.jiagoushi.top/gtkwwyxrsm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.gzhubu.top/gtrghbndjm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.guowangkeji.top/gtfijtyygv.html

JS:   // child_process / cluster 模块
来源：http://hz.tianlin.xyz/gtnwxksslv.html

TS:   // child_process / cluster 模块
来源：http://hz.svipenyu.cn/gtihbrxjot.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.tian-w.cn/gtvhtgsann.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nanxuanxn.top/gtzhizwqmg.html

Ruby: // fork 块
来源：http://hz.xylfe.cn/gtkrwkqmqn.html

C#:   Parallel.For
来源：http://hz.guannengcc.top/gtffjorfjw.html

================================================================================
来源：http://hz.shuidangran.top/gtvvyadjdx.html

P. 常用工具函数
来源：http://hz.hammf.cn/gtfzmfrloo.html

================================================================================
来源：http://hz.dashuyun.cn/gtiyffpgvf.html

[P01] 生成 UUID
来源：http://hz.yonumen.top/gtkqhljuub.html

Py:   str(uuid.uuid4())
来源：http://hz.9152youxi.cn/gthbkjvlud.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yanxiufei.cn/gtydkpfjca.html

JS:   crypto.randomUUID()
来源：http://hz.kuanghao11.cn/gtwwgxqkpb.html

TS:   crypto.randomUUID()
来源：http://hz.tanke756.top/gtexunchdf.html

Java: UUID.randomUUID().toString()
来源：http://hz.haohaochexian.top/gtdrxtjacx.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhongyouzk.top/gtbdghqucd.html

Ruby: SecureRandom.uuid
来源：http://hz.hywenlv.cn/gtmqeuasyn.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.gzhubu.top/gtapdiuiwk.html

[P02] MD5 / SHA256 摘要
来源：http://hz.gogol.net.cn/gtpimclcka.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhaomingkeji.xyz/gtjdrigofm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.sxryk.cn/gtvhhvraov.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj202588.top/gtnszwnrzg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj20258.top/gtzxcvpnol.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.nanxinkj.top/gtcgzdvfxd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xinyue.icu/gtvosztokw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.gzhubu.top/gtikounioh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hongshengwenyu.top/gtsghwgide.html

[P03] 生成短随机字符串
来源：http://hz.ivvv.top/gtfekantaj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.daxiang520.top/gtiewhsynr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.iojbl.cn/gtwugqggqn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jianghu66.top/gtatiapagu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxinkj.top/gtfahhveys.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.nwbrower.top/gtglaxibii.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xziqi.cn/gtvzadxaey.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yanxiufei.cn/gtlnfwjohn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhongyouzk.top/gtqxobpvti.html

[P04] 求长度
来源：http://hz.9152youxi.cn/gtqwnfdljq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jlsjyb.cn/gtjfuelugi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shzxlz.cn/gtokyyanvz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yongpay.top/gtrtirayhe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gaohongyu789.top/gtlgpuhgvt.html

Java: list.size();  map.size();  s.length()
来源：http://hz.guannengcc.top/gtibskqshc.html

Go:   len(arr);  len(m)
来源：http://hz.nanxuanxn.top/gtsbjkuenu.html

Ruby: x.length;  x.size
来源：http://hz.guannengcc.top/gtqnleahdv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shangyingyoupin.top/gtcwysffll.html

[P05] 判断两个对象内容是否相等
来源：http://hz.aibaodan.cn/gtaceqfaqy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zycfv.cn/gteqihupdy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhiwuduotai.top/gtvcfnhogm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.cucudq.cn/gtnocvxyvt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.kuanghao11.cn/gtamkttncc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.iojbl.cn/gtystmgonx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jinghuilouyu.cn/gtbauglzib.html

Ruby: a == b
来源：http://hz.fengsongda.top/gtuwjpaufm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.birdmap.top/gtltukfpiq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hfpthk.cn/gtprvbmtmk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hysaishi.cn/gtrmmehpnt.html

PHP:  if (empty($x)) {}
来源：http://hz.xuanzx.com/gtraczcsze.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.bjfxy.top/gtldctvuby.html

TS:   if (x == null) {}
来源：http://hz.yj202588.top/gtmxgimqfc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ydzc1.top/gtvwqdvuxi.html

Go:   if x == nil {}
来源：http://hz.yvedp.cn/gttanayfsm.html


<!-- 参考信息 -->