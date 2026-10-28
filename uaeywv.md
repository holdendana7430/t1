代发 wailian999

JS:   process.argv.slice(2)
来源：http://hz.shanyushiyangtech.top/gtcaheibiz.html

TS:   process.argv.slice(2)
来源：http://hz.pycfn.com/gtfghokzlg.html

Java: args 数组（main 方法参数）
来源：http://hz.quarkkingdee.top/gtsnulmvlk.html

Go:   os.Args[1:]
来源：http://hz.yonumen.top/gtmceypbad.html

Ruby: ARGV
来源：http://hz.ehwqpu.com/gtsgospbtf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenzaomai.com/gtdumqpqab.html

[M02] 读取环境变量
来源：http://hz.aizwys.cn/gtxgmnorwp.html

Py:   os.environ.get("HOME")
来源：http://hz.tian-w.cn/gtayiqutab.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.feifeiyinyue.top/gtbzusfdki.html

JS:   process.env.HOME
来源：http://hz.fengsongda.top/gtottyvwlq.html

TS:   process.env.HOME
来源：http://hz.fzhhl.top/gtutouoazq.html

Java: System.getenv("HOME")
来源：http://hz.haohaochexian.top/gtrghvzkzr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sufxvd.cn/gtfcmqiaae.html

Ruby: ENV["HOME"]
来源：http://hz.vqdsnc.cn/gtlizwsird.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.birdmap.top/gtkfddnjpy.html

[M03] 执行外部命令
来源：http://hz.zhengqikj.top/gtyolftjqs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yvedp.cn/gtaatyvlvv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.tanke756.top/gtoxbvfhzc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgfzy.top/gtgcpumikx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.snrcjt.cn/gtfjzersad.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.feifeiyinyue.top/gtxwxmujrg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.vqdsnc.cn/gtitdnmdfu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.52xcode.cn/gtzhllfjlh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.fzhhl.top/gttnjsupoo.html

[M04] 获取当前工作目录
来源：http://hz.ydzc1.top/gtatfxzync.html

Py:   os.getcwd()
来源：http://hz.aizwys.cn/gtgcelgcdy.html

PHP:  getcwd();
来源：http://hz.sysykeji.top/gtoizwtpfe.html

JS:   process.cwd()
来源：http://hz.316326.xyz/gtfxffhvwm.html

TS:   process.cwd()
来源：http://hz.daria6918.cn/gttylyinxl.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yanxiufei.cn/gtytdhcako.html

Go:   os.Getwd()
来源：http://hz.aizwys.cn/gtmentccta.html

Ruby: Dir.pwd
来源：http://hz.ydzc1.top/gtywgfooce.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jiagoushi.top/gtyurlvgow.html

[M05] 设置退出码
来源：http://hz.nanxinkj.top/gtspbpzcwy.html

Py:   sys.exit(1)
来源：http://hz.andypj.xyz/gthkskdvco.html

PHP:  exit(1);
来源：http://hz.cdnleiting.top/gtqqewqeum.html

JS:   process.exit(1)
来源：http://hz.yonumen.top/gtfuqnrkyn.html

TS:   process.exit(1)
来源：http://hz.zhijiandao.cn/gtliigheqe.html

Java: System.exit(1)
来源：http://hz.yvedp.cn/gthtrpfudu.html

Go:   os.Exit(1)
来源：http://hz.yj202588.top/gtmowyfvsx.html

Ruby: exit 1
来源：http://hz.shanyushiyangkeji.top/gtppjoienz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.wangdashe.top/gtpidydrkj.html

[M06] 向标准错误输出
来源：http://hz.jiagoushi.top/gtbmdixxhw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.316326.xyz/gtdkkcgvjl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cdnleiting.top/gtacmtshwi.html

JS:   console.error("err")
来源：http://hz.hammf.cn/gtkgkjycwp.html

TS:   console.error("err")
来源：http://hz.zhongyouzk.top/gthboezasa.html

Java: System.err.println("err")
来源：http://hz.tian-w.cn/gtvnegtxvv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.vqdsnc.cn/gtexecvnjj.html

Ruby: warn "err"
来源：http://hz.dianchejie.cn/gtqqonewze.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shzxlz.cn/gtyybokotf.html

[M07] 判断是否为主入口
来源：http://hz.jinqigfzy.top/gteogbwdop.html

