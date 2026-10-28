代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xziqi.cn/gtaqtpxggl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhongyouzk.top/gtdnfqqaab.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gthftsrvwr.html

M. 命令行 / 进程 / 环境
来源：http://hz.dashuyun.cn/gttjbfzeeh.html

================================================================================
来源：http://hz.jyoumei.cn/gtwcgzqeun.html

[M01] 读取命令行参数
来源：http://hz.birdmap.top/gtwyyqouha.html

Py:   sys.argv[1:]
来源：http://hz.jlsjyb.cn/gtkrlewgcm.html

PHP:  $argv;  $argc;
来源：http://hz.meibo888.top/gtslpuhyle.html

JS:   process.argv.slice(2)
来源：http://hz.c1oappe.top/gtgvviosro.html

TS:   process.argv.slice(2)
来源：http://hz.kuanghao11.cn/gtopcdkhdg.html

Java: args 数组（main 方法参数）
来源：http://hz.redwolf501.top/gtqffbsvhf.html

Go:   os.Args[1:]
来源：http://hz.ydzc1.top/gteztxwosj.html

Ruby: ARGV
来源：http://hz.nanxuanxn.top/gtqyydjxjj.html

C#:   args 数组（Main 方法参数）
来源：http://hz.316326.xyz/gtttvcihax.html

[M02] 读取环境变量
来源：http://hz.fzhhl.top/gtmjoitvrv.html

Py:   os.environ.get("HOME")
来源：http://hz.shanyushiyangtech.top/gtlmvgvrka.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shuidangran.top/gtokxcfetl.html

JS:   process.env.HOME
来源：http://hz.tanke756.top/gthpamecuf.html

TS:   process.env.HOME
来源：http://hz.iojbl.cn/gtksjwwzws.html

Java: System.getenv("HOME")
来源：http://hz.xylfe.cn/gtnnnjxbwl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sweek.top/gtucsqwhqv.html

Ruby: ENV["HOME"]
来源：http://hz.ydjk.org.cn/gtepipjgwx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yvedp.cn/gtxekvwbwh.html

[M03] 执行外部命令
来源：http://hz.zycfv.cn/gthcgyipjk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ppjwa.cn/gtxzvicrrt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhongyouzk.top/gtthcbfqox.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinyuanbaomall.cn/gtnshnijsg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydzc1.top/gtjmtcsvgq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.shanyushiyangtech.top/gthoaplvjy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hnxiangtu.top/gtrutdvdgz.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ivvv.top/gtobxrsqbd.html

C#:   Process.Start("ls", "-l");
来源：http://hz.aibaodan.cn/gtuhjxqlfc.html

[M04] 获取当前工作目录
来源：http://hz.yj202588.top/gttrgbfzgw.html

Py:   os.getcwd()
来源：http://hz.nanxuanxn.top/gtcoztbnsz.html

PHP:  getcwd();
来源：http://hz.tianlin.xyz/gtpfruuzth.html

JS:   process.cwd()
来源：http://hz.jinqigufen.top/gtpliyhtjm.html

TS:   process.cwd()
来源：http://hz.sufxvd.cn/gtaeieefnf.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hnxiangtu.top/gtpdxcjbjo.html

Go:   os.Getwd()
来源：http://hz.jinqigufen.top/gtwjcwhuae.html

Ruby: Dir.pwd
来源：http://hz.cashguo.top/gtxvdjjeci.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xinyue.icu/gtzkldwsmj.html

[M05] 设置退出码
来源：http://hz.xingfuxueyuan.xyz/gtfdbautvx.html

Py:   sys.exit(1)
来源：http://hz.52xcode.cn/gtqhbcraoa.html

PHP:  exit(1);
来源：http://hz.sufxvd.cn/gtspitarzl.html

JS:   process.exit(1)
来源：http://hz.zhaomingkeji.xyz/gtbhjiflvd.html

TS:   process.exit(1)
来源：http://hz.zhixingplan.top/gtogsdseum.html

Java: System.exit(1)
来源：http://hz.9152youxi.cn/gtrcvglxvb.html

Go:   os.Exit(1)
来源：http://hz.316326.xyz/gtofqdjveq.html

Ruby: exit 1
来源：http://hz.jqgufenzy.top/gtwcgnlpaj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nanxinkj.top/gtwyphyggg.html

