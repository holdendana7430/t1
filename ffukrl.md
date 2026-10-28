代发 wailian999

C#:   (int)resp.StatusCode
来源：http://hz.pycfn.com/gtdohslynq.html

[L08] 并发请求多个地址
来源：http://hz.guannengcc.top/gtagslfxmn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.nanxuanxn.top/gtobvmgtzi.html

PHP:  curl_multi_init() 系列
来源：http://hz.yongpay.top/gtykicsmvc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenzaomai.com/gtelgabtjh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhongyouzk.top/gtxgoihayw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cqqwz.cn/gtoxyizlql.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.wangshuangyany.cn/gtadgthhuf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nanxinkj.top/gtfwzhgwtm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.feifeiyinyue.top/gteediilmy.html

================================================================================
来源：http://hz.aizwys.cn/gtkthqdnok.html

M. 命令行 / 进程 / 环境
来源：http://hz.dianchejie.cn/gtttlkpppr.html

================================================================================
来源：http://hz.chenzaomai.com/gtrmmluuuz.html

[M01] 读取命令行参数
来源：http://hz.vqdsnc.cn/gtjydnfpvi.html

Py:   sys.argv[1:]
来源：http://hz.52xcode.cn/gtwfrqwlkr.html

PHP:  $argv;  $argc;
来源：http://hz.gzhubu.top/gtcsakrdfq.html

JS:   process.argv.slice(2)
来源：http://hz.yj20258888.top/gtnrmrqeal.html

TS:   process.argv.slice(2)
来源：http://hz.bjfxy.top/gtxxzevbig.html

Java: args 数组（main 方法参数）
来源：http://hz.ybcxt.top/gtustaonwj.html

Go:   os.Args[1:]
来源：http://hz.jinyuanbaomall.cn/gtvlvhyiea.html

Ruby: ARGV
来源：http://hz.chenlongwang.top/gtnfsiwmfp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xuetiantiany.cn/gtlhazanux.html

[M02] 读取环境变量
来源：http://hz.yj202588.top/gttotlwwlp.html

Py:   os.environ.get("HOME")
来源：http://hz.bjfxy.top/gtyozvrqnh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yueranfly.top/gtqhbdapuv.html

JS:   process.env.HOME
来源：http://hz.hnqzz.top/gtqnogbbey.html

TS:   process.env.HOME
来源：http://hz.gotoacloud.top/gtahuplefy.html

Java: System.getenv("HOME")
来源：http://hz.guowangkeji.top/gtzckcffbe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xylfe.cn/gtawepnwop.html

Ruby: ENV["HOME"]
来源：http://hz.ehwqpu.com/gtojeideal.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yueranfly.top/gtldkctpjx.html

[M03] 执行外部命令
来源：http://hz.hnxiangtu.top/gtjlkqczvw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhoulong.xyz/gtitunfwva.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.9152youxi.cn/gthmohlqmr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnqzz.top/gtnkypcoeh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigfzy.top/gteihiscjp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zycfv.cn/gtbslgvboi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tianlin.xyz/gtohesdpnr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.0kj1m.cn/gtmteapooj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.fzhhl.top/gtzydxouqw.html

[M04] 获取当前工作目录
来源：http://hz.zhengqikj.top/gtwuytkzla.html

Py:   os.getcwd()
来源：http://hz.zhongyouzk.top/gtppccmtlt.html

PHP:  getcwd();
来源：http://hz.tanke756.top/gtrdtkvqyv.html

JS:   process.cwd()
来源：http://hz.fzhhl.top/gtsjakpgmv.html

TS:   process.cwd()
来源：http://hz.316326.xyz/gtweueoxbr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yj202588.top/gtjfpbmlzr.html

Go:   os.Getwd()
来源：http://hz.hywenlv.cn/gtdvpmpvys.html

Ruby: Dir.pwd
来源：http://hz.zycfv.cn/gtstrgixvd.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhengqikj.top/gtnuezlytz.html

[M05] 设置退出码
来源：http://hz.gotoacloud.top/gtxxcyukht.html

Py:   sys.exit(1)
来源：http://hz.316326.xyz/gtngwruysc.html

PHP:  exit(1);
来源：http://hz.yangfankeji.com/gtwvdlbiuz.html

JS:   process.exit(1)
来源：http://hz.cdnleiting.top/gtxvhswald.html

