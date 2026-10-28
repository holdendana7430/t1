代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydzc1.top/gteukgivob.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydjk.org.cn/gtpiyptzrt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinyuanbaomall.cn/gtbaanowgs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.fengsongda.top/gtlfjyzvrk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.9152youxi.cn/gtghvteczc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinqigufen.top/gtofdeutpc.html

================================================================================
来源：http://hz.iojbl.cn/gttxqyodmi.html

M. 命令行 / 进程 / 环境
来源：http://hz.gaohongyu789.top/gteifqkbzw.html

================================================================================
来源：http://hz.jinqigfzy.top/gtvvdrmacw.html

[M01] 读取命令行参数
来源：http://hz.zhijiandao.cn/gtqnpynrxx.html

Py:   sys.argv[1:]
来源：http://hz.wangdashe.top/gtlqsgvkjt.html

PHP:  $argv;  $argc;
来源：http://hz.tianlin.xyz/gtrwtvyilo.html

JS:   process.argv.slice(2)
来源：http://hz.fengsongda.top/gtduoibkti.html

TS:   process.argv.slice(2)
来源：http://hz.redwolf501.top/gtxbphiycy.html

Java: args 数组（main 方法参数）
来源：http://hz.nanxuanxn.top/gtnmawvldk.html

Go:   os.Args[1:]
来源：http://hz.bjfxy.top/gttbqdztit.html

Ruby: ARGV
来源：http://hz.gaohongyu789.top/gtjvurbpdp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hongshengwenyu.top/gtpxviykxk.html

[M02] 读取环境变量
来源：http://hz.vqdsnc.cn/gtcmgofoqj.html

Py:   os.environ.get("HOME")
来源：http://hz.yuanzhike.top/gtmxuchqtj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jqgufenzy.top/gtjzsxzjqn.html

JS:   process.env.HOME
来源：http://hz.ydjk.org.cn/gtvcumfhjs.html

TS:   process.env.HOME
来源：http://hz.ehwqpu.com/gtgwiufppq.html

Java: System.getenv("HOME")
来源：http://hz.gotoacloud.top/gtstvcepku.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhiwuduotai.top/gtdvwdacwe.html

Ruby: ENV["HOME"]
来源：http://hz.andypj.xyz/gtrecwcwno.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.snrcjt.cn/gtghtrsfbf.html

[M03] 执行外部命令
来源：http://hz.ppjwa.cn/gtamzmsaou.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shuidangran.top/gtzarfijqm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhixingplan.top/gtyyzvedre.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cdnleiting.top/gtwrnfuxdq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.svipenyu.cn/gtepkafcqq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xingfuxueyuan.xyz/gtizxmpstk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.aizwys.cn/gtcykjctuv.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.52xcode.cn/gtsbjnxeih.html

C#:   Process.Start("ls", "-l");
来源：http://hz.chenlongwang.top/gtrgrgdmha.html

[M04] 获取当前工作目录
来源：http://hz.316326.xyz/gtbozhsckw.html

Py:   os.getcwd()
来源：http://hz.yj20258.top/gtveratvji.html

PHP:  getcwd();
来源：http://hz.ppjwa.cn/gtrcxracgy.html

JS:   process.cwd()
来源：http://hz.vqdsnc.cn/gtstafboty.html

TS:   process.cwd()
来源：http://hz.jlsjyb.cn/gtbzrzzjea.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.bjfxy.top/gtivnseuol.html

Go:   os.Getwd()
来源：http://hz.nanxuanxn.top/gtcrltuefs.html

Ruby: Dir.pwd
来源：http://hz.cashguo.top/gtsrjnymef.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sxryk.cn/gtgopjlvtn.html

[M05] 设置退出码
来源：http://hz.nanxuanxn.top/gtulrtbigw.html

Py:   sys.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtzmsuhhol.html

PHP:  exit(1);
来源：http://hz.jiagoushi.top/gtuetavtlj.html

JS:   process.exit(1)
来源：http://hz.cdnleiting.top/gtloxhypso.html

TS:   process.exit(1)
来源：http://hz.jinghuilouyu.cn/gtsrothflj.html

Java: System.exit(1)
来源：http://hz.yuanzhike.top/gteaucazws.html

Go:   os.Exit(1)
来源：http://hz.bjfxy.top/gtimnplglu.html

