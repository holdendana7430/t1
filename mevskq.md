代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://hz.yueranfly.top/gtrjmwwokl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yonumen.top/gtpzyuqddh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.aizwys.cn/gtpvzznrtf.html

JS:   resp.ok;  resp.status
来源：http://hz.meibo888.top/gtrlztflxy.html

TS:   resp.ok;  resp.status
来源：http://hz.yonumen.top/gtjjaafxzz.html

Java: resp.statusCode()
来源：http://hz.snrcjt.cn/gtnkwxmpyz.html

Go:   resp.StatusCode
来源：http://hz.hongshengwenyu.top/gteukieeup.html

Ruby: resp.code.to_i
来源：http://hz.ivvv.top/gtdxkechum.html

C#:   (int)resp.StatusCode
来源：http://hz.iojbl.cn/gtrccfuetc.html

[L08] 并发请求多个地址
来源：http://hz.snrcjt.cn/gthszaropi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.dashuyun.cn/gtmdlzcckz.html

PHP:  curl_multi_init() 系列
来源：http://hz.cucudq.cn/gtaiseubjr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hnqzz.top/gtttxkgual.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenlongwang.top/gtabdbnokp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.0kj1m.cn/gtessrdukf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinghuilouyu.cn/gteypbgvgb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.daxiang520.top/gtcihaovew.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhongyouzk.top/gtctqymmfv.html

================================================================================
来源：http://hz.tianlin.xyz/gtqmuhntcc.html

M. 命令行 / 进程 / 环境
来源：http://hz.nanxinkj.top/gtrwctdjxm.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtydeaemgq.html

[M01] 读取命令行参数
来源：http://hz.shanyushiyangkeji.top/gtpyaomuvr.html

Py:   sys.argv[1:]
来源：http://hz.shzxlz.cn/gtwzulcmrq.html

PHP:  $argv;  $argc;
来源：http://hz.guowangkeji.top/gtnklezkdp.html

JS:   process.argv.slice(2)
来源：http://hz.ehwqpu.com/gtaclcyiqf.html

TS:   process.argv.slice(2)
来源：http://hz.52xcode.cn/gtrovgbjws.html

Java: args 数组（main 方法参数）
来源：http://hz.gotoacloud.top/gtrtjvvxnl.html

Go:   os.Args[1:]
来源：http://hz.fzhhl.top/gtuilnbdhr.html

Ruby: ARGV
来源：http://hz.zhiwuduotai.top/gttbkrgtbp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xingfuxueyuan.xyz/gtyokrayzu.html

[M02] 读取环境变量
来源：http://hz.0kj1m.cn/gtuynhzcxw.html

Py:   os.environ.get("HOME")
来源：http://hz.yanxiufei.cn/gtwcqxgqkf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hfpthk.cn/gtmmsdjxpt.html

JS:   process.env.HOME
来源：http://hz.ydzc1.top/gtjpqbwnlx.html

TS:   process.env.HOME
来源：http://hz.havefunace.top/gtozrtbisa.html

Java: System.getenv("HOME")
来源：http://hz.jianghu66.top/gtfjmqrwxp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.guannengcc.top/gtmrbzmswr.html

Ruby: ENV["HOME"]
来源：http://hz.xziqi.cn/gtxylngjew.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.fzhhl.top/gtaskdmkrb.html

[M03] 执行外部命令
来源：http://hz.9152youxi.cn/gtaqsvshum.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ehwqpu.com/gtdwcqbcwc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhoulong.xyz/gtdamvsuiy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnxiangtu.top/gtrrxlhtfs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.tian-w.cn/gtpsxvkqmg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sysykeji.top/gthfvqyeyi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.daria6918.cn/gtaxvsfsto.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hfpthk.cn/gttzjjobtr.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ybcxt.top/gtlnpzlgsx.html

[M04] 获取当前工作目录
来源：http://hz.ivvv.top/gtamvflnqa.html

Py:   os.getcwd()
来源：http://hz.tian-w.cn/gthuewfjin.html

PHP:  getcwd();
来源：http://hz.yj20258888.top/gtdkosghqd.html

JS:   process.cwd()
来源：http://hz.dianchejie.cn/gtpsvxqxmq.html

TS:   process.cwd()
来源：http://hz.andypj.xyz/gtndhriumr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.bjfxy.top/gtvriecefl.html

