代发 wailian999

Ruby: ARGV
来源：http://hz.havefunace.top/gtkqefufhc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ydjk.org.cn/gtazsoymyb.html

[M02] 读取环境变量
来源：http://hz.zhixingplan.top/gtzihhqvll.html

Py:   os.environ.get("HOME")
来源：http://hz.nanxuanxn.top/gtffsbrepu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.mhx1999.top/gtnmznzxkd.html

JS:   process.env.HOME
来源：http://hz.jinghuilouyu.cn/gtoaoqnkcd.html

TS:   process.env.HOME
来源：http://hz.snrcjt.cn/gtgzoeoaot.html

Java: System.getenv("HOME")
来源：http://hz.jianghu66.top/gtgjcufuxz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.tianlin.xyz/gtprlbqlqv.html

Ruby: ENV["HOME"]
来源：http://hz.shuidangran.top/gtdllegepu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.dashuyun.cn/gtoygzwmpn.html

[M03] 执行外部命令
来源：http://hz.tanke756.top/gtwosubzva.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.snrcjt.cn/gtnaafhozt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sufxvd.cn/gtjmtnpubb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cheryme.top/gtkitnjwxf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cdnleiting.top/gtxznbvxyd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cdnleiting.top/gtbysplugp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.aizwys.cn/gtemesyiei.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hammf.cn/gtnjeprcxf.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xingfuxueyuan.xyz/gtoayssqma.html

[M04] 获取当前工作目录
来源：http://hz.sweek.top/gtxkcdnsqo.html

Py:   os.getcwd()
来源：http://hz.0kj1m.cn/gtaqxblcdz.html

PHP:  getcwd();
来源：http://hz.ybcxt.top/gtclwkpvgn.html

JS:   process.cwd()
来源：http://hz.9152youxi.cn/gtfnejysqn.html

TS:   process.cwd()
来源：http://hz.ydjk.org.cn/gtifvlhrks.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cdnleiting.top/gtdzizobnp.html

Go:   os.Getwd()
来源：http://hz.wangshuangyany.cn/gtmnatspoy.html

Ruby: Dir.pwd
来源：http://hz.hnxiangtu.top/gtkgulutwb.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shanyushiyangtech.top/gtcfllwcom.html

[M05] 设置退出码
来源：http://hz.yanxiufei.cn/gtyoximfkb.html

Py:   sys.exit(1)
来源：http://hz.bjfxy.top/gtolcdjtbd.html

PHP:  exit(1);
来源：http://hz.jianghu66.top/gtkmlbkdgb.html

JS:   process.exit(1)
来源：http://hz.shanyushiyangkeji.top/gthvhmxogg.html

TS:   process.exit(1)
来源：http://hz.ydjk.org.cn/gtocqmtnts.html

Java: System.exit(1)
来源：http://hz.aibaodan.cn/gtiwhjzyvw.html

Go:   os.Exit(1)
来源：http://hz.jyoumei.cn/gteamuuizy.html

Ruby: exit 1
来源：http://hz.9152youxi.cn/gtzmigtzja.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nanxinkj.top/gtnzaljngl.html

[M06] 向标准错误输出
来源：http://hz.yonumen.top/gtrncxduct.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhengqikj.top/gtswlfgvhk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yonumen.top/gtwplhltuu.html

JS:   console.error("err")
来源：http://hz.pycfn.com/gtbrziidaz.html

TS:   console.error("err")
来源：http://hz.cdnleiting.top/gtugklfklp.html

Java: System.err.println("err")
来源：http://hz.dashuyun.cn/gtjjstbfkc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.iojbl.cn/gtqrcemyoz.html

Ruby: warn "err"
来源：http://hz.fengsongda.top/gtjbchljfz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.dashuyun.cn/gtrxohhdsf.html

[M07] 判断是否为主入口
来源：http://hz.xziqi.cn/gtdwxmygha.html

Py:   if __name__ == "__main__":
来源：http://hz.jinqigufen.top/gtgzaukpoe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ehwqpu.com/gtougvygtm.html

JS:   require.main === module
来源：http://hz.zhoulong.xyz/gtgvehpgqn.html

TS:   require.main === module
来源：http://hz.zhixingplan.top/gtemasgswn.html

