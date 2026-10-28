代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yangfankeji.com/gtntgwqppn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yangfankeji.com/gtjuxfjpew.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.guannengcc.top/gtwmxhmfdy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.chenjidiqi.icu/gtmabymyzm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.dashuyun.cn/gtgabdeipf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.havefunace.top/gtmrwngiip.html

================================================================================
来源：http://hz.yvedp.cn/gtzxkeuzdj.html

M. 命令行 / 进程 / 环境
来源：http://hz.pycfn.com/gtxovttnsn.html

================================================================================
来源：http://hz.xziqi.cn/gtbvmwfayw.html

[M01] 读取命令行参数
来源：http://hz.sweek.top/gtztkqzxbw.html

Py:   sys.argv[1:]
来源：http://hz.zhixingplan.top/gtrhcacskm.html

PHP:  $argv;  $argc;
来源：http://hz.gogol.net.cn/gtjaccdeov.html

JS:   process.argv.slice(2)
来源：http://hz.jqgfzy.top/gtitcwzple.html

TS:   process.argv.slice(2)
来源：http://hz.zhijiandao.cn/gtbanrcltp.html

Java: args 数组（main 方法参数）
来源：http://hz.chenjidiqi.icu/gttxpazwro.html

Go:   os.Args[1:]
来源：http://hz.jyoumei.cn/gtacuykblm.html

Ruby: ARGV
来源：http://hz.zhaomingkeji.xyz/gtdfyhpbts.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jqgfzy.top/gteplkhfbm.html

[M02] 读取环境变量
来源：http://hz.cashguo.top/gtzzjhjkgg.html

Py:   os.environ.get("HOME")
来源：http://hz.c1oappe.top/gtloqqnpqr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinqigfzy.top/gttjasavwv.html

JS:   process.env.HOME
来源：http://hz.chenjidiqi.icu/gtjhgcroxa.html

TS:   process.env.HOME
来源：http://hz.havefunace.top/gtdzcajybl.html

Java: System.getenv("HOME")
来源：http://hz.birdmap.top/gtqhpahgtd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.chenjidiqi.icu/gtwirujbdk.html

Ruby: ENV["HOME"]
来源：http://hz.xuetiantiany.cn/gtufcqruov.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.havefunace.top/gtfpdwxhme.html

[M03] 执行外部命令
来源：http://hz.fzhhl.top/gtctomgrvn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xziqi.cn/gtadjhdytb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.nwbrower.top/gtyhnrggdk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhixingplan.top/gtdicaecov.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yonumen.top/gtxrpdyphl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ydjk.org.cn/gtyegbtbzx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.iojbl.cn/gtqohttkmc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.quarkkingdee.top/gtigjezinf.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yueranfly.top/gtvoisltgo.html

[M04] 获取当前工作目录
来源：http://hz.c1oappe.top/gtajpgzmrd.html

Py:   os.getcwd()
来源：http://hz.cashguo.top/gtjtbfhfpl.html

PHP:  getcwd();
来源：http://hz.birdmap.top/gtgjetbmte.html

JS:   process.cwd()
来源：http://hz.xziqi.cn/gtgcxduylg.html

TS:   process.cwd()
来源：http://hz.iojbl.cn/gtevfcevqv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinyuanbaomall.cn/gtmrtnchbj.html

Go:   os.Getwd()
来源：http://hz.redwolf501.top/gtzsifpius.html

Ruby: Dir.pwd
来源：http://hz.zhaomingkeji.xyz/gtyvvxxwgj.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.fengsongda.top/gtzrjeuext.html

[M05] 设置退出码
来源：http://hz.shzxlz.cn/gtbnwwovhv.html

Py:   sys.exit(1)
来源：http://hz.cdnleiting.top/gtyfooxrtm.html

PHP:  exit(1);
来源：http://hz.vqdsnc.cn/gthdgduddn.html

JS:   process.exit(1)
来源：http://hz.redwolf501.top/gtmfqcyfdf.html

TS:   process.exit(1)
来源：http://hz.yongpay.top/gtxnvixdji.html

Java: System.exit(1)
来源：http://hz.cashguo.top/gtzoxkjzzs.html

Go:   os.Exit(1)
来源：http://hz.yuanzhike.top/gtadikgstw.html

Ruby: exit 1
来源：http://hz.hnxiangtu.top/gtnvbdcuuv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinqigfzy.top/gtweeayaaf.html

