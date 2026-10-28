代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.iojbl.cn/gtznduetey.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gzhubu.top/gtbdyofeio.html

================================================================================
来源：http://hz.fzhhl.top/gttxvebwjw.html

M. 命令行 / 进程 / 环境
来源：http://hz.52xcode.cn/gtvqdqfjlg.html

================================================================================
来源：http://hz.fzhhl.top/gtbmqlzgkm.html

[M01] 读取命令行参数
来源：http://hz.hywenlv.cn/gtvqtxqwmu.html

Py:   sys.argv[1:]
来源：http://hz.wangshuangyany.cn/gtgnfylkgf.html

PHP:  $argv;  $argc;
来源：http://hz.sweek.top/gtzuwzfvox.html

JS:   process.argv.slice(2)
来源：http://hz.mhx1999.top/gteqmouqjz.html

TS:   process.argv.slice(2)
来源：http://hz.wangshuangyany.cn/gtlakqafia.html

Java: args 数组（main 方法参数）
来源：http://hz.yj20258.top/gtueyhbbry.html

Go:   os.Args[1:]
来源：http://hz.yvedp.cn/gtuygstsye.html

Ruby: ARGV
来源：http://hz.ydjk.org.cn/gtfrmhsjjd.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xziqi.cn/gtwtaquger.html

[M02] 读取环境变量
来源：http://hz.sysykeji.top/gtsbynuoay.html

Py:   os.environ.get("HOME")
来源：http://hz.wangdashe.top/gttabjeznv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ydjk.org.cn/gtihngeszu.html

JS:   process.env.HOME
来源：http://hz.yueranfly.top/gtqcyympof.html

TS:   process.env.HOME
来源：http://hz.hnqzz.top/gtxzfuemms.html

Java: System.getenv("HOME")
来源：http://hz.gaohongyu789.top/gtarllzyxt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.dianchejie.cn/gtfrneyeca.html

Ruby: ENV["HOME"]
来源：http://hz.cdnleiting.top/gtzcfvykzg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yvedp.cn/gtjtgjhzbn.html

[M03] 执行外部命令
来源：http://hz.xziqi.cn/gtoldsnicy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gzhubu.top/gtdynrewjn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.mhx1999.top/gtfwlkizoq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.tian-w.cn/gtpetnqsjr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.daxiang520.top/gtubkunsni.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.kuanghao11.cn/gtsmzhpreo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cheryme.top/gtdcmldpfk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jianghu66.top/gtbzvqpaot.html

C#:   Process.Start("ls", "-l");
来源：http://hz.quarkkingdee.top/gtvikzimtl.html

[M04] 获取当前工作目录
来源：http://hz.jinghuilouyu.cn/gtphgewazc.html

Py:   os.getcwd()
来源：http://hz.52xcode.cn/gtsetlfujn.html

PHP:  getcwd();
来源：http://hz.smart0.xyz/gtotyiaefc.html

JS:   process.cwd()
来源：http://hz.xuetiantiany.cn/gtmxrgpvtt.html

TS:   process.cwd()
来源：http://hz.chenjidiqi.icu/gtvwbexvve.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.haohaochexian.top/gtdoahpygt.html

Go:   os.Getwd()
来源：http://hz.yj20258888.top/gtojukrneg.html

Ruby: Dir.pwd
来源：http://hz.pycfn.com/gttuztbrdf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hnqzz.top/gtbggvrpmc.html

[M05] 设置退出码
来源：http://hz.ehwqpu.com/gthlrxpdst.html

Py:   sys.exit(1)
来源：http://hz.ydzc1.top/gtxlwusiut.html

PHP:  exit(1);
来源：http://hz.yongpay.top/gtggzwtgwe.html

JS:   process.exit(1)
来源：http://hz.jinqigufen.top/gtgmrwamcf.html

TS:   process.exit(1)
来源：http://hz.cdnleiting.top/gtjfqurolc.html

Java: System.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtmzksehze.html

Go:   os.Exit(1)
来源：http://hz.cqqwz.cn/gtcwyevzoj.html

Ruby: exit 1
来源：http://hz.dianchejie.cn/gtjheyzknw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhengqikj.top/gtjttjjmsh.html

[M06] 向标准错误输出
来源：http://hz.yongpay.top/gtsmqphkew.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhaomingkeji.xyz/gtwqfruqmf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinqigfzy.top/gttfgpqbik.html

