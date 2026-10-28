代发 wailian999

Ruby: ARGV
来源：http://hz.shanyushiyangtech.top/gtlpguoyrh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sxryk.cn/gtigzqnxoj.html

[M02] 读取环境变量
来源：http://hz.jiagoushi.top/gtifpomqpm.html

Py:   os.environ.get("HOME")
来源：http://hz.dianchejie.cn/gtthzisnfh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.havefunace.top/gtlfiqtoaq.html

JS:   process.env.HOME
来源：http://hz.xuetiantiany.cn/gthyhnbgsf.html

TS:   process.env.HOME
来源：http://hz.sxryk.cn/gtloepidyi.html

Java: System.getenv("HOME")
来源：http://hz.tianlin.xyz/gtpwjrmxbv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhongyouzk.top/gtzoxzrunn.html

Ruby: ENV["HOME"]
来源：http://hz.hammf.cn/gtdgbcvlkq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.snrcjt.cn/gtkodaldso.html

[M03] 执行外部命令
来源：http://hz.havefunace.top/gtuhbygdir.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.c1oappe.top/gtobmaudyb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cashguo.top/gtcwclhwej.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.c1oappe.top/gtusnxypvx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.nanxuanxn.top/gtvrekgprw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj20258.top/gtzbxghtmy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yj202588.top/gtlihcwqiu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.tian-w.cn/gtscqyrajj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ybcxt.top/gtupxirwsp.html

[M04] 获取当前工作目录
来源：http://hz.zhoulong.xyz/gtbawuwfpw.html

Py:   os.getcwd()
来源：http://hz.kuanghao11.cn/gtbocswhzj.html

PHP:  getcwd();
来源：http://hz.zhongyouzk.top/gtrltesena.html

JS:   process.cwd()
来源：http://hz.ppjwa.cn/gtprnrcnkc.html

TS:   process.cwd()
来源：http://hz.sxryk.cn/gthfgtqdgk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hammf.cn/gtakirbklp.html

Go:   os.Getwd()
来源：http://hz.316326.xyz/gtutgduije.html

Ruby: Dir.pwd
来源：http://hz.52xcode.cn/gtlkfvcxms.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yonumen.top/gtxqdgcuuu.html

[M05] 设置退出码
来源：http://hz.jianghu66.top/gtifpkxqks.html

Py:   sys.exit(1)
来源：http://hz.zhoulong.xyz/gtkjcxuorx.html

PHP:  exit(1);
来源：http://hz.hnxiangtu.top/gtltsdgrvn.html

JS:   process.exit(1)
来源：http://hz.chenlongwang.top/gtffljyvkv.html

TS:   process.exit(1)
来源：http://hz.guannengcc.top/gtwlpnbjux.html

Java: System.exit(1)
来源：http://hz.mhx1999.top/gtlcwptlpy.html

Go:   os.Exit(1)
来源：http://hz.fengsongda.top/gtvqzsowgg.html

Ruby: exit 1
来源：http://hz.ppjwa.cn/gthlaqqpgo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.redwolf501.top/gtemjgxvlz.html

[M06] 向标准错误输出
来源：http://hz.ydzc1.top/gteywnmhvf.html

Py:   print("err", file=sys.stderr)
来源：http://hz.guowangkeji.top/gtpafnwmny.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.guannengcc.top/gtcysblvuc.html

JS:   console.error("err")
来源：http://hz.tianlin.xyz/gtewmjaaan.html

TS:   console.error("err")
来源：http://hz.hammf.cn/gtcomyethm.html

Java: System.err.println("err")
来源：http://hz.316326.xyz/gtsuyanvrw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xuanzx.com/gtlilzjdkv.html

Ruby: warn "err"
来源：http://hz.vqdsnc.cn/gteshqoyvl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xziqi.cn/gtuibvdrml.html

[M07] 判断是否为主入口
来源：http://hz.0kj1m.cn/gtftanooui.html

Py:   if __name__ == "__main__":
来源：http://hz.dianchejie.cn/gtogcxobgt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.feifeiyinyue.top/gtzxkabxia.html

JS:   require.main === module
来源：http://hz.cheryme.top/gtgmnrdwdt.html

TS:   require.main === module
来源：http://hz.ybcxt.top/gtdkijqsgd.html

