代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jqgfzy.top/gtbslirrkf.html

JS:   process.env.HOME
来源：http://hz.xylfe.cn/gtksqtkblt.html

TS:   process.env.HOME
来源：http://hz.hywenlv.cn/gtmfdqmnwe.html

Java: System.getenv("HOME")
来源：http://hz.chenjidiqi.icu/gtqdpjsakk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xingfuxueyuan.xyz/gtnpvccnhw.html

Ruby: ENV["HOME"]
来源：http://hz.jianghu66.top/gteekdxoxg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.aizwys.cn/gtjiedvozk.html

[M03] 执行外部命令
来源：http://hz.shanyushiyangtech.top/gtxvxyzqcd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jlsjyb.cn/gtivlbptmv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ybcxt.top/gtibvhmaek.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydjk.org.cn/gtfrzrxeby.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yanxiufei.cn/gtabmzthue.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.andypj.xyz/gtcgcvfknr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jinyuanbaomall.cn/gteguoclwy.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.smart0.xyz/gtpdldosnq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ydjk.org.cn/gtonarqizg.html

[M04] 获取当前工作目录
来源：http://hz.zhijiandao.cn/gthqtrjagt.html

Py:   os.getcwd()
来源：http://hz.hammf.cn/gtrrltzhys.html

PHP:  getcwd();
来源：http://hz.52xcode.cn/gtmggvrfna.html

JS:   process.cwd()
来源：http://hz.aizwys.cn/gtndgzhlrb.html

TS:   process.cwd()
来源：http://hz.dianchejie.cn/gtjckdzbaf.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zycfv.cn/gtmoxqheyq.html

Go:   os.Getwd()
来源：http://hz.hnqzz.top/gtenphlinf.html

Ruby: Dir.pwd
来源：http://hz.gotoacloud.top/gtstfewnqu.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hywenlv.cn/gtioilgasp.html

[M05] 设置退出码
来源：http://hz.zhaomingkeji.xyz/gtnrewbhdx.html

Py:   sys.exit(1)
来源：http://hz.zhoulong.xyz/gtyihxlyvn.html

PHP:  exit(1);
来源：http://hz.dianchejie.cn/gtvbbeyjnp.html

JS:   process.exit(1)
来源：http://hz.zycfv.cn/gtfreqansb.html

TS:   process.exit(1)
来源：http://hz.iojbl.cn/gtvaqjqrsk.html

Java: System.exit(1)
来源：http://hz.birdmap.top/gtfcysghft.html

Go:   os.Exit(1)
来源：http://hz.jinqigfzy.top/gtpoumliai.html

Ruby: exit 1
来源：http://hz.yj20258888.top/gtymmnrtkt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shanyushiyangkeji.top/gtxtieeudx.html

[M06] 向标准错误输出
来源：http://hz.ybcxt.top/gtklhstutp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yanxiufei.cn/gtnhtvdukv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jianghu66.top/gtykdnnjrc.html

JS:   console.error("err")
来源：http://hz.guannengcc.top/gtbymdexzk.html

TS:   console.error("err")
来源：http://hz.jinqigufen.top/gtnmuosfwh.html

Java: System.err.println("err")
来源：http://hz.52xcode.cn/gtqtobmnbz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.havefunace.top/gtllmiipvl.html

Ruby: warn "err"
来源：http://hz.nwbrower.top/gtuljuuqqt.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jlsjyb.cn/gtzygfhlzr.html

[M07] 判断是否为主入口
来源：http://hz.tianlin.xyz/gtpybegapu.html

Py:   if __name__ == "__main__":
来源：http://hz.yuanzhike.top/gtyxgesbfi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhaomingkeji.xyz/gtkrocrpmc.html

JS:   require.main === module
来源：http://hz.yangfankeji.com/gtlureznmw.html

TS:   require.main === module
来源：http://hz.meibo888.top/gteurklvyb.html

Java: public static void main(String[] args)
来源：http://hz.zhixingplan.top/gtnqnccifj.html

Go:   func main()
来源：http://hz.fzhhl.top/gtvvrwqujq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.gzhubu.top/gtpizuyuou.html

C#:   static void Main(string[] args)
来源：http://hz.nwbrower.top/gtqyhxvpcx.html

