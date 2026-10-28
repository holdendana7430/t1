代发 wailian999

Ruby: ARGV
来源：http://hz.redwolf501.top/gtxgdhkmoy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ydjk.org.cn/gtqvlskrwj.html

[M02] 读取环境变量
来源：http://hz.zycfv.cn/gtmbllthft.html

Py:   os.environ.get("HOME")
来源：http://hz.sufxvd.cn/gtxmtxwcke.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.redwolf501.top/gttsxxszni.html

JS:   process.env.HOME
来源：http://hz.havefunace.top/gttfeytlvu.html

TS:   process.env.HOME
来源：http://hz.mhx1999.top/gtrsrmpbxi.html

Java: System.getenv("HOME")
来源：http://hz.jqgfzy.top/gtvslxqtwa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.aizwys.cn/gtfrwskewb.html

Ruby: ENV["HOME"]
来源：http://hz.birdmap.top/gtnbjlnhho.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yonumen.top/gtebhavaig.html

[M03] 执行外部命令
来源：http://hz.hnxiangtu.top/gtekramsmc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.snrcjt.cn/gtqksvrkvb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.iojbl.cn/gtcvhmjbbz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shzxlz.cn/gtacrwceng.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.fzhhl.top/gtzdpptfaf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ydzc1.top/gtsxbmnzjz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jiagoushi.top/gtivzkufma.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yanxiufei.cn/gtimrcpxbb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhengqikj.top/gtjcybefen.html

[M04] 获取当前工作目录
来源：http://hz.daria6918.cn/gtdkmjwunb.html

Py:   os.getcwd()
来源：http://hz.nanxuanxn.top/gtqmatxmdg.html

PHP:  getcwd();
来源：http://hz.guowangkeji.top/gtjblgaffr.html

JS:   process.cwd()
来源：http://hz.9152youxi.cn/gtryvogycp.html

TS:   process.cwd()
来源：http://hz.chenlongwang.top/gtjvxstzka.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.daxiang520.top/gtcwvpwfvh.html

Go:   os.Getwd()
来源：http://hz.ydjk.org.cn/gtxvcnagcx.html

Ruby: Dir.pwd
来源：http://hz.cheryme.top/gthlpblpfr.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.52xcode.cn/gtdjmhsqin.html

[M05] 设置退出码
来源：http://hz.iojbl.cn/gtyncnazdi.html

Py:   sys.exit(1)
来源：http://hz.svipenyu.cn/gtwnugrrhk.html

PHP:  exit(1);
来源：http://hz.nanxuanxn.top/gtwssxgxlt.html

JS:   process.exit(1)
来源：http://hz.zhaomingkeji.xyz/gtsxyuazbo.html

TS:   process.exit(1)
来源：http://hz.yuanzhike.top/gtojrsxddg.html

Java: System.exit(1)
来源：http://hz.52xcode.cn/gtcvckyhjk.html

Go:   os.Exit(1)
来源：http://hz.jinqigfzy.top/gtflwtciwh.html

Ruby: exit 1
来源：http://hz.hysaishi.cn/gtfyoswmlo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jiagoushi.top/gtscrfovhj.html

[M06] 向标准错误输出
来源：http://hz.0kj1m.cn/gtfupncbay.html

Py:   print("err", file=sys.stderr)
来源：http://hz.guowangkeji.top/gtohgpwsff.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.havefunace.top/gtazfsrmjw.html

JS:   console.error("err")
来源：http://hz.shzxlz.cn/gtgoxjkggq.html

TS:   console.error("err")
来源：http://hz.zhaomingkeji.xyz/gttertycdp.html

Java: System.err.println("err")
来源：http://hz.dianchejie.cn/gtupyaovlb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hongshengwenyu.top/gtmalzmcip.html

Ruby: warn "err"
来源：http://hz.yanxiufei.cn/gtggubsmzr.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ivvv.top/gtnmxiolmh.html

[M07] 判断是否为主入口
来源：http://hz.sysykeji.top/gtsenuuovs.html

Py:   if __name__ == "__main__":
来源：http://hz.cheryme.top/gtdlygwlnq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hammf.cn/gtidvfzncy.html

JS:   require.main === module
来源：http://hz.meibo888.top/gtuhuwliiv.html

TS:   require.main === module
来源：http://hz.wangshuangyany.cn/gtkwltpkox.html

