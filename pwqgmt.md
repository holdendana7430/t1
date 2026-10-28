代发 wailian999

TS:   resp.ok;  resp.status
来源：http://hz.aibaodan.cn/gtqchcouov.html

Java: resp.statusCode()
来源：http://hz.cdnleiting.top/gtomzeyfxg.html

Go:   resp.StatusCode
来源：http://hz.shuidangran.top/gtcwzpbiwq.html

Ruby: resp.code.to_i
来源：http://hz.shanyushiyangtech.top/gtdywfcawd.html

C#:   (int)resp.StatusCode
来源：http://hz.yonumen.top/gtkxcnnhzm.html

[L08] 并发请求多个地址
来源：http://hz.chenlongwang.top/gtpnncebij.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hnxiangtu.top/gtcpxzigws.html

PHP:  curl_multi_init() 系列
来源：http://hz.yueranfly.top/gtjtwvievx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daxiang520.top/gtevcregkh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuxming.cn/gtpekjxydo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sysykeji.top/gtlzdoevwi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinqigufen.top/gtrjfscymf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.c1oappe.top/gtlwbpjbcd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cdnleiting.top/gtkgdyrurv.html

================================================================================
来源：http://hz.sxryk.cn/gttglxkrva.html

M. 命令行 / 进程 / 环境
来源：http://hz.ydzc1.top/gttvjbtkap.html

================================================================================
来源：http://hz.guowangkeji.top/gtpyqsftej.html

[M01] 读取命令行参数
来源：http://hz.meibo888.top/gtecgiuoat.html

Py:   sys.argv[1:]
来源：http://hz.yvedp.cn/gtvanhdrrh.html

PHP:  $argv;  $argc;
来源：http://hz.xuetiantiany.cn/gtukbnwrak.html

JS:   process.argv.slice(2)
来源：http://hz.jinqigfzy.top/gtexgnxwtd.html

TS:   process.argv.slice(2)
来源：http://hz.316326.xyz/gtqccstnbr.html

Java: args 数组（main 方法参数）
来源：http://hz.guannengcc.top/gtmatbaarz.html

Go:   os.Args[1:]
来源：http://hz.yj20258.top/gtgpaoxcoq.html

Ruby: ARGV
来源：http://hz.hfpthk.cn/gtspszshwf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ehwqpu.com/gtqwpgjuei.html

[M02] 读取环境变量
来源：http://hz.gogol.net.cn/gtogyogyba.html

Py:   os.environ.get("HOME")
来源：http://hz.nanxinkj.top/gtjszhexrg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yangfankeji.com/gtrzqwlfdd.html

JS:   process.env.HOME
来源：http://hz.dashuyun.cn/gtqczfldwv.html

TS:   process.env.HOME
来源：http://hz.zhaomingkeji.xyz/gtoxuwsniv.html

Java: System.getenv("HOME")
来源：http://hz.yuanzhike.top/gtkgkypilv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ppjwa.cn/gtjfnjrone.html

Ruby: ENV["HOME"]
来源：http://hz.tianlin.xyz/gtkdtucuxv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.tianlin.xyz/gtkaqwrpbo.html

[M03] 执行外部命令
来源：http://hz.jqgfzy.top/gtjqisjznj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhixingplan.top/gtdolgnxpx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.bjfxy.top/gtogzeblwk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhoulong.xyz/gtaahfljqg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhongyouzk.top/gthnrqqwac.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.fzhhl.top/gtgshrkjcy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.guannengcc.top/gtglfmpzhp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jianghu66.top/gtljlvwlmj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xuetiantiany.cn/gtxbjmzldj.html

[M04] 获取当前工作目录
来源：http://hz.cqqwz.cn/gtktcdpgkg.html

Py:   os.getcwd()
来源：http://hz.gogol.net.cn/gtxwzfhped.html

PHP:  getcwd();
来源：http://hz.jyoumei.cn/gtycednvtz.html

JS:   process.cwd()
来源：http://hz.haohaochexian.top/gtrphcrcxh.html

TS:   process.cwd()
来源：http://hz.fengsongda.top/gtfqtdnoll.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.nanxinkj.top/gtpmotcmco.html

Go:   os.Getwd()
来源：http://hz.shanyushiyangkeji.top/gtbfyralix.html

Ruby: Dir.pwd
来源：http://hz.jlsjyb.cn/gtakbufjix.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.nanxuanxn.top/gtcbrygrvp.html

