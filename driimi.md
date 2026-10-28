代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://hz.zhoulong.xyz/gtgxcfkhml.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cdnleiting.top/gtcbqaumpp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hfpthk.cn/gtewuuvmso.html

JS:   resp.ok;  resp.status
来源：http://hz.0kj1m.cn/gtlhcuhelf.html

TS:   resp.ok;  resp.status
来源：http://hz.zhengqikj.top/gtcdbaddba.html

Java: resp.statusCode()
来源：http://hz.yonumen.top/gtwfapklbd.html

Go:   resp.StatusCode
来源：http://hz.fzhhl.top/gtodujchtb.html

Ruby: resp.code.to_i
来源：http://hz.zycfv.cn/gtqtxafwjn.html

C#:   (int)resp.StatusCode
来源：http://hz.shzxlz.cn/gtlkwefpxe.html

[L08] 并发请求多个地址
来源：http://hz.guowangkeji.top/gtcfspfaqj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.52xcode.cn/gtjiotzmfu.html

PHP:  curl_multi_init() 系列
来源：http://hz.guannengcc.top/gtaytiwlqd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtlpquhotu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sweek.top/gtchgeltfh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.chenjidiqi.icu/gtaqokhxkq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zycfv.cn/gticxhefal.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.daxiang520.top/gtpdufnfmm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jiagoushi.top/gtzfqvipur.html

================================================================================
来源：http://hz.yonumen.top/gtudzvqcqf.html

M. 命令行 / 进程 / 环境
来源：http://hz.xuanzx.com/gtsvellnqh.html

================================================================================
来源：http://hz.9152youxi.cn/gtztagowyk.html

[M01] 读取命令行参数
来源：http://hz.0kj1m.cn/gtgjndaidd.html

Py:   sys.argv[1:]
来源：http://hz.wangshuangyany.cn/gtvbstkfsu.html

PHP:  $argv;  $argc;
来源：http://hz.cheryme.top/gtzoiilevl.html

JS:   process.argv.slice(2)
来源：http://hz.nanxuanxn.top/gtnshgygtf.html

TS:   process.argv.slice(2)
来源：http://hz.hongshengwenyu.top/gthzlfhwul.html

Java: args 数组（main 方法参数）
来源：http://hz.gogol.net.cn/gtdincraov.html

Go:   os.Args[1:]
来源：http://hz.zycfv.cn/gtyczgdyuc.html

Ruby: ARGV
来源：http://hz.kuanghao11.cn/gtpxonlqnc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hysaishi.cn/gtvzgjqmtk.html

[M02] 读取环境变量
来源：http://hz.bjfxy.top/gtnzixyske.html

Py:   os.environ.get("HOME")
来源：http://hz.nanxuanxn.top/gtkqagrkfx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jqgufenzy.top/gtbqxrhmxk.html

JS:   process.env.HOME
来源：http://hz.sysykeji.top/gtabvbslpt.html

TS:   process.env.HOME
来源：http://hz.hfpthk.cn/gtqjhafmbt.html

Java: System.getenv("HOME")
来源：http://hz.hfpthk.cn/gtekwzwejv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhoulong.xyz/gtwbdnxsap.html

Ruby: ENV["HOME"]
来源：http://hz.zhiwuduotai.top/gtrayquwhx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hfpthk.cn/gtviwdxhtf.html

[M03] 执行外部命令
来源：http://hz.hnqzz.top/gtrkrydebx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.fengsongda.top/gtddzbvvyn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.redwolf501.top/gtbltbhdzf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuanzx.com/gtwothpclz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhongyouzk.top/gtfxpijilk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.c1oappe.top/gtfpueokam.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ywan-chungtsiang.top/gtuabufdjz.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.chenzaomai.com/gttfndhqgv.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xuanzx.com/gtmldsvwwx.html

[M04] 获取当前工作目录
来源：http://hz.gzhubu.top/gtlkourgus.html

Py:   os.getcwd()
来源：http://hz.sufxvd.cn/gtvojwatru.html

PHP:  getcwd();
来源：http://hz.ehwqpu.com/gtdzsipvgg.html

JS:   process.cwd()
来源：http://hz.xinyue.icu/gtbunrmesc.html

TS:   process.cwd()
来源：http://hz.chenzaomai.com/gtqeualwwy.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yj20258.top/gtheniafks.html

Go:   os.Getwd()
来源：http://hz.zhaomingkeji.xyz/gtmbhvynmq.html