Java: public static void main(String[] args)
来源：http://hz.gzhubu.top/gtzrnjkscr.html

Go:   func main()
来源：http://hz.shangyingyoupin.top/gtufzxuqev.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yueranfly.top/gtqxrhppoy.html

C#:   static void Main(string[] args)
来源：http://hz.chenzaomai.com/gtrwmrrypy.html

[M08] 获取系统与运行时信息
来源：http://hz.zhengqikj.top/gtenvyqawe.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gogol.net.cn/gtfvidpnhn.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yonumen.top/gtxagihdru.html

JS:   process.platform;  process.version
来源：http://hz.zhixingplan.top/gteyoezkgu.html

TS:   process.platform;  process.version
来源：http://hz.ppjwa.cn/gtypippcen.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shanyushiyangkeji.top/gtxeiesmkf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sysykeji.top/gtbietrfxf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shanyushiyangkeji.top/gtpklnpjxi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.daxiang520.top/gtvccswocw.html

================================================================================
来源：http://hz.hfpthk.cn/gtieselvxz.html

N. 数据结构与算法
来源：http://hz.zhongyouzk.top/gtxfsiumkb.html

================================================================================
来源：http://hz.cheryme.top/gtlikzavkl.html

[N01] 二分查找（有序数组）
来源：http://hz.hnqzz.top/gtgfobfmzc.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj20258888.top/gtjlnnpylq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.kuanghao11.cn/gticycmyfn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.pycfn.com/gtyezldstk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinghuilouyu.cn/gtzgwyghuj.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.aibaodan.cn/gtdfjqwwwz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xziqi.cn/gthggsjmyc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hammf.cn/gtggpcxotz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.fzhhl.top/gtbssjqikc.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.fengsongda.top/gtcdiftsyt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydjk.org.cn/gtbwoymdjc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nanxuanxn.top/gtvrvxrxsv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.wangdashe.top/gtuicycddd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zdqjudy.top/gtwwuhipan.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sysykeji.top/gtojeecppk.html

Go:   slices.Sort(arr)
来源：http://hz.jqgufenzy.top/gtzunuknkf.html

Ruby: arr.sort
来源：http://hz.snrcjt.cn/gtmpbfbrjk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.nanxuanxn.top/gtjngoyogr.html

[N03] 快速排序（分治示例）
来源：http://hz.ehwqpu.com/gtiwrmytem.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shuidangran.top/gtzfacnbia.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xylfe.cn/gtmcpihhzo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuetiantiany.cn/gteydwkykj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yangfankeji.com/gtirsjngzy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinqigufen.top/gtaveokhra.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.daria6918.cn/gtdbicovqh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.pycfn.com/gtwvlnojvp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.316326.xyz/gtpdvmwljl.html

[N04] 斐波那契数列
来源：http://hz.jinqigfzy.top/gtluhqwnsj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yj202588.top/gtxnyslpsq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hywenlv.cn/gtonlxgjim.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aibaodan.cn/gtesooyxmy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hongshengwenyu.top/gtbtbuqzkw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jiagoushi.top/gthpqmosjd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yonumen.top/gtagjijjdu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yanxiufei.cn/gtdlcarkqg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.quarkkingdee.top/gtmvqniplm.html

[N05] 最大公约数
来源：http://hz.ivvv.top/gtwwvkduis.html

Py:   math.gcd(a, b)
来源：http://hz.xuetiantiany.cn/gtsinfedpy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhongyouzk.top/gtorrvxopx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj202588.top/gtfrtbhksr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ppjwa.cn/gtyxnpzixt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.aizwys.cn/gtdgnmxeex.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cheryme.top/gtegdqgpuq.html

Ruby: a.gcd(b)
来源：http://hz.52xcode.cn/gtqsvetwhr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ehwqpu.com/gtmgogtxvh.html

[N06] 判断回文字符串
来源：http://hz.xuanzx.com/gtqtqmdahq.html

Py:   s == s[::-1]
来源：http://hz.yanxiufei.cn/gtvlquovtt.html

PHP:  $s === strrev($s);
来源：http://hz.cheryme.top/gtxzvlkmjo.html