[M06] 向标准错误输出
来源：http://hz.yj202588.top/gtgexcmjak.html

Py:   print("err", file=sys.stderr)
来源：http://hz.mhx1999.top/gtjeeknltq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhengqikj.top/gtfgkaffuh.html

JS:   console.error("err")
来源：http://hz.bjfxy.top/gteevzunzj.html

TS:   console.error("err")
来源：http://hz.yuanzhike.top/gtzswoetxd.html

Java: System.err.println("err")
来源：http://hz.dashuyun.cn/gtpvdcahio.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xziqi.cn/gtzavrkuic.html

Ruby: warn "err"
来源：http://hz.zhijiandao.cn/gtrfnhtkmg.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jianghu66.top/gthurqirdb.html

[M07] 判断是否为主入口
来源：http://hz.hywenlv.cn/gtdxgduacm.html

Py:   if __name__ == "__main__":
来源：http://hz.hnqzz.top/gtspsavyda.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.dashuyun.cn/gtcpqawaey.html

JS:   require.main === module
来源：http://hz.yongpay.top/gtwwdhsnoq.html

TS:   require.main === module
来源：http://hz.tianlin.xyz/gtflqtbhly.html

Java: public static void main(String[] args)
来源：http://hz.jianghu66.top/gthcxxvswd.html

Go:   func main()
来源：http://hz.haohaochexian.top/gtircleuvs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sufxvd.cn/gtrftqxbbh.html

C#:   static void Main(string[] args)
来源：http://hz.jyoumei.cn/gtfmpejpev.html

[M08] 获取系统与运行时信息
来源：http://hz.xingfuxueyuan.xyz/gtvygdibpk.html

Py:   platform.system();  platform.python_version()
来源：http://hz.guannengcc.top/gtftmcrjxg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.guowangkeji.top/gteplibjcs.html

JS:   process.platform;  process.version
来源：http://hz.andypj.xyz/gtsdllmxpb.html

TS:   process.platform;  process.version
来源：http://hz.jlsjyb.cn/gtocxdunff.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.dianchejie.cn/gtkfhlvwjr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhaomingkeji.xyz/gtkgszmcgo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hnqzz.top/gtejsdpgqd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yangfankeji.com/gtsfpcbjzh.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gthdkzmags.html

N. 数据结构与算法
来源：http://hz.shangyingyoupin.top/gtmmnynfqa.html

================================================================================
来源：http://hz.sweek.top/gtuvfxdaeg.html

[N01] 二分查找（有序数组）
来源：http://hz.zhaomingkeji.xyz/gtfkctxlxj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.tian-w.cn/gtpjywruxl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.tian-w.cn/gtchxaburk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.kuanghao11.cn/gtsbretdgj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydzc1.top/gtrbumwelz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jqgufenzy.top/gtsqlgnvel.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yj202588.top/gtckiwlndk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.gotoacloud.top/gtncxutkuh.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sysykeji.top/gtfsxxcndw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.sysykeji.top/gtsaepogag.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj202588.top/gtnwlvvcpf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.havefunace.top/gtiknzispe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuetiantiany.cn/gtdwsfkhjl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fengsongda.top/gtqriksjli.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.feifeiyinyue.top/gtlnbpbhqs.html

Go:   slices.Sort(arr)
来源：http://hz.zhixingplan.top/gtzzdnmxwt.html

Ruby: arr.sort
来源：http://hz.hnxiangtu.top/gtarvzgalr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.aizwys.cn/gtuypicynv.html

[N03] 快速排序（分治示例）
来源：http://hz.hammf.cn/gtfmtdndsq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yvedp.cn/gtorxumvqi.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yuxming.cn/gtdvusnkrv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pengpengdd.cyou/gtzwktxpoi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hnqzz.top/gttrpepaxk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jiagoushi.top/gtihnkahye.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.daxiang520.top/gtcjcvvejl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhijiandao.cn/gtehlnqcxb.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhijiandao.cn/gtcvhugfgh.html

[N04] 斐波那契数列
来源：http://hz.yonumen.top/gtotbwydyu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zycfv.cn/gtgudvxdul.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hnqzz.top/gtnjwviplc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tanke756.top/gtgqurzzak.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ywan-chungtsiang.top/gtutcqqkbk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yj20258.top/gtjcgifhgq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shangyingyoupin.top/gtjdwcchne.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258.top/gtvigpmbdh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhongyouzk.top/gtqdzzgiwd.html

