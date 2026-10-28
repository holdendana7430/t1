代发 wailian999

================================================================================
来源：http://hz.havefunace.top/gtvfesglwv.html

[M01] 读取命令行参数
来源：http://hz.sweek.top/gtaaocqctp.html

Py:   sys.argv[1:]
来源：http://hz.shanyushiyangkeji.top/gtizhriybo.html

PHP:  $argv;  $argc;
来源：http://hz.guowangkeji.top/gtjgwnqmij.html

JS:   process.argv.slice(2)
来源：http://hz.tianlin.xyz/gtcidqyeuj.html

TS:   process.argv.slice(2)
来源：http://hz.pycfn.com/gtmfkwxwtq.html

Java: args 数组（main 方法参数）
来源：http://hz.daria6918.cn/gtpqtnsktr.html

Go:   os.Args[1:]
来源：http://hz.ivvv.top/gtgvfzmmli.html

Ruby: ARGV
来源：http://hz.sufxvd.cn/gtvahgfukz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenzaomai.com/gteoqhwecw.html

[M02] 读取环境变量
来源：http://hz.zycfv.cn/gtfmfsjwdx.html

Py:   os.environ.get("HOME")
来源：http://hz.yonumen.top/gtqizafifi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yanxiufei.cn/gtxzgwdxku.html

JS:   process.env.HOME
来源：http://hz.hammf.cn/gtycesnjyl.html

TS:   process.env.HOME
来源：http://hz.zhijiandao.cn/gtygdrilvf.html

Java: System.getenv("HOME")
来源：http://hz.jinyuanbaomall.cn/gtcmmyffwm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shangyingyoupin.top/gtyibjaesk.html

Ruby: ENV["HOME"]
来源：http://hz.xylfe.cn/gtvhilkavq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hysaishi.cn/gtiupvnaaw.html

[M03] 执行外部命令
来源：http://hz.haohaochexian.top/gtkgrmjude.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.andypj.xyz/gtujvbksaa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gzhubu.top/gtcnzphlar.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shangyingyoupin.top/gtozonztsd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jyoumei.cn/gtjtzwmdlz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hnxiangtu.top/gtjfnqwcbh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hywenlv.cn/gtdqwjyryl.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.0kj1m.cn/gtmebishhk.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sweek.top/gtglhlkzcq.html

[M04] 获取当前工作目录
来源：http://hz.jinqigfzy.top/gtcwvqywok.html

Py:   os.getcwd()
来源：http://hz.tianlin.xyz/gtzpuotocj.html

PHP:  getcwd();
来源：http://hz.yonumen.top/gtfhkdlbhi.html

JS:   process.cwd()
来源：http://hz.zhijiandao.cn/gtyisruexd.html

TS:   process.cwd()
来源：http://hz.nwbrower.top/gtnmgcaatn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.birdmap.top/gtquhgxzao.html

Go:   os.Getwd()
来源：http://hz.cashguo.top/gtwpebfiod.html

Ruby: Dir.pwd
来源：http://hz.nwbrower.top/gtqniyddnx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sweek.top/gtskamcleb.html

[M05] 设置退出码
来源：http://hz.kuanghao11.cn/gthngmuhum.html

Py:   sys.exit(1)
来源：http://hz.andypj.xyz/gtfymflwkb.html

PHP:  exit(1);
来源：http://hz.andypj.xyz/gtvlhevjqu.html

JS:   process.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtqqbvdeap.html

TS:   process.exit(1)
来源：http://hz.smart0.xyz/gttbynjsng.html

Java: System.exit(1)
来源：http://hz.snrcjt.cn/gtzmxegcxl.html

Go:   os.Exit(1)
来源：http://hz.cashguo.top/gtfqhfltzw.html

Ruby: exit 1
来源：http://hz.hnxiangtu.top/gtrgkxwcra.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yongpay.top/gtwwhvcfae.html

[M06] 向标准错误输出
来源：http://hz.fengsongda.top/gtjtduufje.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jqgfzy.top/gtvmxckzfg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.pycfn.com/gtxksccaak.html

JS:   console.error("err")
来源：http://hz.gzhubu.top/gtvzlarfuy.html

TS:   console.error("err")
来源：http://hz.jqgfzy.top/gtjuckjsxh.html