Py:   if __name__ == "__main__":
来源：http://hz.xuetiantiany.cn/gtkuefmqlg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jqgufenzy.top/gtpdemfjyx.html

JS:   require.main === module
来源：http://hz.tian-w.cn/gtfylxlbtw.html

TS:   require.main === module
来源：http://hz.yongpay.top/gtrxqijsln.html

Java: public static void main(String[] args)
来源：http://hz.chenlongwang.top/gtttqdfpdv.html

Go:   func main()
来源：http://hz.chenlongwang.top/gtitfsjiwi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jianghu66.top/gtkxackveq.html

C#:   static void Main(string[] args)
来源：http://hz.yongpay.top/gtupmnlvoh.html

[M08] 获取系统与运行时信息
来源：http://hz.yonumen.top/gtsjepittf.html

Py:   platform.system();  platform.python_version()
来源：http://hz.sweek.top/gtlmzubfvu.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.daria6918.cn/gtlzhkdaek.html

JS:   process.platform;  process.version
来源：http://hz.zhoulong.xyz/gtsamloads.html

TS:   process.platform;  process.version
来源：http://hz.guowangkeji.top/gtdtqtgrwl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.fzhhl.top/gturrkfwkq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhengqikj.top/gtxjmcwiun.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.dianchejie.cn/gtspzeznak.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.nwbrower.top/gtanedqrwn.html

================================================================================
来源：http://hz.ybcxt.top/gteupmjvsh.html

N. 数据结构与算法
来源：http://hz.zhoulong.xyz/gtnxzjohxt.html

================================================================================
来源：http://hz.xziqi.cn/gtsfxgldoe.html

[N01] 二分查找（有序数组）
来源：http://hz.gaohongyu789.top/gtarmbztuu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ivvv.top/gtpvaghyzy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.redwolf501.top/gtpfyoimlt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xingfuxueyuan.xyz/gtrdtcmmjx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.316326.xyz/gtxiaiwczu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.tianlin.xyz/gtrylpxnjt.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yongpay.top/gtdkhsejqx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.chenjidiqi.icu/gtbqnwqztk.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhiwuduotai.top/gtgtwkdzvb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.tian-w.cn/gthegalxnq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shangyingyoupin.top/gtvyxpatbh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ivvv.top/gtlezrphjr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shzxlz.cn/gtbtnheocu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gtdxcbxtst.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xingfuxueyuan.xyz/gtwsfzzdgd.html

Go:   slices.Sort(arr)
来源：http://hz.cucudq.cn/gthcovflvs.html

Ruby: arr.sort
来源：http://hz.zhaomingkeji.xyz/gtzghbbuuy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.guannengcc.top/gtulubirxx.html

[N03] 快速排序（分治示例）
来源：http://hz.chenlongwang.top/gtgryhodta.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhijiandao.cn/gtbcvwuvhl.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hfpthk.cn/gtttixxsjj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cashguo.top/gtjaedsbqr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cucudq.cn/gtxuixatyz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.gaohongyu789.top/gtanwvzxcl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.pengpengdd.cyou/gtteqqtwrr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yueranfly.top/gtivmlvnvo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.dianchejie.cn/gtdjykcbpt.html

[N04] 斐波那契数列
来源：http://hz.xylfe.cn/gtrfayvgmh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yuanzhike.top/gtlilztuxl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shuidangran.top/gtsszblvyg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.havefunace.top/gtwucrupwv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxinkj.top/gtupvlztax.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yvedp.cn/gtrkleblwn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xuanzx.com/gtqrcfhxtq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.aizwys.cn/gtcdohwucv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.redwolf501.top/gtmpjopige.html

[N05] 最大公约数
来源：http://hz.zhoulong.xyz/gtemjyoejh.html

Py:   math.gcd(a, b)
来源：http://hz.hfpthk.cn/gtgovibrmc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tian-w.cn/gtnmuoswac.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenlongwang.top/gtiualgkyk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj202588.top/gtymtksuda.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.aizwys.cn/gtkepynoan.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sxryk.cn/gtehvmxiqq.html

Ruby: a.gcd(b)
来源：http://hz.jiagoushi.top/gtpplabtzc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.tianlin.xyz/gtqkdmlays.html