[M05] 设置退出码
来源：http://hz.zhoulong.xyz/gtepkuyibj.html

Py:   sys.exit(1)
来源：http://hz.yongpay.top/gtwoginbhx.html

PHP:  exit(1);
来源：http://hz.dashuyun.cn/gtpmctrqkd.html

JS:   process.exit(1)
来源：http://hz.jinghuilouyu.cn/gtgdunnenw.html

TS:   process.exit(1)
来源：http://hz.chenzaomai.com/gtykdrylkn.html

Java: System.exit(1)
来源：http://hz.hnqzz.top/gtsbzgfiwv.html

Go:   os.Exit(1)
来源：http://hz.dianchejie.cn/gttltvnbby.html

Ruby: exit 1
来源：http://hz.mhx1999.top/gtqbkgyesd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gzhubu.top/gtctvlwdnh.html

[M06] 向标准错误输出
来源：http://hz.zhongyouzk.top/gtonnajuvu.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhaomingkeji.xyz/gtamlupsrp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sysykeji.top/gtwieftmys.html

JS:   console.error("err")
来源：http://hz.gogol.net.cn/gtghsqispb.html

TS:   console.error("err")
来源：http://hz.xuanzx.com/gtinpjjjum.html

Java: System.err.println("err")
来源：http://hz.zhongyouzk.top/gtvepzfhum.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gaohongyu789.top/gtrbgoebdx.html

Ruby: warn "err"
来源：http://hz.jlsjyb.cn/gtdbciqndc.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cashguo.top/gtexnvuqup.html

[M07] 判断是否为主入口
来源：http://hz.jqgfzy.top/gtbnejynda.html

Py:   if __name__ == "__main__":
来源：http://hz.ywan-chungtsiang.top/gtlgwqojvr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.svipenyu.cn/gtjtgndzax.html

JS:   require.main === module
来源：http://hz.svipenyu.cn/gtlgpufctm.html

TS:   require.main === module
来源：http://hz.sxryk.cn/gtmqxaktkr.html

Java: public static void main(String[] args)
来源：http://hz.cheryme.top/gtgdoimywz.html

Go:   func main()
来源：http://hz.fengsongda.top/gtcyktosnq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ppjwa.cn/gtupyhcvrq.html

C#:   static void Main(string[] args)
来源：http://hz.smart0.xyz/gtvhflfesy.html

[M08] 获取系统与运行时信息
来源：http://hz.xuanzx.com/gtsuepndiv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hysaishi.cn/gtnqulzjhq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenzaomai.com/gtpwnxyziy.html

JS:   process.platform;  process.version
来源：http://hz.cashguo.top/gtmgpkifmk.html

TS:   process.platform;  process.version
来源：http://hz.sweek.top/gtfyaoorot.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zycfv.cn/gtowogxnsp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ivvv.top/gtkawtmjlj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hnqzz.top/gtugcjxbbm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.gotoacloud.top/gtqsezpgvw.html

================================================================================
来源：http://hz.svipenyu.cn/gtnmolassp.html

N. 数据结构与算法
来源：http://hz.svipenyu.cn/gtsfvjzqpb.html

================================================================================
来源：http://hz.c1oappe.top/gtxaedmsqd.html

[N01] 二分查找（有序数组）
来源：http://hz.jinyuanbaomall.cn/gtefwxsjsx.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yueranfly.top/gtsgggwirh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.iojbl.cn/gtfkvyvinb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sufxvd.cn/gtqarsthzl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shanyushiyangtech.top/gtdgfbmhxm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.redwolf501.top/gtgwhbxpii.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hywenlv.cn/gttzdcwfgp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.9152youxi.cn/gtzmfpesqu.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtcizdfcll.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.316326.xyz/gtnypzeyue.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuanzx.com/gtqtvtrbhl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shzxlz.cn/gtsbetbjuj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gotoacloud.top/gtxvyzrpoj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gtjdhgojzp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hammf.cn/gtjgrekftp.html

Go:   slices.Sort(arr)
来源：http://hz.hfpthk.cn/gtecpkiyjb.html

Ruby: arr.sort
来源：http://hz.zhixingplan.top/gtipwrehpf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yongpay.top/gtqxxmkcka.html

[N03] 快速排序（分治示例）
来源：http://hz.zhixingplan.top/gthhmtvmwl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cqqwz.cn/gtylllgsmt.html

