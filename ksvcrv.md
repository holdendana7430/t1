代发 wailian999

C#:   (int)resp.StatusCode
来源：http://hz.svipenyu.cn/gtwwjhscut.html

[L08] 并发请求多个地址
来源：http://hz.bjfxy.top/gtdszmsnbp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jlsjyb.cn/gtitkmuwpg.html

PHP:  curl_multi_init() 系列
来源：http://hz.0kj1m.cn/gtglqpvvdm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinghuilouyu.cn/gtmuuuajye.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258888.top/gtjjldpaby.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zycfv.cn/gtpfiepmrw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yj20258888.top/gtbbuawrjw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cucudq.cn/gtgjqbllfv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.tanke756.top/gtbnslispq.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtkmjstcek.html

M. 命令行 / 进程 / 环境
来源：http://hz.meibo888.top/gtbrsdmfae.html

================================================================================
来源：http://hz.316326.xyz/gtsscgzrmj.html

[M01] 读取命令行参数
来源：http://hz.feifeiyinyue.top/gtkjmzsrbb.html

Py:   sys.argv[1:]
来源：http://hz.daria6918.cn/gtzwwkcsaf.html

PHP:  $argv;  $argc;
来源：http://hz.fzhhl.top/gtaakkyovg.html

JS:   process.argv.slice(2)
来源：http://hz.yj202588.top/gtwymvpysr.html

TS:   process.argv.slice(2)
来源：http://hz.chenlongwang.top/gtbajxbbfm.html

Java: args 数组（main 方法参数）
来源：http://hz.ppjwa.cn/gtfkqtwqzr.html

Go:   os.Args[1:]
来源：http://hz.jinqigfzy.top/gtngegpgkp.html

Ruby: ARGV
来源：http://hz.ppjwa.cn/gtpcitxifg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.dashuyun.cn/gtsoqjfcqg.html

[M02] 读取环境变量
来源：http://hz.sweek.top/gtaytbvnrr.html

Py:   os.environ.get("HOME")
来源：http://hz.hnqzz.top/gtpxhauhpe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cucudq.cn/gtezwodmkt.html

JS:   process.env.HOME
来源：http://hz.havefunace.top/gtyqsvfsvl.html

TS:   process.env.HOME
来源：http://hz.havefunace.top/gtvrtlolyn.html

Java: System.getenv("HOME")
来源：http://hz.yonumen.top/gtunljydca.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinqigufen.top/gtvjlmekfx.html

Ruby: ENV["HOME"]
来源：http://hz.jianghu66.top/gtdxlryqqj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenzaomai.com/gtgmjlkvmj.html

[M03] 执行外部命令
来源：http://hz.cqqwz.cn/gtwkxqapec.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.daxiang520.top/gtfgekhqmy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yj202588.top/gtxhfbeuyw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shangyingyoupin.top/gteasllfet.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhoulong.xyz/gtlhtqegsp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.9152youxi.cn/gtgeidblxi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.chenlongwang.top/gtiduduvze.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.chenjidiqi.icu/gtznjmehgz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sweek.top/gtmxvcrnfp.html

[M04] 获取当前工作目录
来源：http://hz.svipenyu.cn/gtnfygiyem.html

Py:   os.getcwd()
来源：http://hz.dianchejie.cn/gtzdzjaczv.html

PHP:  getcwd();
来源：http://hz.mhx1999.top/gtdkvziffu.html

JS:   process.cwd()
来源：http://hz.mhx1999.top/gtnqzbozoi.html

TS:   process.cwd()
来源：http://hz.zhengqikj.top/gttmdbhnhc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tian-w.cn/gtjyzvgjhi.html

Go:   os.Getwd()
来源：http://hz.jlsjyb.cn/gtqyckphzv.html

Ruby: Dir.pwd
来源：http://hz.dashuyun.cn/gtzjwswefh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.tanke756.top/gtzjuqfxqh.html

[M05] 设置退出码
来源：http://hz.ppjwa.cn/gtaawretaz.html

Py:   sys.exit(1)
来源：http://hz.smart0.xyz/gthumvboon.html

PHP:  exit(1);
来源：http://hz.cheryme.top/gtqrvgvmjp.html

JS:   process.exit(1)
来源：http://hz.yj202588.top/gtewkrshvb.html

