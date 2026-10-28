代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.smart0.xyz/gtsmjrkdpy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.daria6918.cn/gtngaiikxt.html

================================================================================
来源：http://hz.yanxiufei.cn/gtnsxrkmsa.html

M. 命令行 / 进程 / 环境
来源：http://hz.pengpengdd.cyou/gtnrdfexwa.html

================================================================================
来源：http://hz.andypj.xyz/gtxubteexz.html

[M01] 读取命令行参数
来源：http://hz.redwolf501.top/gtkiofpnlu.html

Py:   sys.argv[1:]
来源：http://hz.chenzaomai.com/gtfkfctnlm.html

PHP:  $argv;  $argc;
来源：http://hz.cheryme.top/gtealzhnyz.html

JS:   process.argv.slice(2)
来源：http://hz.nwbrower.top/gtzslhhhjr.html

TS:   process.argv.slice(2)
来源：http://hz.snrcjt.cn/gtbyjlvfnd.html

Java: args 数组（main 方法参数）
来源：http://hz.pycfn.com/gtqhdgifef.html

Go:   os.Args[1:]
来源：http://hz.0kj1m.cn/gtdmxittec.html

Ruby: ARGV
来源：http://hz.ywan-chungtsiang.top/gtxkbpmrzh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jianghu66.top/gtrqcbdbrw.html

[M02] 读取环境变量
来源：http://hz.cdnleiting.top/gtmcuqnwkm.html

Py:   os.environ.get("HOME")
来源：http://hz.jlsjyb.cn/gthzwtdkgf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.pengpengdd.cyou/gtbcfkvxex.html

JS:   process.env.HOME
来源：http://hz.yueranfly.top/gtwqhmexso.html

TS:   process.env.HOME
来源：http://hz.xziqi.cn/gtxoazeexy.html

Java: System.getenv("HOME")
来源：http://hz.ydjk.org.cn/gtdqttlvxd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yj20258.top/gtknwfqlzy.html

Ruby: ENV["HOME"]
来源：http://hz.yuanzhike.top/gtnmpolpxb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yj20258888.top/gttehycloi.html

[M03] 执行外部命令
来源：http://hz.sysykeji.top/gtbgnypfmg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.sysykeji.top/gtouummbcq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shzxlz.cn/gtvmyhrvlp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xingfuxueyuan.xyz/gtcvbbiwyw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jianghu66.top/gterscyxif.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhaomingkeji.xyz/gtlfhjaeku.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhiwuduotai.top/gtkaqrxnno.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhixingplan.top/gteolujszb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sweek.top/gtxsudtxdu.html

[M04] 获取当前工作目录
来源：http://hz.yangfankeji.com/gttuhqduyh.html

Py:   os.getcwd()
来源：http://hz.ydzc1.top/gtvnozktlm.html

PHP:  getcwd();
来源：http://hz.shanyushiyangkeji.top/gtjfhnlymt.html

JS:   process.cwd()
来源：http://hz.fzhhl.top/gtbvghnxov.html

TS:   process.cwd()
来源：http://hz.jinghuilouyu.cn/gtfritsrpq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhengqikj.top/gtltxchhoc.html

Go:   os.Getwd()
来源：http://hz.jianghu66.top/gtywehmoxg.html

Ruby: Dir.pwd
来源：http://hz.yj20258888.top/gtjtpkwenu.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.guowangkeji.top/gtbqbegkrk.html

[M05] 设置退出码
来源：http://hz.gzhubu.top/gtgxfvinnf.html

Py:   sys.exit(1)
来源：http://hz.tianlin.xyz/gteywcdxke.html

PHP:  exit(1);
来源：http://hz.xziqi.cn/gtscpadtkf.html

JS:   process.exit(1)
来源：http://hz.cqqwz.cn/gtspzqsrle.html

TS:   process.exit(1)
来源：http://hz.9152youxi.cn/gtzruimxfv.html

Java: System.exit(1)
来源：http://hz.hfpthk.cn/gtchkhnshc.html

Go:   os.Exit(1)
来源：http://hz.jinghuilouyu.cn/gtjxwqdvvf.html

Ruby: exit 1
来源：http://hz.shuidangran.top/gtmlwqlrzu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhongyouzk.top/gtyazdzlbs.html

[M06] 向标准错误输出
来源：http://hz.jqgfzy.top/gtiwbyfxtj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.mhx1999.top/gtsizzwcyw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.bjfxy.top/gtyvtpixjk.html