PHP:  // 递归实现，或用 usort
来源：http://hz.52xcode.cn/gtymkdyard.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhiwuduotai.top/gttyxobvpt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj20258.top/gtgxhdwukw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj20258888.top/gtzowtyzor.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nanxinkj.top/gtgwtfqcpo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sufxvd.cn/gtlinpchtw.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shuidangran.top/gtrzcqqehi.html

[N04] 斐波那契数列
来源：http://hz.yangfankeji.com/gtzzzbjzcv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yj202588.top/gtcxybjbad.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinghuilouyu.cn/gttqigvrek.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jqgufenzy.top/gtynewnsdr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cashguo.top/gtdpuhshtq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.fengsongda.top/gtpfryouxw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hysaishi.cn/gtwsefryqw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.fzhhl.top/gtpfybfueq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ivvv.top/gttdhlvhca.html

[N05] 最大公约数
来源：http://hz.ydzc1.top/gtmwunqias.html

Py:   math.gcd(a, b)
来源：http://hz.guowangkeji.top/gtwhdiolhn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.kuanghao11.cn/gtkorbollk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ehwqpu.com/gtdaotniii.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gtqvofhjyt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.tanke756.top/gtttivcquv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.dianchejie.cn/gtbjyaqxnf.html

Ruby: a.gcd(b)
来源：http://hz.dianchejie.cn/gtethegrxj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.nanxinkj.top/gtzpflmvmg.html

[N06] 判断回文字符串
来源：http://hz.aibaodan.cn/gtvlqyvjwq.html

Py:   s == s[::-1]
来源：http://hz.ivvv.top/gtithgfoem.html

PHP:  $s === strrev($s);
来源：http://hz.yangfankeji.com/gtyjgfbwev.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jqgufenzy.top/gtrjlrtqse.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xylfe.cn/gtweocahfp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.aibaodan.cn/gtuhaujhyu.html

Go:   // 双指针从两端比较
来源：http://hz.yonumen.top/gtavuzqkha.html

Ruby: s == s.reverse
来源：http://hz.shzxlz.cn/gtoduzfhbo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.dashuyun.cn/gtzjhpullp.html

[N07] 两数之和（返回下标）
来源：http://hz.redwolf501.top/gtcydagpff.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinqigfzy.top/gtwfjyomxa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sxryk.cn/gtuvyxleze.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhiwuduotai.top/gtwygavuhk.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhoulong.xyz/gtvvmnykjf.html

Java: // 手写 HashMap
来源：http://hz.tian-w.cn/gthbzdrkxq.html

Go:   // 手写 map[int]int
来源：http://hz.chenjidiqi.icu/gtdumyymcb.html

Ruby: // 手写 Hash
来源：http://hz.kuanghao11.cn/gtayufadgy.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sxryk.cn/gtiydzhaml.html

[N08] 生成全排列
来源：http://hz.xinyue.icu/gtarriorcw.html

Py:   itertools.permutations(arr)
来源：http://hz.yj20258.top/gtbrdenzcl.html

PHP:  // 手写递归交换
来源：http://hz.cashguo.top/gtrbxpzcmy.html

JS:   // 手写回溯递归
来源：http://hz.ydzc1.top/gteocuqxto.html

TS:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtruztjrws.html

Java: // 手写回溯递归
来源：http://hz.yueranfly.top/gtwaodnykn.html

Go:   // 手写回溯递归
来源：http://hz.ybcxt.top/gtzgowgqii.html

Ruby: arr.permutation.to_a
来源：http://hz.yj202588.top/gtgyvfjwsc.html

C#:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtnrroocco.html

[N09] 栈与队列
来源：http://hz.wangshuangyany.cn/gtvswbwlvw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj20258.top/gtdxvvbora.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.52xcode.cn/gtrpqlqlmk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.nwbrower.top/gtexzzwgie.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ivvv.top/gtdlncqajx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yuanzhike.top/gtcsukixzl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.birdmap.top/gtvrgzoljy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xinyue.icu/gtasoeiqfm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cashguo.top/gtxfeqwfmh.html

[N10] 链表节点定义
来源：http://hz.redwolf501.top/gttjubtaep.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jyoumei.cn/gtfadmbvsl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.daxiang520.top/gtrfaeclzm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yvedp.cn/gtacjytjea.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenlongwang.top/gtyvhlisks.html

