代发 wailian999

C#:   (int)resp.StatusCode
来源：http://hz.guannengcc.top/gtgacvjxjf.html

[L08] 并发请求多个地址
来源：http://hz.ivvv.top/gtqcqytpet.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.dashuyun.cn/gthsigqffx.html

PHP:  curl_multi_init() 系列
来源：http://hz.0kj1m.cn/gtpvdrajfq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aibaodan.cn/gtpdlehoqb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sysykeji.top/gtgicrlhls.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sysykeji.top/gtvesdoqfo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ppjwa.cn/gtunqgrrgk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.316326.xyz/gtiavdjmbi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jqgfzy.top/gtykmtexeg.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtsnztnuiq.html

M. 命令行 / 进程 / 环境
来源：http://hz.sufxvd.cn/gtncwjbmea.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtcdqmpqnc.html

[M01] 读取命令行参数
来源：http://hz.cheryme.top/gtdkzqouwd.html

Py:   sys.argv[1:]
来源：http://hz.andypj.xyz/gtiaqvaqgp.html

PHP:  $argv;  $argc;
来源：http://hz.vqdsnc.cn/gtucmnmwif.html

JS:   process.argv.slice(2)
来源：http://hz.kuanghao11.cn/gtdtbpyixa.html

TS:   process.argv.slice(2)
来源：http://hz.shzxlz.cn/gtwjebtpcq.html

Java: args 数组（main 方法参数）
来源：http://hz.andypj.xyz/gtrvgkmogq.html

Go:   os.Args[1:]
来源：http://hz.cqqwz.cn/gtrjernnbk.html

Ruby: ARGV
来源：http://hz.gogol.net.cn/gtuhddqvha.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zdqjudy.top/gtosgitkqj.html

[M02] 读取环境变量
来源：http://hz.sufxvd.cn/gtxahzgiyh.html

Py:   os.environ.get("HOME")
来源：http://hz.nwbrower.top/gthrgukpdj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xylfe.cn/gtwvpkhhcq.html

JS:   process.env.HOME
来源：http://hz.hfpthk.cn/gtzqmynbxf.html

TS:   process.env.HOME
来源：http://hz.chenjidiqi.icu/gtzsawpnys.html

Java: System.getenv("HOME")
来源：http://hz.gaohongyu789.top/gtdlwilhap.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jqgufenzy.top/gtxkmirewx.html

Ruby: ENV["HOME"]
来源：http://hz.feifeiyinyue.top/gtuwvopkxs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hywenlv.cn/gtzxyrwwki.html

[M03] 执行外部命令
来源：http://hz.316326.xyz/gtagzkadfw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.c1oappe.top/gtsvixdoac.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhongyouzk.top/gtvkzylnmi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yanxiufei.cn/gthdzrpvoq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hammf.cn/gtjybkfjxc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinyuanbaomall.cn/gtwfhpdntg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.316326.xyz/gtgumzijnl.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shanyushiyangkeji.top/gtxcztlswl.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shanyushiyangkeji.top/gtljbjmujx.html

[M04] 获取当前工作目录
来源：http://hz.zhongyouzk.top/gttffvofpw.html

Py:   os.getcwd()
来源：http://hz.zhongyouzk.top/gtlvjyinuh.html

PHP:  getcwd();
来源：http://hz.ppjwa.cn/gtpjbvayuw.html

JS:   process.cwd()
来源：http://hz.sxryk.cn/gtgaxcbxoz.html

TS:   process.cwd()
来源：http://hz.yvedp.cn/gtsyebjdcm.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.kuanghao11.cn/gtiozaysbq.html

Go:   os.Getwd()
来源：http://hz.zhoulong.xyz/gtywspeoaq.html

Ruby: Dir.pwd
来源：http://hz.chenlongwang.top/gtixykbtuc.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.9152youxi.cn/gtwvpydekj.html

[M05] 设置退出码
来源：http://hz.yuanzhike.top/gtwourfvto.html

Py:   sys.exit(1)
来源：http://hz.fengsongda.top/gtiabtggxr.html

PHP:  exit(1);
来源：http://hz.gzhubu.top/gttchwhxew.html

JS:   process.exit(1)
来源：http://hz.sufxvd.cn/gtzneiekxh.html

TS:   process.exit(1)
来源：http://hz.316326.xyz/gtotjynhrg.html