Ruby: Dir.pwd
来源：http://hz.ybcxt.top/gtlhyqrebw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.tian-w.cn/gtcfwukzbk.html

[M05] 设置退出码
来源：http://hz.kuanghao11.cn/gtvgtdkqqd.html

Py:   sys.exit(1)
来源：http://hz.yonumen.top/gtoaqfjzvr.html

PHP:  exit(1);
来源：http://hz.jqgfzy.top/gttptwsxec.html

JS:   process.exit(1)
来源：http://hz.cqqwz.cn/gtliqlvpyt.html

TS:   process.exit(1)
来源：http://hz.hywenlv.cn/gtvbkxufiu.html

Java: System.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtpuvuphmu.html

Go:   os.Exit(1)
来源：http://hz.tian-w.cn/gtlwwgpvch.html

Ruby: exit 1
来源：http://hz.gaohongyu789.top/gtwegkxgre.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.chenzaomai.com/gtwgxnffue.html

[M06] 向标准错误输出
来源：http://hz.fengsongda.top/gtnqpkkeng.html

Py:   print("err", file=sys.stderr)
来源：http://hz.c1oappe.top/gtpcaviemf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.fengsongda.top/gtlbrskuym.html

JS:   console.error("err")
来源：http://hz.gzhubu.top/gtzqrhtzqh.html

TS:   console.error("err")
来源：http://hz.jinqigfzy.top/gtnxzgbhxb.html

Java: System.err.println("err")
来源：http://hz.yangfankeji.com/gtzbvzizhf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sweek.top/gtbzqstavp.html

Ruby: warn "err"
来源：http://hz.ivvv.top/gtqjrrbvou.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.9152youxi.cn/gtqboveefw.html

[M07] 判断是否为主入口
来源：http://hz.zhaomingkeji.xyz/gtlgardhso.html

Py:   if __name__ == "__main__":
来源：http://hz.316326.xyz/gtanykfden.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.daxiang520.top/gtikedpjbs.html

JS:   require.main === module
来源：http://hz.daria6918.cn/gtjabhltra.html

TS:   require.main === module
来源：http://hz.zhiwuduotai.top/gtnxwrlnyl.html

Java: public static void main(String[] args)
来源：http://hz.jinghuilouyu.cn/gtcbvycsyy.html

Go:   func main()
来源：http://hz.hongshengwenyu.top/gtelxfcktr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.chenjidiqi.icu/gtwiwmxjjs.html

C#:   static void Main(string[] args)
来源：http://hz.jinghuilouyu.cn/gtpqgghwzu.html

[M08] 获取系统与运行时信息
来源：http://hz.shzxlz.cn/gtapveomoe.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jiagoushi.top/gtoybkbkxi.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.svipenyu.cn/gtosaorfhy.html

JS:   process.platform;  process.version
来源：http://hz.chenlongwang.top/gtowcrdtju.html

TS:   process.platform;  process.version
来源：http://hz.yj202588.top/gtjrdppplv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gaohongyu789.top/gtauknmdgf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cdnleiting.top/gtjqwezsws.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gzhubu.top/gtmaowcagr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cashguo.top/gtyqkfmuuz.html

================================================================================
来源：http://hz.sysykeji.top/gttgworvrp.html

N. 数据结构与算法
来源：http://hz.havefunace.top/gtsuxxpsac.html

================================================================================
来源：http://hz.tian-w.cn/gtznefrtkr.html

[N01] 二分查找（有序数组）
来源：http://hz.daxiang520.top/gtaxbhnftg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hnqzz.top/gtmuhwzfxq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jyoumei.cn/gtxgnrzdls.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ybcxt.top/gtyveqeohz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.quarkkingdee.top/gtvtvmhybf.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenlongwang.top/gthnhzuixo.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shzxlz.cn/gtdylxwnze.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yj20258888.top/gtnqhgszkk.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hnqzz.top/gtazokbyks.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cqqwz.cn/gtlpaquoid.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenjidiqi.icu/gthhtwfjaw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinyuanbaomall.cn/gtojkkdxts.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinqigufen.top/gtblrrhvhs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nwbrower.top/gtsgqejrgb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shzxlz.cn/gtpyliyice.html

Go:   slices.Sort(arr)
来源：http://hz.jinqigufen.top/gtbbfroogs.html

Ruby: arr.sort
来源：http://hz.ybcxt.top/gttrzpyhyi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xuanzx.com/gtsbeotpxj.html