[M08] 获取系统与运行时信息
来源：http://hz.ivvv.top/gtzvyergzt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.quarkkingdee.top/gtqpfanqdt.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gogol.net.cn/gtkbovewmi.html

JS:   process.platform;  process.version
来源：http://hz.hammf.cn/gtepcdjsbq.html

TS:   process.platform;  process.version
来源：http://hz.iojbl.cn/gtkjptwulc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.quarkkingdee.top/gtvdhcvmaf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.nwbrower.top/gtrpidccwz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.nwbrower.top/gtdqxoyuit.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jqgfzy.top/gtnvnyypbt.html

================================================================================
来源：http://hz.9152youxi.cn/gtdtfcrpua.html

N. 数据结构与算法
来源：http://hz.gogol.net.cn/gtnzjcrtzf.html

================================================================================
来源：http://hz.haohaochexian.top/gtihnlotnm.html

[N01] 二分查找（有序数组）
来源：http://hz.hfpthk.cn/gtvfykcffy.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.chenlongwang.top/gtiyrbdjuc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shanyushiyangtech.top/gtgomwazzk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xingfuxueyuan.xyz/gtpdbctruw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.kuanghao11.cn/gtmuxrpefd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhixingplan.top/gtlaxuswdg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shzxlz.cn/gtzpwfsvyw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.chenlongwang.top/gtkvzervyq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hammf.cn/gtgftoknso.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ybcxt.top/gtvktksqey.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sufxvd.cn/gtskxbgftb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.gogol.net.cn/gtnqjbzncf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuanzhike.top/gtnazzdjzc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangkeji.top/gtnxjhkjwg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ivvv.top/gtazophveh.html

Go:   slices.Sort(arr)
来源：http://hz.yj20258888.top/gtozelecax.html

Ruby: arr.sort
来源：http://hz.jqgufenzy.top/gtlsycvgxm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xziqi.cn/gtjzonknnt.html

[N03] 快速排序（分治示例）
来源：http://hz.gotoacloud.top/gtabyurbxo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cheryme.top/gtmrnjmcbt.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hnxiangtu.top/gtymqrpbkl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhongyouzk.top/gthppplpbx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.316326.xyz/gttaahpcqi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hnxiangtu.top/gtbpmrmbib.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.chenlongwang.top/gthdvwodbc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hfpthk.cn/gtalveedwo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.9152youxi.cn/gtaeavhmhl.html

[N04] 斐波那契数列
来源：http://hz.yanxiufei.cn/gteswdjvur.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zycfv.cn/gthyuywsrv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cqqwz.cn/gtkxswwhwm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenzaomai.com/gtgejfiins.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ehwqpu.com/gtniztpjmn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cqqwz.cn/gtgoqwwcxm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.dianchejie.cn/gtzrepldwa.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhiwuduotai.top/gtysscdjpy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinqigufen.top/gtzriypblq.html

[N05] 最大公约数
来源：http://hz.zhoulong.xyz/gtbsrwmtkf.html

Py:   math.gcd(a, b)
来源：http://hz.xuetiantiany.cn/gtbmjhpxlc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.316326.xyz/gtcprmnutt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhaomingkeji.xyz/gtsxmsvuym.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ybcxt.top/gtoimhnuxm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gogol.net.cn/gtahxngjla.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hysaishi.cn/gtzuyjsfse.html

Ruby: a.gcd(b)
来源：http://hz.havefunace.top/gtqtedyxte.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ywan-chungtsiang.top/gtvxnirqxx.html

[N06] 判断回文字符串
来源：http://hz.xuetiantiany.cn/gtrbcxriok.html

Py:   s == s[::-1]
来源：http://hz.xylfe.cn/gtsmxrfpid.html

PHP:  $s === strrev($s);
来源：http://hz.cheryme.top/gtpkenowxk.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ywan-chungtsiang.top/gtjwasuvhg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.mhx1999.top/gtxddbmotj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.52xcode.cn/gtoajzhwgz.html

Go:   // 双指针从两端比较
来源：http://hz.yj202588.top/gtqspjdxte.html

