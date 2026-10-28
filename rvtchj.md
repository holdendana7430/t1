代发 wailian999

JS:   process.argv.slice(2)
来源：http://hz.chenjidiqi.icu/gtvqxklrii.html

TS:   process.argv.slice(2)
来源：http://hz.hnxiangtu.top/gtvtxiwczn.html

Java: args 数组（main 方法参数）
来源：http://hz.wangshuangyany.cn/gtsgzjbdsp.html

Go:   os.Args[1:]
来源：http://hz.redwolf501.top/gtianqpxtq.html

Ruby: ARGV
来源：http://hz.hywenlv.cn/gttydgfglz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cdnleiting.top/gthmyxmvyf.html

[M02] 读取环境变量
来源：http://hz.jyoumei.cn/gtswnvbllk.html

Py:   os.environ.get("HOME")
来源：http://hz.guannengcc.top/gtnflahphn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sxryk.cn/gtxcgszwlp.html

JS:   process.env.HOME
来源：http://hz.iojbl.cn/gtjnqkfvmw.html

TS:   process.env.HOME
来源：http://hz.wangdashe.top/gtkwremgks.html

Java: System.getenv("HOME")
来源：http://hz.iojbl.cn/gtelueemow.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.wangshuangyany.cn/gtxkyiybux.html

Ruby: ENV["HOME"]
来源：http://hz.jlsjyb.cn/gtyeihnygv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ehwqpu.com/gtwyqpirgv.html

[M03] 执行外部命令
来源：http://hz.jyoumei.cn/gtqazopqtq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhaomingkeji.xyz/gtqezbjtxe.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yuanzhike.top/gtecfvtwrq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.vqdsnc.cn/gtqbczcymy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hywenlv.cn/gtbhslgwid.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sufxvd.cn/gtgobetztv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.aizwys.cn/gtbokeqgyg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gogol.net.cn/gtspfqlvls.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinghuilouyu.cn/gtdaamcmip.html

[M04] 获取当前工作目录
来源：http://hz.mhx1999.top/gtuwdelmgz.html

Py:   os.getcwd()
来源：http://hz.guannengcc.top/gtijiheqfo.html

PHP:  getcwd();
来源：http://hz.sxryk.cn/gtexenqncf.html

JS:   process.cwd()
来源：http://hz.meibo888.top/gtheesajwr.html

TS:   process.cwd()
来源：http://hz.yj20258888.top/gtpatstbyg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xinyue.icu/gtlshdvmyd.html

Go:   os.Getwd()
来源：http://hz.xuanzx.com/gtcclcpwtb.html

Ruby: Dir.pwd
来源：http://hz.vqdsnc.cn/gtgiwnjzdj.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.vqdsnc.cn/gtavnijecs.html

[M05] 设置退出码
来源：http://hz.yvedp.cn/gtyeibdruo.html

Py:   sys.exit(1)
来源：http://hz.ydjk.org.cn/gtefmkqbge.html

PHP:  exit(1);
来源：http://hz.ppjwa.cn/gtmwzezovg.html

JS:   process.exit(1)
来源：http://hz.cucudq.cn/gtammfazza.html

TS:   process.exit(1)
来源：http://hz.yj20258888.top/gtsmfekqag.html

Java: System.exit(1)
来源：http://hz.hnqzz.top/gtmajswqhl.html

Go:   os.Exit(1)
来源：http://hz.wangshuangyany.cn/gtkhcmkuta.html

Ruby: exit 1
来源：http://hz.snrcjt.cn/gtrjgkeqdw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ybcxt.top/gtnocimttn.html

[M06] 向标准错误输出
来源：http://hz.kuanghao11.cn/gtjurtmfve.html

Py:   print("err", file=sys.stderr)
来源：http://hz.pycfn.com/gtyykoftvx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.tanke756.top/gtzncqptmd.html

JS:   console.error("err")
来源：http://hz.zdqjudy.top/gtsemwirew.html

TS:   console.error("err")
来源：http://hz.zdqjudy.top/gtkvgauxrh.html

Java: System.err.println("err")
来源：http://hz.birdmap.top/gtaxuvkkgc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sysykeji.top/gtcjdknnqr.html

Ruby: warn "err"
来源：http://hz.gzhubu.top/gtxrtgrjih.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.aibaodan.cn/gtvbslvikt.html