JS:   console.error("err")
来源：http://hz.cqqwz.cn/gtvwloxrdf.html

TS:   console.error("err")
来源：http://hz.hysaishi.cn/gtglieleqq.html

Java: System.err.println("err")
来源：http://hz.ivvv.top/gtpkglfttb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sysykeji.top/gtzjpgwgck.html

Ruby: warn "err"
来源：http://hz.hnqzz.top/gtlsofbeek.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.andypj.xyz/gtpqwjwhfs.html

[M07] 判断是否为主入口
来源：http://hz.aizwys.cn/gtfuaqbdai.html

Py:   if __name__ == "__main__":
来源：http://hz.jiagoushi.top/gtfuytpmfw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.sxryk.cn/gteieulkij.html

JS:   require.main === module
来源：http://hz.zhiwuduotai.top/gtybvxpnri.html

TS:   require.main === module
来源：http://hz.iojbl.cn/gtpronthhf.html

Java: public static void main(String[] args)
来源：http://hz.jinghuilouyu.cn/gtkabuwhsx.html

Go:   func main()
来源：http://hz.zhengqikj.top/gtakplayfs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.daxiang520.top/gtbaresyph.html

C#:   static void Main(string[] args)
来源：http://hz.hywenlv.cn/gtynfjbufe.html

[M08] 获取系统与运行时信息
来源：http://hz.xylfe.cn/gtfclmawnv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gzhubu.top/gtinpqupal.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.9152youxi.cn/gtfqtnamtk.html

JS:   process.platform;  process.version
来源：http://hz.jianghu66.top/gtcdzfbier.html

TS:   process.platform;  process.version
来源：http://hz.shuidangran.top/gtyzrpoxrw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sxryk.cn/gtrbfpggpj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hnxiangtu.top/gthlqjrduq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cashguo.top/gtzgbhwfkf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.aizwys.cn/gtjipylqqe.html

================================================================================
来源：http://hz.yongpay.top/gtcaxumcmz.html

N. 数据结构与算法
来源：http://hz.zhongyouzk.top/gtyivarbei.html

================================================================================
来源：http://hz.cucudq.cn/gthczjmcwz.html

[N01] 二分查找（有序数组）
来源：http://hz.chenjidiqi.icu/gtiiukkuzk.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.cashguo.top/gtdhwnwfgn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yuxming.cn/gtbjpfisni.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.svipenyu.cn/gtywckcwkr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daria6918.cn/gtkfxebvqf.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yj20258.top/gtlkcyyriw.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jyoumei.cn/gtjjxvcchj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yuanzhike.top/gtrtinziul.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jlsjyb.cn/gtuxgddffm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.tian-w.cn/gthyfjvktc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangtech.top/gtgtymmlys.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nanxinkj.top/gtdyexwvkt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.pycfn.com/gtsrgnzfhp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.mhx1999.top/gtzocqanro.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yonumen.top/gtyvqnxvik.html

Go:   slices.Sort(arr)
来源：http://hz.mhx1999.top/gteelhcdbw.html

Ruby: arr.sort
来源：http://hz.chenjidiqi.icu/gttvvbqrls.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.gotoacloud.top/gtqimxqeid.html

[N03] 快速排序（分治示例）
来源：http://hz.zhongyouzk.top/gtzfttzbfx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhijiandao.cn/gtkflodgtx.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sweek.top/gtesgktbmg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aibaodan.cn/gtewipcihv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hfpthk.cn/gtwcnphwow.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xinyue.icu/gtupjcyxqv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hysaishi.cn/gthcqpkkxr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenjidiqi.icu/gtkunacwdr.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.wangshuangyany.cn/gtdscgzwbw.html

[N04] 斐波那契数列
来源：http://hz.yongpay.top/gtozaqfjux.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhaomingkeji.xyz/gtntrljexk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zycfv.cn/gtstbdzagq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigfzy.top/gtmpsrcyyg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jyoumei.cn/gtetdnrwwj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.redwolf501.top/gtispbhije.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhongyouzk.top/gtsotqezpr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.snrcjt.cn/gtugjrhycd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ivvv.top/gtlaprekxy.html

[N05] 最大公约数
来源：http://hz.quarkkingdee.top/gthzzxskcz.html