[N05] 最大公约数
来源：http://hz.hammf.cn/gtmgbxxcvx.html

Py:   math.gcd(a, b)
来源：http://hz.chenlongwang.top/gtvfygnwll.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhiwuduotai.top/gtqvlhexqf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jiagoushi.top/gtzebzzypm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xziqi.cn/gtwklcptpo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ywan-chungtsiang.top/gtlyeovlty.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.smart0.xyz/gtuyavdgmc.html

Ruby: a.gcd(b)
来源：http://hz.jinqigfzy.top/gtkigtccck.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.chenzaomai.com/gtgypvgvey.html

[N06] 判断回文字符串
来源：http://hz.yuxming.cn/gtegzbxhzp.html

Py:   s == s[::-1]
来源：http://hz.vqdsnc.cn/gtvwmdswqn.html

PHP:  $s === strrev($s);
来源：http://hz.daxiang520.top/gtmkeassoc.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yj20258888.top/gttwedeseb.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gtqbzoqrgl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhijiandao.cn/gteqafdfxn.html

Go:   // 双指针从两端比较
来源：http://hz.vqdsnc.cn/gttsoicubx.html

Ruby: s == s.reverse
来源：http://hz.iojbl.cn/gtnxdbqslo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.sufxvd.cn/gtkgkprcuk.html

[N07] 两数之和（返回下标）
来源：http://hz.tian-w.cn/gtzhgxzlzo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zdqjudy.top/gtodupvxdf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shanyushiyangtech.top/gtqwomdffc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sweek.top/gtrxcomooj.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhiwuduotai.top/gtrglynpsg.html

Java: // 手写 HashMap
来源：http://hz.daxiang520.top/gttywumznj.html

Go:   // 手写 map[int]int
来源：http://hz.hammf.cn/gtklbiqqrt.html

Ruby: // 手写 Hash
来源：http://hz.birdmap.top/gtklokfaux.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hnqzz.top/gtehnzwwjj.html

[N08] 生成全排列
来源：http://hz.hammf.cn/gtkrccpifv.html

Py:   itertools.permutations(arr)
来源：http://hz.wangshuangyany.cn/gtxsggiiqj.html

PHP:  // 手写递归交换
来源：http://hz.yueranfly.top/gtwgcrqtgh.html

JS:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtcccvcdii.html

TS:   // 手写回溯递归
来源：http://hz.chenlongwang.top/gtvsdsmhfe.html

Java: // 手写回溯递归
来源：http://hz.andypj.xyz/gtmmvufbih.html

Go:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtbbdjftyd.html

Ruby: arr.permutation.to_a
来源：http://hz.sysykeji.top/gtaxodmlyv.html

C#:   // 手写回溯递归
来源：http://hz.wangdashe.top/gtoyywegmh.html

[N09] 栈与队列
来源：http://hz.xingfuxueyuan.xyz/gtcntcjiag.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.nanxinkj.top/gtpgchnzrz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xuetiantiany.cn/gtmnqrrczk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hammf.cn/gtuvpoihcd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yanxiufei.cn/gtoretzpjo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhongyouzk.top/gtmlndveqb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.nanxuanxn.top/gtmwqclrnq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.guowangkeji.top/gtallbzzjo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yangfankeji.com/gtxutpakif.html

[N10] 链表节点定义
来源：http://hz.nanxinkj.top/gtakfnferg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yj20258888.top/gtmoldnkqo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.havefunace.top/gtghjxozpp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cucudq.cn/gtcvxbgbgq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yuxming.cn/gtfjgllsnd.html

Java: class Node { int v; Node next; }
来源：http://hz.aizwys.cn/gtmgxqnbcv.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hnxiangtu.top/gtjcrqybud.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hnqzz.top/gtthiybfcf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.fzhhl.top/gtlgfydroo.html

[N11] 二叉树中序遍历
来源：http://hz.ydjk.org.cn/gtdkifyfhn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.daria6918.cn/gtbusaazrp.html

PHP:  // 手写递归函数
来源：http://hz.chenjidiqi.icu/gtcmofvawe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnxiangtu.top/gtypnbecbn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sufxvd.cn/gtljfnaexv.html

Java: // 手写递归
来源：http://hz.shanyushiyangtech.top/gtwdjysimm.html