Ruby: exit 1
来源：http://hz.hywenlv.cn/gtczpaaiqm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cucudq.cn/gtneqavmwu.html

[M06] 向标准错误输出
来源：http://hz.pycfn.com/gtxfbmtzmg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hfpthk.cn/gtnoiuerod.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yj202588.top/gtnnpdmzcw.html

JS:   console.error("err")
来源：http://hz.9152youxi.cn/gtefagpezl.html

TS:   console.error("err")
来源：http://hz.shzxlz.cn/gthkdbbtfu.html

Java: System.err.println("err")
来源：http://hz.hongshengwenyu.top/gtslgiqmte.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gzhubu.top/gtysowpico.html

Ruby: warn "err"
来源：http://hz.meibo888.top/gtzuertonp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.sufxvd.cn/gtujqhixtl.html

[M07] 判断是否为主入口
来源：http://hz.xinyue.icu/gtdpigjqmp.html

Py:   if __name__ == "__main__":
来源：http://hz.shzxlz.cn/gtasslnojk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.316326.xyz/gtjfnelvqc.html

JS:   require.main === module
来源：http://hz.guowangkeji.top/gtvqtkfynr.html

TS:   require.main === module
来源：http://hz.xinyue.icu/gtnqfecvad.html

Java: public static void main(String[] args)
来源：http://hz.wangshuangyany.cn/gtsgzymwrc.html

Go:   func main()
来源：http://hz.c1oappe.top/gtfuxywhjs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhongyouzk.top/gtlvotlilv.html

C#:   static void Main(string[] args)
来源：http://hz.nanxinkj.top/gtanfrgdpc.html

[M08] 获取系统与运行时信息
来源：http://hz.cqqwz.cn/gtgpktbxuf.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xylfe.cn/gtidqzelgx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.vqdsnc.cn/gtlbtrbgca.html

JS:   process.platform;  process.version
来源：http://hz.chenzaomai.com/gtehfjgccs.html

TS:   process.platform;  process.version
来源：http://hz.hammf.cn/gtgmmqjxnb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jqgfzy.top/gtbyoccfjt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shzxlz.cn/gtfyuctzui.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.316326.xyz/gtczawzslk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinghuilouyu.cn/gtssythukg.html

================================================================================
来源：http://hz.pycfn.com/gtqemmzyqt.html

N. 数据结构与算法
来源：http://hz.quarkkingdee.top/gtywjqewhj.html

================================================================================
来源：http://hz.nwbrower.top/gtljbjdnbq.html

[N01] 二分查找（有序数组）
来源：http://hz.yonumen.top/gtwzujhrmr.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhixingplan.top/gtnldnxwum.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gogol.net.cn/gtfgwfeffa.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yonumen.top/gtorqghssl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cdnleiting.top/gtynguwmsa.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.pycfn.com/gtpkiqrtxs.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.tian-w.cn/gtviohldcl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sufxvd.cn/gtqbwsgcbi.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xinyue.icu/gtemyrbdzy.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.haohaochexian.top/gtzllojwlu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangkeji.top/gtrczggkhf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.fengsongda.top/gtoxzmabud.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuetiantiany.cn/gtqobqpfwi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhijiandao.cn/gteqhhzgme.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shanyushiyangkeji.top/gtdxfxpysh.html

Go:   slices.Sort(arr)
来源：http://hz.wangshuangyany.cn/gtjfrmxrwk.html

Ruby: arr.sort
来源：http://hz.cheryme.top/gtleuilniz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinqigfzy.top/gtapynibim.html

[N03] 快速排序（分治示例）
来源：http://hz.jyoumei.cn/gtzrltgbfz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinqigufen.top/gtyubnonlg.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhoulong.xyz/gtqnlgctog.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuanzhike.top/gtyssyoxng.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.52xcode.cn/gtamfjnonh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yongpay.top/gtxfhjubdn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jqgfzy.top/gtqhnufmup.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hongshengwenyu.top/gtuevwznsk.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.haohaochexian.top/gtvahxptbp.html

[N04] 斐波那契数列
来源：http://hz.jyoumei.cn/gtxnmlfhds.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zycfv.cn/gtuhexgqce.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ydzc1.top/gtztjgewgj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sweek.top/gtsrlgglik.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gtbplbuaeu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jinqigfzy.top/gtjimdokif.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.tanke756.top/gtzranlhsa.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ivvv.top/gtgbqamxzg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.nanxuanxn.top/gtdnnltrjj.html