[N06] 判断回文字符串
来源：http://hz.hfpthk.cn/gtnbwgbqbw.html

Py:   s == s[::-1]
来源：http://hz.guowangkeji.top/gtjlzbdtar.html

PHP:  $s === strrev($s);
来源：http://hz.snrcjt.cn/gtuihqunbg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtdmnjpetb.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtuwaihmze.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.pycfn.com/gtecsurhqb.html

Go:   // 双指针从两端比较
来源：http://hz.gogol.net.cn/gtfwgxnmao.html

Ruby: s == s.reverse
来源：http://hz.gogol.net.cn/gtarhaxoha.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.vqdsnc.cn/gtwgmxdqsp.html

[N07] 两数之和（返回下标）
来源：http://hz.ivvv.top/gtqndiaclh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yuanzhike.top/gtssagkofl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhaomingkeji.xyz/gtfzbxkqrq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.chenlongwang.top/gtjyezbuwo.html

TS:   // 手写 Map<string, number>
来源：http://hz.yonumen.top/gtxbwhkqfp.html

Java: // 手写 HashMap
来源：http://hz.316326.xyz/gtteisoyfy.html

Go:   // 手写 map[int]int
来源：http://hz.ydjk.org.cn/gthrbugcym.html

Ruby: // 手写 Hash
来源：http://hz.nanxuanxn.top/gtqlhyecqk.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hnxiangtu.top/gtlwqgfhwi.html

[N08] 生成全排列
来源：http://hz.bjfxy.top/gtvpriaxfr.html

Py:   itertools.permutations(arr)
来源：http://hz.daria6918.cn/gtbatrzgif.html

PHP:  // 手写递归交换
来源：http://hz.gogol.net.cn/gthnorqbgj.html

JS:   // 手写回溯递归
来源：http://hz.birdmap.top/gtajzppbun.html

TS:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gtlmbtplhj.html

Java: // 手写回溯递归
来源：http://hz.svipenyu.cn/gttterdabi.html

Go:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtgyfjjkxb.html

Ruby: arr.permutation.to_a
来源：http://hz.ydjk.org.cn/gtgjgseipo.html

C#:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtajuymwzu.html

[N09] 栈与队列
来源：http://hz.yangfankeji.com/gtpggwmtex.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.pycfn.com/gtjgkhrjtt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jqgfzy.top/gtqclxdpfx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jyoumei.cn/gtbshgcoga.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.andypj.xyz/gtmfsjhgyd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.nanxinkj.top/gtlxcvvpvh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ywan-chungtsiang.top/gtdgobitrb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.wangdashe.top/gtscllxtmt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.svipenyu.cn/gtyorspdri.html

[N10] 链表节点定义
来源：http://hz.andypj.xyz/gtbkdiemao.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.chenjidiqi.icu/gtcbkkidtt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sweek.top/gtzslxfthl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhengqikj.top/gtglsehmoh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.nanxinkj.top/gtdkxlaizp.html

Java: class Node { int v; Node next; }
来源：http://hz.ivvv.top/gtxutiuyue.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.aizwys.cn/gtyfzobrag.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sysykeji.top/gtxgccabfj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.gzhubu.top/gtrjtflhus.html

[N11] 二叉树中序遍历
来源：http://hz.svipenyu.cn/gttrxdvggs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.gzhubu.top/gtalfobumo.html

PHP:  // 手写递归函数
来源：http://hz.xinyue.icu/gtbpxsxqll.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yongpay.top/gtprmavsdp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhaomingkeji.xyz/gtkhqrcyza.html

Java: // 手写递归
来源：http://hz.mhx1999.top/gtvhtfrkvv.html

Go:   // 手写递归
来源：http://hz.yj20258.top/gtmfvpqvdr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.birdmap.top/gtogjmjryx.html

C#:   // 手写递归
来源：http://hz.zhongyouzk.top/gtmwppzpge.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.sxryk.cn/gtyaykyvzs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.wangshuangyany.cn/gtsjsebuvi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shanyushiyangtech.top/gtnmfhwnqf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxinkj.top/gtvynczgtv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangtech.top/gtneoycajr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.0kj1m.cn/gtzbchtasp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.aizwys.cn/gtxjctsoza.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinghuilouyu.cn/gtyeccgiir.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258.top/gtiinwvngl.html