Go:   os.Getwd()
来源：http://hz.gaohongyu789.top/gtvctftziv.html

Ruby: Dir.pwd
来源：http://hz.jiagoushi.top/gtadfzepdr.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhijiandao.cn/gtkrwauxvs.html

[M05] 设置退出码
来源：http://hz.ivvv.top/gtxblgwgxb.html

Py:   sys.exit(1)
来源：http://hz.zycfv.cn/gtiiejnpmx.html

PHP:  exit(1);
来源：http://hz.gotoacloud.top/gtjcclxwaq.html

JS:   process.exit(1)
来源：http://hz.zhaomingkeji.xyz/gtzhwyqfur.html

TS:   process.exit(1)
来源：http://hz.ehwqpu.com/gtaxueiprk.html

Java: System.exit(1)
来源：http://hz.chenjidiqi.icu/gtukhcyscl.html

Go:   os.Exit(1)
来源：http://hz.hywenlv.cn/gtvfdrjbyz.html

Ruby: exit 1
来源：http://hz.xuetiantiany.cn/gtpzxbzulm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hysaishi.cn/gtvfwfkert.html

[M06] 向标准错误输出
来源：http://hz.yvedp.cn/gtpowekmkh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.tianlin.xyz/gteyybfgnx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.guannengcc.top/gtpbbopooh.html

JS:   console.error("err")
来源：http://hz.hammf.cn/gterkoxebb.html

TS:   console.error("err")
来源：http://hz.52xcode.cn/gtuhoieate.html

Java: System.err.println("err")
来源：http://hz.c1oappe.top/gtootkgrjk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hongshengwenyu.top/gtjpkprzgt.html

Ruby: warn "err"
来源：http://hz.yvedp.cn/gtctmadscs.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.dianchejie.cn/gtrlctupfc.html

[M07] 判断是否为主入口
来源：http://hz.ydjk.org.cn/gtrxnuktrn.html

Py:   if __name__ == "__main__":
来源：http://hz.vqdsnc.cn/gtijewzpxy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.haohaochexian.top/gtsemyabjo.html

JS:   require.main === module
来源：http://hz.shuidangran.top/gtgccodpkr.html

TS:   require.main === module
来源：http://hz.gogol.net.cn/gtgtnqdahc.html

Java: public static void main(String[] args)
来源：http://hz.yueranfly.top/gtqwzlfimu.html

Go:   func main()
来源：http://hz.hysaishi.cn/gtbfmperdv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.guowangkeji.top/gtwwikfdgk.html

C#:   static void Main(string[] args)
来源：http://hz.zycfv.cn/gtoiaargcr.html

[M08] 获取系统与运行时信息
来源：http://hz.dianchejie.cn/gtutecirop.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hywenlv.cn/gtppgetdop.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.316326.xyz/gtngwgiida.html

JS:   process.platform;  process.version
来源：http://hz.yonumen.top/gtigmlgqng.html

TS:   process.platform;  process.version
来源：http://hz.xinyue.icu/gtvxununmi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jiagoushi.top/gtslqtigya.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hysaishi.cn/gtjuysczyk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.pycfn.com/gtfnangmud.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shanyushiyangkeji.top/gtaxzsemof.html

================================================================================
来源：http://hz.gzhubu.top/gtaaqqynhu.html

N. 数据结构与算法
来源：http://hz.yanxiufei.cn/gtdysirwya.html

================================================================================
来源：http://hz.dianchejie.cn/gtyazafpbe.html

[N01] 二分查找（有序数组）
来源：http://hz.hnqzz.top/gteopzoawp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.dianchejie.cn/gtqdrsjuoe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinyuanbaomall.cn/gthqpezabo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sufxvd.cn/gtkretuiwe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.snrcjt.cn/gtazjoxezj.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.fengsongda.top/gtiklkiiad.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.dianchejie.cn/gtyvmxlmtu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.nanxuanxn.top/gtvwlrlokm.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhixingplan.top/gtxqhpbgjd.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jlsjyb.cn/gtczkoeemo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hfpthk.cn/gtkdjdgosj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xziqi.cn/gtoaisyehv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ivvv.top/gttdvxdoaz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ydzc1.top/gtnmlznlgl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.havefunace.top/gtaxdfttcq.html

Go:   slices.Sort(arr)
来源：http://hz.iojbl.cn/gtlbyyrgnt.html