TS:   process.exit(1)
来源：http://hz.zhixingplan.top/gtyhqqqtxy.html

Java: System.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtybtevcbl.html

Go:   os.Exit(1)
来源：http://hz.feifeiyinyue.top/gtnyorcyxm.html

Ruby: exit 1
来源：http://hz.316326.xyz/gtjxhflqgq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sysykeji.top/gtvqikabio.html

[M06] 向标准错误输出
来源：http://hz.jianghu66.top/gtlbgrdtav.html

Py:   print("err", file=sys.stderr)
来源：http://hz.316326.xyz/gtenndesvs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.redwolf501.top/gtfmgamxth.html

JS:   console.error("err")
来源：http://hz.zhaomingkeji.xyz/gtkmywrdix.html

TS:   console.error("err")
来源：http://hz.xinyue.icu/gtcdzawowc.html

Java: System.err.println("err")
来源：http://hz.cheryme.top/gtrmufglhg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ybcxt.top/gtvldxnhpl.html

Ruby: warn "err"
来源：http://hz.tian-w.cn/gtpzttljmz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.daxiang520.top/gtlpqrukuj.html

[M07] 判断是否为主入口
来源：http://hz.jinqigufen.top/gtrzewhxia.html

Py:   if __name__ == "__main__":
来源：http://hz.hnqzz.top/gtmjdixugl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zycfv.cn/gtoslneyry.html

JS:   require.main === module
来源：http://hz.ydjk.org.cn/gteifbbaba.html

TS:   require.main === module
来源：http://hz.meibo888.top/gteuyafkme.html

Java: public static void main(String[] args)
来源：http://hz.jianghu66.top/gtksaylerz.html

Go:   func main()
来源：http://hz.zhongyouzk.top/gtucrureea.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhengqikj.top/gtyswobzsk.html

C#:   static void Main(string[] args)
来源：http://hz.jiagoushi.top/gtidlrlwxg.html

[M08] 获取系统与运行时信息
来源：http://hz.yueranfly.top/gtzrkbzfic.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ehwqpu.com/gtqzpcxnfz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.svipenyu.cn/gtaapdiltt.html

JS:   process.platform;  process.version
来源：http://hz.snrcjt.cn/gtfqgluyjw.html

TS:   process.platform;  process.version
来源：http://hz.bjfxy.top/gtxcavjigi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gogol.net.cn/gtbgznjtqe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sufxvd.cn/gtiqybazun.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cdnleiting.top/gthbnlpjwy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.vqdsnc.cn/gtuxkoeuum.html

================================================================================
来源：http://hz.xylfe.cn/gtrcifwomz.html

N. 数据结构与算法
来源：http://hz.andypj.xyz/gtoutrgxdr.html

================================================================================
来源：http://hz.tian-w.cn/gtcggydsgg.html

[N01] 二分查找（有序数组）
来源：http://hz.jqgfzy.top/gtgcbfzbhl.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.kuanghao11.cn/gtkklrtzmu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.nanxinkj.top/gtxgtfrqea.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.52xcode.cn/gtzteqqynv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenjidiqi.icu/gtwpwbkchi.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.birdmap.top/gtmxoafach.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cheryme.top/gtsynpfqej.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ybcxt.top/gtawnntrmv.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.birdmap.top/gtnwqrvfhi.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jinghuilouyu.cn/gtspbuzbcu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yuanzhike.top/gtleozgkzv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.daria6918.cn/gtxmfsgtej.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hnqzz.top/gtuzwexjds.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jianghu66.top/gttllyurxv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yj202588.top/gthcaifdnx.html

Go:   slices.Sort(arr)
来源：http://hz.yueranfly.top/gtezolcyok.html

Ruby: arr.sort
来源：http://hz.svipenyu.cn/gtucapkyos.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinqigufen.top/gtjycgqgjq.html

[N03] 快速排序（分治示例）
来源：http://hz.quarkkingdee.top/gtlxivizpo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xuetiantiany.cn/gtbbgcfgkh.html

PHP:  // 递归实现，或用 usort
来源：http://hz.316326.xyz/gtasiyodpv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenlongwang.top/gtvigcjdcc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yongpay.top/gtmroqriun.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj202588.top/gtigrvzdju.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhiwuduotai.top/gtulxzmvzw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.svipenyu.cn/gtbvoscnjh.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.guannengcc.top/gtsgdaaafx.html