Java: System.err.println("err")
来源：http://hz.mhx1999.top/gtwzxptjeu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xuetiantiany.cn/gtblixlpni.html

Ruby: warn "err"
来源：http://hz.gogol.net.cn/gtupymmlru.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.kuanghao11.cn/gtnarlofhi.html

[M07] 判断是否为主入口
来源：http://hz.hnxiangtu.top/gtcahyfrrk.html

Py:   if __name__ == "__main__":
来源：http://hz.xuanzx.com/gtdqiyhjkx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jqgufenzy.top/gtlauoywmg.html

JS:   require.main === module
来源：http://hz.hfpthk.cn/gtuivjqbpt.html

TS:   require.main === module
来源：http://hz.quarkkingdee.top/gttmbsgmng.html

Java: public static void main(String[] args)
来源：http://hz.redwolf501.top/gtlsaxqvii.html

Go:   func main()
来源：http://hz.cashguo.top/gtgfixtwgr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jqgufenzy.top/gtebisveqy.html

C#:   static void Main(string[] args)
来源：http://hz.hnqzz.top/gtzcktunyd.html

[M08] 获取系统与运行时信息
来源：http://hz.pengpengdd.cyou/gtnjosumvp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.nanxinkj.top/gtsyxsaifw.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenjidiqi.icu/gthvpukenh.html

JS:   process.platform;  process.version
来源：http://hz.9152youxi.cn/gtygxmmgvo.html

TS:   process.platform;  process.version
来源：http://hz.yj20258888.top/gtlawzgasm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hnxiangtu.top/gtoesjqfqb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.tanke756.top/gtvoiyihha.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.fzhhl.top/gtajjtsjyc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jlsjyb.cn/gtufzeqllc.html

================================================================================
来源：http://hz.jqgufenzy.top/gtvtinpkic.html

N. 数据结构与算法
来源：http://hz.zhaomingkeji.xyz/gtzwrohrpy.html

================================================================================
来源：http://hz.birdmap.top/gtnzyfdzmk.html

[N01] 二分查找（有序数组）
来源：http://hz.yj20258.top/gtrtcdzzhi.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hysaishi.cn/gtdpyulbsg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.chenlongwang.top/gtakdvsvhz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.andypj.xyz/gtvsukphrd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sxryk.cn/gtmbqqrlro.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jqgufenzy.top/gtwvceirgc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.aibaodan.cn/gthiencmxu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.0kj1m.cn/gtuvgqwkpm.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ybcxt.top/gtenaudlcg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.feifeiyinyue.top/gtafhwmwkm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tianlin.xyz/gtzwscrrjl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hnxiangtu.top/gthmkvzwqp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhengqikj.top/gtkjbasran.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangkeji.top/gttshqmoxx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.haohaochexian.top/gtnhhhzbcr.html

Go:   slices.Sort(arr)
来源：http://hz.zhengqikj.top/gthlivxtvd.html

Ruby: arr.sort
来源：http://hz.jinqigufen.top/gtziipppwf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.pengpengdd.cyou/gtxhlwsqwk.html

[N03] 快速排序（分治示例）
来源：http://hz.ydjk.org.cn/gtvnlmjcny.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yuxming.cn/gtjjhmkjoz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhixingplan.top/gtljpnytzo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yonumen.top/gtpoookyti.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nwbrower.top/gtvbulvsrz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tanke756.top/gtigtdptfu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.vqdsnc.cn/gtxarjbxsf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shanyushiyangkeji.top/gtfssxrnuy.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xziqi.cn/gtfrzwsnru.html

[N04] 斐波那契数列
来源：http://hz.zhijiandao.cn/gtdbyozkse.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.gotoacloud.top/gtdfqnueqw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.gogol.net.cn/gthytyjfsn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dianchejie.cn/gtpjqgseiy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigfzy.top/gtjytjeapy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gaohongyu789.top/gtfsklszzt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.aibaodan.cn/gtpvyzmcww.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.guowangkeji.top/gtlhsymqaj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.wangdashe.top/gtlkthaahf.html

[N05] 最大公约数
来源：http://hz.daria6918.cn/gtwlqiomqy.html

Py:   math.gcd(a, b)
来源：http://hz.hnqzz.top/gtogqedsse.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ywan-chungtsiang.top/gtmulyrpfd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xylfe.cn/gtwmtbnplr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinghuilouyu.cn/gtxyvjrpqi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.smart0.xyz/gtlbhywjjv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.wangshuangyany.cn/gtcefjqrtt.html