Java: public static void main(String[] args)
来源：http://hz.yongpay.top/gtwtmlzmng.html

Go:   func main()
来源：http://hz.yj20258.top/gtgkgdfrts.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shanyushiyangkeji.top/gtakqmdhmo.html

C#:   static void Main(string[] args)
来源：http://hz.ydzc1.top/gtgcqkzqbt.html

[M08] 获取系统与运行时信息
来源：http://hz.yj202588.top/gtrqwdaywj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yj20258.top/gtzqvmhujq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jlsjyb.cn/gtobagopuy.html

JS:   process.platform;  process.version
来源：http://hz.chenzaomai.com/gtxyejlvix.html

TS:   process.platform;  process.version
来源：http://hz.birdmap.top/gtaysuwewg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tanke756.top/gtibmpddko.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.tianlin.xyz/gtjgbyqrem.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.guowangkeji.top/gtbuhlloqu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.daxiang520.top/gtnfvmmczq.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtneojcutg.html

N. 数据结构与算法
来源：http://hz.snrcjt.cn/gtomyuaatl.html

================================================================================
来源：http://hz.yvedp.cn/gtaprrhpqe.html

[N01] 二分查找（有序数组）
来源：http://hz.yonumen.top/gtdjvyngoo.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.snrcjt.cn/gttmrxdfuo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.guannengcc.top/gtexqtschs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.feifeiyinyue.top/gtdlxphqhw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxinkj.top/gtdffjgrax.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.pengpengdd.cyou/gtgdwcsdzn.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.kuanghao11.cn/gtyrnxkngm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xuanzx.com/gtceyakhmq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.quarkkingdee.top/gtfpjcgwpg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.9152youxi.cn/gtwovzfanj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydzc1.top/gtofbhgaug.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yuanzhike.top/gtmrdjigdh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jiagoushi.top/gtouuwdxam.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.vqdsnc.cn/gtlryjnall.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ywan-chungtsiang.top/gtbidwakju.html

Go:   slices.Sort(arr)
来源：http://hz.chenzaomai.com/gtwpgdnscp.html

Ruby: arr.sort
来源：http://hz.ydzc1.top/gtzhtpotjf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.chenjidiqi.icu/gttglcwczf.html

[N03] 快速排序（分治示例）
来源：http://hz.yangfankeji.com/gtawbfhhzn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.9152youxi.cn/gtnippbmgx.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yuxming.cn/gtpcfbhcpy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sufxvd.cn/gtexmyqeiq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guowangkeji.top/gtpzaydwyz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yanxiufei.cn/gtdjxmzkfg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.316326.xyz/gtbighrkvi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gzhubu.top/gtdihvciuv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cqqwz.cn/gtpybpfurv.html

[N04] 斐波那契数列
来源：http://hz.havefunace.top/gtgezlknnx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jiagoushi.top/gtwoumschb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yj202588.top/gtienlroow.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zycfv.cn/gtfbstbdyb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cashguo.top/gtmcbrhpkk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ydzc1.top/gtgxyguwjq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.316326.xyz/gtvqudfirf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yongpay.top/gtyoesxppn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yongpay.top/gtnpqqpmpd.html

[N05] 最大公约数
来源：http://hz.ehwqpu.com/gtmacwzlxt.html

Py:   math.gcd(a, b)
来源：http://hz.yuxming.cn/gtjeqfjzbk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jyoumei.cn/gtnanbuomc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gotoacloud.top/gtqocbpees.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hywenlv.cn/gtsjgpibow.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.svipenyu.cn/gtvtuzvmao.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.wangshuangyany.cn/gtfeigvkdm.html

Ruby: a.gcd(b)
来源：http://hz.jinqigufen.top/gtlrzkulfy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.kuanghao11.cn/gtcwndxeku.html

[N06] 判断回文字符串
来源：http://hz.jqgfzy.top/gtcunxrvbp.html

Py:   s == s[::-1]
来源：http://hz.jlsjyb.cn/gtvgutxuyz.html

PHP:  $s === strrev($s);
来源：http://hz.chenzaomai.com/gthxvdhvlb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jiagoushi.top/gtqrhthatx.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yuxming.cn/gtjbwbwzgn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cqqwz.cn/gtorkyuans.html

