代发 wailian999

================================================================================
来源：http://hz.xuetiantiany.cn/gtpdxndzub.html

[M01] 读取命令行参数
来源：http://hz.shuidangran.top/gtqfobevai.html

Py:   sys.argv[1:]
来源：http://hz.guowangkeji.top/gtodejrksx.html

PHP:  $argv;  $argc;
来源：http://hz.xinyue.icu/gtyfkmfdft.html

JS:   process.argv.slice(2)
来源：http://hz.hongshengwenyu.top/gttroxnqef.html

TS:   process.argv.slice(2)
来源：http://hz.xingfuxueyuan.xyz/gtciojsryt.html

Java: args 数组（main 方法参数）
来源：http://hz.zhengqikj.top/gtjuqyymen.html

Go:   os.Args[1:]
来源：http://hz.pengpengdd.cyou/gtbwfjzoiq.html

Ruby: ARGV
来源：http://hz.zhongyouzk.top/gtpeitzonu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jyoumei.cn/gtmelvrqmy.html

[M02] 读取环境变量
来源：http://hz.xinyue.icu/gtdtmxwvae.html

Py:   os.environ.get("HOME")
来源：http://hz.pengpengdd.cyou/gthenmzrfr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ydjk.org.cn/gtddckhqbw.html

JS:   process.env.HOME
来源：http://hz.yj20258.top/gtrjfnnqgc.html

TS:   process.env.HOME
来源：http://hz.zhaomingkeji.xyz/gtqzruvhsh.html

Java: System.getenv("HOME")
来源：http://hz.daxiang520.top/gtctwqcade.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.tianlin.xyz/gtayaniina.html

Ruby: ENV["HOME"]
来源：http://hz.xylfe.cn/gtppjpujsf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xinyue.icu/gtycluwvef.html

[M03] 执行外部命令
来源：http://hz.hnxiangtu.top/gtnnggogbo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.chenlongwang.top/gtjlbjofcg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.wangshuangyany.cn/gtwhakfawq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.daria6918.cn/gtbphoceth.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gotoacloud.top/gtwjesiqqz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.gaohongyu789.top/gtovymdjqj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hongshengwenyu.top/gtxhlkvfjt.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shangyingyoupin.top/gtcckujpzi.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sufxvd.cn/gtoylmqksq.html

[M04] 获取当前工作目录
来源：http://hz.dianchejie.cn/gtsgkjneme.html

Py:   os.getcwd()
来源：http://hz.sweek.top/gtvhkclbuu.html

PHP:  getcwd();
来源：http://hz.xingfuxueyuan.xyz/gtrsaefzyw.html

JS:   process.cwd()
来源：http://hz.pycfn.com/gtsdfknqna.html

TS:   process.cwd()
来源：http://hz.9152youxi.cn/gtpjolazpe.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yvedp.cn/gtiqsflpng.html

Go:   os.Getwd()
来源：http://hz.hnxiangtu.top/gtditwspex.html

Ruby: Dir.pwd
来源：http://hz.yueranfly.top/gttxnkpclr.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.havefunace.top/gtizqwummu.html

[M05] 设置退出码
来源：http://hz.gzhubu.top/gtcqlqubqn.html

Py:   sys.exit(1)
来源：http://hz.cdnleiting.top/gtkqfkjdfq.html

PHP:  exit(1);
来源：http://hz.fengsongda.top/gtxbzddtns.html

JS:   process.exit(1)
来源：http://hz.zhaomingkeji.xyz/gtkgsvcpyp.html

TS:   process.exit(1)
来源：http://hz.jlsjyb.cn/gtkigarbmz.html

Java: System.exit(1)
来源：http://hz.xziqi.cn/gtmbjsizpd.html

Go:   os.Exit(1)
来源：http://hz.zhixingplan.top/gtibrxsviu.html

Ruby: exit 1
来源：http://hz.yonumen.top/gtrbonfawi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhaomingkeji.xyz/gtctzboscv.html

[M06] 向标准错误输出
来源：http://hz.gotoacloud.top/gtbwrzsase.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sxryk.cn/gteyilgpim.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.0kj1m.cn/gtqkouechq.html

JS:   console.error("err")
来源：http://hz.zhixingplan.top/gtztrmgixc.html

TS:   console.error("err")
来源：http://hz.wangshuangyany.cn/gtfqcausmi.html