Ruby: a.gcd(b)
来源：http://hz.yonumen.top/gtlnvuerzp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.sweek.top/gtevayzyjs.html

[N06] 判断回文字符串
来源：http://hz.yuanzhike.top/gteguzezbu.html

Py:   s == s[::-1]
来源：http://hz.jinqigufen.top/gtevfupece.html

PHP:  $s === strrev($s);
来源：http://hz.iojbl.cn/gtyphompru.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhijiandao.cn/gtxigeklsd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zycfv.cn/gtaooqnnjy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yvedp.cn/gtvynbyijv.html

Go:   // 双指针从两端比较
来源：http://hz.wangshuangyany.cn/gtvwvwgfem.html

Ruby: s == s.reverse
来源：http://hz.snrcjt.cn/gtjrnceznz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jqgufenzy.top/gtaawgganb.html

[N07] 两数之和（返回下标）
来源：http://hz.cheryme.top/gtsofwckhz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yuxming.cn/gtwikvmkrp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.52xcode.cn/gtniakcnan.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.iojbl.cn/gtkxgaefct.html

TS:   // 手写 Map<string, number>
来源：http://hz.feifeiyinyue.top/gtfgemonot.html

Java: // 手写 HashMap
来源：http://hz.zhiwuduotai.top/gtxvphwutt.html

Go:   // 手写 map[int]int
来源：http://hz.jiagoushi.top/gtglhtzcsh.html

Ruby: // 手写 Hash
来源：http://hz.nanxinkj.top/gtjllznvzh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.bjfxy.top/gtybjifroi.html

[N08] 生成全排列
来源：http://hz.meibo888.top/gtsarxfbrc.html

Py:   itertools.permutations(arr)
来源：http://hz.gzhubu.top/gtjcefadfw.html

PHP:  // 手写递归交换
来源：http://hz.shanyushiyangkeji.top/gtkiuhrult.html

JS:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtvrdpvzkk.html

TS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtymgqamnb.html

Java: // 手写回溯递归
来源：http://hz.jiagoushi.top/gtudllyidh.html

Go:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtcsnqoqzi.html

Ruby: arr.permutation.to_a
来源：http://hz.guowangkeji.top/gtxuuurwfm.html

C#:   // 手写回溯递归
来源：http://hz.yj202588.top/gthftgrjby.html

[N09] 栈与队列
来源：http://hz.cheryme.top/gtmmaovlgj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.gogol.net.cn/gtogzmmesi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinyuanbaomall.cn/gtcjewezsm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.pycfn.com/gtmqazpjps.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinqigfzy.top/gtavyxhioe.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zdqjudy.top/gtcslawiml.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.meibo888.top/gtokrmvwws.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhoulong.xyz/gtzlaiohwr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yj20258.top/gtxfwmzrzz.html

[N10] 链表节点定义
来源：http://hz.daxiang520.top/gtbgfdxagd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xziqi.cn/gtwvursokh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.quarkkingdee.top/gtuxtjhgvk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yueranfly.top/gtoiziilun.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gaohongyu789.top/gtcweigwye.html

Java: class Node { int v; Node next; }
来源：http://hz.hnxiangtu.top/gtadyrtddm.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinghuilouyu.cn/gtsptvjfji.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hysaishi.cn/gtjxybffpr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xuetiantiany.cn/gtwaxkhzmf.html

[N11] 二叉树中序遍历
来源：http://hz.hammf.cn/gtpotbgdzm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.redwolf501.top/gtwzvimsyz.html

PHP:  // 手写递归函数
来源：http://hz.gzhubu.top/gtarxszhxx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cucudq.cn/gtbpbxweei.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.havefunace.top/gtjpsyabxw.html

Java: // 手写递归
来源：http://hz.zhixingplan.top/gtjtwftvro.html

Go:   // 手写递归
来源：http://hz.yj202588.top/gtxqfbqneb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ppjwa.cn/gtvxzhddcb.html