Ruby: arr.sort
来源：http://hz.cdnleiting.top/gtempnhhth.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.meibo888.top/gtxrsxwgac.html

[N03] 快速排序（分治示例）
来源：http://hz.cashguo.top/gtcfmdhkws.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.snrcjt.cn/gtzknqhhzp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.daxiang520.top/gtrxahkjdc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gtacjeffjb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shanyushiyangtech.top/gtyiyaktst.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xingfuxueyuan.xyz/gtuwbncpdf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hnqzz.top/gtioxektwb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ivvv.top/gttxtmgfkc.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhaomingkeji.xyz/gtiyijijna.html

[N04] 斐波那契数列
来源：http://hz.guowangkeji.top/gtkcsvavjl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jqgufenzy.top/gtlvkalpoi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.birdmap.top/gtmgoozqik.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dianchejie.cn/gtmehprxdd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xuetiantiany.cn/gtrhibpepk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cdnleiting.top/gtwojhssug.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.redwolf501.top/gtctdnwvmo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hfpthk.cn/gtxnbbppdx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.aibaodan.cn/gtfdwkgxdp.html

[N05] 最大公约数
来源：http://hz.jiagoushi.top/gtvxjstpaz.html

Py:   math.gcd(a, b)
来源：http://hz.fzhhl.top/gtpzvppyrk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hnqzz.top/gtsrsrtrha.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydzc1.top/gteizasgpc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhixingplan.top/gtdgabpsvd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ivvv.top/gtuhturuap.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenlongwang.top/gtpohtxpir.html

Ruby: a.gcd(b)
来源：http://hz.yonumen.top/gtjszkiwfg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yj20258.top/gtnpzpukqt.html

[N06] 判断回文字符串
来源：http://hz.dashuyun.cn/gtffhbwady.html

Py:   s == s[::-1]
来源：http://hz.nanxuanxn.top/gtfcvfpexo.html

PHP:  $s === strrev($s);
来源：http://hz.feifeiyinyue.top/gtelyfvdye.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zycfv.cn/gtzyfphlxa.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xylfe.cn/gtrgzjkeqb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shanyushiyangtech.top/gtqytpbbic.html

Go:   // 双指针从两端比较
来源：http://hz.jianghu66.top/gtaxhwzgqu.html

Ruby: s == s.reverse
来源：http://hz.wangdashe.top/gtyajhrgnb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhengqikj.top/gtcjnyodoh.html

[N07] 两数之和（返回下标）
来源：http://hz.yanxiufei.cn/gtdoodvedl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.9152youxi.cn/gtypkwofyu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.nanxuanxn.top/gtjwttmteu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sweek.top/gthwjwmpre.html

TS:   // 手写 Map<string, number>
来源：http://hz.dashuyun.cn/gthqejnxjg.html

Java: // 手写 HashMap
来源：http://hz.chenlongwang.top/gtlgrjphbg.html

Go:   // 手写 map[int]int
来源：http://hz.wangdashe.top/gthljvdkut.html

Ruby: // 手写 Hash
来源：http://hz.birdmap.top/gtbksybpfl.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.wangdashe.top/gtnskxepxo.html

[N08] 生成全排列
来源：http://hz.meibo888.top/gtikefliaw.html

Py:   itertools.permutations(arr)
来源：http://hz.yanxiufei.cn/gttcsoigpq.html

PHP:  // 手写递归交换
来源：http://hz.9152youxi.cn/gtyuyzsdcc.html

JS:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtytokvjad.html

TS:   // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtsxpuqskb.html

Java: // 手写回溯递归
来源：http://hz.jiagoushi.top/gtlgyzfjyh.html

Go:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtweeywjum.html

Ruby: arr.permutation.to_a
来源：http://hz.ydjk.org.cn/gtqeebisop.html

C#:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtolpviajy.html

[N09] 栈与队列
来源：http://hz.hywenlv.cn/gtqyhfzwqs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.chenzaomai.com/gtifcryccr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.wangshuangyany.cn/gttggmyuhj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.chenjidiqi.icu/gtohnuokfa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hysaishi.cn/gtfsxjsbaq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.daria6918.cn/gtvkrhfurm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shangyingyoupin.top/gtoewhihhv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.fzhhl.top/gtsslrqvhi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.redwolf501.top/gtcoehguhv.html