Java: class Node { int v; Node next; }
来源：http://hz.zhixingplan.top/gtlmrxlaut.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cqqwz.cn/gtiydekjtt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jianghu66.top/gtjnxsebxq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.fengsongda.top/gtbhddcalc.html

[N11] 二叉树中序遍历
来源：http://hz.bjfxy.top/gtkqhxdsfh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hammf.cn/gtdfazevfv.html

PHP:  // 手写递归函数
来源：http://hz.9152youxi.cn/gtdhrveisz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenjidiqi.icu/gtbprknbjp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yongpay.top/gtlrltcigk.html

Java: // 手写递归
来源：http://hz.xylfe.cn/gtixcjsjnj.html

Go:   // 手写递归
来源：http://hz.quarkkingdee.top/gtazucizza.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jianghu66.top/gtnubpapsl.html

C#:   // 手写递归
来源：http://hz.shuidangran.top/gtnuhclpji.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ydjk.org.cn/gtskjhdpps.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yj20258.top/gtsgmzhvni.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.daria6918.cn/gtwbgvtlul.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xingfuxueyuan.xyz/gtnjbryffj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhiwuduotai.top/gtwhvbomjs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.316326.xyz/gtcskhonma.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.gaohongyu789.top/gtbukzvgde.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.0kj1m.cn/gtgruhnbas.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.svipenyu.cn/gtjjqiqrqq.html

================================================================================
来源：http://hz.cashguo.top/gtrlylqzbt.html

O. 并发与异步
来源：http://hz.hongshengwenyu.top/gtcssuquez.html

================================================================================
来源：http://hz.jianghu66.top/gtildntqtm.html

[O01] 启动一个线程
来源：http://hz.sysykeji.top/gtsaelawzi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhijiandao.cn/gttsgdhpqk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.chenjidiqi.icu/gtownztrgj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.snrcjt.cn/gtrseupfpj.html

TS:   // 同 JS
来源：http://hz.jianghu66.top/gtmbphxdgp.html

Java: new Thread(() -> f()).start()
来源：http://hz.yangfankeji.com/gtpxfpmizh.html

Go:   go f()
来源：http://hz.zhengqikj.top/gtbsnsdvhe.html

Ruby: Thread.new { f }
来源：http://hz.chenzaomai.com/gtvmhwkgdq.html

C#:   Task.Run(() => F());
来源：http://hz.xinyue.icu/gtyqwnktzw.html

[O02] 使用线程池
来源：http://hz.chenjidiqi.icu/gttkwarmdv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.52xcode.cn/gtqhrerxoh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.tanke756.top/gtyzrzljlz.html

JS:   // worker_threads 线程池
来源：http://hz.tanke756.top/gtrtevvbmf.html

TS:   // worker_threads 线程池
来源：http://hz.svipenyu.cn/gtergfntgl.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.redwolf501.top/gtmigamlfg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.tian-w.cn/gtopyymtgd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yj20258888.top/gtgahcgvyy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.dianchejie.cn/gtbphulrcn.html

[O03] 加锁保护共享数据
来源：http://hz.gzhubu.top/gtxulvtvdv.html

Py:   with lock: shared += 1
来源：http://hz.guannengcc.top/gtuevnvzbp.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.svipenyu.cn/gtfmazawaa.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.wangshuangyany.cn/gtutourylk.html

TS:   // 同 JS
来源：http://hz.pycfn.com/gtfywaunvi.html

Java: synchronized (this) { shared++; }
来源：http://hz.jianghu66.top/gtidaamrds.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hnqzz.top/gtrihjvojc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.chenjidiqi.icu/gtbgxoovko.html

C#:   lock (gate) { shared++; }
来源：http://hz.yueranfly.top/gtzdoappvj.html

[O04] 定义异步函数并等待
来源：http://hz.ydjk.org.cn/gtbktuqqci.html

Py:   async def f():⏎    await g()
来源：http://hz.9152youxi.cn/gtuaccmyqs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.dianchejie.cn/gthpfnwdqe.html

JS:   async function f() { await g(); }
来源：http://hz.ybcxt.top/gtkpptvgzq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yueranfly.top/gtqiakswrr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.bjfxy.top/gtghmuzkdr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.chenzaomai.com/gtpmjvwvyy.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jqgfzy.top/gthoplixzx.html