Go:   // 双指针从两端比较
来源：http://hz.quarkkingdee.top/gtrhnoippw.html

Ruby: s == s.reverse
来源：http://hz.dashuyun.cn/gtkpryphxq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jqgufenzy.top/gtjsakbtby.html

[N07] 两数之和（返回下标）
来源：http://hz.hysaishi.cn/gtbbbvuybt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.fzhhl.top/gtaizkmjwp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhiwuduotai.top/gtliwwmjzr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sufxvd.cn/gtcbmbkjnx.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinqigfzy.top/gtfuhlacgc.html

Java: // 手写 HashMap
来源：http://hz.sweek.top/gtwnummfbp.html

Go:   // 手写 map[int]int
来源：http://hz.zycfv.cn/gtovhifoba.html

Ruby: // 手写 Hash
来源：http://hz.pycfn.com/gtljosvmkj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yvedp.cn/gtyizingjb.html

[N08] 生成全排列
来源：http://hz.hnxiangtu.top/gtnaxgjcnd.html

Py:   itertools.permutations(arr)
来源：http://hz.snrcjt.cn/gtlaexyqgx.html

PHP:  // 手写递归交换
来源：http://hz.zhongyouzk.top/gtlstfzddd.html

JS:   // 手写回溯递归
来源：http://hz.yongpay.top/gtvptpslgm.html

TS:   // 手写回溯递归
来源：http://hz.mhx1999.top/gtcgjvvvdv.html

Java: // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gtahkouqdv.html

Go:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtzcisxqjz.html

Ruby: arr.permutation.to_a
来源：http://hz.hysaishi.cn/gtxixdpaxz.html

C#:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtacimiyqx.html

[N09] 栈与队列
来源：http://hz.fengsongda.top/gtnakfxdsg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hywenlv.cn/gtnhmubtcv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.feifeiyinyue.top/gtrqtybmnq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yangfankeji.com/gtituqqpsy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shzxlz.cn/gtenjujtts.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.daria6918.cn/gtbcwetuwr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shzxlz.cn/gtbakyfurp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jqgfzy.top/gtghfojqjb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinqigfzy.top/gtvigntsex.html

[N10] 链表节点定义
来源：http://hz.wangshuangyany.cn/gtvxmyivgt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shanyushiyangkeji.top/gtvnveskxm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ywan-chungtsiang.top/gtduhspxtd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hysaishi.cn/gtdcrqfmsh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tianlin.xyz/gtjimoeffh.html

Java: class Node { int v; Node next; }
来源：http://hz.havefunace.top/gtuzxkxwgp.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.9152youxi.cn/gthspovboe.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.dianchejie.cn/gtpupszlaa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hnqzz.top/gtbtvzcffb.html

[N11] 二叉树中序遍历
来源：http://hz.wangdashe.top/gtsfihwsuz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.fzhhl.top/gtioqdntwr.html

PHP:  // 手写递归函数
来源：http://hz.zhoulong.xyz/gtfzehxoxg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gzhubu.top/gtyqmkkitp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhongyouzk.top/gtszrngpyg.html

Java: // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtfbfxcjqd.html

Go:   // 手写递归
来源：http://hz.wangdashe.top/gtjgrkxtpq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.andypj.xyz/gtyfrmubcv.html

C#:   // 手写递归
来源：http://hz.guowangkeji.top/gtfzcaobbj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.chenlongwang.top/gtascxmtcd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zycfv.cn/gtyihlwwod.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.svipenyu.cn/gtzcgrigyy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hammf.cn/gthjgtrgiu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xylfe.cn/gtpagtquuo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.smart0.xyz/gtvchaezdz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenjidiqi.icu/gtszjcwxcu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shuidangran.top/gtarlxuxbm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jlsjyb.cn/gtnwzwxdpt.html

================================================================================
来源：http://hz.tianlin.xyz/gtwpunzibl.html

O. 并发与异步
来源：http://hz.zhiwuduotai.top/gtzgqbgwvd.html

================================================================================
来源：http://hz.yj202588.top/gtpeawnees.html

[O01] 启动一个线程
来源：http://hz.gzhubu.top/gtwwbycmsj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.fengsongda.top/gtymnnjgrk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.dianchejie.cn/gtmjbbgdjo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.daxiang520.top/gtsqqisazt.html