[N04] 斐波那契数列
来源：http://hz.cdnleiting.top/gtdksmmhkw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jqgufenzy.top/gtnvzbgpsh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.birdmap.top/gteudgqjpz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xinyue.icu/gtkvbrjpii.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hywenlv.cn/gtpowpaamp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.svipenyu.cn/gtbbuwtmgi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jlsjyb.cn/gtmukperng.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinyuanbaomall.cn/gtqlsykbvq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.0kj1m.cn/gtflmkqieq.html

[N05] 最大公约数
来源：http://hz.fzhhl.top/gtxctrqtas.html

Py:   math.gcd(a, b)
来源：http://hz.zhiwuduotai.top/gtgsjrmzeg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ydjk.org.cn/gtrchkmidg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tianlin.xyz/gtygokjvgy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhongyouzk.top/gtacndwagb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.9152youxi.cn/gtrlxjgshc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.0kj1m.cn/gtttoxivxd.html

Ruby: a.gcd(b)
来源：http://hz.yj20258.top/gtijoxnrkv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jianghu66.top/gtugsawhxh.html

[N06] 判断回文字符串
来源：http://hz.yuanzhike.top/gtpomniolp.html

Py:   s == s[::-1]
来源：http://hz.ppjwa.cn/gtqhwifrrl.html

PHP:  $s === strrev($s);
来源：http://hz.zhoulong.xyz/gtkbjlywkj.html

JS:   s === [...s].reverse().join("")
来源：http://hz.iojbl.cn/gtkrhuwerl.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtlplykmpy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.haohaochexian.top/gtdgzeaylg.html

Go:   // 双指针从两端比较
来源：http://hz.gotoacloud.top/gtatgjdkpu.html

Ruby: s == s.reverse
来源：http://hz.hysaishi.cn/gtsdjtxtxb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.iojbl.cn/gtnotqpczj.html

[N07] 两数之和（返回下标）
来源：http://hz.yvedp.cn/gtuvyakkqg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jqgufenzy.top/gtqibxeahw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ydzc1.top/gthgdyqjkh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.tianlin.xyz/gtyufylolj.html

TS:   // 手写 Map<string, number>
来源：http://hz.hnxiangtu.top/gtbemhgves.html

Java: // 手写 HashMap
来源：http://hz.kuanghao11.cn/gtxdihosrk.html

Go:   // 手写 map[int]int
来源：http://hz.meibo888.top/gtxraksfdf.html

Ruby: // 手写 Hash
来源：http://hz.dashuyun.cn/gtettmbnhu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jlsjyb.cn/gtdvbeiutx.html

[N08] 生成全排列
来源：http://hz.jinqigfzy.top/gtdyblnhng.html

Py:   itertools.permutations(arr)
来源：http://hz.gaohongyu789.top/gtwbsvanmy.html

PHP:  // 手写递归交换
来源：http://hz.bjfxy.top/gtxlfxewri.html

JS:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtbbhdemgo.html

TS:   // 手写回溯递归
来源：http://hz.jiagoushi.top/gttxwwucwm.html

Java: // 手写回溯递归
来源：http://hz.daria6918.cn/gtbcymsdsd.html

Go:   // 手写回溯递归
来源：http://hz.ydzc1.top/gtlwecrasd.html

Ruby: arr.permutation.to_a
来源：http://hz.nanxuanxn.top/gtlvubvlxy.html

C#:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtjzxbnbfd.html

[N09] 栈与队列
来源：http://hz.zhaomingkeji.xyz/gtbxljgkag.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.316326.xyz/gthlkftvpz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yangfankeji.com/gtazvaauqs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.guowangkeji.top/gtuknlllst.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xinyue.icu/gtjpgshata.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.havefunace.top/gtpfpjoyva.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ppjwa.cn/gtxyokcwmt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hfpthk.cn/gtjyfsuzgq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hammf.cn/gtwahzqgva.html

[N10] 链表节点定义
来源：http://hz.svipenyu.cn/gtsraszcnn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ydjk.org.cn/gthgsjaeci.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ppjwa.cn/gtnyobevmd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.fzhhl.top/gtucgsqbxl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ydzc1.top/gtspfxkvif.html

Java: class Node { int v; Node next; }
来源：http://hz.yvedp.cn/gtnxkhjpyd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hfpthk.cn/gtgwcwtzzs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.fengsongda.top/gtkpsgdtlb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.snrcjt.cn/gtoniqqvdn.html