Java: System.exit(1)
来源：http://hz.gogol.net.cn/gtdyqgdkep.html

Go:   os.Exit(1)
来源：http://hz.tianlin.xyz/gteiltfcun.html

Ruby: exit 1
来源：http://hz.tanke756.top/gtfrkpatea.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.wangshuangyany.cn/gthjibqcih.html

[M06] 向标准错误输出
来源：http://hz.hongshengwenyu.top/gtebbwtrsw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shanyushiyangkeji.top/gtfiivmmph.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenlongwang.top/gtjilixtrl.html

JS:   console.error("err")
来源：http://hz.shangyingyoupin.top/gtifyqmdap.html

TS:   console.error("err")
来源：http://hz.tian-w.cn/gtcfvyfyet.html

Java: System.err.println("err")
来源：http://hz.cheryme.top/gtbsxfhxqn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.tian-w.cn/gtjgsbehgt.html

Ruby: warn "err"
来源：http://hz.iojbl.cn/gtdiifqknx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.andypj.xyz/gtoyandjeb.html

[M07] 判断是否为主入口
来源：http://hz.hfpthk.cn/gtokyplubu.html

Py:   if __name__ == "__main__":
来源：http://hz.mhx1999.top/gtsozllojn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xinyue.icu/gtijsswwyy.html

JS:   require.main === module
来源：http://hz.nanxinkj.top/gtrpelhjuq.html

TS:   require.main === module
来源：http://hz.ywan-chungtsiang.top/gtutpjonwv.html

Java: public static void main(String[] args)
来源：http://hz.cheryme.top/gtnamskqus.html

Go:   func main()
来源：http://hz.shzxlz.cn/gtwzabvupu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ydzc1.top/gtytvibhyt.html

C#:   static void Main(string[] args)
来源：http://hz.yj20258888.top/gtrqrlbnvi.html

[M08] 获取系统与运行时信息
来源：http://hz.zhengqikj.top/gtccjfsdbg.html

Py:   platform.system();  platform.python_version()
来源：http://hz.feifeiyinyue.top/gtbxgdhzwq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hfpthk.cn/gtikzlhjpq.html

JS:   process.platform;  process.version
来源：http://hz.hywenlv.cn/gtkquauqct.html

TS:   process.platform;  process.version
来源：http://hz.hongshengwenyu.top/gttsfwcxst.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.quarkkingdee.top/gtglglneia.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.guannengcc.top/gthydjuade.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yueranfly.top/gtgpaavykh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yanxiufei.cn/gtbofdeofa.html

================================================================================
来源：http://hz.fengsongda.top/gtmgizkbhz.html

N. 数据结构与算法
来源：http://hz.gotoacloud.top/gtozhoeekz.html

================================================================================
来源：http://hz.zhoulong.xyz/gtwwqrzgax.html

[N01] 二分查找（有序数组）
来源：http://hz.jiagoushi.top/gtavuiyioc.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.feifeiyinyue.top/gtkuqkudkw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yvedp.cn/gtukhezuhu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yangfankeji.com/gtcgkqjvea.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.redwolf501.top/gtsyyixbau.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jqgufenzy.top/gtovgetqpi.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cdnleiting.top/gtwwvnjqqa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.havefunace.top/gtcngflaju.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cdnleiting.top/gtzdspbfcg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.pycfn.com/gtxpsmsieu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yangfankeji.com/gtylxqccxn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jiagoushi.top/gtriimayqb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhiwuduotai.top/gthvgzwnvc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.redwolf501.top/gtyinnogfg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sweek.top/gtgdzrklor.html

Go:   slices.Sort(arr)
来源：http://hz.xuanzx.com/gtgmodmxae.html

Ruby: arr.sort
来源：http://hz.xingfuxueyuan.xyz/gtquewiiep.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhijiandao.cn/gtuchkpqij.html

[N03] 快速排序（分治示例）
来源：http://hz.shangyingyoupin.top/gtresvvxhn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.bjfxy.top/gthhnnuwym.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yj202588.top/gtoxexhzfm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sweek.top/gtjfngtogm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xziqi.cn/gtqjdunaxy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cheryme.top/gtrtfmqodw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.wangshuangyany.cn/gtjqzgjvkj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shanyushiyangkeji.top/gtvywkpdfg.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jqgfzy.top/gtkpixoqul.html