Py:   math.gcd(a, b)
来源：http://hz.zdqjudy.top/gtxqvecnha.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.bjfxy.top/gtlzkdempx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.vqdsnc.cn/gtzulkevvw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangtech.top/gtngzvbkgh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.0kj1m.cn/gtbkemhvuf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shangyingyoupin.top/gtjuvhmiqf.html

Ruby: a.gcd(b)
来源：http://hz.jqgufenzy.top/gtywxqinik.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ydjk.org.cn/gtaupjzehh.html

[N06] 判断回文字符串
来源：http://hz.sweek.top/gtfjmjfbiv.html

Py:   s == s[::-1]
来源：http://hz.guannengcc.top/gtzowocfrb.html

PHP:  $s === strrev($s);
来源：http://hz.cheryme.top/gtbhonbvqy.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sweek.top/gtgeopnvra.html

TS:   s === [...s].reverse().join("")
来源：http://hz.aizwys.cn/gtpbmuscco.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.316326.xyz/gtxbunfmdm.html

Go:   // 双指针从两端比较
来源：http://hz.yj202588.top/gtvhfeeugt.html

Ruby: s == s.reverse
来源：http://hz.tanke756.top/gtnwntpwuk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.iojbl.cn/gtgmlhiuac.html

[N07] 两数之和（返回下标）
来源：http://hz.fzhhl.top/gtceycyqgt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhongyouzk.top/gtjszwflby.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.wangshuangyany.cn/gtnfybxxjj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.bjfxy.top/gtkaincoty.html

TS:   // 手写 Map<string, number>
来源：http://hz.shzxlz.cn/gtjjaypifr.html

Java: // 手写 HashMap
来源：http://hz.daria6918.cn/gtdyetlocb.html

Go:   // 手写 map[int]int
来源：http://hz.shzxlz.cn/gtpsfomsrn.html

Ruby: // 手写 Hash
来源：http://hz.tianlin.xyz/gtyzqnelql.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xylfe.cn/gtkxytoxzp.html

[N08] 生成全排列
来源：http://hz.chenlongwang.top/gtpkdegywp.html

Py:   itertools.permutations(arr)
来源：http://hz.tanke756.top/gtruomtpam.html

PHP:  // 手写递归交换
来源：http://hz.tianlin.xyz/gtfvrglucw.html

JS:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtdgecthja.html

TS:   // 手写回溯递归
来源：http://hz.meibo888.top/gtlnivsjlv.html

Java: // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtrigownjm.html

Go:   // 手写回溯递归
来源：http://hz.mhx1999.top/gthkfjnkrq.html

Ruby: arr.permutation.to_a
来源：http://hz.jinghuilouyu.cn/gtiwzzapzn.html

C#:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtnbzmyywx.html

[N09] 栈与队列
来源：http://hz.hysaishi.cn/gtcjtuhsoz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.chenzaomai.com/gthflwhhux.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hnqzz.top/gtckhijtcx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yanxiufei.cn/gtamvrdnmh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ydjk.org.cn/gtxuhkmgdd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinqigufen.top/gtrjgkfdec.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gotoacloud.top/gtcttdehbx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jinghuilouyu.cn/gtvdlxbgii.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.aibaodan.cn/gtrpdgaxez.html

[N10] 链表节点定义
来源：http://hz.guannengcc.top/gtmvgvwwwr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.tian-w.cn/gtjtbolmpk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yanxiufei.cn/gtyobvopru.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zycfv.cn/gttwymkewi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.kuanghao11.cn/gtabiuoekz.html

Java: class Node { int v; Node next; }
来源：http://hz.gaohongyu789.top/gtmtvepscz.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.dashuyun.cn/gttlhbsbkw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yuanzhike.top/gtufunzrqk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hysaishi.cn/gtyhmzdqha.html

[N11] 二叉树中序遍历
来源：http://hz.hysaishi.cn/gtmgkemqkc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yuanzhike.top/gtxzsqqbzr.html

PHP:  // 手写递归函数
来源：http://hz.dianchejie.cn/gtmuqimlxh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.kuanghao11.cn/gtciqowyft.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fengsongda.top/gttbwohrfb.html

Java: // 手写递归
来源：http://hz.nanxuanxn.top/gtmdpadkts.html

Go:   // 手写递归
来源：http://hz.zdqjudy.top/gtlzwkhkhm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.pycfn.com/gtflaqpgrv.html