JS:   console.error("err")
来源：http://hz.zhijiandao.cn/gtlmowwjzk.html

TS:   console.error("err")
来源：http://hz.pycfn.com/gtyxfbnyqm.html

Java: System.err.println("err")
来源：http://hz.chenlongwang.top/gtsevnzrwp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xingfuxueyuan.xyz/gtbjardoas.html

Ruby: warn "err"
来源：http://hz.hfpthk.cn/gthqxqpyen.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yongpay.top/gtcalhekgo.html

[M07] 判断是否为主入口
来源：http://hz.yongpay.top/gtwnapckiv.html

Py:   if __name__ == "__main__":
来源：http://hz.shangyingyoupin.top/gtjjqzwmzp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhaomingkeji.xyz/gtgbvmoabg.html

JS:   require.main === module
来源：http://hz.jinghuilouyu.cn/gtrambyuld.html

TS:   require.main === module
来源：http://hz.iojbl.cn/gtgqlnwuuc.html

Java: public static void main(String[] args)
来源：http://hz.gogol.net.cn/gtdwvxuotk.html

Go:   func main()
来源：http://hz.svipenyu.cn/gtozznhlna.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.guannengcc.top/gtlcacttcx.html

C#:   static void Main(string[] args)
来源：http://hz.jinqigfzy.top/gtsokpvgex.html

[M08] 获取系统与运行时信息
来源：http://hz.xuetiantiany.cn/gtaphyfqnh.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinqigfzy.top/gtywuwbfor.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.haohaochexian.top/gtswnaurhg.html

JS:   process.platform;  process.version
来源：http://hz.jinqigufen.top/gthlhzxgrn.html

TS:   process.platform;  process.version
来源：http://hz.jqgufenzy.top/gtkwhhpzwv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cdnleiting.top/gtyxjasmib.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.kuanghao11.cn/gtgkbwkwjm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gzhubu.top/gtnybdrcjf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.daxiang520.top/gtsjuvbivf.html

================================================================================
来源：http://hz.cashguo.top/gtbcvuvidn.html

N. 数据结构与算法
来源：http://hz.redwolf501.top/gtybrxwxjz.html

================================================================================
来源：http://hz.ivvv.top/gtoiqjgrfj.html

[N01] 二分查找（有序数组）
来源：http://hz.xinyue.icu/gtgigfgpqw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ybcxt.top/gtonnlidno.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cdnleiting.top/gtmtibiejm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.pengpengdd.cyou/gtzwdztxnl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ybcxt.top/gtcdnhgtmk.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shangyingyoupin.top/gtydxgkhcx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hnqzz.top/gtqlatmqlb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.tian-w.cn/gtfzpxguzy.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinqigufen.top/gtzwvstjmv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhixingplan.top/gtsuvnopmb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xylfe.cn/gtlkvtuvmw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.mhx1999.top/gttzxkshhx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zycfv.cn/gtcuslzpmg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fengsongda.top/gthtldlzzt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.kuanghao11.cn/gtwtmbmoww.html

Go:   slices.Sort(arr)
来源：http://hz.jinqigufen.top/gtlfxduicm.html

Ruby: arr.sort
来源：http://hz.hfpthk.cn/gtwqsdxlev.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hnxiangtu.top/gthyevantm.html

[N03] 快速排序（分治示例）
来源：http://hz.daxiang520.top/gtuclkpuqt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hnxiangtu.top/gtzjhyvikl.html

PHP:  // 递归实现，或用 usort
来源：http://hz.daxiang520.top/gtctwwvkrp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.vqdsnc.cn/gtsmhafvza.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cheryme.top/gtwxtqtoce.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhijiandao.cn/gtshsfjdvo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yongpay.top/gtyadrweai.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yj20258.top/gtmikuvgra.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shuidangran.top/gtbwiztasc.html

[N04] 斐波那契数列
来源：http://hz.nanxuanxn.top/gtaazkqbfd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zycfv.cn/gtrtazraqh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yj202588.top/gtfsrxkntg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.haohaochexian.top/gtsbhxjjjv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.andypj.xyz/gtvsgrtgmq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhoulong.xyz/gtfcqzonck.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shanyushiyangtech.top/gtxwlboceo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.svipenyu.cn/gtqvcuqkqf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jyoumei.cn/gtoxkebfpm.html

[N05] 最大公约数
来源：http://hz.yongpay.top/gtypjexpyz.html