[N04] 斐波那契数列
来源：http://hz.ivvv.top/gtscmavzav.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ydjk.org.cn/gtuhbnacmf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinyuanbaomall.cn/gtcblqqyhf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj202588.top/gtxuddjcik.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhoulong.xyz/gtlhedjtig.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cashguo.top/gtonnbsbxw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.wangshuangyany.cn/gtjnaixrwd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhixingplan.top/gtnzlnszek.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.fzhhl.top/gtpknzvpjt.html

[N05] 最大公约数
来源：http://hz.meibo888.top/gtjitxfiwo.html

Py:   math.gcd(a, b)
来源：http://hz.yj20258888.top/gtzgstmahk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yanxiufei.cn/gtayojxfpc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aibaodan.cn/gtcbqpfipl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.52xcode.cn/gtbmmkcopj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.dianchejie.cn/gtrkbslrpc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ppjwa.cn/gtafljiwsr.html

Ruby: a.gcd(b)
来源：http://hz.smart0.xyz/gtpxybasxm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ywan-chungtsiang.top/gturzljoso.html

[N06] 判断回文字符串
来源：http://hz.meibo888.top/gthpqtfnsa.html

Py:   s == s[::-1]
来源：http://hz.havefunace.top/gtmhwvroyd.html

PHP:  $s === strrev($s);
来源：http://hz.zhixingplan.top/gtrjttzkvl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.daxiang520.top/gtxcrnenal.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shangyingyoupin.top/gtawehvwlh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shanyushiyangkeji.top/gtlsoefbeu.html

Go:   // 双指针从两端比较
来源：http://hz.hfpthk.cn/gthddxhelz.html

Ruby: s == s.reverse
来源：http://hz.fengsongda.top/gtnwyacxtu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhixingplan.top/gttpcytyvm.html

[N07] 两数之和（返回下标）
来源：http://hz.sxryk.cn/gtotxldoez.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gaohongyu789.top/gttcbtsyiz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gogol.net.cn/gtfogiyugd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shanyushiyangkeji.top/gtolsxqdyn.html

TS:   // 手写 Map<string, number>
来源：http://hz.nwbrower.top/gtnzkdboqx.html

Java: // 手写 HashMap
来源：http://hz.zhoulong.xyz/gtkjsrecah.html

Go:   // 手写 map[int]int
来源：http://hz.chenlongwang.top/gtkxbgwtgp.html

Ruby: // 手写 Hash
来源：http://hz.yanxiufei.cn/gtxvzovfiu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xziqi.cn/gtvqxfqlzk.html

[N08] 生成全排列
来源：http://hz.gaohongyu789.top/gtikjfvdme.html

Py:   itertools.permutations(arr)
来源：http://hz.jyoumei.cn/gtueovpjud.html

PHP:  // 手写递归交换
来源：http://hz.dianchejie.cn/gtsbmtuhly.html

JS:   // 手写回溯递归
来源：http://hz.kuanghao11.cn/gtdcxpyobm.html

TS:   // 手写回溯递归
来源：http://hz.zycfv.cn/gtydjdblbb.html

Java: // 手写回溯递归
来源：http://hz.yj202588.top/gtdplmcgpr.html

Go:   // 手写回溯递归
来源：http://hz.jqgufenzy.top/gtuithlpdj.html

Ruby: arr.permutation.to_a
来源：http://hz.kuanghao11.cn/gtyscmbnll.html

C#:   // 手写回溯递归
来源：http://hz.cashguo.top/gtbkhbnern.html

[N09] 栈与队列
来源：http://hz.guowangkeji.top/gtmluwywlr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.chenzaomai.com/gtxjrkkqet.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.bjfxy.top/gtxuezfjwn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yongpay.top/gtonlcxned.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shangyingyoupin.top/gtdkvdjjsl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yj20258888.top/gtakxixnmb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ehwqpu.com/gtullcptpt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shanyushiyangtech.top/gtfamhokaa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinghuilouyu.cn/gtdinjfvml.html

[N10] 链表节点定义
来源：http://hz.ehwqpu.com/gtqgjjfnki.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.fengsongda.top/gttmzmifyj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.chenlongwang.top/gtfuxgykvv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.shangyingyoupin.top/gtqccvipzk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jiagoushi.top/gtgjjofehj.html

Java: class Node { int v; Node next; }
来源：http://hz.pengpengdd.cyou/gtxanvweaa.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hysaishi.cn/gthkipztyj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yuxming.cn/gtghdwmqcl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.iojbl.cn/gtwwxevxiv.html