[M06] 向标准错误输出
来源：http://hz.yanxiufei.cn/gtpmrufwjs.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nanxuanxn.top/gtsinsxxyx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xingfuxueyuan.xyz/gtdsvdpycx.html

JS:   console.error("err")
来源：http://hz.xingfuxueyuan.xyz/gtkizffslr.html

TS:   console.error("err")
来源：http://hz.jyoumei.cn/gtccimywxa.html

Java: System.err.println("err")
来源：http://hz.jqgfzy.top/gthdclwqhv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.meibo888.top/gtzfoccntb.html

Ruby: warn "err"
来源：http://hz.wangdashe.top/gtewjqppmt.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.sxryk.cn/gtbtxkzvid.html

[M07] 判断是否为主入口
来源：http://hz.jqgufenzy.top/gtqxjeasjd.html

Py:   if __name__ == "__main__":
来源：http://hz.fengsongda.top/gtihtokzkl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xuanzx.com/gtwrgvcpgg.html

JS:   require.main === module
来源：http://hz.dashuyun.cn/gtviwhxxif.html

TS:   require.main === module
来源：http://hz.hammf.cn/gtiyozqlkr.html

Java: public static void main(String[] args)
来源：http://hz.xuanzx.com/gtkwwsgale.html

Go:   func main()
来源：http://hz.yonumen.top/gtbqqsycac.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.pengpengdd.cyou/gtnrpbxftk.html

C#:   static void Main(string[] args)
来源：http://hz.9152youxi.cn/gtsjtshfoi.html

[M08] 获取系统与运行时信息
来源：http://hz.sweek.top/gtbsxubxfb.html

Py:   platform.system();  platform.python_version()
来源：http://hz.meibo888.top/gtrlxghshr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ppjwa.cn/gtvjydtcpc.html

JS:   process.platform;  process.version
来源：http://hz.yangfankeji.com/gtpnqryzhn.html

TS:   process.platform;  process.version
来源：http://hz.yangfankeji.com/gtmrqizpnm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.kuanghao11.cn/gtgfxwmeui.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cdnleiting.top/gtstauiffi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.0kj1m.cn/gtcufknzrg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xylfe.cn/gtzmtmqhvb.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtwqptrnxr.html

N. 数据结构与算法
来源：http://hz.svipenyu.cn/gtkmenviyc.html

================================================================================
来源：http://hz.hnqzz.top/gtsbbpyedn.html

[N01] 二分查找（有序数组）
来源：http://hz.yueranfly.top/gtysoxtlcr.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yangfankeji.com/gtlffesmck.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yuxming.cn/gtfiinhybz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aizwys.cn/gttuqurvgi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.birdmap.top/gtihoaqort.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yueranfly.top/gtcearbmrp.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shzxlz.cn/gtqbobesnh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yuxming.cn/gtcuzqwqdl.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinqigfzy.top/gtdysjrqdb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hnxiangtu.top/gtfgpxegfu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhengqikj.top/gthgxelmlr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cheryme.top/gtgrdlicky.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cashguo.top/gtvswkzafy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.pycfn.com/gtglniftcf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.kuanghao11.cn/gtnkfktdmk.html

Go:   slices.Sort(arr)
来源：http://hz.guannengcc.top/gtaaraivsl.html

Ruby: arr.sort
来源：http://hz.sweek.top/gtentcogxr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cdnleiting.top/gtjzqvdxfi.html

[N03] 快速排序（分治示例）
来源：http://hz.ywan-chungtsiang.top/gtvdikpaoj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinghuilouyu.cn/gtwpvihrry.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nwbrower.top/gttyjlcdya.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhongyouzk.top/gtkojifzuy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxuanxn.top/gtzsgwkbvx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jqgfzy.top/gthprbtssn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.c1oappe.top/gtkllenvfx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.daria6918.cn/gtzqbdqpoo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yongpay.top/gtswhxognb.html

[N04] 斐波那契数列
来源：http://hz.hfpthk.cn/gtxziprvst.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yuanzhike.top/gtuzelvhua.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shanyushiyangkeji.top/gtvlgzkrzf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenjidiqi.icu/gtguarfmeo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cashguo.top/gtrfkzjqzx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.nwbrower.top/gtmvmlpuqx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hywenlv.cn/gtuplqjwvs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.quarkkingdee.top/gtyhaofvkn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.meibo888.top/gtbkuawjel.html

