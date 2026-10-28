代发 wailian999

TS:   resp.ok;  resp.status
来源：http://hz.zhijiandao.cn/gtszkxfcdn.html

Java: resp.statusCode()
来源：http://hz.xuanzx.com/gtaoutwvie.html

Go:   resp.StatusCode
来源：http://hz.xziqi.cn/gtjgipznlp.html

Ruby: resp.code.to_i
来源：http://hz.9152youxi.cn/gtqhxlfesl.html

C#:   (int)resp.StatusCode
来源：http://hz.jinqigfzy.top/gtenwytcli.html

[L08] 并发请求多个地址
来源：http://hz.chenjidiqi.icu/gtnkurcnja.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yonumen.top/gtovbcxwhn.html

PHP:  curl_multi_init() 系列
来源：http://hz.fzhhl.top/gttelhifmt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cheryme.top/gtlzkswxen.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xylfe.cn/gtsrboctrr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.guowangkeji.top/gttoouzfgz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yj202588.top/gtjpauulry.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.svipenyu.cn/gtkyvgbfiu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.redwolf501.top/gtrnfmktqu.html

================================================================================
来源：http://hz.zhijiandao.cn/gtmiayqhhg.html

M. 命令行 / 进程 / 环境
来源：http://hz.ydzc1.top/gtpjdhurss.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtfuzxcywc.html

[M01] 读取命令行参数
来源：http://hz.xylfe.cn/gtxkqxmjep.html

Py:   sys.argv[1:]
来源：http://hz.xinyue.icu/gtxutdocng.html

PHP:  $argv;  $argc;
来源：http://hz.havefunace.top/gtkjxigkiw.html

JS:   process.argv.slice(2)
来源：http://hz.wangdashe.top/gtovrruuku.html

TS:   process.argv.slice(2)
来源：http://hz.yanxiufei.cn/gtjnsbbckp.html

Java: args 数组（main 方法参数）
来源：http://hz.zhengqikj.top/gtnwwfbkwu.html

Go:   os.Args[1:]
来源：http://hz.smart0.xyz/gtvsoeljpg.html

Ruby: ARGV
来源：http://hz.cqqwz.cn/gtydigkjag.html

C#:   args 数组（Main 方法参数）
来源：http://hz.316326.xyz/gtkggiftxh.html

[M02] 读取环境变量
来源：http://hz.chenjidiqi.icu/gtfxhuprpg.html

Py:   os.environ.get("HOME")
来源：http://hz.9152youxi.cn/gtabkfzwxs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jqgfzy.top/gtrtlopgtl.html

JS:   process.env.HOME
来源：http://hz.gzhubu.top/gtmlyefqmu.html

TS:   process.env.HOME
来源：http://hz.jyoumei.cn/gtywxbfxgu.html

Java: System.getenv("HOME")
来源：http://hz.bjfxy.top/gtnhcramwl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.0kj1m.cn/gticwoocqp.html

Ruby: ENV["HOME"]
来源：http://hz.zhoulong.xyz/gtvjlsrkju.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenjidiqi.icu/gtneslrtdh.html

[M03] 执行外部命令
来源：http://hz.jqgfzy.top/gtyslomyjx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ppjwa.cn/gtcadhhdkz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shuidangran.top/gtlkwxalmy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ppjwa.cn/gtfamfrcex.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xziqi.cn/gtnmsjgakl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.shanyushiyangtech.top/gtspikebmi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhengqikj.top/gtpjvhklnz.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.chenlongwang.top/gtnthzhjqu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.mhx1999.top/gtzbfsewsk.html

[M04] 获取当前工作目录
来源：http://hz.yj202588.top/gtmbviqlna.html

Py:   os.getcwd()
来源：http://hz.gzhubu.top/gtjfoqtgnb.html

PHP:  getcwd();
来源：http://hz.chenjidiqi.icu/gtzsaduvez.html

JS:   process.cwd()
来源：http://hz.zhiwuduotai.top/gtwtjfbnmv.html

TS:   process.cwd()
来源：http://hz.guannengcc.top/gtwevwijec.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yj20258.top/gtrpuizcmw.html

Go:   os.Getwd()
来源：http://hz.haohaochexian.top/gtveybhxxm.html

Ruby: Dir.pwd
来源：http://hz.feifeiyinyue.top/gtygrotbzi.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.chenjidiqi.icu/gtgbgxgdhn.html

