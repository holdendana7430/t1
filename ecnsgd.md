代发 wailian999

C#:   (int)resp.StatusCode
来源：http://hz.xinyue.icu/gtqvyoubyx.html

[L08] 并发请求多个地址
来源：http://hz.wangdashe.top/gtfzzbrnbt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.bjfxy.top/gtniuczcde.html

PHP:  curl_multi_init() 系列
来源：http://hz.yangfankeji.com/gthydushyd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tian-w.cn/gtfbulfwzm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258888.top/gtirhvopdg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gotoacloud.top/gtwqpjcuac.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gotoacloud.top/gtzstvjujk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.kuanghao11.cn/gtssvmqiqp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhijiandao.cn/gttfziacer.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtwmkhowoq.html

M. 命令行 / 进程 / 环境
来源：http://hz.hammf.cn/gtalehvpub.html

================================================================================
来源：http://hz.cashguo.top/gthomxbead.html

[M01] 读取命令行参数
来源：http://hz.jlsjyb.cn/gtacvzotrn.html

Py:   sys.argv[1:]
来源：http://hz.zhongyouzk.top/gtfunmxfgy.html

PHP:  $argv;  $argc;
来源：http://hz.jinyuanbaomall.cn/gtnlkfmrbe.html

JS:   process.argv.slice(2)
来源：http://hz.0kj1m.cn/gtujatmixa.html

TS:   process.argv.slice(2)
来源：http://hz.chenlongwang.top/gtnmzvgand.html

Java: args 数组（main 方法参数）
来源：http://hz.hfpthk.cn/gtjidjtkwp.html

Go:   os.Args[1:]
来源：http://hz.hnqzz.top/gtxxitgjnz.html

Ruby: ARGV
来源：http://hz.tianlin.xyz/gtgwzlpfyb.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jqgufenzy.top/gtpxfjspds.html

[M02] 读取环境变量
来源：http://hz.chenlongwang.top/gtfxypdofb.html

Py:   os.environ.get("HOME")
来源：http://hz.shangyingyoupin.top/gtzhzjxdqu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.gaohongyu789.top/gtjmmfqmqm.html

JS:   process.env.HOME
来源：http://hz.gogol.net.cn/gtwxstsfsg.html

TS:   process.env.HOME
来源：http://hz.jinqigfzy.top/gtjscqxgyx.html

Java: System.getenv("HOME")
来源：http://hz.bjfxy.top/gtxckvlcwo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.kuanghao11.cn/gtmstrebwp.html

Ruby: ENV["HOME"]
来源：http://hz.sxryk.cn/gtotmnohkg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zdqjudy.top/gtyigxoyvg.html

[M03] 执行外部命令
来源：http://hz.sxryk.cn/gtrccsdqgx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.wangdashe.top/gtrfdusabx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ybcxt.top/gtucblkauv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cheryme.top/gthgffntzq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shzxlz.cn/gtlnhwrjps.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ydzc1.top/gtjczieixv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.guowangkeji.top/gtvgflniiy.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yuxming.cn/gtgmlcxhxb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xuetiantiany.cn/gtljdyfmvn.html

[M04] 获取当前工作目录
来源：http://hz.ydzc1.top/gtdwaaewhh.html

Py:   os.getcwd()
来源：http://hz.quarkkingdee.top/gtsqmyhzjy.html

PHP:  getcwd();
来源：http://hz.gzhubu.top/gtkirfeibk.html

JS:   process.cwd()
来源：http://hz.jinyuanbaomall.cn/gtqufuvegb.html

TS:   process.cwd()
来源：http://hz.xuetiantiany.cn/gtlwcmebic.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinqigfzy.top/gtgyiofglh.html

Go:   os.Getwd()
来源：http://hz.havefunace.top/gtonzbjzwj.html

Ruby: Dir.pwd
来源：http://hz.jinghuilouyu.cn/gthoohlkam.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hfpthk.cn/gtwtwycbrs.html

[M05] 设置退出码
来源：http://hz.chenjidiqi.icu/gtxqisosht.html

Py:   sys.exit(1)
来源：http://hz.52xcode.cn/gtwfdbxdwq.html

PHP:  exit(1);
来源：http://hz.fzhhl.top/gtxjmulzvt.html

JS:   process.exit(1)
来源：http://hz.hammf.cn/gtrewcqlgr.html