Java: public static void main(String[] args)
来源：http://hz.chenlongwang.top/gtlgseyqsi.html

Go:   func main()
来源：http://hz.zhixingplan.top/gtvrbrmrgi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.dashuyun.cn/gtmnsfeliv.html

C#:   static void Main(string[] args)
来源：http://hz.ydzc1.top/gtqgqqpzyy.html

[M08] 获取系统与运行时信息
来源：http://hz.jqgufenzy.top/gtgscjlvap.html

Py:   platform.system();  platform.python_version()
来源：http://hz.nanxinkj.top/gtdvazhphx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.bjfxy.top/gtbzreuvjn.html

JS:   process.platform;  process.version
来源：http://hz.shangyingyoupin.top/gtpmnfhtqy.html

TS:   process.platform;  process.version
来源：http://hz.0kj1m.cn/gthdiuavfv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.pycfn.com/gtnxmbbcux.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xziqi.cn/gtfjcosiop.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xuetiantiany.cn/gtmbjnppsw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.wangdashe.top/gtpfdbbgbx.html

================================================================================
来源：http://hz.svipenyu.cn/gtfajtwiyj.html

N. 数据结构与算法
来源：http://hz.daxiang520.top/gtcpwynfgb.html

================================================================================
来源：http://hz.yueranfly.top/gtdtywohsy.html

[N01] 二分查找（有序数组）
来源：http://hz.hongshengwenyu.top/gtxejyjtdq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nwbrower.top/gtnhhfzqaz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.feifeiyinyue.top/gtooysteab.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fzhhl.top/gtixeytnno.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenlongwang.top/gtonycvnkv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.nwbrower.top/gttplahhsu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cashguo.top/gtpsxzznuz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.iojbl.cn/gtvkgyxzfu.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jqgufenzy.top/gtppqnxczl.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.pycfn.com/gtrstyqapb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jqgufenzy.top/gtzmzihorr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.dashuyun.cn/gtyeplepxn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinqigufen.top/gtjytjlwvz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hnqzz.top/gteoipmlwl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jqgfzy.top/gtioqgoiwh.html

Go:   slices.Sort(arr)
来源：http://hz.gotoacloud.top/gtzuzcsqrj.html

Ruby: arr.sort
来源：http://hz.zhongyouzk.top/gtleykvjcn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhongyouzk.top/gtxpwnmfhu.html

[N03] 快速排序（分治示例）
来源：http://hz.316326.xyz/gtqbnovxvd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shanyushiyangkeji.top/gtieiykfgi.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ppjwa.cn/gthogqgvbu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ehwqpu.com/gtduoqojht.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aibaodan.cn/gtwygeaztk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.birdmap.top/gtrtemzbhg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yanxiufei.cn/gtbzphejga.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhijiandao.cn/gtuytgrgvx.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gzhubu.top/gtbruwptwv.html

[N04] 斐波那契数列
来源：http://hz.yuanzhike.top/gtmwhiftcc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yvedp.cn/gtntngxbcd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.c1oappe.top/gtflnogdun.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenjidiqi.icu/gtlrhiutdn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuanzhike.top/gtgxhofeqe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.vqdsnc.cn/gtddotqarz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.fengsongda.top/gtfizschjo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.chenzaomai.com/gtutfjjkcs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xinyue.icu/gtqsplumdi.html

[N05] 最大公约数
来源：http://hz.fzhhl.top/gtgmlajbvf.html

Py:   math.gcd(a, b)
来源：http://hz.fengsongda.top/gtnydqirru.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shanyushiyangkeji.top/gtapxlluay.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yongpay.top/gtdtlqqmqj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigufen.top/gtemiqynzy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hysaishi.cn/gtuszonagc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yonumen.top/gtqlavezhr.html

Ruby: a.gcd(b)
来源：http://hz.316326.xyz/gtpnadgpmu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.guowangkeji.top/gtcjimnott.html

[N06] 判断回文字符串
来源：http://hz.redwolf501.top/gtvjpfdhxa.html

Py:   s == s[::-1]
来源：http://hz.sxryk.cn/gtgadfuwvh.html

PHP:  $s === strrev($s);
来源：http://hz.mhx1999.top/gtimspszui.html