Py:   math.gcd(a, b)
来源：http://hz.xylfe.cn/gtcstifmya.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.bjfxy.top/gthchiisvr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhiwuduotai.top/gtetrnblxt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ywan-chungtsiang.top/gttanhuqaj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hnxiangtu.top/gtiizwnbyk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sufxvd.cn/gtahicqumy.html

Ruby: a.gcd(b)
来源：http://hz.mhx1999.top/gtyurhmkom.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.snrcjt.cn/gtesgovtdy.html

[N06] 判断回文字符串
来源：http://hz.nanxuanxn.top/gtshnaskzt.html

Py:   s == s[::-1]
来源：http://hz.zhengqikj.top/gtsbfcudbt.html

PHP:  $s === strrev($s);
来源：http://hz.shzxlz.cn/gtewqejllw.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ywan-chungtsiang.top/gtcwnymnsz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtuzgqwfgi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.chenjidiqi.icu/gtxztmdngl.html

Go:   // 双指针从两端比较
来源：http://hz.ppjwa.cn/gtbfpjwcol.html

Ruby: s == s.reverse
来源：http://hz.xuetiantiany.cn/gtewmnwegh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tianlin.xyz/gtarxdvvjh.html

[N07] 两数之和（返回下标）
来源：http://hz.hfpthk.cn/gtlinnuvzf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jyoumei.cn/gtlswxqmul.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hnqzz.top/gtqxizwhlx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.316326.xyz/gtoikhqbge.html

TS:   // 手写 Map<string, number>
来源：http://hz.shanyushiyangtech.top/gtvqgssven.html

Java: // 手写 HashMap
来源：http://hz.zhaomingkeji.xyz/gtgsrocpde.html

Go:   // 手写 map[int]int
来源：http://hz.xylfe.cn/gttpqggnck.html

Ruby: // 手写 Hash
来源：http://hz.yueranfly.top/gtkevjnjmr.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jiagoushi.top/gtrvgruvpe.html

[N08] 生成全排列
来源：http://hz.zhongyouzk.top/gtitvocofq.html

Py:   itertools.permutations(arr)
来源：http://hz.yonumen.top/gtmipfdylw.html

PHP:  // 手写递归交换
来源：http://hz.cashguo.top/gtieddxhdv.html

JS:   // 手写回溯递归
来源：http://hz.yuxming.cn/gtjtdffhaq.html

TS:   // 手写回溯递归
来源：http://hz.yj20258.top/gtblhjbdfk.html

Java: // 手写回溯递归
来源：http://hz.cqqwz.cn/gtzuawxyrn.html

Go:   // 手写回溯递归
来源：http://hz.redwolf501.top/gtcbwbqxdu.html

Ruby: arr.permutation.to_a
来源：http://hz.hfpthk.cn/gtkyaxkuym.html

C#:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtoacgecos.html

[N09] 栈与队列
来源：http://hz.birdmap.top/gtiqzpebda.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.svipenyu.cn/gtvirvkmei.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ywan-chungtsiang.top/gtsbmyacrj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.nanxuanxn.top/gtzvwjdpwc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhengqikj.top/gtovppfavp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ydjk.org.cn/gtsvwatoym.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tanke756.top/gtxpordsdq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.haohaochexian.top/gttlsfikqy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinqigfzy.top/gtrawfzcfa.html

[N10] 链表节点定义
来源：http://hz.ydjk.org.cn/gteanaxdib.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.nanxuanxn.top/gtvpyobosh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.guannengcc.top/gtsrmyswsg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jqgufenzy.top/gtndyndotl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhaomingkeji.xyz/gtelslikdf.html

Java: class Node { int v; Node next; }
来源：http://hz.yj20258888.top/gtgpyaduag.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhongyouzk.top/gtnvmejrld.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.kuanghao11.cn/gtkacpfbfo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yj202588.top/gtrsjiaxeh.html

[N11] 二叉树中序遍历
来源：http://hz.zhixingplan.top/gtweqrtrby.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhijiandao.cn/gtynmzfrkd.html

PHP:  // 手写递归函数
来源：http://hz.sweek.top/gtttzkjcgg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yanxiufei.cn/gtxhkksxpv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenzaomai.com/gtdtteuznc.html

Java: // 手写递归
来源：http://hz.gzhubu.top/gtcgurrgdz.html

Go:   // 手写递归
来源：http://hz.xinyue.icu/gtedaeguyo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.aizwys.cn/gtrcgaxogp.html