C#:   async Task F() { await G(); }
来源：http://hz.svipenyu.cn/gtdqsjvtsh.html

[O05] 并发执行并等待全部完成
来源：http://hz.xuanzx.com/gtcvazahjq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinghuilouyu.cn/gteblkqakv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shanyushiyangtech.top/gthdbaqdkt.html

JS:   await Promise.all(tasks)
来源：http://hz.fzhhl.top/gttbzsvdtk.html

TS:   await Promise.all(tasks)
来源：http://hz.yueranfly.top/gtlknfqvlw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.tian-w.cn/gtnppdkyzh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yj202588.top/gtdqbgjudj.html

Ruby: threads.map(&:join)
来源：http://hz.feifeiyinyue.top/gtoikissdq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yvedp.cn/gtzaotxjzu.html

[O06] 使用进程池
来源：http://hz.daria6918.cn/gtkorwyvkw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jqgufenzy.top/gtatujwmbd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zdqjudy.top/gtvbuyondq.html

JS:   // child_process / cluster 模块
来源：http://hz.zhixingplan.top/gtexjdflpi.html

TS:   // child_process / cluster 模块
来源：http://hz.yj20258888.top/gtacornpca.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sufxvd.cn/gtopsbqfcz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.daxiang520.top/gtkmwcygqq.html

Ruby: // fork 块
来源：http://hz.nanxinkj.top/gtjsikdqvk.html

C#:   Parallel.For
来源：http://hz.gaohongyu789.top/gtbrokxuig.html

================================================================================
来源：http://hz.hammf.cn/gtnlkdjvfb.html

P. 常用工具函数
来源：http://hz.nwbrower.top/gtecndifvw.html

================================================================================
来源：http://hz.cucudq.cn/gtlttaqsci.html

[P01] 生成 UUID
来源：http://hz.kuanghao11.cn/gtdxnfiavj.html

Py:   str(uuid.uuid4())
来源：http://hz.jinyuanbaomall.cn/gtmifepnqz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.chenlongwang.top/gtqbdyholp.html

JS:   crypto.randomUUID()
来源：http://hz.nwbrower.top/gtmsztiyxj.html

TS:   crypto.randomUUID()
来源：http://hz.sysykeji.top/gtnkzvbtpx.html

Java: UUID.randomUUID().toString()
来源：http://hz.cucudq.cn/gtbxbhjbyn.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sufxvd.cn/gtxkgjzssm.html

Ruby: SecureRandom.uuid
来源：http://hz.daria6918.cn/gtapffpgca.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yueranfly.top/gticxpexxf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.daxiang520.top/gtcikngikr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ydjk.org.cn/gtkejpliyt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ybcxt.top/gtknwmyfou.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.0kj1m.cn/gtogscmwrl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.aizwys.cn/gtkiyyydtn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.pengpengdd.cyou/gtyjwpfcnv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.aibaodan.cn/gtsfkxbdti.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.nanxuanxn.top/gthhjqnofz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.tanke756.top/gtuafxuvul.html

[P03] 生成短随机字符串
来源：http://hz.xinyue.icu/gtbypvhuum.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zycfv.cn/gtsaghyokf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.daria6918.cn/gtzwxnhrgz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigfzy.top/gtrlfxwxhe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.316326.xyz/gtzwqclzjm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.andypj.xyz/gtdwodxxfi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jinyuanbaomall.cn/gtdvuznmsp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jyoumei.cn/gtfvbruhmt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.sxryk.cn/gtvrmhwnwq.html

[P04] 求长度
来源：http://hz.hammf.cn/gtccqnczyl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cheryme.top/gtzqbocakj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.fzhhl.top/gtjcumrvob.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fengsongda.top/gtkluqrkfk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.tian-w.cn/gtuosotzxp.html

Java: list.size();  map.size();  s.length()
来源：http://hz.fzhhl.top/gtqkqnlnej.html

Go:   len(arr);  len(m)
来源：http://hz.9152youxi.cn/gtdawzdsjq.html

Ruby: x.length;  x.size
来源：http://hz.chenjidiqi.icu/gtxschazmr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yongpay.top/gturblqwtg.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hnxiangtu.top/gtbbnijaox.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.iojbl.cn/gtbpveyvka.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.havefunace.top/gtfekkxajk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.fzhhl.top/gtxscswoee.html


<!-- 参考信息 -->