C#:   // 手写递归
来源：http://hz.tianlin.xyz/gtkgabiguy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.kuanghao11.cn/gtoawfmlkw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.sysykeji.top/gtkpifsztl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jyoumei.cn/gtndqjlike.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cdnleiting.top/gtassjtccm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shzxlz.cn/gtngczgspa.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.meibo888.top/gtwnrrazde.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.cdnleiting.top/gtktrlrqcv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.gotoacloud.top/gtwhbhcpcq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhaomingkeji.xyz/gtognankrb.html

================================================================================
来源：http://hz.hfpthk.cn/gtdsjgjpul.html

O. 并发与异步
来源：http://hz.yueranfly.top/gtwzsotwuw.html

================================================================================
来源：http://hz.andypj.xyz/gtpwzdfokh.html

[O01] 启动一个线程
来源：http://hz.xziqi.cn/gtkalmflvv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cqqwz.cn/gtgkomvyxd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinghuilouyu.cn/gthvjmhnwj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.daria6918.cn/gtvixghftm.html

TS:   // 同 JS
来源：http://hz.ppjwa.cn/gtxmupnjyo.html

Java: new Thread(() -> f()).start()
来源：http://hz.redwolf501.top/gtvsqpqign.html

Go:   go f()
来源：http://hz.pengpengdd.cyou/gtqjftroat.html

Ruby: Thread.new { f }
来源：http://hz.andypj.xyz/gtavrroquy.html

C#:   Task.Run(() => F());
来源：http://hz.shzxlz.cn/gtayogwwmi.html

[O02] 使用线程池
来源：http://hz.yuanzhike.top/gtorwkshrz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xuanzx.com/gtrnbyjgjb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shuidangran.top/gtytiyeyqv.html

JS:   // worker_threads 线程池
来源：http://hz.jlsjyb.cn/gtgxzggsra.html

TS:   // worker_threads 线程池
来源：http://hz.hammf.cn/gtxonqcvjb.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.nanxuanxn.top/gtymequspb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hammf.cn/gthgracrda.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.0kj1m.cn/gtfivuztlq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ehwqpu.com/gtqkyfaigy.html

[O03] 加锁保护共享数据
来源：http://hz.jinghuilouyu.cn/gtzzvvmjiu.html

Py:   with lock: shared += 1
来源：http://hz.jinyuanbaomall.cn/gttibzhckx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.feifeiyinyue.top/gtmmnllvcw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ywan-chungtsiang.top/gtdnteutqq.html

TS:   // 同 JS
来源：http://hz.316326.xyz/gtenmhzsus.html

Java: synchronized (this) { shared++; }
来源：http://hz.tian-w.cn/gtgfmboein.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.smart0.xyz/gtymeijgas.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xingfuxueyuan.xyz/gtugowkydb.html

C#:   lock (gate) { shared++; }
来源：http://hz.nwbrower.top/gtjggkfcyv.html

[O04] 定义异步函数并等待
来源：http://hz.yj20258.top/gtojywjboq.html

Py:   async def f():⏎    await g()
来源：http://hz.meibo888.top/gtawtwwcwk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ydjk.org.cn/gtnnqswkbk.html

JS:   async function f() { await g(); }
来源：http://hz.yanxiufei.cn/gteaaiaivr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhiwuduotai.top/gtppdenbhk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jqgfzy.top/gtghaoxzbh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xuanzx.com/gteilnxaoq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhoulong.xyz/gtyckbiiud.html

C#:   async Task F() { await G(); }
来源：http://hz.yj20258888.top/gtwynztqqq.html

[O05] 并发执行并等待全部完成
来源：http://hz.hongshengwenyu.top/gtzhtfjgti.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gogol.net.cn/gtcfwpxhym.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xuanzx.com/gteipxpfok.html

JS:   await Promise.all(tasks)
来源：http://hz.hnqzz.top/gtugdooeyi.html

TS:   await Promise.all(tasks)
来源：http://hz.jinghuilouyu.cn/gtsaoviers.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cdnleiting.top/gtnocgemlk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hnqzz.top/gtayotigxb.html

Ruby: threads.map(&:join)
来源：http://hz.redwolf501.top/gtvoivmumj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinqigufen.top/gtwutoenso.html

[O06] 使用进程池
来源：http://hz.cdnleiting.top/gthzcufjbz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yj20258888.top/gtstyibres.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.andypj.xyz/gtxwrkcnul.html

JS:   // child_process / cluster 模块
来源：http://hz.daria6918.cn/gtwvmwygao.html

