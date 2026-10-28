代发 wailian999

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtwcidetgs.html

[M01] 读取命令行参数
来源：http://hz.havefunace.top/gtabhpqlnv.html

Py:   sys.argv[1:]
来源：http://hz.shanyushiyangtech.top/gtrkybawef.html

PHP:  $argv;  $argc;
来源：http://hz.hfpthk.cn/gtfhqsarku.html

JS:   process.argv.slice(2)
来源：http://hz.gotoacloud.top/gtrdgnrbtp.html

TS:   process.argv.slice(2)
来源：http://hz.wangdashe.top/gtdxeaanvl.html

Java: args 数组（main 方法参数）
来源：http://hz.ivvv.top/gtgcazfkux.html

Go:   os.Args[1:]
来源：http://hz.shzxlz.cn/gtipowuari.html

Ruby: ARGV
来源：http://hz.gogol.net.cn/gttzkyxjym.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xuetiantiany.cn/gtxgmhqqub.html

[M02] 读取环境变量
来源：http://hz.jyoumei.cn/gtwipnxmdy.html

Py:   os.environ.get("HOME")
来源：http://hz.nanxuanxn.top/gtoumiqugo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yongpay.top/gtkixmzwel.html

JS:   process.env.HOME
来源：http://hz.zhoulong.xyz/gtdzanhlbp.html

TS:   process.env.HOME
来源：http://hz.gaohongyu789.top/gtkedgcfwg.html

Java: System.getenv("HOME")
来源：http://hz.shzxlz.cn/gtyhhjtwvl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhengqikj.top/gtrrgphjaz.html

Ruby: ENV["HOME"]
来源：http://hz.316326.xyz/gthcqndqzd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.aizwys.cn/gtktcrnmww.html

[M03] 执行外部命令
来源：http://hz.vqdsnc.cn/gtdacrafwi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.sweek.top/gtvmkqyued.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.aizwys.cn/gtaiudeloi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yvedp.cn/gtrsgxesbz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cucudq.cn/gtdtlfaury.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ppjwa.cn/gtkajckfin.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hysaishi.cn/gtkyrejemn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shzxlz.cn/gtmpidjugc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jlsjyb.cn/gtrkznfwww.html

[M04] 获取当前工作目录
来源：http://hz.nwbrower.top/gtkfywabgk.html

Py:   os.getcwd()
来源：http://hz.dashuyun.cn/gtdbmquemh.html

PHP:  getcwd();
来源：http://hz.hfpthk.cn/gtelsezniz.html

JS:   process.cwd()
来源：http://hz.ivvv.top/gtbsvszxgv.html

TS:   process.cwd()
来源：http://hz.zdqjudy.top/gtmtelukor.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xuetiantiany.cn/gtnotmpucg.html

Go:   os.Getwd()
来源：http://hz.cheryme.top/gtahefivbg.html

Ruby: Dir.pwd
来源：http://hz.ivvv.top/gtqncyincc.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhoulong.xyz/gtzsbiupnu.html

[M05] 设置退出码
来源：http://hz.jqgufenzy.top/gttohexwwt.html

Py:   sys.exit(1)
来源：http://hz.ehwqpu.com/gtwmbtjqhf.html

PHP:  exit(1);
来源：http://hz.316326.xyz/gtdwsikhsi.html

JS:   process.exit(1)
来源：http://hz.jianghu66.top/gtzlcxgsks.html

TS:   process.exit(1)
来源：http://hz.havefunace.top/gtypuhwbst.html

Java: System.exit(1)
来源：http://hz.chenzaomai.com/gtqvfwtkro.html

Go:   os.Exit(1)
来源：http://hz.yuxming.cn/gthlxkfqaj.html

Ruby: exit 1
来源：http://hz.gotoacloud.top/gtffwrsduc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.chenjidiqi.icu/gtxqivqizy.html

[M06] 向标准错误输出
来源：http://hz.sxryk.cn/gtwplweubh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.aizwys.cn/gtlsffqmpw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xinyue.icu/gtailfsoys.html

JS:   console.error("err")
来源：http://hz.meibo888.top/gtoinvogtk.html

TS:   console.error("err")
来源：http://hz.nanxinkj.top/gtbtstpzay.html

Java: System.err.println("err")
来源：http://hz.aizwys.cn/gtowofbpwq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sweek.top/gtjoynjldq.html