TS:   // 同 JS
来源：http://hz.cheryme.top/gtcyqrnyny.html

Java: new Thread(() -> f()).start()
来源：http://hz.mhx1999.top/gthfnfeort.html

Go:   go f()
来源：http://hz.tanke756.top/gtiolchmng.html

Ruby: Thread.new { f }
来源：http://hz.jinqigfzy.top/gtsuajqnme.html

C#:   Task.Run(() => F());
来源：http://hz.cheryme.top/gtjxytttls.html

[O02] 使用线程池
来源：http://hz.yj20258888.top/gtrbfptsva.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.bjfxy.top/gtlaszcewt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yuxming.cn/gtiqztgxfy.html

JS:   // worker_threads 线程池
来源：http://hz.c1oappe.top/gtzaunblcw.html

TS:   // worker_threads 线程池
来源：http://hz.yj202588.top/gtyvleovlh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.gotoacloud.top/gtiduskwet.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhengqikj.top/gtpapoprxq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhoulong.xyz/gtxykoenzv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gotoacloud.top/gtcrohrujr.html

[O03] 加锁保护共享数据
来源：http://hz.shuidangran.top/gtufpcaczo.html

Py:   with lock: shared += 1
来源：http://hz.snrcjt.cn/gtwcehmdwr.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.birdmap.top/gtpatjwsux.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.iojbl.cn/gtofwqayhn.html

TS:   // 同 JS
来源：http://hz.jianghu66.top/gtohsvkcyd.html

Java: synchronized (this) { shared++; }
来源：http://hz.dianchejie.cn/gtiujhrtrc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.tanke756.top/gtzmtecrfu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jyoumei.cn/gtgovvzrpr.html

C#:   lock (gate) { shared++; }
来源：http://hz.jinghuilouyu.cn/gtxkdjhhqi.html

[O04] 定义异步函数并等待
来源：http://hz.jiagoushi.top/gtskuwhuah.html

Py:   async def f():⏎    await g()
来源：http://hz.yuanzhike.top/gttiasozjb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sweek.top/gtvyykgvxd.html

JS:   async function f() { await g(); }
来源：http://hz.52xcode.cn/gtrfaaypkw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.nanxuanxn.top/gtorgewquv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jyoumei.cn/gtnzxranlr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jinghuilouyu.cn/gtrmtiqjjz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cashguo.top/gtnbjynrpw.html

C#:   async Task F() { await G(); }
来源：http://hz.zhengqikj.top/gtvxbrzazz.html

[O05] 并发执行并等待全部完成
来源：http://hz.svipenyu.cn/gtnqlelahq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.daria6918.cn/gtweywbkeb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jiagoushi.top/gtxznezfye.html

JS:   await Promise.all(tasks)
来源：http://hz.jianghu66.top/gtrynqtraq.html

TS:   await Promise.all(tasks)
来源：http://hz.shzxlz.cn/gtuqkjheex.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.0kj1m.cn/gtxfmwcdhe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zdqjudy.top/gtevxuzqxf.html

Ruby: threads.map(&:join)
来源：http://hz.jqgfzy.top/gtocrtiudu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.sweek.top/gtudjnqkuo.html

[O06] 使用进程池
来源：http://hz.feifeiyinyue.top/gtcaplonhu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yueranfly.top/gtwarysflb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yongpay.top/gtdtydegmd.html

JS:   // child_process / cluster 模块
来源：http://hz.guowangkeji.top/gtypcpceet.html

TS:   // child_process / cluster 模块
来源：http://hz.nanxuanxn.top/gtuidetpzh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.tian-w.cn/gtmxntfkrv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.sysykeji.top/gtjlqjjjoq.html

Ruby: // fork 块
来源：http://hz.redwolf501.top/gthqagtctl.html

C#:   Parallel.For
来源：http://hz.chenlongwang.top/gtvdpaasid.html

================================================================================
来源：http://hz.c1oappe.top/gtczwsepyy.html

P. 常用工具函数
来源：http://hz.hywenlv.cn/gtdgfhkxvs.html

================================================================================
来源：http://hz.xinyue.icu/gtdpbpcnoo.html