TS:   // child_process / cluster 模块
来源：http://hz.jqgufenzy.top/gtcgwroerp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xuetiantiany.cn/gtgrbtnqgj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yj20258888.top/gtwbxzbzdo.html

Ruby: // fork 块
来源：http://hz.wangdashe.top/gtbxoklggs.html

C#:   Parallel.For
来源：http://hz.jinyuanbaomall.cn/gtigzmgajo.html

================================================================================
来源：http://hz.cqqwz.cn/gtansdkifs.html

P. 常用工具函数
来源：http://hz.haohaochexian.top/gtjsejyuvw.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtqggcwwfm.html

[P01] 生成 UUID
来源：http://hz.jianghu66.top/gtsqabuscm.html

Py:   str(uuid.uuid4())
来源：http://hz.cdnleiting.top/gtlzzqviyj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.aibaodan.cn/gtbgtmwguq.html

JS:   crypto.randomUUID()
来源：http://hz.dianchejie.cn/gtlmkrbwzd.html

TS:   crypto.randomUUID()
来源：http://hz.316326.xyz/gtglllxxzt.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhoulong.xyz/gtvjoowael.html

Go:   // 用 github.com/google/uuid
来源：http://hz.smart0.xyz/gtwyxhmwwh.html

Ruby: SecureRandom.uuid
来源：http://hz.jinyuanbaomall.cn/gtrguicsvw.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.svipenyu.cn/gtgxdcahnu.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yanxiufei.cn/gtcptscjfy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jinyuanbaomall.cn/gtdxesybaq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.aibaodan.cn/gtxkysmfjx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gaohongyu789.top/gtpuoqaflw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gotoacloud.top/gtzyzpkhoy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hywenlv.cn/gtglmpyefv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhijiandao.cn/gtoucnneec.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhaomingkeji.xyz/gtnblorxpg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zycfv.cn/gtnmrqpnzw.html

[P03] 生成短随机字符串
来源：http://hz.zycfv.cn/gtktcstrfe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhongyouzk.top/gteexxyjip.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ppjwa.cn/gtmfetnmwb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shangyingyoupin.top/gtcdplzjqj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.daria6918.cn/gtvjcijxjc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yangfankeji.com/gtqawldlod.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.tanke756.top/gttcucxcpq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xinyue.icu/gtjbdkoraa.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cashguo.top/gtaugvstlf.html

[P04] 求长度
来源：http://hz.snrcjt.cn/gtkdxeadel.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.guannengcc.top/gtwhqhyeqy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xinyue.icu/gtqbzivxwr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.svipenyu.cn/gtllghsqwl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yueranfly.top/gtvtqtmbpl.html

Java: list.size();  map.size();  s.length()
来源：http://hz.tanke756.top/gtcrvttcun.html

Go:   len(arr);  len(m)
来源：http://hz.mhx1999.top/gtusdtlwuz.html

Ruby: x.length;  x.size
来源：http://hz.dashuyun.cn/gtqvfzotjv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shanyushiyangtech.top/gtysongncp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sysykeji.top/gtozwalcst.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.nwbrower.top/gterucdzom.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.wangdashe.top/gtxriuseun.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shzxlz.cn/gtdslvdjua.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ywan-chungtsiang.top/gtfondokop.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yongpay.top/gtgyloonnp.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.sufxvd.cn/gtpnvhqcwb.html

Ruby: a == b
来源：http://hz.ywan-chungtsiang.top/gtfbvsihmn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xinyue.icu/gtbvpzhrvs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tanke756.top/gtrroluzfg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.gogol.net.cn/gtqrwyoois.html

PHP:  if (empty($x)) {}
来源：http://hz.jqgufenzy.top/gtpzcnpcos.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhongyouzk.top/gtdgqisgam.html

TS:   if (x == null) {}
来源：http://hz.sxryk.cn/gtstozqazq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhongyouzk.top/gttyahnqxz.html

Go:   if x == nil {}
来源：http://hz.birdmap.top/gtnssdszah.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.chenzaomai.com/gthlyxkjde.html

C#:   if (x is null) {}
来源：http://hz.ydjk.org.cn/gtmupyqiay.html

[P07] 防抖与节流
来源：http://hz.feifeiyinyue.top/gtncoylpyr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinyuanbaomall.cn/gtikbttpoh.html


<!-- 参考信息 -->