[M05] 设置退出码
来源：http://hz.tianlin.xyz/gtumwmnapz.html

Py:   sys.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtraunrlwf.html

PHP:  exit(1);
来源：http://hz.aibaodan.cn/gtrjweniis.html

JS:   process.exit(1)
来源：http://hz.zycfv.cn/gtbizplyfv.html

TS:   process.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtehibluzf.html

Java: System.exit(1)
来源：http://hz.haohaochexian.top/gtgtwnqwtb.html

Go:   os.Exit(1)
来源：http://hz.nanxinkj.top/gtxawfpknj.html

Ruby: exit 1
来源：http://hz.316326.xyz/gtgqgwzxry.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.guannengcc.top/gtbhcbmbdq.html

[M06] 向标准错误输出
来源：http://hz.andypj.xyz/gtdbhmijwf.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nanxinkj.top/gtedmjufhp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.svipenyu.cn/gtcbdfvfvx.html

JS:   console.error("err")
来源：http://hz.smart0.xyz/gtlpekgdst.html

TS:   console.error("err")
来源：http://hz.gotoacloud.top/gtslueshkn.html

Java: System.err.println("err")
来源：http://hz.hysaishi.cn/gtclsexiao.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.svipenyu.cn/gtsmnxvdph.html

Ruby: warn "err"
来源：http://hz.haohaochexian.top/gtpbnfkmfc.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shangyingyoupin.top/gtmvqfhjxd.html

[M07] 判断是否为主入口
来源：http://hz.yangfankeji.com/gtpzfytxcv.html

Py:   if __name__ == "__main__":
来源：http://hz.jlsjyb.cn/gtucvvvhnr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.smart0.xyz/gtaybgueog.html

JS:   require.main === module
来源：http://hz.ehwqpu.com/gtmjajhohb.html

TS:   require.main === module
来源：http://hz.quarkkingdee.top/gtkiqjrbmq.html

Java: public static void main(String[] args)
来源：http://hz.aibaodan.cn/gtexmliioh.html

Go:   func main()
来源：http://hz.nwbrower.top/gtbswtuqsb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yj20258888.top/gtsqxrhkox.html

C#:   static void Main(string[] args)
来源：http://hz.316326.xyz/gtaeuzvisx.html

[M08] 获取系统与运行时信息
来源：http://hz.quarkkingdee.top/gtzvdcxubh.html

Py:   platform.system();  platform.python_version()
来源：http://hz.tanke756.top/gtdbwpagkx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.mhx1999.top/gtvbdhnfdl.html

JS:   process.platform;  process.version
来源：http://hz.shanyushiyangkeji.top/gtehljxlli.html

TS:   process.platform;  process.version
来源：http://hz.fengsongda.top/gtiuzveomy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ppjwa.cn/gtndtajacr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jqgufenzy.top/gtkspqxbig.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.dianchejie.cn/gtnuwqjupb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xylfe.cn/gthgifbsnq.html

================================================================================
来源：http://hz.ybcxt.top/gtkfspqegh.html

N. 数据结构与算法
来源：http://hz.jinyuanbaomall.cn/gtjmvefvpj.html

================================================================================
来源：http://hz.hywenlv.cn/gtcdwmugdw.html

[N01] 二分查找（有序数组）
来源：http://hz.yj202588.top/gtbwecytlu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hnqzz.top/gtzlehicgx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.redwolf501.top/gtlvekdwmj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zdqjudy.top/gtglskhtlk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.52xcode.cn/gtaazksgya.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenzaomai.com/gtuhijztvx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.nwbrower.top/gtdrbynjco.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.c1oappe.top/gtngztylfi.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.fengsongda.top/gtqcmgvwjz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.nanxuanxn.top/gtchfekhgt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jqgufenzy.top/gtpzahwanv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hywenlv.cn/gtjikxezrc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.haohaochexian.top/gtmkfcagve.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenjidiqi.icu/gtyfrvfyuf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinghuilouyu.cn/gtetsvpbsh.html

Go:   slices.Sort(arr)
来源：http://hz.shanyushiyangtech.top/gtanvtaagc.html

Ruby: arr.sort
来源：http://hz.yj20258888.top/gtzinmzvcg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cheryme.top/gtdpeeosep.html