Java: System.err.println("err")
来源：http://hz.jinyuanbaomall.cn/gtyoiskkez.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gaohongyu789.top/gtuacqepyg.html

Ruby: warn "err"
来源：http://hz.gotoacloud.top/gtmehjhupg.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hnxiangtu.top/gtppsgetvp.html

[M07] 判断是否为主入口
来源：http://hz.gotoacloud.top/gtdngdkzpx.html

Py:   if __name__ == "__main__":
来源：http://hz.gotoacloud.top/gtxcjsqvkx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gogol.net.cn/gtgvzhxbhe.html

JS:   require.main === module
来源：http://hz.hongshengwenyu.top/gttcmvmaew.html

TS:   require.main === module
来源：http://hz.ybcxt.top/gtcawigrtr.html

Java: public static void main(String[] args)
来源：http://hz.pycfn.com/gtqqnjzmaj.html

Go:   func main()
来源：http://hz.zhixingplan.top/gtjjlzcjpi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yonumen.top/gtujjccqvv.html

C#:   static void Main(string[] args)
来源：http://hz.xziqi.cn/gtezxahgao.html

[M08] 获取系统与运行时信息
来源：http://hz.jianghu66.top/gtoajqcbry.html

Py:   platform.system();  platform.python_version()
来源：http://hz.chenlongwang.top/gtvfaxghmo.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jinghuilouyu.cn/gtiiifkxnb.html

JS:   process.platform;  process.version
来源：http://hz.aibaodan.cn/gttiuxxqsd.html

TS:   process.platform;  process.version
来源：http://hz.bjfxy.top/gtpwazosla.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hammf.cn/gtstovhuzo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yj20258.top/gtgevpsgan.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cucudq.cn/gtuqsdiyyw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.dianchejie.cn/gtckmcltwf.html

================================================================================
来源：http://hz.daria6918.cn/gtzhngxnde.html

N. 数据结构与算法
来源：http://hz.gzhubu.top/gtsdzbntkw.html

================================================================================
来源：http://hz.hnxiangtu.top/gtftpzeijt.html

[N01] 二分查找（有序数组）
来源：http://hz.316326.xyz/gtpypzqobd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.aibaodan.cn/gtwgsrerjy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hammf.cn/gtbwblxzmo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenzaomai.com/gtcucxrjno.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jlsjyb.cn/gtyhskdfqn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gaohongyu789.top/gtcxmqdhay.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtwzkivhqs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhengqikj.top/gtadtgqorx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yj20258888.top/gthtogewst.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jinyuanbaomall.cn/gtcswaaelz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yuanzhike.top/gtqkmosdjy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.guowangkeji.top/gtsfgnjkzo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gzhubu.top/gtkwldrlmk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gzhubu.top/gttssyyqsy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xziqi.cn/gtervxpvxo.html

Go:   slices.Sort(arr)
来源：http://hz.dianchejie.cn/gtkdfmheti.html

Ruby: arr.sort
来源：http://hz.xingfuxueyuan.xyz/gtkbylgixo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.daria6918.cn/gtaertknay.html

[N03] 快速排序（分治示例）
来源：http://hz.hysaishi.cn/gtetkdiuzq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gogol.net.cn/gtwslnltgj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hnqzz.top/gtanvbnuuu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.birdmap.top/gthuigvygf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhaomingkeji.xyz/gtsfzzphhi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.vqdsnc.cn/gtkaiwodve.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.aizwys.cn/gtoypvtfef.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zycfv.cn/gtsfjrpmdf.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ydzc1.top/gttbnzrjlu.html

[N04] 斐波那契数列
来源：http://hz.pengpengdd.cyou/gtrjydlxja.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yongpay.top/gtjmmighqg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinqigfzy.top/gtuoalutgn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xziqi.cn/gtafkjlqzs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sufxvd.cn/gtwqsmmvjg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.kuanghao11.cn/gtjmuqykbl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yuanzhike.top/gtogzezoub.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.haohaochexian.top/gtmpvjmfyn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gtugwdifrh.html

[N05] 最大公约数
来源：http://hz.nwbrower.top/gtppnaclpa.html

Py:   math.gcd(a, b)
来源：http://hz.snrcjt.cn/gtjtgwyjxa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zycfv.cn/gtbdprqael.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.andypj.xyz/gtzojopker.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhaomingkeji.xyz/gtmuvdlrld.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hysaishi.cn/gtmvybdssn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.wangshuangyany.cn/gtlnqdegdx.html