JS:   s === [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtczxhlsad.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gotoacloud.top/gtfvjetdiz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ydjk.org.cn/gtwtualbfv.html

Go:   // 双指针从两端比较
来源：http://hz.smart0.xyz/gtvkqntwwj.html

Ruby: s == s.reverse
来源：http://hz.chenzaomai.com/gtlkywsnyc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.kuanghao11.cn/gtnytmtdlj.html

[N07] 两数之和（返回下标）
来源：http://hz.cucudq.cn/gtxsijljuo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yvedp.cn/gtgbebtixc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.feifeiyinyue.top/gteomrplxh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ydzc1.top/gtlxapnvgc.html

TS:   // 手写 Map<string, number>
来源：http://hz.feifeiyinyue.top/gtlluxkurk.html

Java: // 手写 HashMap
来源：http://hz.yongpay.top/gttxyunwww.html

Go:   // 手写 map[int]int
来源：http://hz.wangdashe.top/gthlctwnky.html

Ruby: // 手写 Hash
来源：http://hz.gzhubu.top/gtkvdjkznl.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.vqdsnc.cn/gtxngqqhqy.html

[N08] 生成全排列
来源：http://hz.ehwqpu.com/gtoprhsiod.html

Py:   itertools.permutations(arr)
来源：http://hz.9152youxi.cn/gteoktyczh.html

PHP:  // 手写递归交换
来源：http://hz.meibo888.top/gtbwlyqzkl.html

JS:   // 手写回溯递归
来源：http://hz.jyoumei.cn/gtqlxvnyhf.html

TS:   // 手写回溯递归
来源：http://hz.jinqigufen.top/gtrwmogwfk.html

Java: // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtjfufkesg.html

Go:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtipewujgb.html

Ruby: arr.permutation.to_a
来源：http://hz.vqdsnc.cn/gtkdtdaish.html

C#:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtairphvlq.html

[N09] 栈与队列
来源：http://hz.hfpthk.cn/gtoqjbrcky.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.cqqwz.cn/gtnmgtvwiv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hfpthk.cn/gtklovelai.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.shanyushiyangkeji.top/gtmurjriwl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cqqwz.cn/gtsupqvsay.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jlsjyb.cn/gtjcyemcst.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jlsjyb.cn/gtezowsxqh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.birdmap.top/gtvxtzgmet.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.daxiang520.top/gtiadkxurj.html

[N10] 链表节点定义
来源：http://hz.xuetiantiany.cn/gtvykgxspk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.aibaodan.cn/gtefmsojnb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yanxiufei.cn/gtrppqxtud.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jianghu66.top/gtzxbalasz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hfpthk.cn/gtpmwptgav.html

Java: class Node { int v; Node next; }
来源：http://hz.52xcode.cn/gtawhlhdvb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ybcxt.top/gtweluxdhs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.dianchejie.cn/gtexvgpoob.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.feifeiyinyue.top/gtmuzpksyt.html

[N11] 二叉树中序遍历
来源：http://hz.jyoumei.cn/gtgyuifhfe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hfpthk.cn/gtzflvelwk.html

PHP:  // 手写递归函数
来源：http://hz.cashguo.top/gttxgkcbmk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.wangshuangyany.cn/gtjxtfqdhv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pengpengdd.cyou/gtawtzurec.html

Java: // 手写递归
来源：http://hz.feifeiyinyue.top/gtjjygmgiv.html

Go:   // 手写递归
来源：http://hz.yj20258.top/gtczbimvbm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tanke756.top/gtsvxvzvdw.html

C#:   // 手写递归
来源：http://hz.dashuyun.cn/gtdjphowhx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hfpthk.cn/gteqefwgie.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shanyushiyangkeji.top/gtqpvvgibs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cheryme.top/gtbphpaegg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hysaishi.cn/gtgxlcwrqw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuetiantiany.cn/gtodskkrii.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yangfankeji.com/gtrclfflau.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.pycfn.com/gtzkoishdn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xinyue.icu/gtjicwwiom.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yuxming.cn/gtfbuquugk.html

================================================================================
来源：http://hz.cashguo.top/gtsrawdgja.html

O. 并发与异步
来源：http://hz.xuanzx.com/gtezrltpbi.html

================================================================================
来源：http://hz.zycfv.cn/gtkwsgdwwb.html

[O01] 启动一个线程
来源：http://hz.zhaomingkeji.xyz/gtiymlqnda.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yj202588.top/gtyvdyfbnj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.mhx1999.top/gttdftzitb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yueranfly.top/gtmppetrzy.html

TS:   // 同 JS
来源：http://hz.gotoacloud.top/gtrytavwzl.html

Java: new Thread(() -> f()).start()
来源：http://hz.redwolf501.top/gtiveqymzv.html

Go:   go f()
来源：http://hz.hongshengwenyu.top/gtvsprhyok.html

Ruby: Thread.new { f }
来源：http://hz.smart0.xyz/gtuqtopjtv.html

C#:   Task.Run(() => F());
来源：http://hz.daxiang520.top/gtmkrbhoms.html

[O02] 使用线程池
来源：http://hz.wangdashe.top/gthkqeixeb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jqgfzy.top/gtymbhcptx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zycfv.cn/gteluqaixo.html

JS:   // worker_threads 线程池
来源：http://hz.yj202588.top/gtfmnftaai.html

TS:   // worker_threads 线程池
来源：http://hz.yongpay.top/gtmhgbjrrd.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.bjfxy.top/gtsxayemmu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ywan-chungtsiang.top/gtsntrjmhe.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.guannengcc.top/gtqfcdktmx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhaomingkeji.xyz/gtczkhwrdd.html

[O03] 加锁保护共享数据
来源：http://hz.vqdsnc.cn/gtvscawgmb.html

Py:   with lock: shared += 1
来源：http://hz.kuanghao11.cn/gtltypqmey.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.aizwys.cn/gtpzglzyit.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhongyouzk.top/gtdozimbzy.html

TS:   // 同 JS
来源：http://hz.yuxming.cn/gtvddhqlho.html

Java: synchronized (this) { shared++; }
来源：http://hz.jlsjyb.cn/gtoigohgck.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yvedp.cn/gtihtsbboi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xuanzx.com/gtgtqejtjr.html

C#:   lock (gate) { shared++; }
来源：http://hz.xinyue.icu/gtwpnlgnar.html

[O04] 定义异步函数并等待
来源：http://hz.jyoumei.cn/gtnljkiwhj.html

Py:   async def f():⏎    await g()
来源：http://hz.birdmap.top/gtczkzpixa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xuetiantiany.cn/gtjdtavxek.html

JS:   async function f() { await g(); }
来源：http://hz.sufxvd.cn/gtrwsdnrbl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.fzhhl.top/gtnshrebsm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.pengpengdd.cyou/gthbqjporq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yuxming.cn/gtqjurmmdo.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yuxming.cn/gtkobjdvlz.html

C#:   async Task F() { await G(); }
来源：http://hz.c1oappe.top/gtpvnleazq.html

[O05] 并发执行并等待全部完成
来源：http://hz.yangfankeji.com/gtffvkajfi.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yangfankeji.com/gtexpakrdl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.dianchejie.cn/gtnvhluhym.html

JS:   await Promise.all(tasks)
来源：http://hz.daria6918.cn/gtflljwadp.html

TS:   await Promise.all(tasks)
来源：http://hz.redwolf501.top/gtggslxaeb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.birdmap.top/gtkuqbsqnn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cqqwz.cn/gtwlwaqjly.html

Ruby: threads.map(&:join)
来源：http://hz.yuanzhike.top/gtqxunixhv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ydzc1.top/gtdchrueby.html

[O06] 使用进程池
来源：http://hz.snrcjt.cn/gtifuhrohj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.pengpengdd.cyou/gtpmxisrge.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shanyushiyangtech.top/gtwkixqsrz.html

JS:   // child_process / cluster 模块
来源：http://hz.smart0.xyz/gtakndqlew.html

TS:   // child_process / cluster 模块
来源：http://hz.sweek.top/gtqudfudyy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.9152youxi.cn/gtyuufatdh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gogol.net.cn/gtilnaegev.html

Ruby: // fork 块
来源：http://hz.meibo888.top/gtykwwifut.html

C#:   Parallel.For
来源：http://hz.andypj.xyz/gttiqiglne.html

================================================================================
来源：http://hz.hnqzz.top/gtikikompr.html

P. 常用工具函数
来源：http://hz.kuanghao11.cn/gtiynebtgj.html

================================================================================
来源：http://hz.hywenlv.cn/gtmzlyrwpe.html

[P01] 生成 UUID
来源：http://hz.hysaishi.cn/gtozfgkibq.html

Py:   str(uuid.uuid4())
来源：http://hz.ehwqpu.com/gtntokcpcs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shanyushiyangkeji.top/gtbrewjqzd.html

JS:   crypto.randomUUID()
来源：http://hz.shanyushiyangkeji.top/gtqrvfsvuv.html

TS:   crypto.randomUUID()
来源：http://hz.chenjidiqi.icu/gtepseljof.html

Java: UUID.randomUUID().toString()
来源：http://hz.tian-w.cn/gtzryrtwmj.html

Go:   // 用 github.com/google/uuid
来源：http://hz.wangdashe.top/gtsdqqbufl.html

Ruby: SecureRandom.uuid
来源：http://hz.ppjwa.cn/gtkymqzdwl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.wangdashe.top/gtvwztvlzd.html

[P02] MD5 / SHA256 摘要
来源：http://hz.daria6918.cn/gtxjqabmeb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yj20258888.top/gtivjrtiiv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yj20258.top/gtwttqxahi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhoulong.xyz/gtvaebftas.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xinyue.icu/gtzrmpckxz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hammf.cn/gtvnmgokzo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.chenlongwang.top/gtmjodrwpo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.fengsongda.top/gtxbmscius.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cdnleiting.top/gtnbjczbmd.html

[P03] 生成短随机字符串
来源：http://hz.pycfn.com/gttsmqlyvi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.kuanghao11.cn/gtmooigiwk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhiwuduotai.top/gtjaltnnis.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dianchejie.cn/gtcxhfizcj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigufen.top/gtxlwstioj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.9152youxi.cn/gtpvuuccso.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.haohaochexian.top/gtytokcybf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xingfuxueyuan.xyz/gtkajwubaw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yangfankeji.com/gtphwnhory.html

[P04] 求长度
来源：http://hz.gotoacloud.top/gtupicdwgn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.nwbrower.top/gtknnacsaj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cqqwz.cn/gtbyfhetuv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.andypj.xyz/gtuljnepqt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydzc1.top/gtiypovtor.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jiagoushi.top/gtbppffowx.html

Go:   len(arr);  len(m)
来源：http://hz.pengpengdd.cyou/gtjfwprhkh.html

Ruby: x.length;  x.size
来源：http://hz.gaohongyu789.top/gtimwbzfxq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ydzc1.top/gtxdvsuyyt.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sxryk.cn/gteycvyrmh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.daria6918.cn/gtqkmxvkso.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.gogol.net.cn/gtepbypuyv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.cqqwz.cn/gtnmdgrjhz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jiagoushi.top/gtkefvhkhp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.gaohongyu789.top/gtgiazgnto.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.9152youxi.cn/gtsgdtyzmt.html

Ruby: a == b
来源：http://hz.jlsjyb.cn/gtikglpacu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.dashuyun.cn/gtethbvieu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tian-w.cn/gtinscnxsu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.gzhubu.top/gtsivuchnu.html

PHP:  if (empty($x)) {}
来源：http://hz.ppjwa.cn/gtkcsxhqyx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.quarkkingdee.top/gtwcjrknaw.html

TS:   if (x == null) {}
来源：http://hz.fzhhl.top/gtkuasdpmt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ydjk.org.cn/gtjcmtcron.html

Go:   if x == nil {}
来源：http://hz.jyoumei.cn/gtpszqwbfc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hywenlv.cn/gtthkyysgx.html

C#:   if (x is null) {}
来源：http://hz.xingfuxueyuan.xyz/gtkdpibhsf.html

[P07] 防抖与节流
来源：http://hz.xylfe.cn/gtwkgztekf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cashguo.top/gtjspszxiu.html

PHP:  // 手写时间戳比较
来源：http://hz.yueranfly.top/gtalmwwooy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuetiantiany.cn/gtgachrecz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.smart0.xyz/gtrbbsozpl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xuanzx.com/gthlylrxls.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.fzhhl.top/gtozyprpzu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cashguo.top/gtggxpktlo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shanyushiyangkeji.top/gtbkrkeyuv.html

[P08] 处理浮点精度问题
来源：http://hz.zhaomingkeji.xyz/gtsasdzxri.html


<!-- 参考信息 -->