[N03] 快速排序（分治示例）
来源：http://hz.zhixingplan.top/gtubapznrc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.fengsongda.top/gtwupyllmd.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cheryme.top/gtsyrrxuxi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhoulong.xyz/gteomvujpa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenjidiqi.icu/gtnsclnzpg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shzxlz.cn/gtvrxroqos.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.vqdsnc.cn/gtxqjavttl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhixingplan.top/gtyuqauhhc.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ydzc1.top/gtbhgucptz.html

[N04] 斐波那契数列
来源：http://hz.hammf.cn/gttzkuxvpu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.wangshuangyany.cn/gtkloolyes.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zdqjudy.top/gtqdttdbkt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cheryme.top/gtowlvrhws.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.0kj1m.cn/gtygjfoplx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xziqi.cn/gtleyxoekx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.9152youxi.cn/gtpankmhwh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cqqwz.cn/gtpgxuthep.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.daria6918.cn/gtyvgkkgwz.html

[N05] 最大公约数
来源：http://hz.c1oappe.top/gtvyhzpdml.html

Py:   math.gcd(a, b)
来源：http://hz.gaohongyu789.top/gtohjvyeyf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yuanzhike.top/gtcwgiivqp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cqqwz.cn/gtohrfnbqd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sysykeji.top/gtvgnvtoao.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shuidangran.top/gtolkmgpqh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenzaomai.com/gtdyyyxrfc.html

Ruby: a.gcd(b)
来源：http://hz.chenjidiqi.icu/gtwisqdcuk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.nanxinkj.top/gtgwyffghn.html

[N06] 判断回文字符串
来源：http://hz.hfpthk.cn/gtqpzspwef.html

Py:   s == s[::-1]
来源：http://hz.jinqigufen.top/gtbptfkubv.html

PHP:  $s === strrev($s);
来源：http://hz.jinqigfzy.top/gtftyiwvbq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yvedp.cn/gtqvvcwzqz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtthinozzy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ppjwa.cn/gtdhqnzfkt.html

Go:   // 双指针从两端比较
来源：http://hz.ehwqpu.com/gtzufmvtkx.html

Ruby: s == s.reverse
来源：http://hz.fengsongda.top/gtwdzeyija.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yj20258.top/gtyvngvegi.html

[N07] 两数之和（返回下标）
来源：http://hz.xylfe.cn/gtdbifpobc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.316326.xyz/gtrdrtcbau.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.wangdashe.top/gtmhiiapja.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shangyingyoupin.top/gtjvaghamp.html

TS:   // 手写 Map<string, number>
来源：http://hz.ydjk.org.cn/gtszzaoqtp.html

Java: // 手写 HashMap
来源：http://hz.yj202588.top/gtxabhfdec.html

Go:   // 手写 map[int]int
来源：http://hz.pengpengdd.cyou/gtrjmzlsio.html

Ruby: // 手写 Hash
来源：http://hz.jlsjyb.cn/gtmqzywdtx.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xziqi.cn/gtfcimwcov.html

[N08] 生成全排列
来源：http://hz.xuetiantiany.cn/gtuabrxivm.html

Py:   itertools.permutations(arr)
来源：http://hz.nanxuanxn.top/gtmhqmhcdo.html

PHP:  // 手写递归交换
来源：http://hz.guannengcc.top/gtyeiofqcb.html

JS:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtmweypprl.html

TS:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtgvejpknb.html

Java: // 手写回溯递归
来源：http://hz.gzhubu.top/gtdglernqo.html

Go:   // 手写回溯递归
来源：http://hz.zycfv.cn/gtsanvmtoj.html

Ruby: arr.permutation.to_a
来源：http://hz.ivvv.top/gtrhtuaimy.html

C#:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtpgvcnwnh.html

[N09] 栈与队列
来源：http://hz.yuanzhike.top/gtakavvzbi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.quarkkingdee.top/gtwbplmhew.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cdnleiting.top/gtrwarribx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yj202588.top/gtsrxqspyt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.pengpengdd.cyou/gtfmuzsswg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hammf.cn/gtnlbxmush.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.vqdsnc.cn/gtfwlxewku.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cucudq.cn/gtoddlatfu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.pycfn.com/gthjyfzunt.html