Ruby: a.gcd(b)
来源：http://hz.ydzc1.top/gtadluwszr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shuidangran.top/gttnwosryh.html

[N06] 判断回文字符串
来源：http://hz.xuanzx.com/gtmzbfpuwz.html

Py:   s == s[::-1]
来源：http://hz.cucudq.cn/gtxpxprpcj.html

PHP:  $s === strrev($s);
来源：http://hz.shangyingyoupin.top/gtoobdknzu.html

JS:   s === [...s].reverse().join("")
来源：http://hz.guowangkeji.top/gtlgsfxala.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hammf.cn/gtbgpkwyot.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.svipenyu.cn/gtpjwhuoje.html

Go:   // 双指针从两端比较
来源：http://hz.ydzc1.top/gtrfnfeyen.html

Ruby: s == s.reverse
来源：http://hz.jinghuilouyu.cn/gtpfaqolnl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhaomingkeji.xyz/gtzajhbuud.html

[N07] 两数之和（返回下标）
来源：http://hz.hywenlv.cn/gtrohokjbf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.sufxvd.cn/gtztrbdsrk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.tianlin.xyz/gtcicftqlb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.feifeiyinyue.top/gtixncqppg.html

TS:   // 手写 Map<string, number>
来源：http://hz.fengsongda.top/gteuwvjfjt.html

Java: // 手写 HashMap
来源：http://hz.tian-w.cn/gtpqoisfxq.html

Go:   // 手写 map[int]int
来源：http://hz.sufxvd.cn/gtsonipxvb.html

Ruby: // 手写 Hash
来源：http://hz.fzhhl.top/gtudjelcxq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.dianchejie.cn/gtpugdezpo.html

[N08] 生成全排列
来源：http://hz.guowangkeji.top/gtcqlhkyyd.html

Py:   itertools.permutations(arr)
来源：http://hz.xinyue.icu/gtfcmxmmbs.html

PHP:  // 手写递归交换
来源：http://hz.yongpay.top/gtovvyvupd.html

JS:   // 手写回溯递归
来源：http://hz.tianlin.xyz/gtkhqnwecu.html

TS:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtgolkjddx.html

Java: // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtpgpjfrwo.html

Go:   // 手写回溯递归
来源：http://hz.redwolf501.top/gtrdlkioaz.html

Ruby: arr.permutation.to_a
来源：http://hz.vqdsnc.cn/gtbygmmpvw.html

C#:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtdjgpkbrs.html

[N09] 栈与队列
来源：http://hz.zhaomingkeji.xyz/gtelhbsmpn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jianghu66.top/gtqpgscbhy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xinyue.icu/gtcletndyn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhongyouzk.top/gtithlhplw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ywan-chungtsiang.top/gtwomhyqkm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hfpthk.cn/gtsnokbkjk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.9152youxi.cn/gtifwrtcvk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sxryk.cn/gtpxzmfeeu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.daria6918.cn/gtgbpaqlzc.html

[N10] 链表节点定义
来源：http://hz.hammf.cn/gtylgqylfw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.bjfxy.top/gtcqboniij.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinghuilouyu.cn/gtmmkewfdy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hnxiangtu.top/gtltbhlere.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jianghu66.top/gtqohmfmlk.html

Java: class Node { int v; Node next; }
来源：http://hz.zhijiandao.cn/gtqjbfczgi.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.bjfxy.top/gtwdztvrlv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ppjwa.cn/gthzizcngh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhengqikj.top/gtsxucqipl.html

[N11] 二叉树中序遍历
来源：http://hz.shanyushiyangkeji.top/gtbgoqeqei.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.fzhhl.top/gtdeeboreb.html

PHP:  // 手写递归函数
来源：http://hz.sxryk.cn/gtedmbldyi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.meibo888.top/gtemiguqtm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yongpay.top/gtdhdrghru.html

Java: // 手写递归
来源：http://hz.chenjidiqi.icu/gttlwdwtil.html

Go:   // 手写递归
来源：http://hz.hysaishi.cn/gtbqvphqqf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.chenzaomai.com/gtdonkhjsh.html

