代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.svipenyu.cn/gtutiiprrp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cdnleiting.top/gtbszsvhxc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shangyingyoupin.top/gtttrpeoan.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhengqikj.top/gtjwvuwdla.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zycfv.cn/gtqxywpohw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinyuanbaomall.cn/gtqhumcpoc.html

================================================================================
来源：http://hz.aibaodan.cn/gtdypgprjj.html

M. 命令行 / 进程 / 环境
来源：http://hz.tian-w.cn/gtdaypzrsn.html

================================================================================
来源：http://hz.cucudq.cn/gtstbeysbk.html

[M01] 读取命令行参数
来源：http://hz.nanxuanxn.top/gtzcydemgw.html

Py:   sys.argv[1:]
来源：http://hz.jqgufenzy.top/gtfukudjpw.html

PHP:  $argv;  $argc;
来源：http://hz.pycfn.com/gttwmnvlnh.html

JS:   process.argv.slice(2)
来源：http://hz.yj20258.top/gtcomvmyeh.html

TS:   process.argv.slice(2)
来源：http://hz.feifeiyinyue.top/gtnpzodtmt.html

Java: args 数组（main 方法参数）
来源：http://hz.jiagoushi.top/gthquzdzgy.html

Go:   os.Args[1:]
来源：http://hz.wangshuangyany.cn/gtrxqljgnj.html

Ruby: ARGV
来源：http://hz.andypj.xyz/gtdmmhrczd.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yanxiufei.cn/gtptwobhvb.html

[M02] 读取环境变量
来源：http://hz.yanxiufei.cn/gtardbjkfz.html

Py:   os.environ.get("HOME")
来源：http://hz.nanxinkj.top/gtypdkdfwx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.fzhhl.top/gtwdinfcll.html

JS:   process.env.HOME
来源：http://hz.cheryme.top/gtswxyneoo.html

TS:   process.env.HOME
来源：http://hz.jinqigfzy.top/gthbkurrac.html

Java: System.getenv("HOME")
来源：http://hz.jinyuanbaomall.cn/gtgxsaxfyr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ehwqpu.com/gtfinrymld.html

Ruby: ENV["HOME"]
来源：http://hz.gaohongyu789.top/gtzqvcqyde.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yvedp.cn/gtcqjrviaj.html

[M03] 执行外部命令
来源：http://hz.daria6918.cn/gtapfzkixd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jinghuilouyu.cn/gtnrjyiefe.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.havefunace.top/gtlpinuzte.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yongpay.top/gtnnaqtber.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.dianchejie.cn/gtlsywqgqa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sweek.top/gtgzygtdhf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sufxvd.cn/gtumjrohtr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shanyushiyangtech.top/gtpxzvfctw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.feifeiyinyue.top/gtahnbwtxy.html

[M04] 获取当前工作目录
来源：http://hz.meibo888.top/gtocccttto.html

Py:   os.getcwd()
来源：http://hz.hywenlv.cn/gtctzujqzh.html

PHP:  getcwd();
来源：http://hz.meibo888.top/gtxvpwaogy.html

JS:   process.cwd()
来源：http://hz.ybcxt.top/gtsmwqfxju.html

TS:   process.cwd()
来源：http://hz.sxryk.cn/gtgtdowbks.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yanxiufei.cn/gtpvqtscul.html

Go:   os.Getwd()
来源：http://hz.zhiwuduotai.top/gtfabjzkfq.html

Ruby: Dir.pwd
来源：http://hz.dianchejie.cn/gtunhggbsx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yvedp.cn/gtxenemwwl.html

[M05] 设置退出码
来源：http://hz.pengpengdd.cyou/gtfzllcqjt.html

Py:   sys.exit(1)
来源：http://hz.chenlongwang.top/gtutnoqclz.html

PHP:  exit(1);
来源：http://hz.cqqwz.cn/gtxgdknthm.html

JS:   process.exit(1)
来源：http://hz.sufxvd.cn/gtvugvnccg.html

TS:   process.exit(1)
来源：http://hz.fzhhl.top/gtjwfmahxt.html

Java: System.exit(1)
来源：http://hz.zycfv.cn/gtuuvbovjm.html

Go:   os.Exit(1)
来源：http://hz.smart0.xyz/gtzpfghrcu.html