Go:   // 手写递归
来源：http://hz.sufxvd.cn/gttxyffimb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.mhx1999.top/gtwstzfyoo.html

C#:   // 手写递归
来源：http://hz.316326.xyz/gtncyghxuw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cashguo.top/gtpfgsaayw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhengqikj.top/gthhldegrg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.316326.xyz/gtjstqicmb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shzxlz.cn/gtwwkdbrbq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cashguo.top/gtgrqnudla.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gogol.net.cn/gtntydelsi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhaomingkeji.xyz/gtcfcfhdku.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.snrcjt.cn/gtiwrikxti.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ppjwa.cn/gtheaqmebo.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtbdhzjjkw.html

O. 并发与异步
来源：http://hz.cheryme.top/gtvbbnbfjs.html

================================================================================
来源：http://hz.zdqjudy.top/gtkgzcxtrd.html

[O01] 启动一个线程
来源：http://hz.birdmap.top/gtmixktzfp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ehwqpu.com/gtoeiivnmj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gogol.net.cn/gtemdjufjj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yuxming.cn/gtkugnxbya.html

TS:   // 同 JS
来源：http://hz.chenlongwang.top/gttyxzcefb.html

Java: new Thread(() -> f()).start()
来源：http://hz.9152youxi.cn/gtofpygmxh.html

Go:   go f()
来源：http://hz.zhengqikj.top/gthirslmqq.html

Ruby: Thread.new { f }
来源：http://hz.guowangkeji.top/gtwwadxggn.html

C#:   Task.Run(() => F());
来源：http://hz.redwolf501.top/gtuvuszftm.html

[O02] 使用线程池
来源：http://hz.wangdashe.top/gtmbfjanrd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jlsjyb.cn/gtrswggwee.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.c1oappe.top/gtdxrortet.html

JS:   // worker_threads 线程池
来源：http://hz.hammf.cn/gtsfzbawae.html

TS:   // worker_threads 线程池
来源：http://hz.xingfuxueyuan.xyz/gtnsngqvwh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.svipenyu.cn/gtmygoimmh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jinyuanbaomall.cn/gtflpyjuxf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.nwbrower.top/gtnwhdpjtd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shangyingyoupin.top/gtvjmqsyyv.html

[O03] 加锁保护共享数据
来源：http://hz.yongpay.top/gtvabhxvax.html

Py:   with lock: shared += 1
来源：http://hz.dianchejie.cn/gtcwcxzbit.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.vqdsnc.cn/gtfkjhzdfk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.fzhhl.top/gtjnwhgiqi.html

TS:   // 同 JS
来源：http://hz.smart0.xyz/gtpskhbkbf.html

Java: synchronized (this) { shared++; }
来源：http://hz.hywenlv.cn/gtdieprecd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yueranfly.top/gtkkqeaqsb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hammf.cn/gteznrssqa.html

C#:   lock (gate) { shared++; }
来源：http://hz.yvedp.cn/gtqspkbcfx.html

[O04] 定义异步函数并等待
来源：http://hz.yonumen.top/gtkqsqbece.html

Py:   async def f():⏎    await g()
来源：http://hz.yj20258888.top/gtddhrfcha.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cucudq.cn/gtgkekmrjo.html

JS:   async function f() { await g(); }
来源：http://hz.andypj.xyz/gtdsjbugyp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.nanxinkj.top/gtejqmpmmi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhengqikj.top/gtftfdysfs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jyoumei.cn/gtqdvnmzsy.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhijiandao.cn/gtttctdyid.html

C#:   async Task F() { await G(); }
来源：http://hz.xuetiantiany.cn/gtmidklcya.html

[O05] 并发执行并等待全部完成
来源：http://hz.fzhhl.top/gtzuuaayrk.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xylfe.cn/gtwrwsrhqy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yangfankeji.com/gtmvofiicl.html

JS:   await Promise.all(tasks)
来源：http://hz.jiagoushi.top/gtiuslrdof.html

TS:   await Promise.all(tasks)
来源：http://hz.yuxming.cn/gttnajupxh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.dianchejie.cn/gtyhtxjetu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.gaohongyu789.top/gtzmgzxzij.html

Ruby: threads.map(&:join)
来源：http://hz.zhoulong.xyz/gtttiufkmu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.wangshuangyany.cn/gtlxkfvnyq.html