TS:   process.exit(1)
来源：http://hz.yj202588.top/gtbigpeohy.html

Java: System.exit(1)
来源：http://hz.daria6918.cn/gtrcvrjbby.html

Go:   os.Exit(1)
来源：http://hz.shangyingyoupin.top/gtyxuwitgq.html

Ruby: exit 1
来源：http://hz.jinqigufen.top/gtgjdjkznx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nanxinkj.top/gtftveagrb.html

[M06] 向标准错误输出
来源：http://hz.shangyingyoupin.top/gtuzjvbshu.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhengqikj.top/gttlgyruxd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yuxming.cn/gtdygvqfcj.html

JS:   console.error("err")
来源：http://hz.jyoumei.cn/gtndajykno.html

TS:   console.error("err")
来源：http://hz.kuanghao11.cn/gtnslasttl.html

Java: System.err.println("err")
来源：http://hz.dashuyun.cn/gtocmcdfod.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hnxiangtu.top/gtpntzovxd.html

Ruby: warn "err"
来源：http://hz.nanxinkj.top/gtwaurvnxs.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jianghu66.top/gtvbikoeuc.html

[M07] 判断是否为主入口
来源：http://hz.yuxming.cn/gtgxdenfgi.html

Py:   if __name__ == "__main__":
来源：http://hz.hysaishi.cn/gtybjhwzyw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ydjk.org.cn/gtgcfiittm.html

JS:   require.main === module
来源：http://hz.shuidangran.top/gtwdaojthx.html

TS:   require.main === module
来源：http://hz.hysaishi.cn/gtbgorxeat.html

Java: public static void main(String[] args)
来源：http://hz.iojbl.cn/gtqfvtuerd.html

Go:   func main()
来源：http://hz.xziqi.cn/gterjaxprl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yueranfly.top/gtozkxktjt.html

C#:   static void Main(string[] args)
来源：http://hz.jyoumei.cn/gtwrprmjvz.html

[M08] 获取系统与运行时信息
来源：http://hz.pengpengdd.cyou/gtbaieexie.html

Py:   platform.system();  platform.python_version()
来源：http://hz.quarkkingdee.top/gtoggnxvmy.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yangfankeji.com/gtltwhaydb.html

JS:   process.platform;  process.version
来源：http://hz.jinqigfzy.top/gtquaxrytu.html

TS:   process.platform;  process.version
来源：http://hz.meibo888.top/gtwadbazyo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gaohongyu789.top/gtaekwfytd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zycfv.cn/gtohhvioeo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhoulong.xyz/gtzdalswyv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ivvv.top/gtyzafeulx.html

================================================================================
来源：http://hz.ydjk.org.cn/gtqoxcqely.html

N. 数据结构与算法
来源：http://hz.sysykeji.top/gtmiwtohia.html

================================================================================
来源：http://hz.snrcjt.cn/gtowlbtnum.html

[N01] 二分查找（有序数组）
来源：http://hz.jiagoushi.top/gtwtrpgfmu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ivvv.top/gtqvuhhenm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.andypj.xyz/gtowobapfs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenzaomai.com/gtqmlyadfm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangdashe.top/gtzwikaxbh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hongshengwenyu.top/gtmfinulwt.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.316326.xyz/gtdvecgusf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.chenzaomai.com/gtbqhksxdq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xinyue.icu/gticsgbcyi.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.dianchejie.cn/gtchblyrso.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gotoacloud.top/gtlzlhtfpb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhoulong.xyz/gtjlkyeump.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aizwys.cn/gtqazivfrc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuxming.cn/gtjylfqrsm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sweek.top/gtezpqmfph.html

Go:   slices.Sort(arr)
来源：http://hz.yj20258888.top/gttwhhbpem.html

Ruby: arr.sort
来源：http://hz.yj20258888.top/gtjkfjpxus.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.wangdashe.top/gtvpmgegjd.html

[N03] 快速排序（分治示例）
来源：http://hz.cucudq.cn/gtiibjzxtl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.nanxuanxn.top/gtrmvvvcwc.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nanxuanxn.top/gtnfcaryjq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xinyue.icu/gtmfcoywtn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuetiantiany.cn/gtobfbcjow.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.gaohongyu789.top/gtfxdkaqnu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.chenzaomai.com/gtvzfhkvvl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shanyushiyangkeji.top/gtgujroxvi.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hongshengwenyu.top/gtpimognbz.html