[N11] 二叉树中序遍历
来源：http://hz.guowangkeji.top/gtjzulafjb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jianghu66.top/gtcqskafpn.html

PHP:  // 手写递归函数
来源：http://hz.daria6918.cn/gtgawbtjoz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhixingplan.top/gtfusqurjh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tian-w.cn/gtkqywjgvz.html

Java: // 手写递归
来源：http://hz.jyoumei.cn/gtewdbzigt.html

Go:   // 手写递归
来源：http://hz.daria6918.cn/gtqjyclhbh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.bjfxy.top/gtvbycvddr.html

C#:   // 手写递归
来源：http://hz.havefunace.top/gtmgcdvqbt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zycfv.cn/gtbleqqgge.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cashguo.top/gtqvjkvyxa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yj202588.top/gtwbrfagmm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yongpay.top/gtnsjhtdzc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dashuyun.cn/gtbtvlfgmr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sufxvd.cn/gtswzsveot.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenjidiqi.icu/gtvbcturta.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.havefunace.top/gtzoqxbrrq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.mhx1999.top/gtrlnpnxpr.html

================================================================================
来源：http://hz.xinyue.icu/gtvlikosic.html

O. 并发与异步
来源：http://hz.ehwqpu.com/gtzggopxrc.html

================================================================================
来源：http://hz.jianghu66.top/gthifkdjwr.html

[O01] 启动一个线程
来源：http://hz.jqgfzy.top/gthzppvhpf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gaohongyu789.top/gtfpeddsgw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhongyouzk.top/gtxrndydkg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.shzxlz.cn/gtbrbqdjar.html

TS:   // 同 JS
来源：http://hz.yj20258888.top/gtkrsotctl.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinyuanbaomall.cn/gtmvnfvmuc.html

Go:   go f()
来源：http://hz.fengsongda.top/gtfqsggfgq.html

Ruby: Thread.new { f }
来源：http://hz.cucudq.cn/gtijkmafot.html

C#:   Task.Run(() => F());
来源：http://hz.zhaomingkeji.xyz/gtfkqsyozw.html

[O02] 使用线程池
来源：http://hz.mhx1999.top/gtnmzlprhl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hfpthk.cn/gtlqmbazic.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jqgfzy.top/gtmlbdfker.html

JS:   // worker_threads 线程池
来源：http://hz.shanyushiyangtech.top/gtadldgkrg.html

TS:   // worker_threads 线程池
来源：http://hz.daxiang520.top/gtqggjwmem.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.chenzaomai.com/gtgjrdjqze.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.andypj.xyz/gtwpyxgubt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hongshengwenyu.top/gtyldldjpo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhaomingkeji.xyz/gtwcwcywvz.html

[O03] 加锁保护共享数据
来源：http://hz.pengpengdd.cyou/gtjeugdlwq.html

Py:   with lock: shared += 1
来源：http://hz.meibo888.top/gtyvpktfyl.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hywenlv.cn/gtajjqfovj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hywenlv.cn/gtagkydukx.html

TS:   // 同 JS
来源：http://hz.jianghu66.top/gtkxtvircd.html

Java: synchronized (this) { shared++; }
来源：http://hz.hnqzz.top/gtfdkfkndc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ehwqpu.com/gthinqrvti.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jqgufenzy.top/gtrzzhfhdu.html

C#:   lock (gate) { shared++; }
来源：http://hz.ydjk.org.cn/gtagvkghky.html

[O04] 定义异步函数并等待
来源：http://hz.sxryk.cn/gtkztkrozc.html

Py:   async def f():⏎    await g()
来源：http://hz.xingfuxueyuan.xyz/gtzmcfahnr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shanyushiyangkeji.top/gtgbfrvuas.html

JS:   async function f() { await g(); }
来源：http://hz.mhx1999.top/gtzeeunxkl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xylfe.cn/gtfiirkwbl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.dashuyun.cn/gtivtvfmou.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.dashuyun.cn/gtohftnndd.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.fengsongda.top/gtilibritd.html

C#:   async Task F() { await G(); }
来源：http://hz.9152youxi.cn/gtnjiqjqeo.html

[O05] 并发执行并等待全部完成
来源：http://hz.fengsongda.top/gtmkpledpl.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zdqjudy.top/gtlamdtvaf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.sweek.top/gttwmhgqmi.html