[N05] 最大公约数
来源：http://hz.zhoulong.xyz/gthrvzyfjk.html

Py:   math.gcd(a, b)
来源：http://hz.fzhhl.top/gtswtoxlvd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.pengpengdd.cyou/gtujilsyyq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shzxlz.cn/gtdrrmarok.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cdnleiting.top/gtfvluvzfk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cucudq.cn/gtraqpnghn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ppjwa.cn/gtrsjqsoyi.html

Ruby: a.gcd(b)
来源：http://hz.hnqzz.top/gtnxlndqrz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jqgfzy.top/gtmgekkpnc.html

[N06] 判断回文字符串
来源：http://hz.quarkkingdee.top/gtymbhfirc.html

Py:   s == s[::-1]
来源：http://hz.shzxlz.cn/gtfovlzfkl.html

PHP:  $s === strrev($s);
来源：http://hz.jinghuilouyu.cn/gthqzpwtcm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.316326.xyz/gtjebludyo.html

TS:   s === [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtxmeqcfsu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.havefunace.top/gtbszcewap.html

Go:   // 双指针从两端比较
来源：http://hz.nwbrower.top/gtooddtrtr.html

Ruby: s == s.reverse
来源：http://hz.shanyushiyangkeji.top/gtthpxrdze.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhixingplan.top/gtxfvlgbmt.html

[N07] 两数之和（返回下标）
来源：http://hz.wangdashe.top/gtbudgrqwc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.dashuyun.cn/gtyxlprbpy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ybcxt.top/gtrsphrtsr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.birdmap.top/gteszvzqex.html

TS:   // 手写 Map<string, number>
来源：http://hz.hfpthk.cn/gthsmkpgjf.html

Java: // 手写 HashMap
来源：http://hz.chenjidiqi.icu/gterxyuzcl.html

Go:   // 手写 map[int]int
来源：http://hz.andypj.xyz/gtwpxtsbuz.html

Ruby: // 手写 Hash
来源：http://hz.bjfxy.top/gtnknorhsj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.guannengcc.top/gtfrimooqr.html

[N08] 生成全排列
来源：http://hz.chenjidiqi.icu/gtgxcjubij.html

Py:   itertools.permutations(arr)
来源：http://hz.cdnleiting.top/gtzgpppdbb.html

PHP:  // 手写递归交换
来源：http://hz.fengsongda.top/gtfmmhzalf.html

JS:   // 手写回溯递归
来源：http://hz.zycfv.cn/gtyotgdaqf.html

TS:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtakooyfce.html

Java: // 手写回溯递归
来源：http://hz.ivvv.top/gtmrapyyvx.html

Go:   // 手写回溯递归
来源：http://hz.hammf.cn/gtquvjrcdp.html

Ruby: arr.permutation.to_a
来源：http://hz.daxiang520.top/gtirhmzzpo.html

C#:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gthsgekgfd.html

[N09] 栈与队列
来源：http://hz.yvedp.cn/gtlywzramy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sxryk.cn/gtpjpdhrjn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinghuilouyu.cn/gtvgebdaba.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ppjwa.cn/gtgepzrpwo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yuxming.cn/gtnoobmych.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xziqi.cn/gtqbhcysgm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhoulong.xyz/gtntdgdyfe.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sweek.top/gticznxuaw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinqigufen.top/gtkkprqsws.html

[N10] 链表节点定义
来源：http://hz.bjfxy.top/gtcqoutgno.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhaomingkeji.xyz/gtriwpmybv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shzxlz.cn/gtitsubegr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sysykeji.top/gteqyvfdds.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shuidangran.top/gtlytnnkce.html

Java: class Node { int v; Node next; }
来源：http://hz.chenzaomai.com/gtvalgcwvk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.aibaodan.cn/gtpmryekwb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cashguo.top/gtwdjvezoe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jinqigufen.top/gtjyysshjd.html

[N11] 二叉树中序遍历
来源：http://hz.xinyue.icu/gtdulchlgb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.aizwys.cn/gtepmbllxv.html

PHP:  // 手写递归函数
来源：http://hz.jinghuilouyu.cn/gtzdwxjknj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ppjwa.cn/gtyninkvco.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gzhubu.top/gtozvxmbyi.html

Java: // 手写递归
来源：http://hz.9152youxi.cn/gtocbpiclp.html

Go:   // 手写递归
来源：http://hz.yueranfly.top/gtxjgnevfe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xuetiantiany.cn/gtxbsyjnfm.html

C#:   // 手写递归
来源：http://hz.yanxiufei.cn/gtximhcsam.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.fzhhl.top/gtgppzxwyu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hywenlv.cn/gtwkqrjomc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.aibaodan.cn/gtcwvrnbvz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhoulong.xyz/gtezewqwrh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.0kj1m.cn/gtduddnzqt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigfzy.top/gtnopeesrb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.andypj.xyz/gtujqbjpew.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cucudq.cn/gttemsyyso.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydjk.org.cn/gtelequlfl.html

================================================================================
来源：http://hz.daxiang520.top/gtblemcspk.html

O. 并发与异步
来源：http://hz.tian-w.cn/gtauiuanbn.html

================================================================================
来源：http://hz.zhoulong.xyz/gtnzvhbgmj.html

[O01] 启动一个线程
来源：http://hz.yangfankeji.com/gttuekbozh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ppjwa.cn/gtmgypxdsg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.snrcjt.cn/gthwmwrmbe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xylfe.cn/gtlrymnmtu.html

TS:   // 同 JS
来源：http://hz.zhixingplan.top/gtxehzliqg.html

Java: new Thread(() -> f()).start()
来源：http://hz.hfpthk.cn/gtbnfjpmvr.html

Go:   go f()
来源：http://hz.jinghuilouyu.cn/gtytlwatdq.html

Ruby: Thread.new { f }
来源：http://hz.0kj1m.cn/gtaobodafq.html

C#:   Task.Run(() => F());
来源：http://hz.dashuyun.cn/gtmdigfhyv.html

[O02] 使用线程池
来源：http://hz.ydzc1.top/gtycctplhz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jlsjyb.cn/gtmjgqryel.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.dashuyun.cn/gtrkngcoae.html

JS:   // worker_threads 线程池
来源：http://hz.xingfuxueyuan.xyz/gtbsnvyfjv.html

TS:   // worker_threads 线程池
来源：http://hz.zhongyouzk.top/gtfetjcpey.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.iojbl.cn/gtpzlbupfj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.9152youxi.cn/gthavdspbl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.aibaodan.cn/gtvgkpodoi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xuetiantiany.cn/gtkabrqzkp.html

[O03] 加锁保护共享数据
来源：http://hz.jinyuanbaomall.cn/gtsdyatgbk.html

Py:   with lock: shared += 1
来源：http://hz.hnxiangtu.top/gtvrrccsyd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sufxvd.cn/gttqliampc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yuanzhike.top/gtbywkpzjm.html

TS:   // 同 JS
来源：http://hz.pengpengdd.cyou/gtrolfhzhu.html

Java: synchronized (this) { shared++; }
来源：http://hz.zycfv.cn/gtzzybpppd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.nanxuanxn.top/gtwwlqxfgh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.aizwys.cn/gtkokpkwal.html

C#:   lock (gate) { shared++; }
来源：http://hz.gaohongyu789.top/gtfrahtaan.html

[O04] 定义异步函数并等待
来源：http://hz.jinghuilouyu.cn/gtcxjicodw.html

Py:   async def f():⏎    await g()
来源：http://hz.cqqwz.cn/gtcmztwawm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhixingplan.top/gtszrrkhnz.html

JS:   async function f() { await g(); }
来源：http://hz.gogol.net.cn/gtfggzpwvg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cashguo.top/gthmnkxqig.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cucudq.cn/gtzmqrdnrc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shanyushiyangtech.top/gtfjxuycuv.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.meibo888.top/gtqiydwvjv.html

C#:   async Task F() { await G(); }
来源：http://hz.jinghuilouyu.cn/gtoytnqfcl.html

[O05] 并发执行并等待全部完成
来源：http://hz.shzxlz.cn/gtfnjvtrrq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.sufxvd.cn/gtgtmpieik.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ybcxt.top/gtycuadmin.html

JS:   await Promise.all(tasks)
来源：http://hz.hammf.cn/gtlpabroxf.html

TS:   await Promise.all(tasks)
来源：http://hz.aibaodan.cn/gtrssqkzfi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shanyushiyangkeji.top/gtlrykypdh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xinyue.icu/gtgtjwfvbd.html

Ruby: threads.map(&:join)
来源：http://hz.jinqigfzy.top/gtibixjpbv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.feifeiyinyue.top/gtyikfylml.html

[O06] 使用进程池
来源：http://hz.vqdsnc.cn/gtnrmtfihu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.pengpengdd.cyou/gtwlrwbkso.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hongshengwenyu.top/gtbrfgezkq.html

JS:   // child_process / cluster 模块
来源：http://hz.aibaodan.cn/gtgkclizld.html

TS:   // child_process / cluster 模块
来源：http://hz.yonumen.top/gtaoweiapa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.redwolf501.top/gtcgtpexop.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.aibaodan.cn/gtcibdutbb.html

Ruby: // fork 块
来源：http://hz.0kj1m.cn/gtcpkygmwf.html

C#:   Parallel.For
来源：http://hz.hywenlv.cn/gtqznxpqkp.html

================================================================================
来源：http://hz.xinyue.icu/gtqkcbxfuy.html

P. 常用工具函数
来源：http://hz.yuxming.cn/gtzncvjjyc.html

================================================================================
来源：http://hz.hfpthk.cn/gtxlskuwuo.html

[P01] 生成 UUID
来源：http://hz.yanxiufei.cn/gtnmhtuqkg.html

Py:   str(uuid.uuid4())
来源：http://hz.zhixingplan.top/gtjruuusiu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yj202588.top/gtjhwgywdx.html

JS:   crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtjfqcpklv.html

TS:   crypto.randomUUID()
来源：http://hz.fzhhl.top/gtxlqyyori.html

Java: UUID.randomUUID().toString()
来源：http://hz.shzxlz.cn/gtovgvoyef.html

Go:   // 用 github.com/google/uuid
来源：http://hz.316326.xyz/gtxdsqquhc.html

Ruby: SecureRandom.uuid
来源：http://hz.yj202588.top/gtaodhxbzx.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinqigfzy.top/gtqjxvloeg.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cheryme.top/gttsoarbvh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jiagoushi.top/gtynaamifk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shuidangran.top/gtefeylpfa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.sweek.top/gtggnrsima.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.haohaochexian.top/gtvhgtwzxy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zdqjudy.top/gtclnobwsp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhoulong.xyz/gtahxfbzey.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhaomingkeji.xyz/gtpbkhupig.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jqgufenzy.top/gtsdcmxyey.html

[P03] 生成短随机字符串
来源：http://hz.hywenlv.cn/gttuhvagsc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cdnleiting.top/gtirmzknqd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.fengsongda.top/gtzvuzanov.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuanzhike.top/gtqydtjdwk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydzc1.top/gttphrevrr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.tanke756.top/gtfmgjksgt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.fzhhl.top/gtrhzosyss.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.havefunace.top/gtgeyqanwi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.smart0.xyz/gtfqqvanpr.html

[P04] 求长度
来源：http://hz.meibo888.top/gtvcxlymmh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ehwqpu.com/gtygmomwuz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.0kj1m.cn/gtwwklakpi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.316326.xyz/gtwinktxle.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yonumen.top/gthyndxael.html

Java: list.size();  map.size();  s.length()
来源：http://hz.feifeiyinyue.top/gtyokxzxqo.html

Go:   len(arr);  len(m)
来源：http://hz.havefunace.top/gtzlwfbqqe.html

Ruby: x.length;  x.size
来源：http://hz.dianchejie.cn/gtzuzvpkmw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zdqjudy.top/gtarvbsqfp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hfpthk.cn/gtauueaxop.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.aizwys.cn/gtvlojaxid.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.tian-w.cn/gtzobpwpza.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nwbrower.top/gtpoqtggwz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hammf.cn/gtljwfwats.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yanxiufei.cn/gtnnwoncho.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hnxiangtu.top/gtsrclosst.html

Ruby: a == b
来源：http://hz.svipenyu.cn/gtdrfvxfhw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.c1oappe.top/gtcssdhhpz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xuanzx.com/gtuqkpxhgb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.9152youxi.cn/gtumyjnset.html

PHP:  if (empty($x)) {}
来源：http://hz.cdnleiting.top/gtfeuedafh.html


<!-- 参考信息 -->