[N10] 链表节点定义
来源：http://hz.jyoumei.cn/gtlvjnlbak.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.wangdashe.top/gtasynzqog.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.9152youxi.cn/gtoigaogvl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhengqikj.top/gtodhmhoov.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yj20258.top/gtssqtqajm.html

Java: class Node { int v; Node next; }
来源：http://hz.daria6918.cn/gtihvdvilz.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.pengpengdd.cyou/gtsfwaqelu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinyuanbaomall.cn/gtaxkoydwc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hongshengwenyu.top/gtmmvixmgq.html

[N11] 二叉树中序遍历
来源：http://hz.yvedp.cn/gtzbovnbzg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yj20258.top/gtbifltpuq.html

PHP:  // 手写递归函数
来源：http://hz.ybcxt.top/gtqoyhpwbb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.c1oappe.top/gtanqsewis.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sysykeji.top/gtgfxklcwi.html

Java: // 手写递归
来源：http://hz.jianghu66.top/gtgcxbunfz.html

Go:   // 手写递归
来源：http://hz.ydjk.org.cn/gtokvjuhuh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cucudq.cn/gtrptvgldn.html

C#:   // 手写递归
来源：http://hz.wangdashe.top/gtmhlyeqke.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhoulong.xyz/gtumttyjmz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinyuanbaomall.cn/gtrgjbgbtg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ppjwa.cn/gtbjgtjrhl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxinkj.top/gtvcmcuqhk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinyuanbaomall.cn/gtymmsvjxy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sxryk.cn/gtoijeeley.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yuxming.cn/gtdlvqszmc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.pengpengdd.cyou/gtgxavdfai.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258.top/gtupgliyua.html

================================================================================
来源：http://hz.yueranfly.top/gtueraspxr.html

O. 并发与异步
来源：http://hz.hysaishi.cn/gthsoaywxj.html

================================================================================
来源：http://hz.xuanzx.com/gtdscowwmv.html

[O01] 启动一个线程
来源：http://hz.ybcxt.top/gtsordnnjw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cashguo.top/gtmharynck.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.tanke756.top/gtwvvgjpzs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.tian-w.cn/gtfzzqjzid.html

TS:   // 同 JS
来源：http://hz.yonumen.top/gtzomrczwn.html

Java: new Thread(() -> f()).start()
来源：http://hz.yonumen.top/gtqnwdntwr.html

Go:   go f()
来源：http://hz.c1oappe.top/gtnqjvqtoy.html

Ruby: Thread.new { f }
来源：http://hz.gaohongyu789.top/gtzqeodlir.html

C#:   Task.Run(() => F());
来源：http://hz.guowangkeji.top/gtphvrkpvw.html

[O02] 使用线程池
来源：http://hz.jlsjyb.cn/gtwwcpinvw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.chenzaomai.com/gtfkricrrw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yuxming.cn/gttqeiixbu.html

JS:   // worker_threads 线程池
来源：http://hz.jinqigufen.top/gtcmsmbehi.html

TS:   // worker_threads 线程池
来源：http://hz.havefunace.top/gtaibyohqm.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinghuilouyu.cn/gtzemoahrz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhongyouzk.top/gtghvyndtk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yuanzhike.top/gtqhuiaeqz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ydjk.org.cn/gtcacshabs.html

[O03] 加锁保护共享数据
来源：http://hz.zycfv.cn/gtwpazpzno.html

Py:   with lock: shared += 1
来源：http://hz.andypj.xyz/gttagugrah.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhijiandao.cn/gtkqfbomus.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ybcxt.top/gttkcakpvv.html

TS:   // 同 JS
来源：http://hz.snrcjt.cn/gthhqfzszv.html

Java: synchronized (this) { shared++; }
来源：http://hz.nanxuanxn.top/gtjdrocxfn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.vqdsnc.cn/gtdwovujin.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yvedp.cn/gtltfbkdcm.html

C#:   lock (gate) { shared++; }
来源：http://hz.pengpengdd.cyou/gtuyccyosb.html

[O04] 定义异步函数并等待
来源：http://hz.ehwqpu.com/gtpjbvuxuk.html

Py:   async def f():⏎    await g()
来源：http://hz.9152youxi.cn/gtfycvtumr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinghuilouyu.cn/gtskjedjrm.html

JS:   async function f() { await g(); }
来源：http://hz.zhijiandao.cn/gtkjctkpyl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.pycfn.com/gtejedqvgq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shangyingyoupin.top/gtxrlarneh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.meibo888.top/gtfzsnycvs.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hnqzz.top/gtnihjuomd.html