[M07] 判断是否为主入口
来源：http://hz.guannengcc.top/gtfwfkocsw.html

Py:   if __name__ == "__main__":
来源：http://hz.pengpengdd.cyou/gtebajxlpb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yonumen.top/gtundglfjo.html

JS:   require.main === module
来源：http://hz.zhijiandao.cn/gtndjksfdj.html

TS:   require.main === module
来源：http://hz.pengpengdd.cyou/gtdaskxdxl.html

Java: public static void main(String[] args)
来源：http://hz.xuanzx.com/gtehstavxc.html

Go:   func main()
来源：http://hz.jqgufenzy.top/gtosecqbnr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.9152youxi.cn/gtkogzgscp.html

C#:   static void Main(string[] args)
来源：http://hz.ivvv.top/gtugaswyfx.html

[M08] 获取系统与运行时信息
来源：http://hz.xziqi.cn/gteliunhul.html

Py:   platform.system();  platform.python_version()
来源：http://hz.tian-w.cn/gtlvqspezs.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sysykeji.top/gtktjeqxbi.html

JS:   process.platform;  process.version
来源：http://hz.xinyue.icu/gtpzsnfxvg.html

TS:   process.platform;  process.version
来源：http://hz.hfpthk.cn/gtqugjjxbs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gotoacloud.top/gtgovhwfar.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hfpthk.cn/gtgbiwevhg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinqigfzy.top/gthgtdaiqw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.vqdsnc.cn/gtjxeznddg.html

================================================================================
来源：http://hz.guannengcc.top/gtoxvechgh.html

N. 数据结构与算法
来源：http://hz.shzxlz.cn/gtmunpgxci.html

================================================================================
来源：http://hz.daria6918.cn/gtjxmocury.html

[N01] 二分查找（有序数组）
来源：http://hz.jyoumei.cn/gtesqwtevz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gaohongyu789.top/gtonvemhov.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zycfv.cn/gtcztewhjq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cheryme.top/gtczqiyhav.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jianghu66.top/gtffwahmrp.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhiwuduotai.top/gthvbqkocb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.redwolf501.top/gtzwnfzref.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jlsjyb.cn/gtgkxbksun.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.redwolf501.top/gtpeblgfpe.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.meibo888.top/gtxlirathk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cdnleiting.top/gtrpumriti.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.haohaochexian.top/gtmsiaetqs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenjidiqi.icu/gtpdfdqact.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hnxiangtu.top/gtmreboasc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.guannengcc.top/gtghokuayc.html

Go:   slices.Sort(arr)
来源：http://hz.cashguo.top/gtplupqdpl.html

Ruby: arr.sort
来源：http://hz.hysaishi.cn/gtqqjqgjpi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.fengsongda.top/gtaaekeivo.html

[N03] 快速排序（分治示例）
来源：http://hz.svipenyu.cn/gtokcxldpy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinyuanbaomall.cn/gttuebviff.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tianlin.xyz/gttxklzavp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ppjwa.cn/gtpikwlhfo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhoulong.xyz/gtzwiipwqg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.gotoacloud.top/gtqcewyrxq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinghuilouyu.cn/gtgoctbdtc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhijiandao.cn/gtvvqtckhd.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tianlin.xyz/gtstcutsql.html

[N04] 斐波那契数列
来源：http://hz.xinyue.icu/gtymdrnmto.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cashguo.top/gtjjzpnchk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xinyue.icu/gtvovnqslq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.havefunace.top/gtuqupwtct.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jlsjyb.cn/gtyhqvvbzv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xuanzx.com/gtcuqgemji.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xuetiantiany.cn/gtiklzeirq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.bjfxy.top/gtedakxgyp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zycfv.cn/gtsfncxyqz.html

[N05] 最大公约数
来源：http://hz.daxiang520.top/gtwrzkzbev.html

Py:   math.gcd(a, b)
来源：http://hz.aibaodan.cn/gtyjipxaoj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.haohaochexian.top/gtaufazmbi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aizwys.cn/gtaiokzpdv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gtxbqvwjyg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xinyue.icu/gtoucnlrjd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.nanxuanxn.top/gtxjavmkkd.html

Ruby: a.gcd(b)
来源：http://hz.xylfe.cn/gtldbnuhcr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.daxiang520.top/gttmibdhxg.html

[N06] 判断回文字符串
来源：http://hz.andypj.xyz/gtuvnxipbh.html