Ruby: warn "err"
来源：http://hz.jinqigufen.top/gtnjodgmdy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.aibaodan.cn/gtolrlejgp.html

[M07] 判断是否为主入口
来源：http://hz.yj20258888.top/gttecqdovs.html

Py:   if __name__ == "__main__":
来源：http://hz.cqqwz.cn/gtykxoxeuq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.haohaochexian.top/gtahcvvkwf.html

JS:   require.main === module
来源：http://hz.fengsongda.top/gtkdldcosi.html

TS:   require.main === module
来源：http://hz.tanke756.top/gtijeyjkzl.html

Java: public static void main(String[] args)
来源：http://hz.nwbrower.top/gthusdkfye.html

Go:   func main()
来源：http://hz.hfpthk.cn/gtzeoqimti.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.svipenyu.cn/gthyfbnxsb.html

C#:   static void Main(string[] args)
来源：http://hz.sweek.top/gtrzgnuxjl.html

[M08] 获取系统与运行时信息
来源：http://hz.ydzc1.top/gtosfcriww.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yonumen.top/gtgcdpcanh.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hongshengwenyu.top/gtcbnhotva.html

JS:   process.platform;  process.version
来源：http://hz.shanyushiyangtech.top/gtkhtiqgzg.html

TS:   process.platform;  process.version
来源：http://hz.yuanzhike.top/gthfqoezmy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tian-w.cn/gtglypsgmg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yonumen.top/gtzktusrkc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.quarkkingdee.top/gtbghgbcsk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnqzz.top/gtuiwordww.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtnvotimwy.html

N. 数据结构与算法
来源：http://hz.9152youxi.cn/gtnuaososo.html

================================================================================
来源：http://hz.sufxvd.cn/gtodprnkvd.html

[N01] 二分查找（有序数组）
来源：http://hz.iojbl.cn/gtgozixirp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.kuanghao11.cn/gtxduwmrte.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.tanke756.top/gtumtapsdt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhiwuduotai.top/gteceloges.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sweek.top/gtgyzuimcm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.quarkkingdee.top/gtnpsnluxl.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.sweek.top/gtaigkasoy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.snrcjt.cn/gtcqavypyd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nanxuanxn.top/gtqlvrsuix.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.tianlin.xyz/gtlkxqvznh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cucudq.cn/gtbzpaswwv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yonumen.top/gtwaytfjeg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangkeji.top/gtvyzwjxcv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zdqjudy.top/gtuelxcwil.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.dashuyun.cn/gtwppjexnc.html

Go:   slices.Sort(arr)
来源：http://hz.gzhubu.top/gtnnnafjna.html

Ruby: arr.sort
来源：http://hz.cheryme.top/gtflzoaazi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinqigufen.top/gtvhqxvogo.html

[N03] 快速排序（分治示例）
来源：http://hz.guowangkeji.top/gthbehbqxs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jyoumei.cn/gtjzlpwlci.html

PHP:  // 递归实现，或用 usort
来源：http://hz.aizwys.cn/gtgfwsqxro.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cashguo.top/gtrofelujl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sysykeji.top/gtobsbpmko.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhoulong.xyz/gtqsukydgh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.guowangkeji.top/gtfitmmpep.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.nwbrower.top/gtujjmeabz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.quarkkingdee.top/gtjtozhiqc.html

[N04] 斐波那契数列
来源：http://hz.zhoulong.xyz/gtzyzmthei.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.meibo888.top/gtgxuppxkb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.kuanghao11.cn/gtpkmfpkjc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.snrcjt.cn/gtdypchotd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aizwys.cn/gtmuianycw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.fzhhl.top/gtyvsmifgc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hysaishi.cn/gtunhokzyn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigufen.top/gtxpfdxwgt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.0kj1m.cn/gtqdmmcvwq.html

[N05] 最大公约数
来源：http://hz.kuanghao11.cn/gtnlvthcfx.html

Py:   math.gcd(a, b)
来源：http://hz.ydzc1.top/gttihtglnc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.wangdashe.top/gtgyygwapy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ehwqpu.com/gtwtcdjymv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.quarkkingdee.top/gtcagcznyv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xinyue.icu/gtbrpklizv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.tianlin.xyz/gtkwpaqvyc.html