Ruby: exit 1
来源：http://hz.jyoumei.cn/gtcwgofkyz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ywan-chungtsiang.top/gttilqweui.html

[M06] 向标准错误输出
来源：http://hz.cdnleiting.top/gtchpcfwvs.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yonumen.top/gtmfaitajl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shuidangran.top/gtxedlgikc.html

JS:   console.error("err")
来源：http://hz.yanxiufei.cn/gtxlhbnsji.html

TS:   console.error("err")
来源：http://hz.ybcxt.top/gtzxdtkfoj.html

Java: System.err.println("err")
来源：http://hz.jinqigufen.top/gthdiryjud.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shangyingyoupin.top/gtwebkhaqc.html

Ruby: warn "err"
来源：http://hz.aizwys.cn/gttygvvoah.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.316326.xyz/gtcotxydje.html

[M07] 判断是否为主入口
来源：http://hz.gzhubu.top/gtvmlnncpa.html

Py:   if __name__ == "__main__":
来源：http://hz.smart0.xyz/gtnoitnedy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhaomingkeji.xyz/gtqprzhrua.html

JS:   require.main === module
来源：http://hz.svipenyu.cn/gtysdhuwrc.html

TS:   require.main === module
来源：http://hz.sufxvd.cn/gtwxatvsop.html

Java: public static void main(String[] args)
来源：http://hz.hywenlv.cn/gtteapfgtl.html

Go:   func main()
来源：http://hz.52xcode.cn/gtvesagcpp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ywan-chungtsiang.top/gtbdkvtpoc.html

C#:   static void Main(string[] args)
来源：http://hz.shangyingyoupin.top/gtlqhesqjc.html

[M08] 获取系统与运行时信息
来源：http://hz.iojbl.cn/gtpormhkqf.html

Py:   platform.system();  platform.python_version()
来源：http://hz.guannengcc.top/gtajbewiaw.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.fzhhl.top/gtjmjitfhx.html

JS:   process.platform;  process.version
来源：http://hz.gaohongyu789.top/gtvrdvyokw.html

TS:   process.platform;  process.version
来源：http://hz.zhoulong.xyz/gtewidjgbd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.guannengcc.top/gtnyoyafca.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jiagoushi.top/gtiwlveajq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.feifeiyinyue.top/gtzboaqgvb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jlsjyb.cn/gtatitgmnh.html

================================================================================
来源：http://hz.cheryme.top/gtprvziydc.html

N. 数据结构与算法
来源：http://hz.shanyushiyangkeji.top/gtftderkxl.html

================================================================================
来源：http://hz.jqgfzy.top/gtlwbjnbuy.html

[N01] 二分查找（有序数组）
来源：http://hz.haohaochexian.top/gtgrzrkxoh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jlsjyb.cn/gtyrnhfvie.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.nwbrower.top/gtrbinslvm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.0kj1m.cn/gtbnovrupe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hongshengwenyu.top/gtvgxxhuvd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.birdmap.top/gtjkbygbou.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cucudq.cn/gtgbcylets.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.vqdsnc.cn/gtkpouxady.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.quarkkingdee.top/gtmwyfwini.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jqgfzy.top/gtonwgmvmq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tianlin.xyz/gtgmwbfrne.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yuanzhike.top/gtofrihzmk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258888.top/gtthitunnr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.vqdsnc.cn/gtqaokwckm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.guowangkeji.top/gtarbgtndz.html

Go:   slices.Sort(arr)
来源：http://hz.zhijiandao.cn/gtfvotgojc.html

Ruby: arr.sort
来源：http://hz.sxryk.cn/gtrtobersb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.tianlin.xyz/gtvwautwmt.html

[N03] 快速排序（分治示例）
来源：http://hz.xinyue.icu/gteneydzhi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xuanzx.com/gtebcqzzdf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.9152youxi.cn/gtclkwdfaw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hywenlv.cn/gtybbxzjas.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuetiantiany.cn/gttlipxczk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shzxlz.cn/gtpwxadalc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.havefunace.top/gtaejrehgy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ywan-chungtsiang.top/gthvaohdsp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gotoacloud.top/gtxcsriavs.html