================================================================================
来源：http://hz.9152youxi.cn/gtnkhyylxh.html

O. 并发与异步
来源：http://hz.gogol.net.cn/gtvgxsebol.html

================================================================================
来源：http://hz.snrcjt.cn/gtlsklkiik.html

[O01] 启动一个线程
来源：http://hz.jqgufenzy.top/gtfhpitcgw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.meibo888.top/gtjoihfclt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.bjfxy.top/gtihcvuwnr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hywenlv.cn/gtzxwybidb.html

TS:   // 同 JS
来源：http://hz.zhijiandao.cn/gtayuxrooq.html

Java: new Thread(() -> f()).start()
来源：http://hz.yj202588.top/gtgeeiekdn.html

Go:   go f()
来源：http://hz.haohaochexian.top/gtkqbbaooe.html

Ruby: Thread.new { f }
来源：http://hz.zhaomingkeji.xyz/gtfgsuswpy.html

C#:   Task.Run(() => F());
来源：http://hz.jqgufenzy.top/gtsflnullm.html

[O02] 使用线程池
来源：http://hz.zycfv.cn/gtntqvtcts.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.daria6918.cn/gtgnuswxrw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.bjfxy.top/gtyejmfdez.html

JS:   // worker_threads 线程池
来源：http://hz.yongpay.top/gtklhcugak.html

TS:   // worker_threads 线程池
来源：http://hz.gogol.net.cn/gtvwazoehy.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yuxming.cn/gtbdrxtzkz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.guannengcc.top/gticshhroo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xingfuxueyuan.xyz/gtuukwdiij.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gotoacloud.top/gttzcohtph.html

[O03] 加锁保护共享数据
来源：http://hz.ydzc1.top/gttzgsjmgt.html

Py:   with lock: shared += 1
来源：http://hz.jlsjyb.cn/gtlkoxgkyk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.dashuyun.cn/gtosnlnjjo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.tian-w.cn/gtyvuymplk.html

TS:   // 同 JS
来源：http://hz.ivvv.top/gtucyvvjqc.html

Java: synchronized (this) { shared++; }
来源：http://hz.yuanzhike.top/gtqwpoltkg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhixingplan.top/gtltdreduu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.havefunace.top/gtgzyqqpnz.html

C#:   lock (gate) { shared++; }
来源：http://hz.daria6918.cn/gtjddtgplo.html

[O04] 定义异步函数并等待
来源：http://hz.yanxiufei.cn/gtzvcbvill.html

Py:   async def f():⏎    await g()
来源：http://hz.daxiang520.top/gtljzcyqda.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhoulong.xyz/gtexxcygjv.html

JS:   async function f() { await g(); }
来源：http://hz.ppjwa.cn/gtbcvnlhvz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yanxiufei.cn/gtelvyjhef.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.iojbl.cn/gtqczwokej.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.gotoacloud.top/gtxcustuvg.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.vqdsnc.cn/gtmsyzbscs.html

C#:   async Task F() { await G(); }
来源：http://hz.mhx1999.top/gtstrwnllg.html

[O05] 并发执行并等待全部完成
来源：http://hz.quarkkingdee.top/gtbypfwdof.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cashguo.top/gtrqhcrsit.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.vqdsnc.cn/gtjjzkcbuw.html

JS:   await Promise.all(tasks)
来源：http://hz.hnxiangtu.top/gtkklgppyk.html

TS:   await Promise.all(tasks)
来源：http://hz.wangdashe.top/gtjlxsiltu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ybcxt.top/gtqwfovpbl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hammf.cn/gtzsdrjorr.html

Ruby: threads.map(&:join)
来源：http://hz.shanyushiyangkeji.top/gtynkkpgoi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhoulong.xyz/gtpgtwaqwl.html

[O06] 使用进程池
来源：http://hz.yongpay.top/gtoafkvwhm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.haohaochexian.top/gtpimpqiio.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yj202588.top/gtxmilmzhw.html

JS:   // child_process / cluster 模块
来源：http://hz.nwbrower.top/gtvssyvfuf.html

TS:   // child_process / cluster 模块
来源：http://hz.yuanzhike.top/gthztdetws.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ydjk.org.cn/gtgwaphpkj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.tianlin.xyz/gtidbualqj.html