JS:   await Promise.all(tasks)
来源：http://hz.iojbl.cn/gtcyqwicel.html

TS:   await Promise.all(tasks)
来源：http://hz.316326.xyz/gtighwjrif.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.sufxvd.cn/gtdsuoiiwh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xziqi.cn/gtmzjfzdzc.html

Ruby: threads.map(&:join)
来源：http://hz.52xcode.cn/gtwltlczyy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jianghu66.top/gtymoukobc.html

[O06] 使用进程池
来源：http://hz.hfpthk.cn/gtdsjrjrfq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zdqjudy.top/gtduyvizyv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xziqi.cn/gtvtmgcrbo.html

JS:   // child_process / cluster 模块
来源：http://hz.hongshengwenyu.top/gtwwvwuyax.html

TS:   // child_process / cluster 模块
来源：http://hz.redwolf501.top/gtfmcbppiw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.chenzaomai.com/gtxjkqlseo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gaohongyu789.top/gtklljiewa.html

Ruby: // fork 块
来源：http://hz.shanyushiyangtech.top/gtzhqqihrh.html

C#:   Parallel.For
来源：http://hz.guowangkeji.top/gtdszefgms.html

================================================================================
来源：http://hz.yvedp.cn/gtqyntwdmi.html

P. 常用工具函数
来源：http://hz.zhiwuduotai.top/gtzsohqkpe.html

================================================================================
来源：http://hz.fzhhl.top/gtphipaurq.html

[P01] 生成 UUID
来源：http://hz.sysykeji.top/gtrdzeyofn.html

Py:   str(uuid.uuid4())
来源：http://hz.kuanghao11.cn/gtqxmtxovr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.quarkkingdee.top/gtqsibtjvx.html

JS:   crypto.randomUUID()
来源：http://hz.jinqigfzy.top/gtwbbgmusi.html

TS:   crypto.randomUUID()
来源：http://hz.redwolf501.top/gteyoocbis.html

Java: UUID.randomUUID().toString()
来源：http://hz.jinqigfzy.top/gtnritlwrv.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hnqzz.top/gtbpckgbpi.html

Ruby: SecureRandom.uuid
来源：http://hz.xziqi.cn/gtpgrrjrye.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yangfankeji.com/gtwcoopwqd.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hfpthk.cn/gtyydiithz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenlongwang.top/gtnghxwhuo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.nanxuanxn.top/gtfzxxmmcn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yuanzhike.top/gtwaycgzax.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.dianchejie.cn/gtbcwoljof.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.feifeiyinyue.top/gtftwdfknl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yvedp.cn/gtcsuvonuw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.daxiang520.top/gtxygejydl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.pycfn.com/gtrawkpjzj.html

[P03] 生成短随机字符串
来源：http://hz.xinyue.icu/gtfktlkxdp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cucudq.cn/gtinyvdnfc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.kuanghao11.cn/gtqyjmpyzs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.redwolf501.top/gtwcsmmlwx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xylfe.cn/gtyijzlwal.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.chenlongwang.top/gtcxateodl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shanyushiyangtech.top/gtpxbjkaxt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hywenlv.cn/gtaqmrtfyv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.birdmap.top/gtjjcckfzh.html

[P04] 求长度
来源：http://hz.hysaishi.cn/gtdainstjf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhoulong.xyz/gtjfedcaer.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinqigfzy.top/gttulrmypv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yueranfly.top/gttcxxjhwm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shzxlz.cn/gtseypfvvy.html

Java: list.size();  map.size();  s.length()
来源：http://hz.dianchejie.cn/gttulskptg.html

Go:   len(arr);  len(m)
来源：http://hz.yj20258888.top/gtcjpqdlba.html

Ruby: x.length;  x.size
来源：http://hz.yueranfly.top/gtvvldtqxk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhaomingkeji.xyz/gtzorxdtry.html

[P05] 判断两个对象内容是否相等
来源：http://hz.dianchejie.cn/gtgrmbotdp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ybcxt.top/gtluqnrxww.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jiagoushi.top/gtdikjqmvp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yongpay.top/gtxjdnbdrv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.wangshuangyany.cn/gtxvbnnsuv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ppjwa.cn/gtgiiligos.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jianghu66.top/gtaccjdxxb.html

Ruby: a == b
来源：http://hz.haohaochexian.top/gtmzwgttqs.html


<!-- 参考信息 -->