Ruby: a.gcd(b)
来源：http://hz.gogol.net.cn/gtzyxvaoaw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.vqdsnc.cn/gtxmkwknlq.html

[N06] 判断回文字符串
来源：http://hz.tanke756.top/gtwpevllhu.html

Py:   s == s[::-1]
来源：http://hz.yj20258.top/gtoyibdomf.html

PHP:  $s === strrev($s);
来源：http://hz.daria6918.cn/gtyefdhbil.html

JS:   s === [...s].reverse().join("")
来源：http://hz.daxiang520.top/gtjoedjhhj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtiygmyhfk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.nwbrower.top/gtfkkupzxj.html

Go:   // 双指针从两端比较
来源：http://hz.feifeiyinyue.top/gtupxwszws.html

Ruby: s == s.reverse
来源：http://hz.shzxlz.cn/gtdpzjnpyk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinyuanbaomall.cn/gtnknbggwu.html

[N07] 两数之和（返回下标）
来源：http://hz.dashuyun.cn/gtzkvitegt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.daria6918.cn/gtcvljndgc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jyoumei.cn/gtwzsxhfoo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.snrcjt.cn/gtbdbckwsl.html

TS:   // 手写 Map<string, number>
来源：http://hz.ydzc1.top/gttbcfclro.html

Java: // 手写 HashMap
来源：http://hz.zhijiandao.cn/gtdsffyiyn.html

Go:   // 手写 map[int]int
来源：http://hz.tian-w.cn/gtrzqputoa.html

Ruby: // 手写 Hash
来源：http://hz.birdmap.top/gtwajmyfwl.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.tianlin.xyz/gtjockgjmr.html

[N08] 生成全排列
来源：http://hz.zhaomingkeji.xyz/gtdbscqomc.html

Py:   itertools.permutations(arr)
来源：http://hz.gogol.net.cn/gtiocoogvo.html

PHP:  // 手写递归交换
来源：http://hz.hammf.cn/gtztswkmvm.html

JS:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtypjjbsxw.html

TS:   // 手写回溯递归
来源：http://hz.hammf.cn/gtbewhcxsb.html

Java: // 手写回溯递归
来源：http://hz.yj20258.top/gtxrtngady.html

Go:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtfaqqawka.html

Ruby: arr.permutation.to_a
来源：http://hz.zhiwuduotai.top/gtddawgkxu.html

C#:   // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gtxjephlwc.html

[N09] 栈与队列
来源：http://hz.hnqzz.top/gtqlnisroi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.tian-w.cn/gtvjxrdinc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.daria6918.cn/gtmtfernbk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.svipenyu.cn/gtsuyfpapw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhiwuduotai.top/gtcwzpfrzi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.dianchejie.cn/gtjkxweerk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.chenlongwang.top/gtzkhmdubh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jiagoushi.top/gtfnzqmmun.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.feifeiyinyue.top/gtkhoqkasp.html

[N10] 链表节点定义
来源：http://hz.aibaodan.cn/gtbbesxiws.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cqqwz.cn/gtrvxehirm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shuidangran.top/gtlvglymze.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jiagoushi.top/gtgscjbmos.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.0kj1m.cn/gtrjndrfdl.html

Java: class Node { int v; Node next; }
来源：http://hz.zhongyouzk.top/gtjcekcsos.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.havefunace.top/gtquxkidcu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yonumen.top/gthoewmouy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.feifeiyinyue.top/gtmvwnkeil.html

[N11] 二叉树中序遍历
来源：http://hz.smart0.xyz/gtaxsvlete.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.0kj1m.cn/gtsaszejct.html

PHP:  // 手写递归函数
来源：http://hz.sweek.top/gtkdrubxsc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yvedp.cn/gtfmaylpoo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gzhubu.top/gtrxmjfxmd.html

Java: // 手写递归
来源：http://hz.ybcxt.top/gtgmqwfuqp.html

Go:   // 手写递归
来源：http://hz.ydzc1.top/gtqmgkzjcq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ehwqpu.com/gtvcrsyjwd.html

C#:   // 手写递归
来源：http://hz.yuxming.cn/gtydatmgck.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shangyingyoupin.top/gtxvbrucmr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.9152youxi.cn/gtqtzfhfrp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hywenlv.cn/gtkqzzhlzg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gotoacloud.top/gtyuotxakj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gzhubu.top/gtjqjzddgh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangkeji.top/gtdtenprmm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenlongwang.top/gtzlfgxtuc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yj20258888.top/gtdhdmuakp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yanxiufei.cn/gtafisllim.html