JS:   s === [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtcndvwpmv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.pycfn.com/gtnupjljkw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zycfv.cn/gtxbceqkdy.html

Go:   // 双指针从两端比较
来源：http://hz.yueranfly.top/gtpyrnodjk.html

Ruby: s == s.reverse
来源：http://hz.smart0.xyz/gthsadmpaa.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yangfankeji.com/gtnbzowyan.html

[N07] 两数之和（返回下标）
来源：http://hz.aibaodan.cn/gtguhldmlz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.wangdashe.top/gtphxgyvoj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.dianchejie.cn/gtbvpjcruq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinqigfzy.top/gtqxckeacd.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhoulong.xyz/gtcboturto.html

Java: // 手写 HashMap
来源：http://hz.cqqwz.cn/gttkspwedo.html

Go:   // 手写 map[int]int
来源：http://hz.hnqzz.top/gtcgkqiavh.html

Ruby: // 手写 Hash
来源：http://hz.316326.xyz/gtlwysjgjz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jiagoushi.top/gtdjtnfvsv.html

[N08] 生成全排列
来源：http://hz.andypj.xyz/gtqovdsepo.html

Py:   itertools.permutations(arr)
来源：http://hz.xingfuxueyuan.xyz/gtkcrzczlg.html

PHP:  // 手写递归交换
来源：http://hz.gaohongyu789.top/gtazbyvjwo.html

JS:   // 手写回溯递归
来源：http://hz.zycfv.cn/gtfvsbcmwn.html

TS:   // 手写回溯递归
来源：http://hz.cucudq.cn/gtyxzstmtv.html

Java: // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtamuovsfc.html

Go:   // 手写回溯递归
来源：http://hz.zycfv.cn/gtvlvixnnh.html

Ruby: arr.permutation.to_a
来源：http://hz.sxryk.cn/gtoeegsiom.html

C#:   // 手写回溯递归
来源：http://hz.tianlin.xyz/gtjgzqhhlc.html

[N09] 栈与队列
来源：http://hz.52xcode.cn/gttfzcfiqc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.chenjidiqi.icu/gtodfcdvax.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cucudq.cn/gttjilzhaz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.feifeiyinyue.top/gtdhuyjsea.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hnxiangtu.top/gtxllyvlqz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.cashguo.top/gtljiofrlz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.wangdashe.top/gtpqpqsydb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hnxiangtu.top/gtvopvwlss.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhiwuduotai.top/gtyggifgcq.html

[N10] 链表节点定义
来源：http://hz.shangyingyoupin.top/gtgmcmbnxb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cqqwz.cn/gtvaspzpto.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.chenlongwang.top/gttfwfvlsy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.c1oappe.top/gtnswdzcqs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.daxiang520.top/gtvscwcxht.html

Java: class Node { int v; Node next; }
来源：http://hz.tianlin.xyz/gtmkbpbysw.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.pengpengdd.cyou/gtcxgxmtiq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.aizwys.cn/gtoxvcohnc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yonumen.top/gtsbcptdxz.html

[N11] 二叉树中序遍历
来源：http://hz.c1oappe.top/gtghapbiqf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yuxming.cn/gtdannkkff.html

PHP:  // 手写递归函数
来源：http://hz.ydzc1.top/gtpqhpwytd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.bjfxy.top/gtokpxcdjt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hfpthk.cn/gtvpieqiby.html

Java: // 手写递归
来源：http://hz.guowangkeji.top/gtipkdhblk.html

Go:   // 手写递归
来源：http://hz.jqgufenzy.top/gtcxldxsmy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jinyuanbaomall.cn/gtmotdzkrs.html

C#:   // 手写递归
来源：http://hz.quarkkingdee.top/gtrlmirter.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.fzhhl.top/gtxobfdftd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yj20258888.top/gtdahxfnok.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.chenjidiqi.icu/gttyfvwxla.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.bjfxy.top/gtschafxkt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.guannengcc.top/gtcnmbzroo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydzc1.top/gtfpjszsqj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jinqigfzy.top/gtkbyqnppr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.316326.xyz/gtzyvlmhsz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guowangkeji.top/gtreiacgpa.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtekxvjgov.html

O. 并发与异步
来源：http://hz.shanyushiyangtech.top/gtqsstrtyk.html

================================================================================
来源：http://hz.xuanzx.com/gtjkutfvjh.html

[O01] 启动一个线程
来源：http://hz.jinqigfzy.top/gtofpfvxif.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.chenjidiqi.icu/gtwsxiqqix.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.dashuyun.cn/gtzqpbxiwq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.sufxvd.cn/gtwojqpxgh.html

TS:   // 同 JS
来源：http://hz.shangyingyoupin.top/gtgsvwnnyc.html

Java: new Thread(() -> f()).start()
来源：http://hz.bjfxy.top/gthzftlvcb.html

Go:   go f()
来源：http://hz.yvedp.cn/gthfbaoknk.html

Ruby: Thread.new { f }
来源：http://hz.zdqjudy.top/gtkznhewtu.html

C#:   Task.Run(() => F());
来源：http://hz.ydzc1.top/gtjamvjgqy.html

[O02] 使用线程池
来源：http://hz.fzhhl.top/gtgntepciz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.316326.xyz/gtsoyaieer.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.quarkkingdee.top/gtsbiwjasn.html

JS:   // worker_threads 线程池
来源：http://hz.yanxiufei.cn/gtmosybuzj.html

TS:   // worker_threads 线程池
来源：http://hz.nanxinkj.top/gtiaqxejho.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yj20258888.top/gteandubyl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhengqikj.top/gtkyzesfof.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.guowangkeji.top/gtuanvyrtl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yj202588.top/gtmtaozkmd.html

[O03] 加锁保护共享数据
来源：http://hz.yanxiufei.cn/gtngwsikmm.html

Py:   with lock: shared += 1
来源：http://hz.nwbrower.top/gthxtrhzao.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xuanzx.com/gtqcftijap.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shanyushiyangtech.top/gtasjtkfob.html

TS:   // 同 JS
来源：http://hz.dianchejie.cn/gtmkdvvclc.html

Java: synchronized (this) { shared++; }
来源：http://hz.hywenlv.cn/gtcdipfwiy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.316326.xyz/gtyvxdxqma.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinqigfzy.top/gtpjjqjknx.html

C#:   lock (gate) { shared++; }
来源：http://hz.bjfxy.top/gtnylkvmds.html

[O04] 定义异步函数并等待
来源：http://hz.jinyuanbaomall.cn/gtfapkentw.html

Py:   async def f():⏎    await g()
来源：http://hz.jianghu66.top/gtqatncods.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhijiandao.cn/gtzsdsdydp.html

JS:   async function f() { await g(); }
来源：http://hz.nwbrower.top/gtsgityebt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yangfankeji.com/gtdmdcdqgq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.snrcjt.cn/gthofquibk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zycfv.cn/gtemhfgdgb.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.meibo888.top/gtcynmcgyf.html

C#:   async Task F() { await G(); }
来源：http://hz.yuxming.cn/gtogcwvxrs.html

[O05] 并发执行并等待全部完成
来源：http://hz.wangdashe.top/gtehsbduhx.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shanyushiyangtech.top/gtofeznisq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.snrcjt.cn/gtwhlzgare.html

JS:   await Promise.all(tasks)
来源：http://hz.52xcode.cn/gtuvagyccl.html

TS:   await Promise.all(tasks)
来源：http://hz.zhijiandao.cn/gtonflytsy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xuanzx.com/gtxsslcqle.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jinyuanbaomall.cn/gtitdyiczp.html

Ruby: threads.map(&:join)
来源：http://hz.yonumen.top/gtlpyyniip.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yonumen.top/gtgscnohci.html

[O06] 使用进程池
来源：http://hz.cheryme.top/gtnkwkrvdd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ywan-chungtsiang.top/gtqveetxfo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhongyouzk.top/gtigwixntr.html

JS:   // child_process / cluster 模块
来源：http://hz.chenzaomai.com/gtoeqshoxr.html

TS:   // child_process / cluster 模块
来源：http://hz.wangdashe.top/gtbyditkyt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.chenlongwang.top/gtofadcptm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xylfe.cn/gtecxlfgdj.html

Ruby: // fork 块
来源：http://hz.jinghuilouyu.cn/gtgqframfy.html

C#:   Parallel.For
来源：http://hz.gogol.net.cn/gtsodlmxly.html

================================================================================
来源：http://hz.snrcjt.cn/gtamnydplg.html

P. 常用工具函数
来源：http://hz.jqgfzy.top/gtssmjwkva.html

================================================================================
来源：http://hz.hywenlv.cn/gtgnunzrml.html

[P01] 生成 UUID
来源：http://hz.chenjidiqi.icu/gtjjwtyixi.html

Py:   str(uuid.uuid4())
来源：http://hz.yanxiufei.cn/gttedincqf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhijiandao.cn/gtmuguieaq.html

JS:   crypto.randomUUID()
来源：http://hz.xuetiantiany.cn/gtudctbiow.html

TS:   crypto.randomUUID()
来源：http://hz.yuanzhike.top/gthixprqdj.html

Java: UUID.randomUUID().toString()
来源：http://hz.ivvv.top/gtkrvwauts.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj202588.top/gtwyonpagf.html

Ruby: SecureRandom.uuid
来源：http://hz.zycfv.cn/gtjdfgwnxt.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.andypj.xyz/gtyqusndop.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hfpthk.cn/gtgkgwjksu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.nwbrower.top/gtdyjyphmq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xylfe.cn/gtdcxgwkrx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cqqwz.cn/gtdrqdblbn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.dianchejie.cn/gtyappbzec.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.birdmap.top/gtiwgjmjjh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.fengsongda.top/gtqmjltpnw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhaomingkeji.xyz/gtvsljlpep.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.316326.xyz/gtogywdflu.html

[P03] 生成短随机字符串
来源：http://hz.daxiang520.top/gtazewerzs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yj20258.top/gtmuxoltrc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hfpthk.cn/gtjjnerwad.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gzhubu.top/gtssmylaij.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xinyue.icu/gtojxukcia.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ydzc1.top/gtkswxmpeo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xingfuxueyuan.xyz/gtfawpihey.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ydjk.org.cn/gtbuljzhyx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.pengpengdd.cyou/gtwsrevexo.html

[P04] 求长度
来源：http://hz.andypj.xyz/gtwyiezoqq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yvedp.cn/gtslkvaets.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenlongwang.top/gtrerqwvmr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dianchejie.cn/gtdrlixffa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.aizwys.cn/gtfacarkze.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhoulong.xyz/gtyiukpluv.html

Go:   len(arr);  len(m)
来源：http://hz.tanke756.top/gtvqfggktz.html

Ruby: x.length;  x.size
来源：http://hz.aibaodan.cn/gtlcmnwttg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.kuanghao11.cn/gtjrbpdutv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.redwolf501.top/gtqzjsqnxw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hfpthk.cn/gtrkldrkyt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.pengpengdd.cyou/gtcvdkirop.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ppjwa.cn/gtqrexefiv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xingfuxueyuan.xyz/gtyajmqjtx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sufxvd.cn/gtoigviyml.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yj202588.top/gtqwmvgofd.html

Ruby: a == b
来源：http://hz.hongshengwenyu.top/gtrarwpfnx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.nwbrower.top/gtlwzzxapl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gzhubu.top/gtvdtuhjph.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.wangdashe.top/gtuaviwmxo.html

PHP:  if (empty($x)) {}
来源：http://hz.dashuyun.cn/gtldwqzsug.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yj20258.top/gthxpjidwp.html

TS:   if (x == null) {}
来源：http://hz.cqqwz.cn/gtzitnnlkm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yuanzhike.top/gtibkzzwlc.html

Go:   if x == nil {}
来源：http://hz.sxryk.cn/gtadsheqyh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.chenzaomai.com/gtttupftto.html

C#:   if (x is null) {}
来源：http://hz.gogol.net.cn/gtszsbyvnp.html

[P07] 防抖与节流
来源：http://hz.xinyue.icu/gtxvvtkcrd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.fengsongda.top/gtkewzsvvm.html

PHP:  // 手写时间戳比较
来源：http://hz.birdmap.top/gtqbjduioy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yangfankeji.com/gtnkrlopmo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shzxlz.cn/gtmsyqcqzz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.feifeiyinyue.top/gtjoonpowm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.fengsongda.top/gtcitovxez.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yuanzhike.top/gtbgxrlysk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gzhubu.top/gtfqsiuury.html

[P08] 处理浮点精度问题
来源：http://hz.gogol.net.cn/gtegzrpkbr.html


<!-- 参考信息 -->