[N10] 链表节点定义
来源：http://hz.yueranfly.top/gtdqcvwpaq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.guowangkeji.top/gttqmooivd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gzhubu.top/gtwhcysflh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.chenjidiqi.icu/gtaflgjkew.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gaohongyu789.top/gtgptckefo.html

Java: class Node { int v; Node next; }
来源：http://hz.kuanghao11.cn/gtidrgqkkp.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zdqjudy.top/gtawfrbcax.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.snrcjt.cn/gtrzbmlkku.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.andypj.xyz/gtkdbmlhky.html

[N11] 二叉树中序遍历
来源：http://hz.yangfankeji.com/gtetcweyma.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhiwuduotai.top/gtjagqtdku.html

PHP:  // 手写递归函数
来源：http://hz.chenjidiqi.icu/gtofmdwtzr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gzhubu.top/gtetdnolzu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yanxiufei.cn/gtundkbety.html

Java: // 手写递归
来源：http://hz.xuetiantiany.cn/gtkqhjdaij.html

Go:   // 手写递归
来源：http://hz.gzhubu.top/gtptdaayxb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hongshengwenyu.top/gtkxsaxisz.html

C#:   // 手写递归
来源：http://hz.quarkkingdee.top/gtuduqldqr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gzhubu.top/gtqluwgswq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cashguo.top/gtmxpbdwro.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yonumen.top/gtktehzmpx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.316326.xyz/gtqsqodvze.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hywenlv.cn/gtssmfcxjc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.redwolf501.top/gtyleujbsi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.daxiang520.top/gtnqpncoio.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.9152youxi.cn/gtzpyjnaoj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.c1oappe.top/gtrjssmpco.html

================================================================================
来源：http://hz.jyoumei.cn/gtimlalyxr.html

O. 并发与异步
来源：http://hz.redwolf501.top/gtozwpkmzx.html

================================================================================
来源：http://hz.kuanghao11.cn/gtwntocsyn.html

[O01] 启动一个线程
来源：http://hz.sweek.top/gthuxwyjvm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhijiandao.cn/gtclmjojvr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yongpay.top/gtjuohgvsv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhixingplan.top/gtcobgjfwn.html

TS:   // 同 JS
来源：http://hz.xuetiantiany.cn/gtoiaqrqog.html

Java: new Thread(() -> f()).start()
来源：http://hz.wangdashe.top/gtfkuypmrj.html

Go:   go f()
来源：http://hz.mhx1999.top/gtgjlyanlr.html

Ruby: Thread.new { f }
来源：http://hz.snrcjt.cn/gtesttkplh.html

C#:   Task.Run(() => F());
来源：http://hz.daria6918.cn/gtwabqwdmi.html

[O02] 使用线程池
来源：http://hz.smart0.xyz/gtwymnqqjg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.andypj.xyz/gtcettqaad.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.fengsongda.top/gtxbttzqwe.html

JS:   // worker_threads 线程池
来源：http://hz.tianlin.xyz/gtanwfqbvk.html

TS:   // worker_threads 线程池
来源：http://hz.aibaodan.cn/gtuuvwaqtb.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yanxiufei.cn/gthuorciga.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.meibo888.top/gtixnzxbrw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yj20258888.top/gtnkmlxoov.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinqigufen.top/gtfuszeogc.html

[O03] 加锁保护共享数据
来源：http://hz.jlsjyb.cn/gtrahfwkbv.html

Py:   with lock: shared += 1
来源：http://hz.yueranfly.top/gthymcdosi.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ehwqpu.com/gtihqgtoyh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yj202588.top/gtgjohivwb.html

TS:   // 同 JS
来源：http://hz.xuetiantiany.cn/gtnifouwso.html

Java: synchronized (this) { shared++; }
来源：http://hz.ybcxt.top/gtbbduitte.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.haohaochexian.top/gtywrnxxcm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shanyushiyangkeji.top/gtmjhuqgyl.html

C#:   lock (gate) { shared++; }
来源：http://hz.gaohongyu789.top/gtpiaradcc.html

[O04] 定义异步函数并等待
来源：http://hz.ybcxt.top/gtwmgszify.html

Py:   async def f():⏎    await g()
来源：http://hz.haohaochexian.top/gtggowdiyo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gzhubu.top/gtgiwrwram.html

JS:   async function f() { await g(); }
来源：http://hz.gotoacloud.top/gttpnqxxkz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yonumen.top/gtwqmrjgvj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sufxvd.cn/gtqvvkutvd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xinyue.icu/gtkappuwgx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ydjk.org.cn/gtzirwejki.html