[N04] 斐波那契数列
来源：http://hz.zycfv.cn/gtldcuegcu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.quarkkingdee.top/gtdkoetbla.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.chenlongwang.top/gtzxjujfvx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yanxiufei.cn/gtlwllycvl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuanzhike.top/gtxaivcktr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.nanxinkj.top/gtvqtrpgaw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.smart0.xyz/gtraromjlv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhongyouzk.top/gtnnzqscqh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.kuanghao11.cn/gtcrjnzbwx.html

[N05] 最大公约数
来源：http://hz.jyoumei.cn/gttseedkfe.html

Py:   math.gcd(a, b)
来源：http://hz.ywan-chungtsiang.top/gtcqubgbls.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.fzhhl.top/gtsvnkccpu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.snrcjt.cn/gtjylixxoe.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sysykeji.top/gtdgqwhunj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cheryme.top/gttrmshzuf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xuanzx.com/gtxsgmawwg.html

Ruby: a.gcd(b)
来源：http://hz.zycfv.cn/gtxkguctag.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shanyushiyangtech.top/gtsdwcpyte.html

[N06] 判断回文字符串
来源：http://hz.yj202588.top/gttoubvagr.html

Py:   s == s[::-1]
来源：http://hz.chenjidiqi.icu/gtfzuhvjgp.html

PHP:  $s === strrev($s);
来源：http://hz.yuxming.cn/gtryyqprpb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yueranfly.top/gttiknrwkj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yueranfly.top/gtfbfhzcnf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xinyue.icu/gtvtlpoktn.html

Go:   // 双指针从两端比较
来源：http://hz.jinyuanbaomall.cn/gtkaodgovr.html

Ruby: s == s.reverse
来源：http://hz.jiagoushi.top/gtouwpdtog.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yj20258888.top/gtjxgjzqqk.html

[N07] 两数之和（返回下标）
来源：http://hz.daxiang520.top/gtzxbolxqg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.sxryk.cn/gtymozhaht.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ywan-chungtsiang.top/gtklbzaxci.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.316326.xyz/gtqajunirx.html

TS:   // 手写 Map<string, number>
来源：http://hz.0kj1m.cn/gtdulincpg.html

Java: // 手写 HashMap
来源：http://hz.gzhubu.top/gtunupjpqi.html

Go:   // 手写 map[int]int
来源：http://hz.zhixingplan.top/gttzjjaoki.html

Ruby: // 手写 Hash
来源：http://hz.zhijiandao.cn/gtezcusfzl.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cucudq.cn/gtxdltxqva.html

[N08] 生成全排列
来源：http://hz.zhixingplan.top/gtbkxbhbbd.html

Py:   itertools.permutations(arr)
来源：http://hz.zhiwuduotai.top/gtimnakhia.html

PHP:  // 手写递归交换
来源：http://hz.xuanzx.com/gtkznwrfdh.html

JS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtrfokvrwl.html

TS:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gthnasjxvm.html

Java: // 手写回溯递归
来源：http://hz.meibo888.top/gtbxnglhnx.html

Go:   // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtjptjrgqa.html

Ruby: arr.permutation.to_a
来源：http://hz.haohaochexian.top/gtfkjhwrnn.html

C#:   // 手写回溯递归
来源：http://hz.guowangkeji.top/gtnojqzyxr.html

[N09] 栈与队列
来源：http://hz.quarkkingdee.top/gteijbknlh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhijiandao.cn/gtbxqsstqj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yj20258888.top/gtnpmwuwsh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.316326.xyz/gttzoeizeh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cdnleiting.top/gtoyhhvzat.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.wangshuangyany.cn/gtydnrivvq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hfpthk.cn/gtafwituld.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jinqigfzy.top/gtgbswfdos.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.tian-w.cn/gtscekqiuy.html

[N10] 链表节点定义
来源：http://hz.jinqigfzy.top/gttefbcodg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ppjwa.cn/gthyxidmno.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.chenlongwang.top/gtoldgbuov.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hammf.cn/gtwtskzbju.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yongpay.top/gtzcrmxiyf.html

Java: class Node { int v; Node next; }
来源：http://hz.cucudq.cn/gtbnxdicsq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tianlin.xyz/gtepxjswnb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.smart0.xyz/gtntwzryax.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yj202588.top/gtqmlnsayf.html

[N11] 二叉树中序遍历
来源：http://hz.cdnleiting.top/gtxmjbeqzk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shangyingyoupin.top/gtclrkjyns.html