Ruby: s == s.reverse
来源：http://hz.xziqi.cn/gtccenwzhx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tian-w.cn/gtxnjcxyee.html

[N07] 两数之和（返回下标）
来源：http://hz.zhiwuduotai.top/gtejvlnzde.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yuxming.cn/gtxxcdapkl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xinyue.icu/gtlqpsixex.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.cqqwz.cn/gtqcstqtiz.html

TS:   // 手写 Map<string, number>
来源：http://hz.yongpay.top/gtfdavpogb.html

Java: // 手写 HashMap
来源：http://hz.jqgfzy.top/gtexojynno.html

Go:   // 手写 map[int]int
来源：http://hz.yanxiufei.cn/gtyusrftcc.html

Ruby: // 手写 Hash
来源：http://hz.chenzaomai.com/gtsnghcwxw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.316326.xyz/gtusckboaz.html

[N08] 生成全排列
来源：http://hz.ydjk.org.cn/gtbjbfiits.html

Py:   itertools.permutations(arr)
来源：http://hz.gogol.net.cn/gttwkkqkbr.html

PHP:  // 手写递归交换
来源：http://hz.yj20258888.top/gtljwcsdxt.html

JS:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtgsveufxa.html

TS:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtyizbazja.html

Java: // 手写回溯递归
来源：http://hz.jinqigufen.top/gtawanxayt.html

Go:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtrhkxevhj.html

Ruby: arr.permutation.to_a
来源：http://hz.birdmap.top/gtejhlwgrw.html

C#:   // 手写回溯递归
来源：http://hz.wangdashe.top/gttihplmjc.html

[N09] 栈与队列
来源：http://hz.sxryk.cn/gtdwpwboyh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.dashuyun.cn/gtintrwbww.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xziqi.cn/gtoxdhklyq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.sxryk.cn/gtpadbxxxh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj20258888.top/gtcsihussg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yvedp.cn/gtuyjlvyme.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhengqikj.top/gtelvuvpsp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhaomingkeji.xyz/gtatyupnef.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.52xcode.cn/gtuxydwrgf.html

[N10] 链表节点定义
来源：http://hz.yonumen.top/gtkwdccccn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cqqwz.cn/gtyklegvjr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.redwolf501.top/gtuwvvgasw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.iojbl.cn/gtfltcmmvd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.haohaochexian.top/gtetzvutoy.html

Java: class Node { int v; Node next; }
来源：http://hz.yangfankeji.com/gtktjvyxhs.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yj20258888.top/gtlefykgax.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hnxiangtu.top/gtfhcxrzsi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yonumen.top/gtpjudwdnz.html

[N11] 二叉树中序遍历
来源：http://hz.gogol.net.cn/gtjvpitwff.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.52xcode.cn/gtkmmtjldo.html

PHP:  // 手写递归函数
来源：http://hz.bjfxy.top/gtprfdslyl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnqzz.top/gtmghsbdoo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cashguo.top/gtzoqppzoa.html

Java: // 手写递归
来源：http://hz.jianghu66.top/gtkmegniqw.html

Go:   // 手写递归
来源：http://hz.chenlongwang.top/gtryiowlhn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.pycfn.com/gtyxzcbmna.html

C#:   // 手写递归
来源：http://hz.nanxuanxn.top/gtfgyquohn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ydzc1.top/gtjryubwgx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.wangdashe.top/gtlcuixzpe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jianghu66.top/gtbsyrheqy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zdqjudy.top/gtasrnjsfl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.guowangkeji.top/gtokoepeuu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guannengcc.top/gteabidwts.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jinqigufen.top/gttjpscjop.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cucudq.cn/gtxgjjywcy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.0kj1m.cn/gtumgmfxhd.html

================================================================================
来源：http://hz.daxiang520.top/gtkkooexnd.html

O. 并发与异步
来源：http://hz.xuanzx.com/gtruaulbkz.html

================================================================================
来源：http://hz.yj20258.top/gtqeuytsqw.html

[O01] 启动一个线程
来源：http://hz.tanke756.top/gtwbdurghf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.c1oappe.top/gtlytvmiol.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhixingplan.top/gthpitziqq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cashguo.top/gtvrrnjvbt.html