C#:   async Task F() { await G(); }
来源：http://hz.cdnleiting.top/gtagbqzpzj.html

[O05] 并发执行并等待全部完成
来源：http://hz.dashuyun.cn/gtomxwcvdt.html

Py:   asyncio.gather(*tasks)
来源：http://hz.nanxinkj.top/gtpnllopmc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.tianlin.xyz/gtnckvkyib.html

JS:   await Promise.all(tasks)
来源：http://hz.jinqigfzy.top/gtryootark.html

TS:   await Promise.all(tasks)
来源：http://hz.ppjwa.cn/gtvbzgrazv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinqigufen.top/gtihtefzzc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cqqwz.cn/gtthtysogu.html

Ruby: threads.map(&:join)
来源：http://hz.zhixingplan.top/gthmmrzmsd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.gotoacloud.top/gtgyhuvnbi.html

[O06] 使用进程池
来源：http://hz.yongpay.top/gtnsbkqszo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.dianchejie.cn/gtxwunckzr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hysaishi.cn/gtaapubirb.html

JS:   // child_process / cluster 模块
来源：http://hz.zdqjudy.top/gtgcwviutn.html

TS:   // child_process / cluster 模块
来源：http://hz.redwolf501.top/gtzviyiiwa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinyuanbaomall.cn/gtnkwnhvma.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gaohongyu789.top/gthgchihhb.html

Ruby: // fork 块
来源：http://hz.meibo888.top/gtnzjwcocn.html

C#:   Parallel.For
来源：http://hz.9152youxi.cn/gtlyefhygk.html

================================================================================
来源：http://hz.iojbl.cn/gtxshlylcl.html

P. 常用工具函数
来源：http://hz.jqgfzy.top/gtnbhkyjmq.html

================================================================================
来源：http://hz.aibaodan.cn/gtbxwzguqb.html

[P01] 生成 UUID
来源：http://hz.fzhhl.top/gtxgxlfwdb.html

Py:   str(uuid.uuid4())
来源：http://hz.0kj1m.cn/gtkxglsltx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yueranfly.top/gtbywxjvwv.html

JS:   crypto.randomUUID()
来源：http://hz.ywan-chungtsiang.top/gtaerpfpqe.html

TS:   crypto.randomUUID()
来源：http://hz.cheryme.top/gtdwlqpoke.html

Java: UUID.randomUUID().toString()
来源：http://hz.316326.xyz/gtpixvfgcs.html

Go:   // 用 github.com/google/uuid
来源：http://hz.aizwys.cn/gtlkwkynzi.html

Ruby: SecureRandom.uuid
来源：http://hz.vqdsnc.cn/gtvgdmmbax.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ppjwa.cn/gtsuxzqkqw.html

[P02] MD5 / SHA256 摘要
来源：http://hz.0kj1m.cn/gtzeqvgvli.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.redwolf501.top/gtqdqahkdi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.pengpengdd.cyou/gtltafmfzg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.snrcjt.cn/gtrgtqjcxt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hongshengwenyu.top/gtsdoartlq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.sxryk.cn/gtevggizoh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.snrcjt.cn/gtztkcevsg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenlongwang.top/gtsdkzwnnr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ppjwa.cn/gteaclbfvk.html

[P03] 生成短随机字符串
来源：http://hz.tanke756.top/gtnpyrumak.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shangyingyoupin.top/gtesxoxgrz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yangfankeji.com/gttiigtpyx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hywenlv.cn/gtnaphgzfk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jyoumei.cn/gtfvrotutz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhongyouzk.top/gtfcjstent.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shangyingyoupin.top/gtdwwmlxfy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.0kj1m.cn/gthtkptvka.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.dianchejie.cn/gtgetwwsia.html

[P04] 求长度
来源：http://hz.hnxiangtu.top/gtblahuzzh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shanyushiyangtech.top/gtdkunjlbn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.snrcjt.cn/gtuixrejro.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yanxiufei.cn/gtcvgedruv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.havefunace.top/gtpqqzwiei.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ehwqpu.com/gtrrntlnrl.html

Go:   len(arr);  len(m)
来源：http://hz.haohaochexian.top/gtmyghvhmy.html

Ruby: x.length;  x.size
来源：http://hz.xinyue.icu/gtkovagows.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hongshengwenyu.top/gtvsuflvcw.html


<!-- 参考信息 -->