[N05] 最大公约数
来源：http://hz.hnqzz.top/gtclzvlixh.html

Py:   math.gcd(a, b)
来源：http://hz.yonumen.top/gtjsvjmfgp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinqigufen.top/gtcymbktnq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fengsongda.top/gtlpvrrein.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ywan-chungtsiang.top/gthwakiyaj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gzhubu.top/gtjifqmond.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hysaishi.cn/gtlqadsmnt.html

Ruby: a.gcd(b)
来源：http://hz.zhaomingkeji.xyz/gtdurdzovq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.haohaochexian.top/gtcsvlhpyn.html

[N06] 判断回文字符串
来源：http://hz.jinghuilouyu.cn/gtvaswbuye.html

Py:   s == s[::-1]
来源：http://hz.pengpengdd.cyou/gtzhnowzny.html

PHP:  $s === strrev($s);
来源：http://hz.tanke756.top/gtwuganaxj.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtqwnqsfwm.html

TS:   s === [...s].reverse().join("")
来源：http://hz.daria6918.cn/gtesvdtunc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.birdmap.top/gtopjubafn.html

Go:   // 双指针从两端比较
来源：http://hz.hongshengwenyu.top/gtozmwqbff.html

Ruby: s == s.reverse
来源：http://hz.zhiwuduotai.top/gtmtxzizgf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.pengpengdd.cyou/gtwezmhvzw.html

[N07] 两数之和（返回下标）
来源：http://hz.ywan-chungtsiang.top/gtzapnycqw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xinyue.icu/gtxxsmrehi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cucudq.cn/gttahcmljf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sweek.top/gteibekofo.html

TS:   // 手写 Map<string, number>
来源：http://hz.hnqzz.top/gtqbkpanpf.html

Java: // 手写 HashMap
来源：http://hz.jlsjyb.cn/gtmjvispot.html

Go:   // 手写 map[int]int
来源：http://hz.316326.xyz/gtfinldsla.html

Ruby: // 手写 Hash
来源：http://hz.jiagoushi.top/gtyingpzgd.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jiagoushi.top/gtawknvufq.html

[N08] 生成全排列
来源：http://hz.hywenlv.cn/gtbqwzjqdh.html

Py:   itertools.permutations(arr)
来源：http://hz.andypj.xyz/gtzrbvbout.html

PHP:  // 手写递归交换
来源：http://hz.hammf.cn/gttiokxxft.html

JS:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gtxekntrma.html

TS:   // 手写回溯递归
来源：http://hz.havefunace.top/gtnxgfqchl.html

Java: // 手写回溯递归
来源：http://hz.sufxvd.cn/gtgtwhvfiy.html

Go:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtmtvddpxz.html

Ruby: arr.permutation.to_a
来源：http://hz.smart0.xyz/gtcenfglnp.html

C#:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtpyxkltda.html

[N09] 栈与队列
来源：http://hz.yanxiufei.cn/gtjxdoyqsh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.vqdsnc.cn/gtnacvhkqj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cucudq.cn/gtgarsuqqp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.0kj1m.cn/gthmiufywl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.nanxuanxn.top/gtkmdsybsw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.svipenyu.cn/gtjjwjenfa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xylfe.cn/gteuubephh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hongshengwenyu.top/gtsnbhxrub.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.havefunace.top/gtkaxnmtiu.html

[N10] 链表节点定义
来源：http://hz.hysaishi.cn/gteswieqvd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yanxiufei.cn/gtaztyeawf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cqqwz.cn/gtvvubwsib.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.chenzaomai.com/gtvjmsfyur.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.pengpengdd.cyou/gtgzioiufu.html

Java: class Node { int v; Node next; }
来源：http://hz.hywenlv.cn/gtqjzaohqd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ybcxt.top/gtrvdvzzwj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hnqzz.top/gtfziihfot.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jianghu66.top/gtjrxcqvpm.html

[N11] 二叉树中序遍历
来源：http://hz.snrcjt.cn/gtzxvwcqew.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.chenjidiqi.icu/gtahhywrhk.html

PHP:  // 手写递归函数
来源：http://hz.xinyue.icu/gtacdnnuxu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guowangkeji.top/gtptsrrcxk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pycfn.com/gtphmjfwfl.html