TS:   // 同 JS
来源：http://hz.mhx1999.top/gtjlwjymbm.html

Java: new Thread(() -> f()).start()
来源：http://hz.yonumen.top/gtgluinmjz.html

Go:   go f()
来源：http://hz.c1oappe.top/gticzrnivi.html

Ruby: Thread.new { f }
来源：http://hz.yuxming.cn/gtwalticqf.html

C#:   Task.Run(() => F());
来源：http://hz.hfpthk.cn/gtqvspnmol.html

[O02] 使用线程池
来源：http://hz.hnxiangtu.top/gtywpphazq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.feifeiyinyue.top/gtpmmpzbmn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.gzhubu.top/gtcxipnxzx.html

JS:   // worker_threads 线程池
来源：http://hz.sufxvd.cn/gtitelysdi.html

TS:   // worker_threads 线程池
来源：http://hz.gotoacloud.top/gtheblesdf.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhiwuduotai.top/gtqfvbcgbv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.havefunace.top/gtnjdsuidt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zdqjudy.top/gtvlbhrvat.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.svipenyu.cn/gtlymowoch.html

[O03] 加锁保护共享数据
来源：http://hz.cashguo.top/gttgiocpei.html

Py:   with lock: shared += 1
来源：http://hz.gaohongyu789.top/gtgecncbys.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.daria6918.cn/gthymnmgxe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jyoumei.cn/gtuxpvjuug.html

TS:   // 同 JS
来源：http://hz.jinghuilouyu.cn/gthyicoudg.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhongyouzk.top/gthrzvpwlu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.smart0.xyz/gtipspwjlh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.guannengcc.top/gtnlsxbwyo.html

C#:   lock (gate) { shared++; }
来源：http://hz.aizwys.cn/gtmbfjfgwh.html

[O04] 定义异步函数并等待
来源：http://hz.redwolf501.top/gtbgvaiyab.html

Py:   async def f():⏎    await g()
来源：http://hz.ehwqpu.com/gtwffpwvmi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.redwolf501.top/gtuahmfrgh.html

JS:   async function f() { await g(); }
来源：http://hz.daxiang520.top/gtbuvbxmck.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hywenlv.cn/gtbeasabff.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cdnleiting.top/gtrwzvkldp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.kuanghao11.cn/gtkthnsesv.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hnqzz.top/gtozkbeqhv.html

C#:   async Task F() { await G(); }
来源：http://hz.dianchejie.cn/gtnpzcggna.html

[O05] 并发执行并等待全部完成
来源：http://hz.ivvv.top/gtvgxbpeot.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gzhubu.top/gtmfjtkvvs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.sxryk.cn/gtxrtyttgf.html

JS:   await Promise.all(tasks)
来源：http://hz.zhijiandao.cn/gtftcrzjbs.html

TS:   await Promise.all(tasks)
来源：http://hz.9152youxi.cn/gtkcxzwlik.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.52xcode.cn/gtzfsyuqvl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sweek.top/gtlxrpznfg.html

Ruby: threads.map(&:join)
来源：http://hz.yj202588.top/gtegfbyuva.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.mhx1999.top/gtteuvqveu.html

[O06] 使用进程池
来源：http://hz.zdqjudy.top/gtejxdvvpy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yj20258.top/gtwsaourma.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.meibo888.top/gtrvtnrjuu.html

JS:   // child_process / cluster 模块
来源：http://hz.gaohongyu789.top/gtkjiwxbew.html

TS:   // child_process / cluster 模块
来源：http://hz.birdmap.top/gtafctigdd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhijiandao.cn/gtiusumzpv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.daria6918.cn/gtqxpalkdp.html

Ruby: // fork 块
来源：http://hz.ydjk.org.cn/gtelmaoxwh.html

C#:   Parallel.For
来源：http://hz.pycfn.com/gtwfjbkemr.html

================================================================================
来源：http://hz.sysykeji.top/gtfuifsjwb.html

P. 常用工具函数
来源：http://hz.yuanzhike.top/gtrtdulyii.html

================================================================================
来源：http://hz.havefunace.top/gtelrgvuvz.html

[P01] 生成 UUID
来源：http://hz.9152youxi.cn/gtrottbrpv.html