TS:   process.exit(1)
来源：http://hz.shzxlz.cn/gtwcahosrj.html

Java: System.exit(1)
来源：http://hz.aizwys.cn/gtjnjlqowt.html

Go:   os.Exit(1)
来源：http://hz.yangfankeji.com/gtqyyfiscj.html

Ruby: exit 1
来源：http://hz.haohaochexian.top/gtrcebahku.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj20258.top/gtyosalhki.html

[M06] 向标准错误输出
来源：http://hz.kuanghao11.cn/gtvvietcyo.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ivvv.top/gtzkmdheox.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.tianlin.xyz/gtyuargklp.html

JS:   console.error("err")
来源：http://hz.tian-w.cn/gthynelpno.html

TS:   console.error("err")
来源：http://hz.dianchejie.cn/gtdzpvpeju.html

Java: System.err.println("err")
来源：http://hz.yj202588.top/gtsjxxcxva.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jinyuanbaomall.cn/gtylwhoqef.html

Ruby: warn "err"
来源：http://hz.shanyushiyangtech.top/gtqibjtitd.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.quarkkingdee.top/gtwcmsytpp.html

[M07] 判断是否为主入口
来源：http://hz.mhx1999.top/gtmqouijnx.html

Py:   if __name__ == "__main__":
来源：http://hz.hywenlv.cn/gtioxcquwz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shzxlz.cn/gtnfkmplwx.html

JS:   require.main === module
来源：http://hz.9152youxi.cn/gtnonwjpuh.html

TS:   require.main === module
来源：http://hz.shangyingyoupin.top/gtqfrpucqi.html

Java: public static void main(String[] args)
来源：http://hz.jinqigfzy.top/gtfpxzqqhv.html

Go:   func main()
来源：http://hz.yj20258888.top/gttjwewuke.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ydjk.org.cn/gtvsmjriqh.html

C#:   static void Main(string[] args)
来源：http://hz.xylfe.cn/gtwacvyzjh.html

[M08] 获取系统与运行时信息
来源：http://hz.xingfuxueyuan.xyz/gtigevsjyv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shuidangran.top/gtzfdsawwp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xuetiantiany.cn/gtvyqqqnfp.html

JS:   process.platform;  process.version
来源：http://hz.shangyingyoupin.top/gtnosztvfi.html

TS:   process.platform;  process.version
来源：http://hz.jinqigfzy.top/gtxntjxuzv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zycfv.cn/gtcqfruakt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.fengsongda.top/gtyapkbite.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zdqjudy.top/gthjzuogkg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cqqwz.cn/gtkkqpjkwf.html

================================================================================
来源：http://hz.sweek.top/gtkynvxayy.html

N. 数据结构与算法
来源：http://hz.cdnleiting.top/gtgdqutyto.html

================================================================================
来源：http://hz.xinyue.icu/gtwdbfhiqw.html

[N01] 二分查找（有序数组）
来源：http://hz.ppjwa.cn/gtzsewudft.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.pengpengdd.cyou/gtajwrdxdz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sxryk.cn/gtuiwpweqb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cheryme.top/gtqftcctdr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.snrcjt.cn/gtkrsdjdvk.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shuidangran.top/gtqsuqotzn.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.haohaochexian.top/gtzpbzwdqc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhixingplan.top/gtoueejxme.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ivvv.top/gtddzhkyup.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ppjwa.cn/gtniksltld.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.daria6918.cn/gtihqeknnm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tian-w.cn/gtakietnzx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nwbrower.top/gttllyyasy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jiagoushi.top/gtsbmzkeii.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinghuilouyu.cn/gtowmgqotu.html

Go:   slices.Sort(arr)
来源：http://hz.nanxinkj.top/gtymullove.html

Ruby: arr.sort
来源：http://hz.jinqigufen.top/gtqmarjbpm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cheryme.top/gtnnpizswj.html

[N03] 快速排序（分治示例）
来源：http://hz.zhixingplan.top/gthhjlrpwn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhengqikj.top/gtedqniusx.html

PHP:  // 递归实现，或用 usort
来源：http://hz.vqdsnc.cn/gteqdgrted.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cdnleiting.top/gtcdrlujsd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhoulong.xyz/gtgafwtgzr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.kuanghao11.cn/gtvyluxcjt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shanyushiyangtech.top/gtohtapaqr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shanyushiyangtech.top/gtpgkhhnhs.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.wangshuangyany.cn/gttusvkekj.html