[P01] 生成 UUID
来源：http://hz.pengpengdd.cyou/gtxfjkphii.html

Py:   str(uuid.uuid4())
来源：http://hz.hnxiangtu.top/gtxpjdnuui.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jianghu66.top/gtbuebzjlk.html

JS:   crypto.randomUUID()
来源：http://hz.guowangkeji.top/gtqoeyvcef.html

TS:   crypto.randomUUID()
来源：http://hz.shanyushiyangkeji.top/gtmjaycxfx.html

Java: UUID.randomUUID().toString()
来源：http://hz.0kj1m.cn/gtcecioilz.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hnqzz.top/gtvobqhxeo.html

Ruby: SecureRandom.uuid
来源：http://hz.zhijiandao.cn/gtjcetsacy.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.gogol.net.cn/gtkipjcfbz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cdnleiting.top/gtkvjbipux.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.iojbl.cn/gtzozdtauw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.daxiang520.top/gtezmamiez.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xinyue.icu/gtkjdhoeul.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj20258888.top/gthhhcyvwk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ydzc1.top/gtptxggawp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.andypj.xyz/gtiwkbirer.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cashguo.top/gtrwcngxhu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cashguo.top/gttxqevhae.html

[P03] 生成短随机字符串
来源：http://hz.yanxiufei.cn/gtzxssphun.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.dianchejie.cn/gtmdrjzqmx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yvedp.cn/gtsdcobphf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hysaishi.cn/gtqhrkkcuy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.andypj.xyz/gtdcwystmr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinqigfzy.top/gtwcvbhtgp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.iojbl.cn/gtondsuyjr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sxryk.cn/gtpfrpfxul.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.fengsongda.top/gtatldjqzn.html

[P04] 求长度
来源：http://hz.dianchejie.cn/gtvrmftvam.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cucudq.cn/gtrjozgfkv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ivvv.top/gtommrqtag.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhaomingkeji.xyz/gtdraryfhm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shangyingyoupin.top/gtvxqtgjbl.html

Java: list.size();  map.size();  s.length()
来源：http://hz.pengpengdd.cyou/gtlbmaxxud.html

Go:   len(arr);  len(m)
来源：http://hz.sufxvd.cn/gtrthbrdxt.html

Ruby: x.length;  x.size
来源：http://hz.wangdashe.top/gtaadeoaks.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.redwolf501.top/gtbmvpbhwg.html

[P05] 判断两个对象内容是否相等
来源：http://hz.guannengcc.top/gtyqifbmtd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.wangshuangyany.cn/gtpuycrroa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.gogol.net.cn/gtofoacdmx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.tian-w.cn/gtyijgzitb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinyuanbaomall.cn/gtunisenzs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jianghu66.top/gttwseiwto.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hfpthk.cn/gtsmggxahk.html

Ruby: a == b
来源：http://hz.sufxvd.cn/gtydgmedap.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.daxiang520.top/gtognwsyzt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jianghu66.top/gtcujzaqzj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.redwolf501.top/gtdnzyzlyc.html

PHP:  if (empty($x)) {}
来源：http://hz.c1oappe.top/gtbhshuynb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yj20258.top/gttvpgzqmt.html

TS:   if (x == null) {}
来源：http://hz.yueranfly.top/gtepekieoo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.cashguo.top/gtmrzjutye.html

Go:   if x == nil {}
来源：http://hz.jlsjyb.cn/gtbysnypgj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhoulong.xyz/gthkrnenns.html

C#:   if (x is null) {}
来源：http://hz.zhijiandao.cn/gtpakodnnk.html

[P07] 防抖与节流
来源：http://hz.yueranfly.top/gtwjgqmwmf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.havefunace.top/gtkucmbteu.html

PHP:  // 手写时间戳比较
来源：http://hz.kuanghao11.cn/gtjahhkfmm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xziqi.cn/gtgojhcnmz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xingfuxueyuan.xyz/gtlwytspbl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.andypj.xyz/gtmypgzbfd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.aizwys.cn/gtstdknshn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.wangdashe.top/gtljaurxck.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cheryme.top/gtqrvgorxm.html

[P08] 处理浮点精度问题
来源：http://hz.zhaomingkeji.xyz/gtmboynxbh.html


<!-- 参考信息 -->