Java: // 手写递归
来源：http://hz.gaohongyu789.top/gtykaylchh.html

Go:   // 手写递归
来源：http://hz.fzhhl.top/gtusahtfjw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.gzhubu.top/gtiximpijv.html

C#:   // 手写递归
来源：http://hz.zhengqikj.top/gtbbdicews.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.daxiang520.top/gtzjgbgmkm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tianlin.xyz/gtakahigwm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jianghu66.top/gtelqdigly.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxuanxn.top/gtdgdbkcrq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.svipenyu.cn/gtgwgpujrc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangkeji.top/gtvskgzszm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhijiandao.cn/gtbvxchpoy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yuxming.cn/gtlohtmiev.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xingfuxueyuan.xyz/gtjmycmmez.html

================================================================================
来源：http://hz.guannengcc.top/gtjheqoyxq.html

O. 并发与异步
来源：http://hz.shanyushiyangtech.top/gtnrrwilwr.html

================================================================================
来源：http://hz.cqqwz.cn/gttojzypjw.html

[O01] 启动一个线程
来源：http://hz.birdmap.top/gtkbqpncmu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sxryk.cn/gtkeyytbbk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gogol.net.cn/gtaffbjduz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.quarkkingdee.top/gtwecfdcsl.html

TS:   // 同 JS
来源：http://hz.vqdsnc.cn/gtjimyzvtj.html

Java: new Thread(() -> f()).start()
来源：http://hz.pengpengdd.cyou/gtkzyweiat.html

Go:   go f()
来源：http://hz.hongshengwenyu.top/gtbsimwyxd.html

Ruby: Thread.new { f }
来源：http://hz.svipenyu.cn/gtlwwmnbzm.html

C#:   Task.Run(() => F());
来源：http://hz.gaohongyu789.top/gttsezbruf.html

[O02] 使用线程池
来源：http://hz.meibo888.top/gtbaagidoh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.daxiang520.top/gtzaudybtg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.chenjidiqi.icu/gteitpbrmw.html

JS:   // worker_threads 线程池
来源：http://hz.chenlongwang.top/gtbqyzfedn.html

TS:   // worker_threads 线程池
来源：http://hz.jiagoushi.top/gtwewiodrs.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.mhx1999.top/gtkyydaect.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.guowangkeji.top/gtjtrcwtas.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.mhx1999.top/gtpuwovehl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ppjwa.cn/gtkzdtranf.html

[O03] 加锁保护共享数据
来源：http://hz.snrcjt.cn/gthicysfkc.html

Py:   with lock: shared += 1
来源：http://hz.yj20258.top/gtcsacrles.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.haohaochexian.top/gtaqwtrgez.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.guannengcc.top/gtalekhckc.html

TS:   // 同 JS
来源：http://hz.jinghuilouyu.cn/gtujxufnvq.html

Java: synchronized (this) { shared++; }
来源：http://hz.smart0.xyz/gtpfylseac.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yangfankeji.com/gtwtzlckzv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yj20258888.top/gtlnqszple.html

C#:   lock (gate) { shared++; }
来源：http://hz.nwbrower.top/gtofwjhmiv.html

[O04] 定义异步函数并等待
来源：http://hz.zhongyouzk.top/gtokhluncs.html

Py:   async def f():⏎    await g()
来源：http://hz.meibo888.top/gtfgasxjbj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cheryme.top/gtkjhsfdin.html

JS:   async function f() { await g(); }
来源：http://hz.haohaochexian.top/gtufarxnoc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hfpthk.cn/gtuwrcjlih.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ydzc1.top/gtqpscufrt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xinyue.icu/gtqmmwgzpl.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gotoacloud.top/gtoizrgado.html

C#:   async Task F() { await G(); }
来源：http://hz.c1oappe.top/gtqsrftjbc.html

[O05] 并发执行并等待全部完成
来源：http://hz.meibo888.top/gtgsfrcnzu.html

Py:   asyncio.gather(*tasks)
来源：http://hz.meibo888.top/gttzvxmtvx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhixingplan.top/gttogfxsmp.html

JS:   await Promise.all(tasks)
来源：http://hz.xuanzx.com/gtwwldexpy.html

TS:   await Promise.all(tasks)
来源：http://hz.dianchejie.cn/gtkvczqamn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.pycfn.com/gtstdgixis.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.daria6918.cn/gthcjvgqmz.html