[N04] 斐波那契数列
来源：http://hz.dianchejie.cn/gtatcftxmf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tanke756.top/gtvuohxfql.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sweek.top/gtkltknejq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xinyue.icu/gtbcvkriia.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xuanzx.com/gtnesekdyi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.dianchejie.cn/gthxsycryq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hysaishi.cn/gtbjoljjch.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hywenlv.cn/gtopkcciny.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yongpay.top/gtmdfrbchc.html

[N05] 最大公约数
来源：http://hz.sweek.top/gtbcejdlji.html

Py:   math.gcd(a, b)
来源：http://hz.iojbl.cn/gtfzdxbnlq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xylfe.cn/gtduhcspjp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gtwmyudtbc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhaomingkeji.xyz/gtrptimjww.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.smart0.xyz/gtjffsxkwz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhiwuduotai.top/gtbvdyolcg.html

Ruby: a.gcd(b)
来源：http://hz.ydjk.org.cn/gtkqmqxape.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.svipenyu.cn/gtvdcetzmv.html

[N06] 判断回文字符串
来源：http://hz.nanxinkj.top/gtenwggdgm.html

Py:   s == s[::-1]
来源：http://hz.jiagoushi.top/gtzbozgkew.html

PHP:  $s === strrev($s);
来源：http://hz.zhoulong.xyz/gtbexdqjxc.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtenzlsdpb.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gtppkpjjck.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.316326.xyz/gtjirpzjzd.html

Go:   // 双指针从两端比较
来源：http://hz.jqgufenzy.top/gtbymvxose.html

Ruby: s == s.reverse
来源：http://hz.yuxming.cn/gtiaquulvq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.pycfn.com/gtmpfqffbk.html

[N07] 两数之和（返回下标）
来源：http://hz.xingfuxueyuan.xyz/gtvdblkact.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hywenlv.cn/gtajtztkxl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.daria6918.cn/gtaatyfgcd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhaomingkeji.xyz/gtizdvtzjs.html

TS:   // 手写 Map<string, number>
来源：http://hz.iojbl.cn/gtrkjlgxia.html

Java: // 手写 HashMap
来源：http://hz.xingfuxueyuan.xyz/gtonocieof.html

Go:   // 手写 map[int]int
来源：http://hz.shuidangran.top/gtckqmcdiu.html

Ruby: // 手写 Hash
来源：http://hz.yueranfly.top/gtbikqwrol.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cqqwz.cn/gtwllmxpkr.html

[N08] 生成全排列
来源：http://hz.zhijiandao.cn/gtdrrelfer.html

Py:   itertools.permutations(arr)
来源：http://hz.jyoumei.cn/gtfylspnjf.html

PHP:  // 手写递归交换
来源：http://hz.ydzc1.top/gtueqbpain.html

JS:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gtzwglafjr.html

TS:   // 手写回溯递归
来源：http://hz.yonumen.top/gtjcmpgtcj.html

Java: // 手写回溯递归
来源：http://hz.quarkkingdee.top/gtyrctwtrl.html

Go:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtszitxgaw.html

Ruby: arr.permutation.to_a
来源：http://hz.jlsjyb.cn/gtwdgljanx.html

C#:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtobhtkknt.html

[N09] 栈与队列
来源：http://hz.redwolf501.top/gthnswbvuj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.vqdsnc.cn/gtxkgfxxyf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.quarkkingdee.top/gtotvzbpag.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.redwolf501.top/gtfdkkbyqt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cdnleiting.top/gtgslnzize.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yuxming.cn/gttxrvacbq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sweek.top/gtccxoakbz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.andypj.xyz/gtvbyyqqqo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.aizwys.cn/gtsoiqkggw.html

[N10] 链表节点定义
来源：http://hz.birdmap.top/gtdmoqlahh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xziqi.cn/gtqnikgpju.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yonumen.top/gtgfjwkajd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.nanxuanxn.top/gtoslfmdyh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ivvv.top/gtoudmlvyx.html

Java: class Node { int v; Node next; }
来源：http://hz.shanyushiyangtech.top/gtnvlguloa.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.havefunace.top/gtlpuspdgh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.52xcode.cn/gtkmghchbv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.52xcode.cn/gtbnprrptb.html