Ruby: // fork 块
来源：http://hz.nwbrower.top/gtqvfcvmks.html

C#:   Parallel.For
来源：http://hz.gotoacloud.top/gtxdqrkrkk.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtmrfdviju.html

P. 常用工具函数
来源：http://hz.andypj.xyz/gtlxjgnsvy.html

================================================================================
来源：http://hz.yj20258888.top/gtmwhrkrte.html

[P01] 生成 UUID
来源：http://hz.cucudq.cn/gtaierdtoq.html

Py:   str(uuid.uuid4())
来源：http://hz.shangyingyoupin.top/gtqhfchker.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jiagoushi.top/gtkcnjzhoe.html

JS:   crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtavpupacn.html

TS:   crypto.randomUUID()
来源：http://hz.sweek.top/gtwuwkbyks.html

Java: UUID.randomUUID().toString()
来源：http://hz.daria6918.cn/gtbptqomrs.html

Go:   // 用 github.com/google/uuid
来源：http://hz.pycfn.com/gtizizjwpn.html

Ruby: SecureRandom.uuid
来源：http://hz.zhiwuduotai.top/gtsrqitmhg.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sufxvd.cn/gtfqtckvpa.html

[P02] MD5 / SHA256 摘要
来源：http://hz.aizwys.cn/gtrzskucxx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shuidangran.top/gtclfgkjgh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.chenlongwang.top/gtynpqvenx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gaohongyu789.top/gtgtpfpiwg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.aizwys.cn/gtrkpegzdq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.sweek.top/gtkvoentoc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ivvv.top/gtbrbbqjec.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.gogol.net.cn/gtwvewqjvz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xylfe.cn/gtcodvijwk.html

[P03] 生成短随机字符串
来源：http://hz.316326.xyz/gthrokbkqy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhengqikj.top/gtawgmnohf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.sxryk.cn/gttviynhmm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jiagoushi.top/gtanzuyacv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258.top/gtfhreaojk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hysaishi.cn/gtjvphqfxr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nanxinkj.top/gtmlcagzfl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhaomingkeji.xyz/gtgrzshikz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zycfv.cn/gtopzeiguj.html

[P04] 求长度
来源：http://hz.zhiwuduotai.top/gtjjnubnza.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xuetiantiany.cn/gtbkpcviwq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yangfankeji.com/gtstqeckvr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jianghu66.top/gttcdesbib.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnxiangtu.top/gtgstztirj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.smart0.xyz/gteksujbun.html

Go:   len(arr);  len(m)
来源：http://hz.hammf.cn/gtwpznupdt.html

Ruby: x.length;  x.size
来源：http://hz.yongpay.top/gtdtwjbvzj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ehwqpu.com/gtprpqihpd.html

[P05] 判断两个对象内容是否相等
来源：http://hz.cashguo.top/gtadpjobgw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cdnleiting.top/gtwqraeftq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shzxlz.cn/gtvvirevsy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.gotoacloud.top/gtfijalqsh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.guowangkeji.top/gtwajdwazv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xylfe.cn/gtcpuhvctz.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cqqwz.cn/gttzfbxruq.html

Ruby: a == b
来源：http://hz.jinqigufen.top/gtsipspfzf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.sxryk.cn/gtiswnburw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xuetiantiany.cn/gtlsycjvyp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shuidangran.top/gteqahuqbf.html

PHP:  if (empty($x)) {}
来源：http://hz.iojbl.cn/gtzqzwickr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shanyushiyangtech.top/gtrwofyrtq.html

TS:   if (x == null) {}
来源：http://hz.tian-w.cn/gtxxwapals.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhoulong.xyz/gtamtkxkqx.html

Go:   if x == nil {}
来源：http://hz.sweek.top/gtzgjfgaof.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.fzhhl.top/gtmczanbze.html

C#:   if (x is null) {}
来源：http://hz.ydzc1.top/gtlkduwnzb.html

[P07] 防抖与节流
来源：http://hz.zhixingplan.top/gtoancqiyq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hfpthk.cn/gtdhmrahuq.html

PHP:  // 手写时间戳比较
来源：http://hz.tianlin.xyz/gtfymofqgm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yangfankeji.com/gtrdyheeju.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.iojbl.cn/gtojxferzb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.iojbl.cn/gtphpgenyv.html


<!-- 参考信息 -->