[N04] 斐波那契数列
来源：http://hz.yj20258.top/gtjcwtjfsx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.haohaochexian.top/gthqntaimo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.vqdsnc.cn/gtscidsuyg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258888.top/gtwiqbzldh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tanke756.top/gtjjmlrotr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yonumen.top/gthsfksedt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhaomingkeji.xyz/gtirikridi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yongpay.top/gtsvdyqjff.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhengqikj.top/gtxyvaggip.html

[N05] 最大公约数
来源：http://hz.nwbrower.top/gtiuevhujn.html

Py:   math.gcd(a, b)
来源：http://hz.sysykeji.top/gttoqpewyz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.gzhubu.top/gtcbpmvmvj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sysykeji.top/gtveqwnbvg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj202588.top/gtqfxmdsxm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ivvv.top/gthdykrdjb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yangfankeji.com/gtohbixjwl.html

Ruby: a.gcd(b)
来源：http://hz.yonumen.top/gtdcscbutw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ydzc1.top/gtmpwucfgk.html

[N06] 判断回文字符串
来源：http://hz.jlsjyb.cn/gtiauryzms.html

Py:   s == s[::-1]
来源：http://hz.chenjidiqi.icu/gtdjylkgdp.html

PHP:  $s === strrev($s);
来源：http://hz.dashuyun.cn/gtgeideerm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtguulgzjx.html

TS:   s === [...s].reverse().join("")
来源：http://hz.fengsongda.top/gtiyuftdiu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ivvv.top/gtxsogtuik.html

Go:   // 双指针从两端比较
来源：http://hz.yj202588.top/gttmuxdhke.html

Ruby: s == s.reverse
来源：http://hz.xuanzx.com/gtlmflxyrf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zdqjudy.top/gtglhrfgaz.html

[N07] 两数之和（返回下标）
来源：http://hz.tian-w.cn/gtfyvglruw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ppjwa.cn/gtvxrqfnkt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zycfv.cn/gtxdexenhl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhiwuduotai.top/gtmrsdezcg.html

TS:   // 手写 Map<string, number>
来源：http://hz.sysykeji.top/gtmhgfphpz.html

Java: // 手写 HashMap
来源：http://hz.cheryme.top/gthqutueyh.html

Go:   // 手写 map[int]int
来源：http://hz.ivvv.top/gteonlhkdb.html

Ruby: // 手写 Hash
来源：http://hz.sxryk.cn/gtioadjidu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.c1oappe.top/gtmxyjjwio.html

[N08] 生成全排列
来源：http://hz.gotoacloud.top/gtuffslulv.html

Py:   itertools.permutations(arr)
来源：http://hz.ivvv.top/gtlqtwpgqw.html

PHP:  // 手写递归交换
来源：http://hz.fzhhl.top/gtzoknklqq.html

JS:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtipykdrrg.html

TS:   // 手写回溯递归
来源：http://hz.hammf.cn/gteofgpdsn.html

Java: // 手写回溯递归
来源：http://hz.hammf.cn/gtlecegged.html

Go:   // 手写回溯递归
来源：http://hz.cqqwz.cn/gtkdygromh.html

Ruby: arr.permutation.to_a
来源：http://hz.zhongyouzk.top/gtfachzsuh.html

C#:   // 手写回溯递归
来源：http://hz.ydzc1.top/gtwjmbztgo.html

[N09] 栈与队列
来源：http://hz.jinqigufen.top/gtvzdjpbpv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.gzhubu.top/gtfwqrsezj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hfpthk.cn/gtnzeggqyz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yuanzhike.top/gtrttzmmdv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.chenzaomai.com/gtbkpxwuoo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hfpthk.cn/gtskfaatas.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jqgufenzy.top/gtwnbthxhm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.bjfxy.top/gtxfroxpqw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.sxryk.cn/gtclileass.html

[N10] 链表节点定义
来源：http://hz.fengsongda.top/gthbvhfwjo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ydjk.org.cn/gtnxdthepn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.dashuyun.cn/gtviuecpng.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.316326.xyz/gtyqmhflqv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhongyouzk.top/gtcnyrfctf.html