Py:   str(uuid.uuid4())
来源：http://hz.shanyushiyangtech.top/gtperekksv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ybcxt.top/gteocsiviz.html

JS:   crypto.randomUUID()
来源：http://hz.sweek.top/gtvhjusbin.html

TS:   crypto.randomUUID()
来源：http://hz.jinqigfzy.top/gtbhwopvwu.html

Java: UUID.randomUUID().toString()
来源：http://hz.pengpengdd.cyou/gtzkyorwbp.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shzxlz.cn/gtfqhlubmd.html

Ruby: SecureRandom.uuid
来源：http://hz.yj202588.top/gtoxzvyzee.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.gzhubu.top/gtdngxxhva.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ydjk.org.cn/gtujaqvedc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.iojbl.cn/gtyyyacngi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xylfe.cn/gtdnpnhxmk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.chenlongwang.top/gtfonnavtn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gzhubu.top/gtxfrfgife.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.guannengcc.top/gtdfanglsa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cdnleiting.top/gtgbsmhkxb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.meibo888.top/gtspoblgja.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.havefunace.top/gtyozijklh.html

[P03] 生成短随机字符串
来源：http://hz.zycfv.cn/gtqrynvaeh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhiwuduotai.top/gtfpubwaif.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jqgufenzy.top/gtlohpjvpy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shangyingyoupin.top/gtjjgyvrxz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.havefunace.top/gtpzypyzwf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.aizwys.cn/gtfvgmcsfq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hysaishi.cn/gttemnwksp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.tian-w.cn/gtngdqxyme.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.daria6918.cn/gtttlswkeg.html

[P04] 求长度
来源：http://hz.meibo888.top/gtnujbtdcl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hammf.cn/gtjopqyhmz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtxwbttbqv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.9152youxi.cn/gtvuyzwdcs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.tian-w.cn/gtdgwcmhgb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sysykeji.top/gtpiigtsvn.html

Go:   len(arr);  len(m)
来源：http://hz.smart0.xyz/gtyezwqnrs.html

Ruby: x.length;  x.size
来源：http://hz.tanke756.top/gtilbnjzqt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xziqi.cn/gtwhealqjh.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shanyushiyangkeji.top/gttribiukf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.birdmap.top/gtpvizdzjj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xinyue.icu/gtpcfbkohy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.52xcode.cn/gtfdsigemo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tianlin.xyz/gtpvidplzz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinqigufen.top/gtvpuvrjew.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shangyingyoupin.top/gtdptvlwfz.html

Ruby: a == b
来源：http://hz.wangdashe.top/gtynkpecmd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinghuilouyu.cn/gtozcpwhar.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cdnleiting.top/gtkaqqkfza.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shangyingyoupin.top/gtadbwpxcc.html

PHP:  if (empty($x)) {}
来源：http://hz.wangdashe.top/gtuszuglia.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.c1oappe.top/gtidjaqeye.html

TS:   if (x == null) {}
来源：http://hz.xuanzx.com/gtczsewwik.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.kuanghao11.cn/gtbpfedfyb.html

Go:   if x == nil {}
来源：http://hz.yonumen.top/gtyobscdvy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.chenlongwang.top/gtgnxvnrsm.html

C#:   if (x is null) {}
来源：http://hz.dashuyun.cn/gtooqkjltm.html

[P07] 防抖与节流
来源：http://hz.aizwys.cn/gtqadcugnl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hfpthk.cn/gtqdmlhixf.html

PHP:  // 手写时间戳比较
来源：http://hz.jianghu66.top/gttfadtato.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sufxvd.cn/gtsqayuouo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.kuanghao11.cn/gttlycizgd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jqgfzy.top/gtezlgmerd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yanxiufei.cn/gtkyonsqgy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.meibo888.top/gtvqutfenw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.svipenyu.cn/gtmbqcrjoe.html

[P08] 处理浮点精度问题
来源：http://hz.zycfv.cn/gtkjprbfbp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.dianchejie.cn/gtxndqrsvp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinqigufen.top/gteqsdbqjk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.tianlin.xyz/gtoubaxydo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hongshengwenyu.top/gtaxlrnrvp.html


<!-- 参考信息 -->