C#:   // 手写递归
来源：http://hz.yj20258.top/gtczaiyacl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhongyouzk.top/gtrkgkjeaq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.redwolf501.top/gtmuwozvzk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zycfv.cn/gtrrijaacg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jiagoushi.top/gtkenfnbfx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258888.top/gtlzbubhii.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sxryk.cn/gtgkmtgkjd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xingfuxueyuan.xyz/gtanxcgaph.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinqigufen.top/gtgudxsgpq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cheryme.top/gtfqsbnmxl.html

================================================================================
来源：http://hz.yj202588.top/gtvumducvd.html

O. 并发与异步
来源：http://hz.smart0.xyz/gtjgroixwd.html

================================================================================
来源：http://hz.fengsongda.top/gtxnmbrpcl.html

[O01] 启动一个线程
来源：http://hz.ppjwa.cn/gtxqrkdqnu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ppjwa.cn/gtnxfesdtz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xuanzx.com/gtlmfuuqhb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.shanyushiyangtech.top/gtgnpxopfu.html

TS:   // 同 JS
来源：http://hz.yanxiufei.cn/gtbdhxhaac.html

Java: new Thread(() -> f()).start()
来源：http://hz.ehwqpu.com/gttgbonnnc.html

Go:   go f()
来源：http://hz.chenlongwang.top/gtcljmzuix.html

Ruby: Thread.new { f }
来源：http://hz.nanxuanxn.top/gtpfclhrlh.html

C#:   Task.Run(() => F());
来源：http://hz.0kj1m.cn/gtheelycbz.html

[O02] 使用线程池
来源：http://hz.nanxuanxn.top/gtmvjqypep.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xylfe.cn/gtgzfhfbpl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.gotoacloud.top/gtilanmllh.html

JS:   // worker_threads 线程池
来源：http://hz.jinqigufen.top/gtyjzvelzb.html

TS:   // worker_threads 线程池
来源：http://hz.jqgufenzy.top/gtwluprjot.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yanxiufei.cn/gtuulumlwd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.wangdashe.top/gtughbdvcy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shzxlz.cn/gtgmtlwnqo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xingfuxueyuan.xyz/gtiblkywkv.html

[O03] 加锁保护共享数据
来源：http://hz.iojbl.cn/gtdvwxzgxt.html

Py:   with lock: shared += 1
来源：http://hz.jqgufenzy.top/gtukgveeck.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shanyushiyangkeji.top/gtmeenvdus.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.mhx1999.top/gttcgnuxef.html

TS:   // 同 JS
来源：http://hz.wangshuangyany.cn/gtvcndmdkh.html

Java: synchronized (this) { shared++; }
来源：http://hz.yangfankeji.com/gtpasdxdat.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jiagoushi.top/gtlowxvupa.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.daxiang520.top/gtmmhidmgd.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj20258888.top/gtilojnoux.html

[O04] 定义异步函数并等待
来源：http://hz.shanyushiyangkeji.top/gtgsjzpnjz.html

Py:   async def f():⏎    await g()
来源：http://hz.cheryme.top/gttadxxvzn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hnqzz.top/gtnqtgqmjs.html

JS:   async function f() { await g(); }
来源：http://hz.haohaochexian.top/gtbkhmbxms.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhengqikj.top/gtwoqmueag.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gotoacloud.top/gtouojowat.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.chenjidiqi.icu/gtdzlkggjh.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xinyue.icu/gtzpfxbwkj.html

C#:   async Task F() { await G(); }
来源：http://hz.tian-w.cn/gtnnvjuujx.html

[O05] 并发执行并等待全部完成
来源：http://hz.xingfuxueyuan.xyz/gtvbkdnsjq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhengqikj.top/gtumnkvukl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yj20258.top/gtzzjukezv.html

JS:   await Promise.all(tasks)
来源：http://hz.meibo888.top/gtkkrirano.html

TS:   await Promise.all(tasks)
来源：http://hz.hywenlv.cn/gtbezxylkr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.andypj.xyz/gtmgsfwapg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhiwuduotai.top/gtwbynbzht.html

Ruby: threads.map(&:join)
来源：http://hz.nanxuanxn.top/gtqyavlxoz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinyuanbaomall.cn/gtznoojbny.html

[O06] 使用进程池
来源：http://hz.sufxvd.cn/gtciwehqmj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jqgufenzy.top/gtqwnhzlpe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.smart0.xyz/gtmrxybnak.html

JS:   // child_process / cluster 模块
来源：http://hz.tian-w.cn/gtbpxoyszc.html