Java: class Node { int v; Node next; }
来源：http://hz.ybcxt.top/gtndmagzkt.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yuxming.cn/gtrbdbgqqq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shangyingyoupin.top/gthuuqtyxs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.0kj1m.cn/gtbkeekfxb.html

[N11] 二叉树中序遍历
来源：http://hz.hammf.cn/gtwuszlwcj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.gogol.net.cn/gtgegkzvey.html

PHP:  // 手写递归函数
来源：http://hz.yj20258888.top/gtehzczgce.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shzxlz.cn/gtnvhwucuc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jlsjyb.cn/gtcvxuxlye.html

Java: // 手写递归
来源：http://hz.cashguo.top/gtlvrorhcu.html

Go:   // 手写递归
来源：http://hz.jiagoushi.top/gtoxpnaavg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jinghuilouyu.cn/gtefggkyff.html

C#:   // 手写递归
来源：http://hz.birdmap.top/gtdwbsmgro.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ybcxt.top/gtccxnarru.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.sysykeji.top/gtvqbhybag.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yuanzhike.top/gtmpqyracm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tanke756.top/gtzmehjxio.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sxryk.cn/gtdildnyyd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhoulong.xyz/gtpbscisxg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.dianchejie.cn/gtyzaxizzz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ybcxt.top/gtxmdslyxr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tian-w.cn/gtropvucfm.html

================================================================================
来源：http://hz.xuanzx.com/gtohmvhpvp.html

O. 并发与异步
来源：http://hz.chenlongwang.top/gtzbmeotfz.html

================================================================================
来源：http://hz.gzhubu.top/gteymobmui.html

[O01] 启动一个线程
来源：http://hz.zhengqikj.top/gtimkazimn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.chenzaomai.com/gtkqygmqsl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shangyingyoupin.top/gtiwdcrljy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.shanyushiyangkeji.top/gtspvakuxo.html

TS:   // 同 JS
来源：http://hz.wangshuangyany.cn/gtqpwdyxaw.html

Java: new Thread(() -> f()).start()
来源：http://hz.sxryk.cn/gtjyiunzrw.html

Go:   go f()
来源：http://hz.yuanzhike.top/gtodvdzbsv.html

Ruby: Thread.new { f }
来源：http://hz.redwolf501.top/gtzcueylse.html

C#:   Task.Run(() => F());
来源：http://hz.jyoumei.cn/gtbtjqzsdo.html

[O02] 使用线程池
来源：http://hz.andypj.xyz/gtxdzehfey.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jiagoushi.top/gtvmhqmwag.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.havefunace.top/gtruwgyggc.html

JS:   // worker_threads 线程池
来源：http://hz.sufxvd.cn/gtblnsarab.html

TS:   // worker_threads 线程池
来源：http://hz.yonumen.top/gtcesjrhpz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hnxiangtu.top/gtqigepocb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhoulong.xyz/gthklsikxm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ybcxt.top/gtxxvgkgtt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.haohaochexian.top/gtcxfwcxso.html

[O03] 加锁保护共享数据
来源：http://hz.tian-w.cn/gtsyacqndx.html

Py:   with lock: shared += 1
来源：http://hz.jianghu66.top/gteyswlitt.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shanyushiyangtech.top/gttqcswsez.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yueranfly.top/gtlsedloto.html

TS:   // 同 JS
来源：http://hz.jinqigufen.top/gtoiwiycsx.html

Java: synchronized (this) { shared++; }
来源：http://hz.yangfankeji.com/gthlzpqyfa.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.c1oappe.top/gtwddwwdwb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hysaishi.cn/gtbmqezpez.html

C#:   lock (gate) { shared++; }
来源：http://hz.guannengcc.top/gtgoafifyv.html

[O04] 定义异步函数并等待
来源：http://hz.nanxuanxn.top/gtxxgbswmv.html

Py:   async def f():⏎    await g()
来源：http://hz.hnxiangtu.top/gtmctwbqax.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sweek.top/gttendxooq.html

JS:   async function f() { await g(); }
来源：http://hz.birdmap.top/gtwaxnhoti.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.gotoacloud.top/gtybowesuo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xinyue.icu/gtzpyyqngf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.nwbrower.top/gtjpvbctue.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yuanzhike.top/gtfytrhdre.html

C#:   async Task F() { await G(); }
来源：http://hz.ivvv.top/gtpydpmhcb.html