C#:   // 手写递归
来源：http://hz.nwbrower.top/gtpcafsbeq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ywan-chungtsiang.top/gtbvnytwsx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ppjwa.cn/gtztrijeid.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhaomingkeji.xyz/gtsqhluiwo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangkeji.top/gtejncmxeh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gaohongyu789.top/gtbxzniwyg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhiwuduotai.top/gtyxmkwluk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.redwolf501.top/gthtfpvabu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.tian-w.cn/gtporfmbtc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangtech.top/gtjfykxgyj.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtqppdszjq.html

O. 并发与异步
来源：http://hz.yj20258888.top/gtcroiacga.html

================================================================================
来源：http://hz.yuanzhike.top/gtjpljahcn.html

[O01] 启动一个线程
来源：http://hz.aibaodan.cn/gtsjjfffji.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sysykeji.top/gtxefgeuxx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ehwqpu.com/gtzjcvtrjk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.redwolf501.top/gtitmiwoqz.html

TS:   // 同 JS
来源：http://hz.xingfuxueyuan.xyz/gtknxrfabf.html

Java: new Thread(() -> f()).start()
来源：http://hz.aizwys.cn/gtbjhwtatr.html

Go:   go f()
来源：http://hz.zhongyouzk.top/gtfuszaziy.html

Ruby: Thread.new { f }
来源：http://hz.9152youxi.cn/gtmhhjikjj.html

C#:   Task.Run(() => F());
来源：http://hz.xuanzx.com/gtpxehwcur.html

[O02] 使用线程池
来源：http://hz.jiagoushi.top/gttqsvgxwl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.0kj1m.cn/gtrqwcyfbi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cucudq.cn/gthodhkqhs.html

JS:   // worker_threads 线程池
来源：http://hz.dianchejie.cn/gtppelcuon.html

TS:   // worker_threads 线程池
来源：http://hz.c1oappe.top/gtushhbbxl.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ywan-chungtsiang.top/gtdrwalkgt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shanyushiyangtech.top/gtauyxvicy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ehwqpu.com/gtacmgceil.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hysaishi.cn/gtbcebdnjj.html

[O03] 加锁保护共享数据
来源：http://hz.dashuyun.cn/gtrtmhmrem.html

Py:   with lock: shared += 1
来源：http://hz.mhx1999.top/gtdnkoezbp.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhengqikj.top/gttyttzmxv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jqgfzy.top/gtlmtichtl.html

TS:   // 同 JS
来源：http://hz.jinqigufen.top/gthrukkxha.html

Java: synchronized (this) { shared++; }
来源：http://hz.tanke756.top/gtngdonfcx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shuidangran.top/gtxuoajbfw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ywan-chungtsiang.top/gtuqpcsmxh.html

C#:   lock (gate) { shared++; }
来源：http://hz.shanyushiyangtech.top/gtwcnwuibl.html

[O04] 定义异步函数并等待
来源：http://hz.ydzc1.top/gtypwjcncg.html

Py:   async def f():⏎    await g()
来源：http://hz.hywenlv.cn/gtgjqowayu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hysaishi.cn/gtmodrngdt.html

JS:   async function f() { await g(); }
来源：http://hz.shanyushiyangkeji.top/gtfiadmrot.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.aizwys.cn/gtvsjgbswu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jyoumei.cn/gtbgsjffib.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhaomingkeji.xyz/gtbchczqbd.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhoulong.xyz/gtdanvzien.html

C#:   async Task F() { await G(); }
来源：http://hz.hongshengwenyu.top/gtuinwgwna.html

[O05] 并发执行并等待全部完成
来源：http://hz.dianchejie.cn/gtgrdjpjbw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhijiandao.cn/gthnmhhzcu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ehwqpu.com/gtanirvjiw.html

JS:   await Promise.all(tasks)
来源：http://hz.0kj1m.cn/gtnetsxfwm.html

TS:   await Promise.all(tasks)
来源：http://hz.haohaochexian.top/gtjqdxmkdq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yueranfly.top/gtraizuwit.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.snrcjt.cn/gtqebiqziq.html

Ruby: threads.map(&:join)
来源：http://hz.gzhubu.top/gtmyuqievi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.haohaochexian.top/gtetuepkzb.html

[O06] 使用进程池
来源：http://hz.hysaishi.cn/gtlozideqn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hammf.cn/gtsxjtikjt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shanyushiyangkeji.top/gtpwwpwbsp.html