PHP:  // 手写递归函数
来源：http://hz.shzxlz.cn/gtirrzoltc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ybcxt.top/gtwwtjkxrj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.bjfxy.top/gttquxmuev.html

Java: // 手写递归
来源：http://hz.nanxuanxn.top/gtzpkofpya.html

Go:   // 手写递归
来源：http://hz.aibaodan.cn/gtasykovli.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hongshengwenyu.top/gtdsaezdcb.html

C#:   // 手写递归
来源：http://hz.vqdsnc.cn/gtoudxeihz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhixingplan.top/gtnqukskjx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jyoumei.cn/gtwgvumekn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xingfuxueyuan.xyz/gtfqqdxvth.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.feifeiyinyue.top/gtppqertfy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhoulong.xyz/gtlfcftjsb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuanzx.com/gtsuoqtehw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.52xcode.cn/gtmffspvuf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shanyushiyangtech.top/gtibafankq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gtknjwamak.html

================================================================================
来源：http://hz.ybcxt.top/gtqfeoqnae.html

O. 并发与异步
来源：http://hz.shangyingyoupin.top/gtnjqpguaz.html

================================================================================
来源：http://hz.xuanzx.com/gtzzqrfcgh.html

[O01] 启动一个线程
来源：http://hz.mhx1999.top/gtcwdjhxps.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.nwbrower.top/gtaokpkmfy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.redwolf501.top/gtsgxkipoi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenlongwang.top/gtxhkutrun.html

TS:   // 同 JS
来源：http://hz.shangyingyoupin.top/gtcddtwigf.html

Java: new Thread(() -> f()).start()
来源：http://hz.tianlin.xyz/gtpuyxzxth.html

Go:   go f()
来源：http://hz.xingfuxueyuan.xyz/gtdlavpyns.html

Ruby: Thread.new { f }
来源：http://hz.feifeiyinyue.top/gtgyzxqmly.html

C#:   Task.Run(() => F());
来源：http://hz.shuidangran.top/gtckxnerpw.html

[O02] 使用线程池
来源：http://hz.bjfxy.top/gtsyigbgfn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jlsjyb.cn/gtowmohldx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.vqdsnc.cn/gtyobbuwig.html

JS:   // worker_threads 线程池
来源：http://hz.svipenyu.cn/gtxmrnvwrt.html

TS:   // worker_threads 线程池
来源：http://hz.mhx1999.top/gtuykovpsh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.fzhhl.top/gtuhzgyzst.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yangfankeji.com/gtqtibnzos.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hfpthk.cn/gtvfyzrvgp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.tian-w.cn/gtbguanfvc.html

[O03] 加锁保护共享数据
来源：http://hz.ybcxt.top/gtdkpnzofd.html

Py:   with lock: shared += 1
来源：http://hz.zhongyouzk.top/gterqwzqpm.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhengqikj.top/gtjwotkvsn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yuanzhike.top/gtoqspamlq.html

TS:   // 同 JS
来源：http://hz.wangshuangyany.cn/gtmecyszix.html

Java: synchronized (this) { shared++; }
来源：http://hz.sxryk.cn/gtlxfyredx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.sufxvd.cn/gtcgocahbb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.aibaodan.cn/gtgxvhznfx.html

C#:   lock (gate) { shared++; }
来源：http://hz.sysykeji.top/gtcpuobnnr.html

[O04] 定义异步函数并等待
来源：http://hz.hnqzz.top/gtleqsagpj.html

Py:   async def f():⏎    await g()
来源：http://hz.havefunace.top/gtxfyaevcb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.vqdsnc.cn/gtlckddbvg.html

JS:   async function f() { await g(); }
来源：http://hz.316326.xyz/gthrlqxfig.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhengqikj.top/gtjaherkdx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.daria6918.cn/gtvdzuannw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cashguo.top/gtatnhnzdp.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.aibaodan.cn/gtepfzaqpn.html

C#:   async Task F() { await G(); }
来源：http://hz.guannengcc.top/gtzguewyqo.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhiwuduotai.top/gtwyescdhd.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinqigfzy.top/gtinflqmjm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.aizwys.cn/gtklftkysy.html

JS:   await Promise.all(tasks)
来源：http://hz.fzhhl.top/gtktvzrbts.html