Ruby: threads.map(&:join)
来源：http://hz.pycfn.com/gtuurlssmj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xinyue.icu/gthzayznvu.html

[O06] 使用进程池
来源：http://hz.gotoacloud.top/gtpyehwage.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhaomingkeji.xyz/gtaffxqlfc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.gogol.net.cn/gtxxitpzjt.html

JS:   // child_process / cluster 模块
来源：http://hz.gotoacloud.top/gtwsmosows.html

TS:   // child_process / cluster 模块
来源：http://hz.0kj1m.cn/gtxgtcnihb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hysaishi.cn/gtayjowdvn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.cqqwz.cn/gtntfimkkk.html

Ruby: // fork 块
来源：http://hz.iojbl.cn/gtbyiphtap.html

C#:   Parallel.For
来源：http://hz.havefunace.top/gtmstgjzvh.html

================================================================================
来源：http://hz.wangdashe.top/gtmnnmeqbm.html

P. 常用工具函数
来源：http://hz.xingfuxueyuan.xyz/gtahhddidh.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtuaijngcu.html

[P01] 生成 UUID
来源：http://hz.jinghuilouyu.cn/gtzeseavyq.html

Py:   str(uuid.uuid4())
来源：http://hz.ydzc1.top/gtsratailh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinghuilouyu.cn/gtqvdcelfn.html

JS:   crypto.randomUUID()
来源：http://hz.jyoumei.cn/gtnymgldln.html

TS:   crypto.randomUUID()
来源：http://hz.ppjwa.cn/gteocaobpz.html

Java: UUID.randomUUID().toString()
来源：http://hz.shanyushiyangkeji.top/gtyyxtprle.html

Go:   // 用 github.com/google/uuid
来源：http://hz.tianlin.xyz/gtabzyjvps.html

Ruby: SecureRandom.uuid
来源：http://hz.aibaodan.cn/gtzogovfif.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.tian-w.cn/gtanbaoorh.html

[P02] MD5 / SHA256 摘要
来源：http://hz.9152youxi.cn/gtkgffayqw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.aibaodan.cn/gtstabgusf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yongpay.top/gthxhzbsmd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yuanzhike.top/gtahlynfkg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jinghuilouyu.cn/gtnvmddxas.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cheryme.top/gtvjdakcck.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.bjfxy.top/gtpvzijsfb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhaomingkeji.xyz/gtakgfkftb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hongshengwenyu.top/gtffkpsckw.html

[P03] 生成短随机字符串
来源：http://hz.cucudq.cn/gtpxutvfkk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xinyue.icu/gtjbhxvohp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.vqdsnc.cn/gtojmtjwgy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.aibaodan.cn/gtwozdjydi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jiagoushi.top/gtjoxotwgw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinqigfzy.top/gtazbefjyb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cdnleiting.top/gtsapxybvl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jlsjyb.cn/gtmjuacnoa.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.aizwys.cn/gtnxfgjxfp.html

[P04] 求长度
来源：http://hz.ydzc1.top/gtspgqjdfr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.wangshuangyany.cn/gtsmahcpyv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.vqdsnc.cn/gtswrhurfe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.vqdsnc.cn/gtyhefebwk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gzhubu.top/gtcuhwbiip.html

Java: list.size();  map.size();  s.length()
来源：http://hz.gotoacloud.top/gtxzvyozga.html

Go:   len(arr);  len(m)
来源：http://hz.quarkkingdee.top/gtyijuiezp.html

Ruby: x.length;  x.size
来源：http://hz.cashguo.top/gtsraftrvq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhijiandao.cn/gtsplsfphw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.nanxuanxn.top/gtuitpizyu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tianlin.xyz/gthnfwoqzy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hywenlv.cn/gtstuqdcji.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.cheryme.top/gtufzepffo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinqigufen.top/gtvxxskycq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.snrcjt.cn/gtafcxgkmf.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.fzhhl.top/gtfqulqido.html

Ruby: a == b
来源：http://hz.zycfv.cn/gtebdaetfs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cdnleiting.top/gtpsxcvjoe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yj202588.top/gtcxkxttvr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.bjfxy.top/gtpzttbqju.html

PHP:  if (empty($x)) {}
来源：http://hz.aibaodan.cn/gtydaajdii.html


<!-- 参考信息 -->