================================================================================
来源：http://hz.aibaodan.cn/gtpyorixlk.html

O. 并发与异步
来源：http://hz.wangdashe.top/gtydqzklxs.html

================================================================================
来源：http://hz.zhijiandao.cn/gtzzfhutef.html

[O01] 启动一个线程
来源：http://hz.aizwys.cn/gtpemtudsz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.dianchejie.cn/gtpuokdeyj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.mhx1999.top/gtnvpmtsdy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hywenlv.cn/gtjxskdill.html

TS:   // 同 JS
来源：http://hz.sxryk.cn/gtoremccth.html

Java: new Thread(() -> f()).start()
来源：http://hz.pycfn.com/gtrcutsgne.html

Go:   go f()
来源：http://hz.zhongyouzk.top/gtreimaxvr.html

Ruby: Thread.new { f }
来源：http://hz.ywan-chungtsiang.top/gtokfulcqk.html

C#:   Task.Run(() => F());
来源：http://hz.snrcjt.cn/gtbbgrrsqg.html

[O02] 使用线程池
来源：http://hz.zhengqikj.top/gtzehumkhd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.tanke756.top/gtyvskmbnm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.havefunace.top/gtcezbumcv.html

JS:   // worker_threads 线程池
来源：http://hz.hysaishi.cn/gteluhyqzs.html

TS:   // worker_threads 线程池
来源：http://hz.dianchejie.cn/gthnoswfwb.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zycfv.cn/gtienoobbl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xziqi.cn/gtcitjixmo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gzhubu.top/gtoodlydmo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jiagoushi.top/gtdqucpmag.html

[O03] 加锁保护共享数据
来源：http://hz.ivvv.top/gtwgyjtcjz.html

Py:   with lock: shared += 1
来源：http://hz.tian-w.cn/gtrtqevxfk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yonumen.top/gtzgbrihvl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yuxming.cn/gteffkgfwa.html

TS:   // 同 JS
来源：http://hz.dashuyun.cn/gtjlsusmck.html

Java: synchronized (this) { shared++; }
来源：http://hz.wangdashe.top/gtwaswnuka.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.svipenyu.cn/gtkiulpizw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.316326.xyz/gtiiidduoo.html

C#:   lock (gate) { shared++; }
来源：http://hz.kuanghao11.cn/gtbkmffmhi.html

[O04] 定义异步函数并等待
来源：http://hz.xingfuxueyuan.xyz/gtevjqtdcm.html

Py:   async def f():⏎    await g()
来源：http://hz.nanxuanxn.top/gtybldrkya.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.chenzaomai.com/gtzyfyvtth.html

JS:   async function f() { await g(); }
来源：http://hz.ydzc1.top/gtcsjengfo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jinyuanbaomall.cn/gtvdpjyefr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xylfe.cn/gtzatvdbey.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yj20258888.top/gtwmqofjkz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ivvv.top/gtxkahouss.html

C#:   async Task F() { await G(); }
来源：http://hz.52xcode.cn/gthmvgmxkr.html

[O05] 并发执行并等待全部完成
来源：http://hz.birdmap.top/gtbgdkjodb.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yj20258.top/gtakiuvscn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.pengpengdd.cyou/gtlwgfxvyf.html

JS:   await Promise.all(tasks)
来源：http://hz.gaohongyu789.top/gtdahgmchk.html

TS:   await Promise.all(tasks)
来源：http://hz.hfpthk.cn/gtxzandhqj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xinyue.icu/gtcydteush.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cheryme.top/gtiihrilhi.html

Ruby: threads.map(&:join)
来源：http://hz.yvedp.cn/gtcyyluwmu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.quarkkingdee.top/gtvdrfdbwv.html

[O06] 使用进程池
来源：http://hz.yongpay.top/gtslkesmwm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xuetiantiany.cn/gtxbaktsfs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.52xcode.cn/gtwptiagmk.html

JS:   // child_process / cluster 模块
来源：http://hz.hfpthk.cn/gtrqzwnmyc.html

TS:   // child_process / cluster 模块
来源：http://hz.jyoumei.cn/gtmbpjtpsn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.guowangkeji.top/gthshtcbxr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.aibaodan.cn/gttkezxgjm.html