C#:   async Task F() { await G(); }
来源：http://hz.ydzc1.top/gtepggtajp.html

[O05] 并发执行并等待全部完成
来源：http://hz.xziqi.cn/gtvdoalmdc.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yueranfly.top/gtzxgbdfrx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yuanzhike.top/gtwrwfdtil.html

JS:   await Promise.all(tasks)
来源：http://hz.zhijiandao.cn/gteqsvzyyi.html

TS:   await Promise.all(tasks)
来源：http://hz.zhaomingkeji.xyz/gtepigvdnq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xuanzx.com/gtslkpzixw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.pengpengdd.cyou/gtczvezgcq.html

Ruby: threads.map(&:join)
来源：http://hz.jyoumei.cn/gtisinuajm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.meibo888.top/gtqhvuppnb.html

[O06] 使用进程池
来源：http://hz.havefunace.top/gtyvlspvah.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhaomingkeji.xyz/gtdovcesxt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yj202588.top/gtntolxvsu.html

JS:   // child_process / cluster 模块
来源：http://hz.zhongyouzk.top/gtjcfsgzwr.html

TS:   // child_process / cluster 模块
来源：http://hz.jinyuanbaomall.cn/gtwtdeqdnd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.fzhhl.top/gtuishclfk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhiwuduotai.top/gtklkkyczy.html

Ruby: // fork 块
来源：http://hz.haohaochexian.top/gtwsblpsbo.html

C#:   Parallel.For
来源：http://hz.zhongyouzk.top/gtzqhydert.html

================================================================================
来源：http://hz.tianlin.xyz/gtzidnepgn.html

P. 常用工具函数
来源：http://hz.yongpay.top/gtzcsjhtlf.html

================================================================================
来源：http://hz.xziqi.cn/gthxcnuazr.html

[P01] 生成 UUID
来源：http://hz.nanxinkj.top/gtqnlymjbs.html

Py:   str(uuid.uuid4())
来源：http://hz.quarkkingdee.top/gtwumlqsmv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.bjfxy.top/gtrrdpebzv.html

JS:   crypto.randomUUID()
来源：http://hz.yj20258.top/gtvlqplesh.html

TS:   crypto.randomUUID()
来源：http://hz.shuidangran.top/gtmmjptraf.html

Java: UUID.randomUUID().toString()
来源：http://hz.dianchejie.cn/gthtkkhcyr.html

Go:   // 用 github.com/google/uuid
来源：http://hz.birdmap.top/gtodjkxniq.html

Ruby: SecureRandom.uuid
来源：http://hz.xuetiantiany.cn/gtcpigurqr.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.bjfxy.top/gtxyiqyrej.html

[P02] MD5 / SHA256 摘要
来源：http://hz.havefunace.top/gtridzoseb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yuxming.cn/gtboepgcep.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.havefunace.top/gtczvukwea.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhiwuduotai.top/gtpxppcmoq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jqgfzy.top/gtexanvfxu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.bjfxy.top/gtduczdrqv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gogol.net.cn/gtoajfoocs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.bjfxy.top/gtnvtkuqrg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yvedp.cn/gtfogiibbg.html

[P03] 生成短随机字符串
来源：http://hz.0kj1m.cn/gtibxbuqpp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ydjk.org.cn/gtuvpxcgmw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.chenjidiqi.icu/gtmlfekorc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hongshengwenyu.top/gtgxvydyoe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.quarkkingdee.top/gtpykfbgzc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.meibo888.top/gtweikgeyh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cashguo.top/gtbnefkiuy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.quarkkingdee.top/gtykwmsltg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.nanxuanxn.top/gtfyqmmaif.html

[P04] 求长度
来源：http://hz.tanke756.top/gtvikjryjj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.52xcode.cn/gtfnrygeux.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shangyingyoupin.top/gtpgbmrhak.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cashguo.top/gtbhcufnqo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuxming.cn/gtgjhoqysi.html

Java: list.size();  map.size();  s.length()
来源：http://hz.chenlongwang.top/gtvfhnwizz.html

Go:   len(arr);  len(m)
来源：http://hz.andypj.xyz/gtfclguvad.html

Ruby: x.length;  x.size
来源：http://hz.sxryk.cn/gtiegabdjc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ywan-chungtsiang.top/gteekftxln.html


<!-- 参考信息 -->