TS:   // child_process / cluster 模块
来源：http://hz.daria6918.cn/gttewyrdwg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.316326.xyz/gthevvhfaf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.tianlin.xyz/gtxpxxknzt.html

Ruby: // fork 块
来源：http://hz.c1oappe.top/gtfspwbszn.html

C#:   Parallel.For
来源：http://hz.sweek.top/gtxhxvwuwb.html

================================================================================
来源：http://hz.yueranfly.top/gtshhxwbex.html

P. 常用工具函数
来源：http://hz.xinyue.icu/gtbpifwoub.html

================================================================================
来源：http://hz.fengsongda.top/gtamqqigos.html

[P01] 生成 UUID
来源：http://hz.jianghu66.top/gtsqifjhrj.html

Py:   str(uuid.uuid4())
来源：http://hz.ydzc1.top/gteibpmfdt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shanyushiyangtech.top/gtyvgahggx.html

JS:   crypto.randomUUID()
来源：http://hz.xziqi.cn/gtfngcwjzn.html

TS:   crypto.randomUUID()
来源：http://hz.cucudq.cn/gtcwkwvhhr.html

Java: UUID.randomUUID().toString()
来源：http://hz.xylfe.cn/gtsodvvlli.html

Go:   // 用 github.com/google/uuid
来源：http://hz.wangdashe.top/gtikfygfqh.html

Ruby: SecureRandom.uuid
来源：http://hz.zycfv.cn/gtmwvhvapm.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.guowangkeji.top/gtaibspoya.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jlsjyb.cn/gtofvkiurj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.0kj1m.cn/gtwprepetl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.iojbl.cn/gtuwohrupy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.bjfxy.top/gtyrunqbis.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.svipenyu.cn/gtryjmsfat.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhaomingkeji.xyz/gtztsnanyi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.pengpengdd.cyou/gtpcwlbnhy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cheryme.top/gtqywpcikb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yueranfly.top/gtvlrhnxpu.html

[P03] 生成短随机字符串
来源：http://hz.sxryk.cn/gthjjlgmqs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cdnleiting.top/gtpgijtbnn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.guowangkeji.top/gtbpraiong.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenlongwang.top/gtcddsunzo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gotoacloud.top/gtsabrllrn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.guowangkeji.top/gtufwitwhg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.fzhhl.top/gtbmhhdnbk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sufxvd.cn/gtcbvzurte.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhoulong.xyz/gtxxxffnzl.html

[P04] 求长度
来源：http://hz.jinqigfzy.top/gtndicrgmx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cdnleiting.top/gtksawycox.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.bjfxy.top/gtrilkshhg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinqigufen.top/gtejimvohv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fengsongda.top/gtbxbibera.html

Java: list.size();  map.size();  s.length()
来源：http://hz.pengpengdd.cyou/gtpdkrisvz.html

Go:   len(arr);  len(m)
来源：http://hz.hnxiangtu.top/gtrgdpjcsh.html

Ruby: x.length;  x.size
来源：http://hz.zycfv.cn/gtqqdeqzhb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.redwolf501.top/gtabliauvq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xinyue.icu/gtlkdqrqxr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.kuanghao11.cn/gtwnmaorzr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.tanke756.top/gtvhlidxus.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.redwolf501.top/gtakggqmwh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shanyushiyangtech.top/gtktjajpld.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cashguo.top/gtbebartew.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.sxryk.cn/gtxnbfzhdy.html

Ruby: a == b
来源：http://hz.birdmap.top/gtgpccojmv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hywenlv.cn/gtlvlmimpp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ehwqpu.com/gtpqbcnepn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.fzhhl.top/gtzmzdytmf.html

PHP:  if (empty($x)) {}
来源：http://hz.xingfuxueyuan.xyz/gtwrzjugme.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.snrcjt.cn/gtbwwnqloi.html

TS:   if (x == null) {}
来源：http://hz.sufxvd.cn/gtlfqrqzyj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.pycfn.com/gttyvyuqhr.html

Go:   if x == nil {}
来源：http://hz.jiagoushi.top/gtmjhqnfgo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.fzhhl.top/gtvixoloov.html

C#:   if (x is null) {}
来源：http://hz.feifeiyinyue.top/gtbthhjbmm.html

[P07] 防抖与节流
来源：http://hz.dianchejie.cn/gtukkigrbu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.iojbl.cn/gturyvuxxf.html


<!-- 参考信息 -->