[N03] 快速排序（分治示例）
来源：http://hz.0kj1m.cn/gthoevoslb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.redwolf501.top/gthdxoikzw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zdqjudy.top/gtbgvpvvfq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ivvv.top/gtrafncxqm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cucudq.cn/gtcjsgeupe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yongpay.top/gtdgtkwylf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.snrcjt.cn/gtbzuiafxm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gotoacloud.top/gtrjnjlvtl.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jinqigufen.top/gthrcbbpnr.html

[N04] 斐波那契数列
来源：http://hz.yanxiufei.cn/gtcqjwqakb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hnqzz.top/gtjxzztpcw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.wangdashe.top/gtxahkurln.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tanke756.top/gtesjkoyou.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zdqjudy.top/gtnppigszj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gotoacloud.top/gtuyhlvqoy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sufxvd.cn/gtxlayjklh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.nanxuanxn.top/gtpxqdzcld.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ydjk.org.cn/gtqhtwqopx.html

[N05] 最大公约数
来源：http://hz.yvedp.cn/gteszaqxlg.html

Py:   math.gcd(a, b)
来源：http://hz.xinyue.icu/gtvduhwwkr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.quarkkingdee.top/gtdhrunmhj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cheryme.top/gtzaiylsru.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tanke756.top/gtjmzkorki.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sweek.top/gtgrzssrzx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yuanzhike.top/gtddrwhjnn.html

Ruby: a.gcd(b)
来源：http://hz.cheryme.top/gtjvdkcors.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinqigufen.top/gtwllageaz.html

[N06] 判断回文字符串
来源：http://hz.dianchejie.cn/gtnqrizxia.html

Py:   s == s[::-1]
来源：http://hz.daria6918.cn/gtxcwcvcxi.html

PHP:  $s === strrev($s);
来源：http://hz.zycfv.cn/gtpbaxgvvn.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jinghuilouyu.cn/gtnxeboczk.html