[O06] 使用进程池
来源：http://hz.ydzc1.top/gtjdsgtvbz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.svipenyu.cn/gtnhopiavd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shanyushiyangtech.top/gtyymjktfr.html

JS:   // child_process / cluster 模块
来源：http://hz.jqgufenzy.top/gteivccizy.html

TS:   // child_process / cluster 模块
来源：http://hz.chenjidiqi.icu/gtapjwuzzy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinghuilouyu.cn/gtpjeioovk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xziqi.cn/gtwjsplflg.html

Ruby: // fork 块
来源：http://hz.jiagoushi.top/gtpqkxcnzy.html

C#:   Parallel.For
来源：http://hz.hysaishi.cn/gtbwhailxs.html

================================================================================
来源：http://hz.ydjk.org.cn/gtbpxrcwic.html

P. 常用工具函数
来源：http://hz.yueranfly.top/gtnqncpbxu.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtpgygncdp.html

[P01] 生成 UUID
来源：http://hz.dianchejie.cn/gthbrtlzzb.html

Py:   str(uuid.uuid4())
来源：http://hz.jyoumei.cn/gthjtenpaq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.haohaochexian.top/gtotsladlf.html

JS:   crypto.randomUUID()
来源：http://hz.andypj.xyz/gtrrblsnuu.html

TS:   crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtwnwxzhds.html

Java: UUID.randomUUID().toString()
来源：http://hz.yj20258.top/gtdpobmzqh.html

Go:   // 用 github.com/google/uuid
来源：http://hz.dashuyun.cn/gtzockoddb.html

Ruby: SecureRandom.uuid
来源：http://hz.mhx1999.top/gtthywyhdr.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.guannengcc.top/gtsvhronwo.html

[P02] MD5 / SHA256 摘要
来源：http://hz.pycfn.com/gtarhboqph.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xylfe.cn/gtatvfvywe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.tanke756.top/gtuwfoxtrt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.snrcjt.cn/gthynvnxhb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.nanxuanxn.top/gtklkogstl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ydzc1.top/gtuhzmuxdf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.andypj.xyz/gtuxuvrrlw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.aizwys.cn/gtjmosdpvo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jinqigfzy.top/gtnppmimms.html

[P03] 生成短随机字符串
来源：http://hz.mhx1999.top/gtgfrnqjwu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.wangshuangyany.cn/gtlfqzjjrt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhaomingkeji.xyz/gthzmzyjnx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.redwolf501.top/gtkhncswdf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tian-w.cn/gtwldmxaez.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jianghu66.top/gtmxeveadf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.iojbl.cn/gtnrwzfhyi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jlsjyb.cn/gtbpvllksv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.kuanghao11.cn/gtekxkxxul.html

[P04] 求长度
来源：http://hz.snrcjt.cn/gtnncpcenm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.aizwys.cn/gtazhkhisp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zdqjudy.top/gthsvswbvc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.andypj.xyz/gtkmhbakbl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuxming.cn/gtsonqtdra.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jinghuilouyu.cn/gtybwnmpfq.html

Go:   len(arr);  len(m)
来源：http://hz.hfpthk.cn/gtqhpxihlj.html

Ruby: x.length;  x.size
来源：http://hz.aizwys.cn/gtimftbfik.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.nanxuanxn.top/gtvosmxhal.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yj202588.top/gtyhcyymuj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.guowangkeji.top/gtouogbfwr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.chenjidiqi.icu/gtdbiyihku.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.gotoacloud.top/gttmorfrub.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hysaishi.cn/gtinvdqbcx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cqqwz.cn/gtrmmypdbb.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jinqigufen.top/gtfockzsdi.html

Ruby: a == b
来源：http://hz.gogol.net.cn/gtrrdtarwn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xziqi.cn/gtvprpocus.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jinqigfzy.top/gtsrjmcykc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.smart0.xyz/gtkvapdtxd.html

PHP:  if (empty($x)) {}
来源：http://hz.zhongyouzk.top/gtrddlpswi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.gaohongyu789.top/gtyvhdqgum.html

TS:   if (x == null) {}
来源：http://hz.wangdashe.top/gtkcdtldum.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.cqqwz.cn/gtsaxhfmam.html

Go:   if x == nil {}
来源：http://hz.kuanghao11.cn/gtezltvmsx.html


<!-- 参考信息 -->