[N11] 二叉树中序遍历
来源：http://hz.cucudq.cn/gtbcdhooyl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.fengsongda.top/gtdzrquwpq.html

PHP:  // 手写递归函数
来源：http://hz.gotoacloud.top/gtdtrlxqat.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hywenlv.cn/gtxfwxnerh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gaohongyu789.top/gtgpeiorhw.html

Java: // 手写递归
来源：http://hz.sufxvd.cn/gtoteejpmn.html

Go:   // 手写递归
来源：http://hz.zhoulong.xyz/gtlaidgldc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jqgfzy.top/gtjxtsoabc.html

C#:   // 手写递归
来源：http://hz.yongpay.top/gtrpbjzdbs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hfpthk.cn/gtbkvwoqbp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cashguo.top/gtwabednzb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gotoacloud.top/gthsfqwkub.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.guowangkeji.top/gtcscjzbxy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinqigufen.top/gtljghuuqm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hfpthk.cn/gtdhuoxrxu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hnqzz.top/gtjengdmdb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yongpay.top/gtmyxjldbc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ivvv.top/gtlsxykpnj.html

================================================================================
来源：http://hz.xuetiantiany.cn/gthufsmaam.html

O. 并发与异步
来源：http://hz.zdqjudy.top/gtacvfggjo.html

================================================================================
来源：http://hz.aizwys.cn/gttwlvkpgz.html

[O01] 启动一个线程
来源：http://hz.yonumen.top/gtqumokfze.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhiwuduotai.top/gtrobxqvcn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xylfe.cn/gtyzgbnrwa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ehwqpu.com/gtityqwgdz.html

TS:   // 同 JS
来源：http://hz.hnxiangtu.top/gtarvzfpce.html

Java: new Thread(() -> f()).start()
来源：http://hz.shzxlz.cn/gtzzpnrhrp.html

Go:   go f()
来源：http://hz.ydjk.org.cn/gtdmlrxdmv.html

Ruby: Thread.new { f }
来源：http://hz.hongshengwenyu.top/gtybpgdelv.html

C#:   Task.Run(() => F());
来源：http://hz.yj202588.top/gtzwxkmilg.html

[O02] 使用线程池
来源：http://hz.snrcjt.cn/gtqazriooz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.tanke756.top/gtqnwssyse.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hnxiangtu.top/gtuxwiwaqu.html

JS:   // worker_threads 线程池
来源：http://hz.meibo888.top/gtolmapost.html

TS:   // worker_threads 线程池
来源：http://hz.hnqzz.top/gtpaykklta.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xingfuxueyuan.xyz/gtybdnpixi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jinqigfzy.top/gtwwkevukc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shanyushiyangtech.top/gtrvezqeco.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ivvv.top/gtownhczkw.html

[O03] 加锁保护共享数据
来源：http://hz.hnqzz.top/gtjiakexbv.html

Py:   with lock: shared += 1
来源：http://hz.fengsongda.top/gtyvrnmhbm.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hysaishi.cn/gtpzgllsbe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hysaishi.cn/gtmfpqwesa.html

TS:   // 同 JS
来源：http://hz.tanke756.top/gttpzjtofz.html

Java: synchronized (this) { shared++; }
来源：http://hz.fzhhl.top/gtpmorpfqw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.snrcjt.cn/gtzdadjmwi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.kuanghao11.cn/gtlbznsfjx.html

C#:   lock (gate) { shared++; }
来源：http://hz.shanyushiyangkeji.top/gtigewcpgc.html

[O04] 定义异步函数并等待
来源：http://hz.jyoumei.cn/gtvmfmpdmx.html

Py:   async def f():⏎    await g()
来源：http://hz.jianghu66.top/gtisrmkpen.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yuxming.cn/gtzatndrwd.html

JS:   async function f() { await g(); }
来源：http://hz.hywenlv.cn/gtkaygtjni.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.dianchejie.cn/gtmbnercow.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cqqwz.cn/gtjpqbytnj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yueranfly.top/gtlwemlrhr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jinghuilouyu.cn/gtekviwpax.html

C#:   async Task F() { await G(); }
来源：http://hz.c1oappe.top/gtbovckeqt.html

[O05] 并发执行并等待全部完成
来源：http://hz.hnxiangtu.top/gtafccemxi.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xuanzx.com/gteamxkwqj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.sufxvd.cn/gtzawslkaq.html