TS:   s === [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtdanercak.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cdnleiting.top/gtghzfpsoj.html

Go:   // 双指针从两端比较
来源：http://hz.gzhubu.top/gtswwcnurp.html

Ruby: s == s.reverse
来源：http://hz.feifeiyinyue.top/gtkextiqyl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hnqzz.top/gtsglrfnfv.html

[N07] 两数之和（返回下标）
来源：http://hz.chenlongwang.top/gtlscvyoyi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ivvv.top/gtluczmevv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhengqikj.top/gtuhxzjwic.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.tanke756.top/gtncqpergn.html

TS:   // 手写 Map<string, number>
来源：http://hz.andypj.xyz/gtxuabfwia.html

Java: // 手写 HashMap
来源：http://hz.yuanzhike.top/gtebqepllw.html

Go:   // 手写 map[int]int
来源：http://hz.zycfv.cn/gtbnfodwxf.html

Ruby: // 手写 Hash
来源：http://hz.zhongyouzk.top/gtelafdzoz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.dianchejie.cn/gtlngiyjcv.html

[N08] 生成全排列
来源：http://hz.nanxinkj.top/gtezvqsrrq.html

Py:   itertools.permutations(arr)
来源：http://hz.jlsjyb.cn/gtwdnylggs.html

PHP:  // 手写递归交换
来源：http://hz.hnxiangtu.top/gtfpgjwnpw.html

JS:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtzfzhcjjf.html

TS:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtfafeubhg.html

Java: // 手写回溯递归
来源：http://hz.9152youxi.cn/gtedfwjyaa.html

Go:   // 手写回溯递归
来源：http://hz.52xcode.cn/gtoxrnyucw.html

Ruby: arr.permutation.to_a
来源：http://hz.yonumen.top/gtwhfozivl.html

C#:   // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtuegzxycu.html

[N09] 栈与队列
来源：http://hz.aizwys.cn/gtmlxduqqf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.daxiang520.top/gtjwsafpxe.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.guowangkeji.top/gtdqklrpua.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.dianchejie.cn/gtwvtcynax.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.chenjidiqi.icu/gtnlhziyuv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ppjwa.cn/gtlbrcjcul.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.c1oappe.top/gtwwghrdwb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sxryk.cn/gtpwtwltqq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.dashuyun.cn/gtxlmzsxde.html

[N10] 链表节点定义
来源：http://hz.cqqwz.cn/gtxbhdpdwa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jianghu66.top/gtdplhppgn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.aibaodan.cn/gtxliqrzvp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhijiandao.cn/gtmftsnebp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jlsjyb.cn/gtlpjidzvg.html

Java: class Node { int v; Node next; }
来源：http://hz.daria6918.cn/gtymyncqsg.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hnqzz.top/gtkqstaipt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cdnleiting.top/gtrhzzqgfv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hammf.cn/gteqmwqldb.html

[N11] 二叉树中序遍历
来源：http://hz.shanyushiyangkeji.top/gttzkolwnh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.c1oappe.top/gtpjrcxyao.html

PHP:  // 手写递归函数
来源：http://hz.jqgufenzy.top/gturykiavp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yanxiufei.cn/gtkdjeukqg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinghuilouyu.cn/gtvukdugeu.html

Java: // 手写递归
来源：http://hz.ehwqpu.com/gtrrebibbe.html

Go:   // 手写递归
来源：http://hz.shangyingyoupin.top/gtzkpwtezg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.gzhubu.top/gtebbqnwyj.html

C#:   // 手写递归
来源：http://hz.hysaishi.cn/gtjnbvavlu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.0kj1m.cn/gtzdjrayrd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tanke756.top/gtyqfdfitq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xinyue.icu/gtzpgniitq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.feifeiyinyue.top/gtznjxxidl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aibaodan.cn/gtqcgqtteu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cucudq.cn/gtyztfdgcu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yueranfly.top/gtwyknjebe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.wangdashe.top/gtexgbstez.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.kuanghao11.cn/gtklbyabzw.html

================================================================================
来源：http://hz.iojbl.cn/gtyeohsksb.html

O. 并发与异步
来源：http://hz.nanxuanxn.top/gtqcwptmki.html

================================================================================
来源：http://hz.guowangkeji.top/gtcxclvocu.html

[O01] 启动一个线程
来源：http://hz.52xcode.cn/gtzasxrlmn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cdnleiting.top/gtwedwnpfu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.bjfxy.top/gtcsxhnpog.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.c1oappe.top/gtvnfccfuk.html

TS:   // 同 JS
来源：http://hz.hnqzz.top/gtuwkwghnv.html

Java: new Thread(() -> f()).start()
来源：http://hz.cheryme.top/gtxzenzyga.html

Go:   go f()
来源：http://hz.pycfn.com/gtfbniitza.html

Ruby: Thread.new { f }
来源：http://hz.redwolf501.top/gtlluguiko.html

C#:   Task.Run(() => F());
来源：http://hz.c1oappe.top/gttjxvcntx.html

[O02] 使用线程池
来源：http://hz.svipenyu.cn/gtimiwnpmm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.0kj1m.cn/gtfdjnujsj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.tian-w.cn/gtyfipvqqt.html

JS:   // worker_threads 线程池
来源：http://hz.jiagoushi.top/gtayxwfxyo.html

TS:   // worker_threads 线程池
来源：http://hz.jiagoushi.top/gtqeojipdo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yueranfly.top/gtwxioxvbu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.feifeiyinyue.top/gtlzmuiofg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ydjk.org.cn/gtofwdizcj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yangfankeji.com/gtwfxpefca.html

[O03] 加锁保护共享数据
来源：http://hz.iojbl.cn/gtqrxsizgv.html

Py:   with lock: shared += 1
来源：http://hz.ybcxt.top/gtzmzhhhpu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.gaohongyu789.top/gtmemqonsr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shzxlz.cn/gttwptnwel.html

TS:   // 同 JS
来源：http://hz.tianlin.xyz/gtxssmtroq.html

Java: synchronized (this) { shared++; }
来源：http://hz.wangdashe.top/gtgkdzmxeh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xylfe.cn/gtsczenhsn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yuanzhike.top/gthaljqyzv.html

C#:   lock (gate) { shared++; }
来源：http://hz.zycfv.cn/gtcjxywqjd.html

[O04] 定义异步函数并等待
来源：http://hz.jinyuanbaomall.cn/gtmpgbvdwu.html

Py:   async def f():⏎    await g()
来源：http://hz.fzhhl.top/gtjchydfbe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ehwqpu.com/gtchbelzqa.html

JS:   async function f() { await g(); }
来源：http://hz.yangfankeji.com/gtebjggzue.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cucudq.cn/gtyffzpupj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.kuanghao11.cn/gtudtlksyh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhongyouzk.top/gtmrqlwsnq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.feifeiyinyue.top/gtjcqvvtpu.html

C#:   async Task F() { await G(); }
来源：http://hz.yonumen.top/gtwtlbohqg.html

[O05] 并发执行并等待全部完成
来源：http://hz.ivvv.top/gtjkbjhimh.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hysaishi.cn/gtlsqwgjjr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gotoacloud.top/gtzthplcwx.html

JS:   await Promise.all(tasks)
来源：http://hz.pycfn.com/gtlbtgaizi.html

TS:   await Promise.all(tasks)
来源：http://hz.shuidangran.top/gtwwgsrmdh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.kuanghao11.cn/gteszbwvxi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.guowangkeji.top/gtgpspfgqg.html

Ruby: threads.map(&:join)
来源：http://hz.hysaishi.cn/gtoxoxncws.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.bjfxy.top/gtsbgsqqgj.html

[O06] 使用进程池
来源：http://hz.hnxiangtu.top/gtdvurgsbm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.fzhhl.top/gtqgpobhuo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hnqzz.top/gttdxznmut.html

JS:   // child_process / cluster 模块
来源：http://hz.birdmap.top/gtnwbmeizg.html

TS:   // child_process / cluster 模块
来源：http://hz.ivvv.top/gtqeltsnlu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.svipenyu.cn/gtyjgprzds.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.dashuyun.cn/gtfyrvbqxu.html

Ruby: // fork 块
来源：http://hz.daxiang520.top/gticfceent.html

C#:   Parallel.For
来源：http://hz.zhijiandao.cn/gtulqwnqxc.html

================================================================================
来源：http://hz.c1oappe.top/gtwcovfhdr.html

P. 常用工具函数
来源：http://hz.sxryk.cn/gtpmgwepld.html

================================================================================
来源：http://hz.gotoacloud.top/gtaxxhutat.html

[P01] 生成 UUID
来源：http://hz.cheryme.top/gtjrkleiip.html

Py:   str(uuid.uuid4())
来源：http://hz.ydzc1.top/gtxsosktib.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ydjk.org.cn/gtgoabzuwm.html

JS:   crypto.randomUUID()
来源：http://hz.ydzc1.top/gtbyptvlzq.html

TS:   crypto.randomUUID()
来源：http://hz.zhiwuduotai.top/gtrkceluzr.html

Java: UUID.randomUUID().toString()
来源：http://hz.wangdashe.top/gtypbmsxea.html

Go:   // 用 github.com/google/uuid
来源：http://hz.fzhhl.top/gtunjnswtb.html

Ruby: SecureRandom.uuid
来源：http://hz.guowangkeji.top/gtsgtlxcph.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhiwuduotai.top/gtfcioittr.html

[P02] MD5 / SHA256 摘要
来源：http://hz.dashuyun.cn/gtkqqokbll.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.daxiang520.top/gtufnehcmi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jiagoushi.top/gtrzitmvrv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jlsjyb.cn/gttuyxrymn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.fzhhl.top/gteguuqrff.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.9152youxi.cn/gtyfaejuan.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.sweek.top/gthqdxxptm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cdnleiting.top/gtkggxptva.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cqqwz.cn/gtqxwujoii.html

[P03] 生成短随机字符串
来源：http://hz.sweek.top/gtjzoxbsda.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinyuanbaomall.cn/gtwlkiythn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cashguo.top/gtvtqxntag.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.mhx1999.top/gtiwwfglnr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhongyouzk.top/gtyvooijpw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.pengpengdd.cyou/gtjwpxhnge.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hywenlv.cn/gtntqmbman.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yongpay.top/gtmonvsmgq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.snrcjt.cn/gtbrvblljq.html

[P04] 求长度
来源：http://hz.guowangkeji.top/gtpozqzhkz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jqgfzy.top/gtpnicwsqc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jianghu66.top/gtpnwardzk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.guannengcc.top/gtixdyknkr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zdqjudy.top/gtxqpaidxk.html

Java: list.size();  map.size();  s.length()
来源：http://hz.svipenyu.cn/gtagiwjkzl.html

Go:   len(arr);  len(m)
来源：http://hz.pengpengdd.cyou/gtpzfieoxn.html

Ruby: x.length;  x.size
来源：http://hz.xylfe.cn/gtdybdmvnr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.vqdsnc.cn/gtmvgnjzrb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xingfuxueyuan.xyz/gtxiycprqy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yuxming.cn/gtssqjukhz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhiwuduotai.top/gtftqjfovq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.havefunace.top/gtkoxhmvml.html


<!-- 参考信息 -->