C#:   // 手写递归
来源：http://hz.daxiang520.top/gtmtwqpwda.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cqqwz.cn/gtdzeviamr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.dianchejie.cn/gtddqphhji.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhongyouzk.top/gtmuxjbnct.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.guowangkeji.top/gtesxymghv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgfzy.top/gtjutzwsqf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hfpthk.cn/gtmzumkpfs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.gotoacloud.top/gtqgeoidyl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xziqi.cn/gtzkjjzrax.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigufen.top/gtrpzytokr.html

================================================================================
来源：http://hz.52xcode.cn/gttpfaojkm.html

O. 并发与异步
来源：http://hz.xylfe.cn/gtbibqsomj.html

================================================================================
来源：http://hz.52xcode.cn/gtsuxcvzpi.html

[O01] 启动一个线程
来源：http://hz.yj20258.top/gtodtbyhwr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shangyingyoupin.top/gtxowjmssa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.52xcode.cn/gtexdxhjka.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jinghuilouyu.cn/gtuggwrkyn.html

TS:   // 同 JS
来源：http://hz.tanke756.top/gtwhvuizpf.html

Java: new Thread(() -> f()).start()
来源：http://hz.cashguo.top/gtnxkgonxz.html

Go:   go f()
来源：http://hz.tian-w.cn/gtyfjlhwoh.html

Ruby: Thread.new { f }
来源：http://hz.xinyue.icu/gtmhkuzwbz.html

C#:   Task.Run(() => F());
来源：http://hz.c1oappe.top/gtcdotmmom.html

[O02] 使用线程池
来源：http://hz.xziqi.cn/gtivpmkslk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.redwolf501.top/gttadpcwyd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cucudq.cn/gtqtgxwufi.html

JS:   // worker_threads 线程池
来源：http://hz.jinghuilouyu.cn/gtszclhzws.html

TS:   // worker_threads 线程池
来源：http://hz.zhixingplan.top/gteqlqfxbp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinqigfzy.top/gtouyhfraj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.nwbrower.top/gtqbkxoebu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yanxiufei.cn/gtjejxzvwc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yongpay.top/gtymfioufz.html

[O03] 加锁保护共享数据
来源：http://hz.redwolf501.top/gtoxauljic.html

Py:   with lock: shared += 1
来源：http://hz.sufxvd.cn/gtxonebaso.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xingfuxueyuan.xyz/gtuqygskjv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jqgfzy.top/gtwrscjhns.html

TS:   // 同 JS
来源：http://hz.haohaochexian.top/gtimmatztu.html

Java: synchronized (this) { shared++; }
来源：http://hz.pengpengdd.cyou/gtndqywmxq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.fengsongda.top/gtpfethjcd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.andypj.xyz/gtwetclnhm.html

C#:   lock (gate) { shared++; }
来源：http://hz.sufxvd.cn/gtpsuzdlxl.html

[O04] 定义异步函数并等待
来源：http://hz.daxiang520.top/gtdtvlxfia.html

Py:   async def f():⏎    await g()
来源：http://hz.jqgufenzy.top/gtegjculof.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yj20258.top/gtwgsxktuv.html

JS:   async function f() { await g(); }
来源：http://hz.hammf.cn/gtbohslqrm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.wangshuangyany.cn/gtlkfhkzxr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yongpay.top/gtofsmyqvx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.chenzaomai.com/gtppxyaujg.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hywenlv.cn/gtqaiwnwrd.html

C#:   async Task F() { await G(); }
来源：http://hz.zhengqikj.top/gtsxnjygsx.html

[O05] 并发执行并等待全部完成
来源：http://hz.hongshengwenyu.top/gtqcsgflmn.html

Py:   asyncio.gather(*tasks)
来源：http://hz.pycfn.com/gtvypeshej.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.316326.xyz/gtsferdzxx.html

JS:   await Promise.all(tasks)
来源：http://hz.kuanghao11.cn/gtxcbakjmh.html

TS:   await Promise.all(tasks)
来源：http://hz.sufxvd.cn/gtgztbqtrt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.tian-w.cn/gtvoyzesly.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.redwolf501.top/gtfuvhmaaq.html

Ruby: threads.map(&:join)
来源：http://hz.nwbrower.top/gtfouwjclz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shangyingyoupin.top/gtqqabbhzs.html

[O06] 使用进程池
来源：http://hz.gogol.net.cn/gtyvsadqhf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.kuanghao11.cn/gtonxhesye.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hnxiangtu.top/gtptyrlqdd.html