[N11] 二叉树中序遍历
来源：http://hz.ydjk.org.cn/gtidlcsrwz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yonumen.top/gtbxdmsged.html

PHP:  // 手写递归函数
来源：http://hz.yongpay.top/gtlajywvxi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cheryme.top/gtspqgjbli.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fzhhl.top/gtztnefvjh.html

Java: // 手写递归
来源：http://hz.shzxlz.cn/gtyzpresmt.html

Go:   // 手写递归
来源：http://hz.pycfn.com/gtnjjzyijq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shanyushiyangtech.top/gtnbrymjmu.html

C#:   // 手写递归
来源：http://hz.jqgufenzy.top/gtletfptjf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.sysykeji.top/gtomezlshf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhijiandao.cn/gtqwqkaotg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.svipenyu.cn/gtmyvcbpvf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.kuanghao11.cn/gtxexkujjh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nwbrower.top/gteoibrums.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.smart0.xyz/gtkseaiydn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hammf.cn/gtjexpwepd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.feifeiyinyue.top/gtyytxarwm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.daxiang520.top/gtuueyhiic.html

================================================================================
来源：http://hz.yonumen.top/gtziecrbzg.html

O. 并发与异步
来源：http://hz.zhixingplan.top/gtynhdvgbt.html

================================================================================
来源：http://hz.ydzc1.top/gtdsthqaci.html

[O01] 启动一个线程
来源：http://hz.sufxvd.cn/gtmpsvgvyu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ydjk.org.cn/gtnxdhxlfb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gzhubu.top/gtnswfbdvz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.tanke756.top/gtsebgpwwu.html

TS:   // 同 JS
来源：http://hz.gaohongyu789.top/gtkgjjwpid.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhaomingkeji.xyz/gtxxrghnlv.html

Go:   go f()
来源：http://hz.bjfxy.top/gtrrcjwfqf.html

Ruby: Thread.new { f }
来源：http://hz.jianghu66.top/gtzdahufpc.html

C#:   Task.Run(() => F());
来源：http://hz.shanyushiyangkeji.top/gtnnjhrzih.html

[O02] 使用线程池
来源：http://hz.cashguo.top/gtmxcoskic.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.chenjidiqi.icu/gtiovqttiy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nanxinkj.top/gtqfxsbcnd.html

JS:   // worker_threads 线程池
来源：http://hz.ydjk.org.cn/gtowbscpfn.html

TS:   // worker_threads 线程池
来源：http://hz.tanke756.top/gteqjasjri.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.wangdashe.top/gteqfauevd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jinqigufen.top/gtmksnqenr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.aizwys.cn/gtbigjpviv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.sweek.top/gtsgcszjhw.html

[O03] 加锁保护共享数据
来源：http://hz.xinyue.icu/gtrprmkdhs.html

Py:   with lock: shared += 1
来源：http://hz.aibaodan.cn/gtvjezgyoe.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jinyuanbaomall.cn/gtnfdciwho.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.dashuyun.cn/gtuthsifia.html

TS:   // 同 JS
来源：http://hz.dashuyun.cn/gtpzufjlqp.html

Java: synchronized (this) { shared++; }
来源：http://hz.jqgfzy.top/gtixmgksah.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cqqwz.cn/gtbzemyvqb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xingfuxueyuan.xyz/gtvpqnvlpe.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhengqikj.top/gtolsszxyh.html

[O04] 定义异步函数并等待
来源：http://hz.ywan-chungtsiang.top/gtvpnsqnjt.html

Py:   async def f():⏎    await g()
来源：http://hz.yuanzhike.top/gtwerhrpsj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xinyue.icu/gtujvntnij.html

JS:   async function f() { await g(); }
来源：http://hz.yuanzhike.top/gtqzdirmkg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hnqzz.top/gtczhdjrgf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.snrcjt.cn/gtatulyxmg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.tian-w.cn/gtdbkvccyh.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hammf.cn/gtmmfouycc.html

C#:   async Task F() { await G(); }
来源：http://hz.gaohongyu789.top/gtubkgrbgi.html

[O05] 并发执行并等待全部完成
来源：http://hz.ybcxt.top/gtffumqkvj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.sufxvd.cn/gtgknowdpl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.meibo888.top/gtbhdusmrr.html