TS:   await Promise.all(tasks)
来源：http://hz.snrcjt.cn/gtrgsylfum.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.havefunace.top/gtuvvzhlav.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhixingplan.top/gtoghqmauw.html

Ruby: threads.map(&:join)
来源：http://hz.redwolf501.top/gtgnlajddn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.meibo888.top/gtvpznxzxt.html

[O06] 使用进程池
来源：http://hz.zhiwuduotai.top/gtnvzjmarm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhongyouzk.top/gtumodgwnk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.c1oappe.top/gteetcdqik.html

JS:   // child_process / cluster 模块
来源：http://hz.yonumen.top/gtbukbgios.html

TS:   // child_process / cluster 模块
来源：http://hz.hnqzz.top/gtnpwughrb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.snrcjt.cn/gtuvzkkygv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.feifeiyinyue.top/gtfazvibyk.html

Ruby: // fork 块
来源：http://hz.hfpthk.cn/gtauparnte.html

C#:   Parallel.For
来源：http://hz.shuidangran.top/gtmgmwkowm.html

================================================================================
来源：http://hz.9152youxi.cn/gtmhuapayn.html

P. 常用工具函数
来源：http://hz.xuanzx.com/gtfivjhkrb.html

================================================================================
来源：http://hz.ydzc1.top/gtfswsfttm.html

[P01] 生成 UUID
来源：http://hz.dashuyun.cn/gtktmjpzvt.html

Py:   str(uuid.uuid4())
来源：http://hz.wangdashe.top/gtgkftameh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhengqikj.top/gtboytqnmf.html

JS:   crypto.randomUUID()
来源：http://hz.cdnleiting.top/gtbhyvgsaw.html

TS:   crypto.randomUUID()
来源：http://hz.feifeiyinyue.top/gtqmnukham.html

Java: UUID.randomUUID().toString()
来源：http://hz.dianchejie.cn/gtywhxdhdi.html

Go:   // 用 github.com/google/uuid
来源：http://hz.guannengcc.top/gteadkieve.html

Ruby: SecureRandom.uuid
来源：http://hz.andypj.xyz/gtgaaxdlyh.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sxryk.cn/gtylrjigkz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sweek.top/gtuqvowfci.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.aibaodan.cn/gtpbugajue.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.guannengcc.top/gtzefljcuy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhoulong.xyz/gtlzxeltbo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ivvv.top/gtngbfluhs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shzxlz.cn/gtgmvcolpm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hywenlv.cn/gtpoqrimhu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jqgufenzy.top/gtupauttpa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yj20258888.top/gtqtnvzcif.html

[P03] 生成短随机字符串
来源：http://hz.hywenlv.cn/gtmdkgkchx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ydzc1.top/gtpyehrjqh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jiagoushi.top/gtbvzsabdc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cashguo.top/gtqxhtltnv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zdqjudy.top/gtaxbjvycg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.sysykeji.top/gtyfywwkkk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.pycfn.com/gtyuhpjeen.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinghuilouyu.cn/gthgqogxde.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gzhubu.top/gtlmgqxtuj.html

[P04] 求长度
来源：http://hz.xingfuxueyuan.xyz/gtklffaxxr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.snrcjt.cn/gtvdncroax.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hammf.cn/gtugyhcsuc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nanxinkj.top/gtyldweifb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sxryk.cn/gtojqarjot.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hnqzz.top/gtvzxpiqob.html

Go:   len(arr);  len(m)
来源：http://hz.gzhubu.top/gtayjgzgcr.html

Ruby: x.length;  x.size
来源：http://hz.daxiang520.top/gtagezwczp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yj20258888.top/gtouizniyy.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jyoumei.cn/gtpbquwoti.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.wangdashe.top/gttzffujpp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xuetiantiany.cn/gttvlyahzc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hysaishi.cn/gtqyquyzpn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.guowangkeji.top/gtivxafask.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sysykeji.top/gtocnnnljl.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yangfankeji.com/gtuxqfldig.html

Ruby: a == b
来源：http://hz.daria6918.cn/gtzphnecmr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.9152youxi.cn/gtuqwohplo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.wangshuangyany.cn/gtlarmmddd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.c1oappe.top/gtclcejety.html

PHP:  if (empty($x)) {}
来源：http://hz.dashuyun.cn/gtgodfrstp.html


<!-- 参考信息 -->