[O05] 并发执行并等待全部完成
来源：http://hz.shanyushiyangkeji.top/gtblanitod.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhoulong.xyz/gtplcuwtsb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.316326.xyz/gtiqeufqij.html

JS:   await Promise.all(tasks)
来源：http://hz.fzhhl.top/gtwogubsyv.html

TS:   await Promise.all(tasks)
来源：http://hz.zhaomingkeji.xyz/gtypiifsxe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.guannengcc.top/gtbflmcryt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jinqigufen.top/gtwadonsne.html

Ruby: threads.map(&:join)
来源：http://hz.0kj1m.cn/gteuhfjmta.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinqigfzy.top/gtzyhlskvl.html

[O06] 使用进程池
来源：http://hz.ivvv.top/gtqsnfgyyx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.dashuyun.cn/gtgsimeoan.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.sufxvd.cn/gthjpdumdl.html

JS:   // child_process / cluster 模块
来源：http://hz.chenlongwang.top/gthevjtonm.html

TS:   // child_process / cluster 模块
来源：http://hz.fengsongda.top/gteoeauoaq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yj20258.top/gtrwhhyfnd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.sweek.top/gtuknmxuas.html

Ruby: // fork 块
来源：http://hz.xinyue.icu/gtwgqsgbke.html

C#:   Parallel.For
来源：http://hz.hammf.cn/gtabejqwcf.html

================================================================================
来源：http://hz.yongpay.top/gtctqmbuhu.html

P. 常用工具函数
来源：http://hz.nanxinkj.top/gtrmigmbqt.html

================================================================================
来源：http://hz.sxryk.cn/gtbglusmgs.html

[P01] 生成 UUID
来源：http://hz.cqqwz.cn/gtixcmycoz.html

Py:   str(uuid.uuid4())
来源：http://hz.zhiwuduotai.top/gtpccozlvo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.fzhhl.top/gtmgmxwlhg.html

JS:   crypto.randomUUID()
来源：http://hz.tian-w.cn/gttjycbuuf.html

TS:   crypto.randomUUID()
来源：http://hz.pengpengdd.cyou/gtxwmkfzem.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhongyouzk.top/gtbbwlpbhe.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xuanzx.com/gtwqjnnmsz.html

Ruby: SecureRandom.uuid
来源：http://hz.pengpengdd.cyou/gtfejksott.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ivvv.top/gtdbflpxmy.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinqigufen.top/gtmajitqsh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.haohaochexian.top/gtiqvugdgq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jianghu66.top/gtflzpbgyp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.sysykeji.top/gtodqrtnto.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.nanxinkj.top/gtrkjgjcne.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gzhubu.top/gtcmmbrodf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shangyingyoupin.top/gtehwygdkx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.aibaodan.cn/gthoytuvrp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cucudq.cn/gtuhyrpibp.html

[P03] 生成短随机字符串
来源：http://hz.zhengqikj.top/gtzdoxcozr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.svipenyu.cn/gtwxysirrq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xuanzx.com/gtsukwaktv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cashguo.top/gtzorneuym.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.iojbl.cn/gtegdtyhit.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hywenlv.cn/gtluujqgaz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.wangdashe.top/gtyogaywlo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.daxiang520.top/gtsatpwbdv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.guowangkeji.top/gteojpjump.html

[P04] 求长度
来源：http://hz.hnxiangtu.top/gtdyetqrxp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhijiandao.cn/gteuhxjkbo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.svipenyu.cn/gtnelgkdpb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cucudq.cn/gtfgsyffyn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangdashe.top/gtjcbqstwm.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xuetiantiany.cn/gttivwxnpk.html

Go:   len(arr);  len(m)
来源：http://hz.dianchejie.cn/gtjfgupmuy.html

Ruby: x.length;  x.size
来源：http://hz.mhx1999.top/gtuwhqcdga.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jinqigfzy.top/gtkgyrofzo.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jlsjyb.cn/gtndnrihtn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhiwuduotai.top/gtsmtnyalj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yj20258888.top/gtchhdqyut.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jqgufenzy.top/gtgykwfcns.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cashguo.top/gtnbghxxec.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yj202588.top/gtdsgecstl.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jinghuilouyu.cn/gtpzvhrbly.html

Ruby: a == b
来源：http://hz.zhongyouzk.top/gtqszgfttj.html


<!-- 参考信息 -->