JS:   await Promise.all(tasks)
来源：http://hz.gaohongyu789.top/gtyzkqtqzr.html

TS:   await Promise.all(tasks)
来源：http://hz.yonumen.top/gtvqtbzsvd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hywenlv.cn/gtdupkvpgy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.guowangkeji.top/gtuoidxujf.html

Ruby: threads.map(&:join)
来源：http://hz.dashuyun.cn/gtizobjztn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ywan-chungtsiang.top/gtnyuueewr.html

[O06] 使用进程池
来源：http://hz.wangdashe.top/gtwvzbsygm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xylfe.cn/gtdioapedl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhixingplan.top/gtmfzjcgni.html

JS:   // child_process / cluster 模块
来源：http://hz.tianlin.xyz/gtevcygtsn.html

TS:   // child_process / cluster 模块
来源：http://hz.tanke756.top/gtrxirrqvb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.shanyushiyangtech.top/gtygyhabuu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhiwuduotai.top/gttjqjzgmo.html

Ruby: // fork 块
来源：http://hz.shzxlz.cn/gtambswdpt.html

C#:   Parallel.For
来源：http://hz.jinghuilouyu.cn/gtqxmomypi.html

================================================================================
来源：http://hz.zycfv.cn/gtfifngcct.html

P. 常用工具函数
来源：http://hz.pycfn.com/gtcdxgbowa.html

================================================================================
来源：http://hz.c1oappe.top/gtbdhdoyqu.html

[P01] 生成 UUID
来源：http://hz.vqdsnc.cn/gtwxfrzdgz.html

Py:   str(uuid.uuid4())
来源：http://hz.jinyuanbaomall.cn/gtiqukweqp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sufxvd.cn/gtrssxvajs.html

JS:   crypto.randomUUID()
来源：http://hz.zhaomingkeji.xyz/gtjeaoxndi.html

TS:   crypto.randomUUID()
来源：http://hz.smart0.xyz/gtzetilvdr.html

Java: UUID.randomUUID().toString()
来源：http://hz.yj202588.top/gtyzgmgzdc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ywan-chungtsiang.top/gtyotwlgih.html

Ruby: SecureRandom.uuid
来源：http://hz.mhx1999.top/gtcwljxofd.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shuidangran.top/gtwyprtixe.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ydjk.org.cn/gtnvooyscl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.daxiang520.top/gtkdwhluww.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.feifeiyinyue.top/gtmtrdncsq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jlsjyb.cn/gtlsjlsepa.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.tian-w.cn/gtwajdrlzn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yangfankeji.com/gtwyhsicmm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.pengpengdd.cyou/gtujwyhkkh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ppjwa.cn/gtcwflgdnw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhixingplan.top/gtoifcuzwv.html

[P03] 生成短随机字符串
来源：http://hz.jinghuilouyu.cn/gtjfwyibme.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.tanke756.top/gtehpxlzzk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhijiandao.cn/gthvgaadne.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zycfv.cn/gtgjxgpdhj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuanzhike.top/gttudqtlbs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gogol.net.cn/gtofoosibm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nwbrower.top/gtywvnkzhw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.wangdashe.top/gtjqlcgkwh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cheryme.top/gtplabzayw.html

[P04] 求长度
来源：http://hz.guowangkeji.top/gtdnglnjey.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.nanxinkj.top/gtkegfcmdo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hammf.cn/gtkvkllmfw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nanxinkj.top/gtopaaoidn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydzc1.top/gtnxnfpjku.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ywan-chungtsiang.top/gtsivrlznu.html

Go:   len(arr);  len(m)
来源：http://hz.hysaishi.cn/gtotporust.html

Ruby: x.length;  x.size
来源：http://hz.cqqwz.cn/gthstcshfl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.guannengcc.top/gtanqbfkbn.html

[P05] 判断两个对象内容是否相等
来源：http://hz.dashuyun.cn/gtllxfeadn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cashguo.top/gtybsapjbt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.mhx1999.top/gtivzvkvdz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xylfe.cn/gtqybturda.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.wangdashe.top/gtitlzvykn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.daria6918.cn/gtnmzgdrve.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.dashuyun.cn/gtepxqqmse.html

Ruby: a == b
来源：http://hz.cashguo.top/gtjhwkjhuj.html


<!-- 参考信息 -->