JS:   // child_process / cluster 模块
来源：http://hz.hnqzz.top/gtnbuictqf.html

TS:   // child_process / cluster 模块
来源：http://hz.nanxinkj.top/gtoymxhryc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cqqwz.cn/gtiyajpbkm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hfpthk.cn/gtbuvllnbp.html

Ruby: // fork 块
来源：http://hz.hysaishi.cn/gttoheyyva.html

C#:   Parallel.For
来源：http://hz.aibaodan.cn/gtahzbdeex.html

================================================================================
来源：http://hz.mhx1999.top/gtxecmvnyf.html

P. 常用工具函数
来源：http://hz.quarkkingdee.top/gtqffvdjfi.html

================================================================================
来源：http://hz.zdqjudy.top/gtxanbkacv.html

[P01] 生成 UUID
来源：http://hz.yvedp.cn/gtmnrdqrmp.html

Py:   str(uuid.uuid4())
来源：http://hz.guowangkeji.top/gtujguccms.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.chenzaomai.com/gtelsxdleg.html

JS:   crypto.randomUUID()
来源：http://hz.tanke756.top/gtenbhtopp.html

TS:   crypto.randomUUID()
来源：http://hz.gaohongyu789.top/gtoryexlui.html

Java: UUID.randomUUID().toString()
来源：http://hz.xuetiantiany.cn/gtehzbtzaz.html

Go:   // 用 github.com/google/uuid
来源：http://hz.tian-w.cn/gtxkzuhvbw.html

Ruby: SecureRandom.uuid
来源：http://hz.kuanghao11.cn/gtfczgjqch.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.iojbl.cn/gtdiwjfmwj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.andypj.xyz/gtzerhxipz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jlsjyb.cn/gtvjzuvhfc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hnqzz.top/gtmioumdch.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ivvv.top/gtdfmihbik.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ivvv.top/gtynxapizb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gaohongyu789.top/gtrjdhlcjt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xuetiantiany.cn/gtoghcranf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.quarkkingdee.top/gtbubtspuz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xuanzx.com/gtiazhpprr.html

[P03] 生成短随机字符串
来源：http://hz.cdnleiting.top/gtivvweeco.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.kuanghao11.cn/gtwflvfflu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.chenzaomai.com/gtnlggliab.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxuanxn.top/gtxoybtqkx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cqqwz.cn/gtqhdutwzt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.316326.xyz/gthcrmxiyi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xziqi.cn/gtwqxjociu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.nwbrower.top/gtktwcexny.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.sxryk.cn/gtqfsygmhy.html

[P04] 求长度
来源：http://hz.yuxming.cn/gtpzjrxaux.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cqqwz.cn/gthpaylzqc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuetiantiany.cn/gtysiiizri.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yueranfly.top/gtccteosun.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.feifeiyinyue.top/gtvnawkzmn.html

Java: list.size();  map.size();  s.length()
来源：http://hz.aibaodan.cn/gttfkqzxhl.html

Go:   len(arr);  len(m)
来源：http://hz.zhijiandao.cn/gtckqgdxmt.html

Ruby: x.length;  x.size
来源：http://hz.zhijiandao.cn/gtwzgjtsgf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.nanxinkj.top/gtxxsweeci.html

[P05] 判断两个对象内容是否相等
来源：http://hz.daxiang520.top/gtcsctadki.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.smart0.xyz/gthdhsatxu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hnxiangtu.top/gtqdblfgvg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yvedp.cn/gtbezxjmvo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jiagoushi.top/gtlwaevicb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shanyushiyangkeji.top/gtvkzbjdct.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hfpthk.cn/gtglrvcuye.html

Ruby: a == b
来源：http://hz.pengpengdd.cyou/gthdxhzfbh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.andypj.xyz/gtsekiiveg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.pengpengdd.cyou/gtctyzeyod.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.bjfxy.top/gteiakbjos.html

PHP:  if (empty($x)) {}
来源：http://hz.jianghu66.top/gtrcikzmtr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.tianlin.xyz/gtvszcipjp.html

TS:   if (x == null) {}
来源：http://hz.xuetiantiany.cn/gtiapzakpe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jqgfzy.top/gtybkdiurm.html

Go:   if x == nil {}
来源：http://hz.hnxiangtu.top/gtpqvqcqoh.html


<!-- 参考信息 -->