JS:   // child_process / cluster 模块
来源：http://hz.haohaochexian.top/gtngvmjslh.html

TS:   // child_process / cluster 模块
来源：http://hz.birdmap.top/gthcbuljeg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jqgfzy.top/gtjskituls.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.sysykeji.top/gtiiliwcnz.html

Ruby: // fork 块
来源：http://hz.sufxvd.cn/gtdaccjqsv.html

C#:   Parallel.For
来源：http://hz.wangshuangyany.cn/gtiapzoxwx.html

================================================================================
来源：http://hz.hysaishi.cn/gtbdagwfah.html

P. 常用工具函数
来源：http://hz.guannengcc.top/gtcvgqawze.html

================================================================================
来源：http://hz.yj202588.top/gtnnxfjbdv.html

[P01] 生成 UUID
来源：http://hz.mhx1999.top/gtqhgxogjl.html

Py:   str(uuid.uuid4())
来源：http://hz.chenjidiqi.icu/gtjdibersx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yuanzhike.top/gtrrnzjole.html

JS:   crypto.randomUUID()
来源：http://hz.meibo888.top/gtnqjwhtrz.html

TS:   crypto.randomUUID()
来源：http://hz.jinyuanbaomall.cn/gtzahhsrcm.html

Java: UUID.randomUUID().toString()
来源：http://hz.nanxinkj.top/gtxlunllzv.html

Go:   // 用 github.com/google/uuid
来源：http://hz.daxiang520.top/gtxorwcydw.html

Ruby: SecureRandom.uuid
来源：http://hz.0kj1m.cn/gtvtyqjaef.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.fzhhl.top/gtiozhtdrs.html

[P02] MD5 / SHA256 摘要
来源：http://hz.kuanghao11.cn/gtjnqqsovr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.birdmap.top/gtvgoosjfh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.snrcjt.cn/gticncbeci.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zycfv.cn/gtosxfrtcm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jlsjyb.cn/gtlugcxygx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hfpthk.cn/gtuqdmumsx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.wangdashe.top/gtzztecyfx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.kuanghao11.cn/gtbyilkgyr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.pengpengdd.cyou/gtcnughkut.html

[P03] 生成短随机字符串
来源：http://hz.c1oappe.top/gthwtrvyiy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jlsjyb.cn/gthpvjggrj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhengqikj.top/gtbjzpxstm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.0kj1m.cn/gtaaxtpgmx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.guowangkeji.top/gtiscidiyh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shzxlz.cn/gtlofkporj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xingfuxueyuan.xyz/gtkegthcmy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.9152youxi.cn/gtrindmjkp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.svipenyu.cn/gtlkfhxcej.html

[P04] 求长度
来源：http://hz.jinyuanbaomall.cn/gtswwljjgl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.quarkkingdee.top/gtaueaktzj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.meibo888.top/gtuisylcap.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yvedp.cn/gtvjxmoafg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xziqi.cn/gtevcybwbe.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jinghuilouyu.cn/gtgizklvzv.html

Go:   len(arr);  len(m)
来源：http://hz.jinqigufen.top/gttlsgceew.html

Ruby: x.length;  x.size
来源：http://hz.pengpengdd.cyou/gtduenligj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shzxlz.cn/gtklfzupmk.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sysykeji.top/gtuhoqbyil.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.havefunace.top/gtvlkhsegr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hammf.cn/gtkdqqugrw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.sweek.top/gtihpbxclr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.andypj.xyz/gtgpcctuor.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinghuilouyu.cn/gtfnejjlxx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.haohaochexian.top/gtghdtguky.html

Ruby: a == b
来源：http://hz.jqgufenzy.top/gtffqdjzkf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gogol.net.cn/gtjkrdeyru.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.dianchejie.cn/gtrdaxrclf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.iojbl.cn/gtpxdiyjoa.html

PHP:  if (empty($x)) {}
来源：http://hz.sysykeji.top/gtkdeklwsi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinyuanbaomall.cn/gtdakeuxwd.html

TS:   if (x == null) {}
来源：http://hz.ydjk.org.cn/gtlzhdbwai.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sufxvd.cn/gtdscfqqcn.html

Go:   if x == nil {}
来源：http://hz.cheryme.top/gtobdfxaor.html


<!-- 参考信息 -->