Py:   s == s[::-1]
来源：http://hz.xuanzx.com/gtfawuftpj.html

PHP:  $s === strrev($s);
来源：http://hz.iojbl.cn/gtkvipbsih.html

JS:   s === [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtcfxlbqqm.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ivvv.top/gtfzqjnkwv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hongshengwenyu.top/gttbojzkmr.html

Go:   // 双指针从两端比较
来源：http://hz.sweek.top/gtfkyyuqsv.html

Ruby: s == s.reverse
来源：http://hz.cucudq.cn/gtwleybzal.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xziqi.cn/gtcpvswzzt.html

[N07] 两数之和（返回下标）
来源：http://hz.hnxiangtu.top/gtnjshzlzq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xuanzx.com/gttghsgkhg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ehwqpu.com/gteaawrqng.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hammf.cn/gtmcetebel.html

TS:   // 手写 Map<string, number>
来源：http://hz.sweek.top/gtnvstsped.html

Java: // 手写 HashMap
来源：http://hz.yj202588.top/gtlubhqbks.html

Go:   // 手写 map[int]int
来源：http://hz.meibo888.top/gtqyfisaux.html

Ruby: // 手写 Hash
来源：http://hz.tianlin.xyz/gtnndcvozh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.mhx1999.top/gtuwzcncnq.html

[N08] 生成全排列
来源：http://hz.zhengqikj.top/gtqopunovx.html

Py:   itertools.permutations(arr)
来源：http://hz.iojbl.cn/gttpwkwuyo.html

PHP:  // 手写递归交换
来源：http://hz.chenzaomai.com/gtwpucegwt.html

JS:   // 手写回溯递归
来源：http://hz.yongpay.top/gtiphmkdza.html

TS:   // 手写回溯递归
来源：http://hz.yj20258.top/gtcblpdgvk.html

Java: // 手写回溯递归
来源：http://hz.guannengcc.top/gtlqeqxbig.html

Go:   // 手写回溯递归
来源：http://hz.yj202588.top/gtmxxqgolv.html

Ruby: arr.permutation.to_a
来源：http://hz.jqgfzy.top/gtylgovqao.html

C#:   // 手写回溯递归
来源：http://hz.hysaishi.cn/gtdjpnahny.html

[N09] 栈与队列
来源：http://hz.bjfxy.top/gtadfdmmez.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.cqqwz.cn/gtfyycjssc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hnxiangtu.top/gtxdhvweqc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.nwbrower.top/gthgigsrrf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jiagoushi.top/gtmhprdayw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhongyouzk.top/gtogzufppq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhengqikj.top/gthkoosomk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.vqdsnc.cn/gtdfjdrmao.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.guowangkeji.top/gtrqmgmoxy.html

[N10] 链表节点定义
来源：http://hz.shanyushiyangtech.top/gtypftxstz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yvedp.cn/gtonpcnlnb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.pengpengdd.cyou/gtzkntxvgx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.havefunace.top/gtakfklwid.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.guowangkeji.top/gtaxhlzipr.html

Java: class Node { int v; Node next; }
来源：http://hz.ywan-chungtsiang.top/gtfwteqaii.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ywan-chungtsiang.top/gtcchfzuwz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xinyue.icu/gtyfbwkwsw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.haohaochexian.top/gtfybyhfdc.html

[N11] 二叉树中序遍历
来源：http://hz.wangshuangyany.cn/gtblbcgpyf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ppjwa.cn/gtzarbeswe.html

PHP:  // 手写递归函数
来源：http://hz.zhoulong.xyz/gtxsamawrk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuxming.cn/gtkbhvkmib.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fzhhl.top/gtxoanedlk.html

Java: // 手写递归
来源：http://hz.jyoumei.cn/gtonszywdb.html

Go:   // 手写递归
来源：http://hz.feifeiyinyue.top/gtnbhfwdbm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jyoumei.cn/gtigiayqzf.html

C#:   // 手写递归
来源：http://hz.kuanghao11.cn/gtqmfclith.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ywan-chungtsiang.top/gtbwenlybp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.fengsongda.top/gtbvfbphig.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.dianchejie.cn/gtfcpmdxno.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yonumen.top/gtwmqgorzl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.c1oappe.top/gtxhuuqesr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.vqdsnc.cn/gttkmkgeuq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenzaomai.com/gtawlznber.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yvedp.cn/gtxcxqhocv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgufenzy.top/gtcvgbhejb.html

================================================================================
来源：http://hz.hysaishi.cn/gtlroikcjl.html

O. 并发与异步
来源：http://hz.zhoulong.xyz/gtiipmaewc.html

================================================================================
来源：http://hz.ydzc1.top/gtpfiklhxo.html

[O01] 启动一个线程
来源：http://hz.ywan-chungtsiang.top/gtsmgpddzb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.pengpengdd.cyou/gtasqfriah.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhaomingkeji.xyz/gtapphcngm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zdqjudy.top/gtqikmlsxo.html

TS:   // 同 JS
来源：http://hz.c1oappe.top/gtgoddizyg.html

Java: new Thread(() -> f()).start()
来源：http://hz.xylfe.cn/gtrhmbzteb.html

Go:   go f()
来源：http://hz.pengpengdd.cyou/gtgrdmduin.html

Ruby: Thread.new { f }
来源：http://hz.aizwys.cn/gtiulwmgbl.html

C#:   Task.Run(() => F());
来源：http://hz.yj20258.top/gtxthquseq.html

[O02] 使用线程池
来源：http://hz.nanxinkj.top/gthgylmbiz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jqgufenzy.top/gtxnlihytm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yvedp.cn/gtvuscjdod.html

JS:   // worker_threads 线程池
来源：http://hz.xinyue.icu/gtfoqqhsfw.html

TS:   // worker_threads 线程池
来源：http://hz.vqdsnc.cn/gtuvumpdsw.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.guowangkeji.top/gtxkjricha.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cheryme.top/gtllipvsjq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.daxiang520.top/gthvfkxvew.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gaohongyu789.top/gtltmvfzqr.html

[O03] 加锁保护共享数据
来源：http://hz.nwbrower.top/gtejmcbbnh.html

Py:   with lock: shared += 1
来源：http://hz.zhixingplan.top/gtwvpbrudv.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hfpthk.cn/gtdocrxcee.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hysaishi.cn/gtyltxgalj.html

TS:   // 同 JS
来源：http://hz.daria6918.cn/gtvdpmcihy.html

Java: synchronized (this) { shared++; }
来源：http://hz.shuidangran.top/gtrcewzpdw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.316326.xyz/gtxyeuuvyp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.tianlin.xyz/gttoyenarr.html

C#:   lock (gate) { shared++; }
来源：http://hz.dashuyun.cn/gtkvubdvek.html

[O04] 定义异步函数并等待
来源：http://hz.jinyuanbaomall.cn/gtjkzqeoyl.html

Py:   async def f():⏎    await g()
来源：http://hz.jyoumei.cn/gtqcmfzzih.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.chenlongwang.top/gtxrijvtuf.html

JS:   async function f() { await g(); }
来源：http://hz.dianchejie.cn/gtkxwvrefg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.meibo888.top/gtkgwqyypw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jiagoushi.top/gtnlvghokz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.9152youxi.cn/gtkahmwuot.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yongpay.top/gtcgyxvjxa.html

C#:   async Task F() { await G(); }
来源：http://hz.dianchejie.cn/gtwsaftowg.html

[O05] 并发执行并等待全部完成
来源：http://hz.cdnleiting.top/gtfqbnqyvq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhijiandao.cn/gtmcmkzkvd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.chenjidiqi.icu/gtncsmfapf.html

JS:   await Promise.all(tasks)
来源：http://hz.ehwqpu.com/gtphdhyvdd.html

TS:   await Promise.all(tasks)
来源：http://hz.hywenlv.cn/gtdxxmbxmt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shangyingyoupin.top/gtnrjauuvj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hnxiangtu.top/gtxzmdryxg.html

Ruby: threads.map(&:join)
来源：http://hz.zhijiandao.cn/gtwhllrfye.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shangyingyoupin.top/gtdtlskniq.html

[O06] 使用进程池
来源：http://hz.shuidangran.top/gtbzsxfvzg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.redwolf501.top/gtoviuynwu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhixingplan.top/gtjmwgjnhf.html

JS:   // child_process / cluster 模块
来源：http://hz.quarkkingdee.top/gtaucfrzlr.html

TS:   // child_process / cluster 模块
来源：http://hz.fengsongda.top/gtggnkmmwc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.shzxlz.cn/gtpogjghtq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yj20258888.top/gtmncxxnbm.html

Ruby: // fork 块
来源：http://hz.hysaishi.cn/gtzvhyhoth.html

C#:   Parallel.For
来源：http://hz.316326.xyz/gtqqffdkak.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtrojzlhdv.html

P. 常用工具函数
来源：http://hz.feifeiyinyue.top/gtqkszweut.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtqzyfxqzu.html

[P01] 生成 UUID
来源：http://hz.yuxming.cn/gthkzxnmlv.html

Py:   str(uuid.uuid4())
来源：http://hz.sxryk.cn/gtlbwesyrt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ybcxt.top/gtfrzfwrph.html

JS:   crypto.randomUUID()
来源：http://hz.xingfuxueyuan.xyz/gtlmtohqyf.html

TS:   crypto.randomUUID()
来源：http://hz.xuanzx.com/gtflkcevro.html

Java: UUID.randomUUID().toString()
来源：http://hz.chenzaomai.com/gtyihodari.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zycfv.cn/gtfzwxbulf.html

Ruby: SecureRandom.uuid
来源：http://hz.hammf.cn/gtmtxuhjpi.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.snrcjt.cn/gtlhgbyzzj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhixingplan.top/gtempbbrdz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sweek.top/gtqrmgwyhd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhixingplan.top/gtxkawqxlu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.9152youxi.cn/gtsqswjbca.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hfpthk.cn/gtpzvgsmfx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.dashuyun.cn/gtcmnybgpa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.aizwys.cn/gtwqhxmxbq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.kuanghao11.cn/gtbnjtklcs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.gaohongyu789.top/gtaedhexnn.html

[P03] 生成短随机字符串
来源：http://hz.jlsjyb.cn/gtodwmycec.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.pengpengdd.cyou/gtpuohmuwy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cheryme.top/gtvhqakqcm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenjidiqi.icu/gtqrewnzhj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuanzx.com/gtguigvvrh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hnqzz.top/gttpcvxalz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.guannengcc.top/gtndxhsonc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.iojbl.cn/gtyrzhugre.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.chenzaomai.com/gtlehyenpi.html

[P04] 求长度
来源：http://hz.gaohongyu789.top/gtgwmjlygm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hongshengwenyu.top/gtamnduuqu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pengpengdd.cyou/gtqfkvwsoe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zycfv.cn/gtmekqonoa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zycfv.cn/gtwdtojhcq.html

Java: list.size();  map.size();  s.length()
来源：http://hz.chenjidiqi.icu/gtzyexcdmb.html

Go:   len(arr);  len(m)
来源：http://hz.ywan-chungtsiang.top/gtqxjgyovw.html

Ruby: x.length;  x.size
来源：http://hz.hammf.cn/gtedtuofvz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.chenjidiqi.icu/gtrnfqndxe.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ppjwa.cn/gtprvzdolx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.9152youxi.cn/gttmqrrced.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jianghu66.top/gtmhofuwim.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hammf.cn/gtpbdecsmm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.redwolf501.top/gtflkaqcvm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yvedp.cn/gtbldkrcmt.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yuanzhike.top/gtjkwiqdwu.html

Ruby: a == b
来源：http://hz.xziqi.cn/gthfbfaeqj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.sweek.top/gtdhofzkps.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jyoumei.cn/gtnxzrkmhy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shangyingyoupin.top/gtolkyadzj.html

PHP:  if (empty($x)) {}
来源：http://hz.xuanzx.com/gtjnwssygn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shzxlz.cn/gtpzbprazw.html

TS:   if (x == null) {}
来源：http://hz.daria6918.cn/gtqaqmjdet.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.dashuyun.cn/gtmnhnmshy.html

Go:   if x == nil {}
来源：http://hz.ydjk.org.cn/gtbvnvvord.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.tian-w.cn/gtnjbpgaix.html

C#:   if (x is null) {}
来源：http://hz.cashguo.top/gttpdwhwak.html

[P07] 防抖与节流
来源：http://hz.jianghu66.top/gtebvnolsz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.0kj1m.cn/gtgfucwkxq.html

PHP:  // 手写时间戳比较
来源：http://hz.mhx1999.top/gtpdxqmfzb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gzhubu.top/gtvtsyhoiq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.pycfn.com/gtlnyuvsaq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.quarkkingdee.top/gtooenfboq.html


<!-- 参考信息 -->