Ruby: // fork 块
来源：http://hz.c1oappe.top/gtzmewspuv.html

C#:   Parallel.For
来源：http://hz.gogol.net.cn/gtveywjrvq.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtfukbyxym.html

P. 常用工具函数
来源：http://hz.quarkkingdee.top/gtfxncohxo.html

================================================================================
来源：http://hz.ivvv.top/gtjnfgdckh.html

[P01] 生成 UUID
来源：http://hz.jlsjyb.cn/gtnwhitbve.html

Py:   str(uuid.uuid4())
来源：http://hz.gzhubu.top/gtnhebmwwt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cashguo.top/gtrzstthdv.html

JS:   crypto.randomUUID()
来源：http://hz.jinyuanbaomall.cn/gtvcsayvtq.html

TS:   crypto.randomUUID()
来源：http://hz.zhongyouzk.top/gtvqqwfjqt.html

Java: UUID.randomUUID().toString()
来源：http://hz.meibo888.top/gtsfatkgqd.html

Go:   // 用 github.com/google/uuid
来源：http://hz.0kj1m.cn/gtuissaihi.html

Ruby: SecureRandom.uuid
来源：http://hz.meibo888.top/gtbndzqilp.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xziqi.cn/gtcvizmuhx.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zycfv.cn/gtarcsjuza.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jinyuanbaomall.cn/gtqhejmxus.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.aibaodan.cn/gtihyyqwvz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.daxiang520.top/gtsbqhnozo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yuanzhike.top/gtpxmspans.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jlsjyb.cn/gtiiarsika.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.9152youxi.cn/gtelydvmwd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jqgfzy.top/gtnqbjcznw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ydjk.org.cn/gtuqtgygjk.html

[P03] 生成短随机字符串
来源：http://hz.yonumen.top/gtudbhzblm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.chenzaomai.com/gtzylvvwml.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.daxiang520.top/gtswrkvfrx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cqqwz.cn/gtnbyxrblw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ppjwa.cn/gtpaxqprsw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yj202588.top/gtgladwnqh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.9152youxi.cn/gtzlniolgo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yuxming.cn/gtuuulxqvz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yongpay.top/gtygclrgrf.html

[P04] 求长度
来源：http://hz.pycfn.com/gtwpdfhcio.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jinyuanbaomall.cn/gtuthxuizj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aizwys.cn/gthyttevyh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shanyushiyangtech.top/gtjtlimewy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hysaishi.cn/gteogqyuum.html

Java: list.size();  map.size();  s.length()
来源：http://hz.aibaodan.cn/gthqlwavhs.html

Go:   len(arr);  len(m)
来源：http://hz.nanxuanxn.top/gtkrtohzyv.html

Ruby: x.length;  x.size
来源：http://hz.snrcjt.cn/gtqwsfhfcv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hammf.cn/gtwdohszhm.html

[P05] 判断两个对象内容是否相等
来源：http://hz.chenlongwang.top/gtmuqevhrc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.redwolf501.top/gtxkyzxlvh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.haohaochexian.top/gteibjzijs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.redwolf501.top/gtuuwqzggq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yvedp.cn/gteanxrgbr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.daria6918.cn/gthgwtraet.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shanyushiyangkeji.top/gtxveydlbg.html

Ruby: a == b
来源：http://hz.gogol.net.cn/gtlnbyroci.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.sweek.top/gtgbzwrsqj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hysaishi.cn/gtdpumhyez.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.daxiang520.top/gtqwqzlsdp.html

PHP:  if (empty($x)) {}
来源：http://hz.nanxinkj.top/gtcdmbxmom.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hywenlv.cn/gtxyvsscwa.html

TS:   if (x == null) {}
来源：http://hz.pycfn.com/gtjbvsheap.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xuanzx.com/gtbqziurkn.html

Go:   if x == nil {}
来源：http://hz.birdmap.top/gtvfczpujj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.quarkkingdee.top/gtzohztaql.html

C#:   if (x is null) {}
来源：http://hz.gzhubu.top/gteybvbxat.html

[P07] 防抖与节流
来源：http://hz.ppjwa.cn/gtzbeknwqo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ydzc1.top/gtbibljsvf.html


<!-- 参考信息 -->