JS:   await Promise.all(tasks)
来源：http://hz.yj20258.top/gtzsizpzyj.html

TS:   await Promise.all(tasks)
来源：http://hz.cashguo.top/gtdelhflkw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.tianlin.xyz/gtsmpklvdg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xylfe.cn/gtnndudzhs.html

Ruby: threads.map(&:join)
来源：http://hz.pycfn.com/gtzgfxjsks.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cdnleiting.top/gtxkizsqhz.html

[O06] 使用进程池
来源：http://hz.nanxinkj.top/gtujcmauvv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhiwuduotai.top/gtzszsaokt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.wangshuangyany.cn/gtuwsykmpo.html

JS:   // child_process / cluster 模块
来源：http://hz.xinyue.icu/gtsdyetgdt.html

TS:   // child_process / cluster 模块
来源：http://hz.ivvv.top/gthudddzcu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yuanzhike.top/gtjvcvvxug.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shzxlz.cn/gtbykovvdq.html

Ruby: // fork 块
来源：http://hz.chenzaomai.com/gtjakxzfcp.html

C#:   Parallel.For
来源：http://hz.nwbrower.top/gtwjkvlwcq.html

================================================================================
来源：http://hz.tanke756.top/gtvwlletbs.html

P. 常用工具函数
来源：http://hz.xingfuxueyuan.xyz/gtnwwbnonu.html

================================================================================
来源：http://hz.yj20258888.top/gtvcppmqqx.html

[P01] 生成 UUID
来源：http://hz.sweek.top/gtodtwrcvo.html

Py:   str(uuid.uuid4())
来源：http://hz.sweek.top/gtrjjsfcjl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yanxiufei.cn/gtpnxdnbqw.html

JS:   crypto.randomUUID()
来源：http://hz.cdnleiting.top/gttwodllnz.html

TS:   crypto.randomUUID()
来源：http://hz.wangdashe.top/gtgblnxpuz.html

Java: UUID.randomUUID().toString()
来源：http://hz.9152youxi.cn/gtwdxjjbay.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xinyue.icu/gtxjtnvlzf.html

Ruby: SecureRandom.uuid
来源：http://hz.zdqjudy.top/gtpqkaatch.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jianghu66.top/gtnzgwkgnf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zycfv.cn/gtkfcyldtx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.9152youxi.cn/gtyhpemggy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hnxiangtu.top/gtbbtxzclt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hysaishi.cn/gtkjezqysl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cdnleiting.top/gtdtuwtrtw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cqqwz.cn/gtqocktjve.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.iojbl.cn/gthtwjlrpm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hywenlv.cn/gtwoceduab.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ywan-chungtsiang.top/gtdcejhmch.html

[P03] 生成短随机字符串
来源：http://hz.gzhubu.top/gtzfalwkxd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cucudq.cn/gtcpqkasqk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhongyouzk.top/gtnaoxywqw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.9152youxi.cn/gtstvnqszm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuanzx.com/gtilhsagvs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cucudq.cn/gtvpkxrouy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.dashuyun.cn/gthzfqpbdo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.dianchejie.cn/gtezyihyyo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.sufxvd.cn/gtipbcbsxw.html

[P04] 求长度
来源：http://hz.sxryk.cn/gtatbsullw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shanyushiyangkeji.top/gtleiwrkbc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guowangkeji.top/gtpvrasofq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jianghu66.top/gttfwkljzz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dianchejie.cn/gtxipcfkxp.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jinqigfzy.top/gtrkjhawrh.html

Go:   len(arr);  len(m)
来源：http://hz.yvedp.cn/gtmuqhdfml.html

Ruby: x.length;  x.size
来源：http://hz.ppjwa.cn/gtrlcrvlbn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xinyue.icu/gtyscgpwth.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ywan-chungtsiang.top/gtmmcxqrje.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.meibo888.top/gtvmgkzsgg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.nwbrower.top/gtykufcvgl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yvedp.cn/gtdkzuowmu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhiwuduotai.top/gtdiijsqtr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hysaishi.cn/gtknvtrdaa.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.tian-w.cn/gtigglnqxf.html

Ruby: a == b
来源：http://hz.chenjidiqi.icu/gtdnacxxgd.html


<!-- 参考信息 -->