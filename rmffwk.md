代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://hz.redwolf501.top/gthmjrwuza.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shangyingyoupin.top/gtzmezrtki.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhixingplan.top/gtzeyuqcdl.html

JS:   resp.ok;  resp.status
来源：http://hz.yongpay.top/gtffcvhrgq.html

TS:   resp.ok;  resp.status
来源：http://hz.svipenyu.cn/gtwuhguodz.html

Java: resp.statusCode()
来源：http://hz.cqqwz.cn/gthpwjhgcf.html

Go:   resp.StatusCode
来源：http://hz.jinghuilouyu.cn/gtyeyfppbi.html

Ruby: resp.code.to_i
来源：http://hz.jqgfzy.top/gtjkpyjuko.html

C#:   (int)resp.StatusCode
来源：http://hz.jlsjyb.cn/gtnodqocnr.html

[L08] 并发请求多个地址
来源：http://hz.jqgufenzy.top/gtlrxeiyxv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ppjwa.cn/gtqsrbzlet.html

PHP:  curl_multi_init() 系列
来源：http://hz.hnxiangtu.top/gtvszifcgx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhongyouzk.top/gtxzqwyrvs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtoykbtdmk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shzxlz.cn/gtpwzyiexe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.sysykeji.top/gtgtzpiomj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.dashuyun.cn/gtryixipvr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xuanzx.com/gtlsmbgzri.html

================================================================================
来源：http://hz.zycfv.cn/gtpjbmcvem.html

M. 命令行 / 进程 / 环境
来源：http://hz.ydjk.org.cn/gtlbwypvdk.html

================================================================================
来源：http://hz.haohaochexian.top/gtxbmiegot.html

[M01] 读取命令行参数
来源：http://hz.jinghuilouyu.cn/gtvpvsmrka.html

Py:   sys.argv[1:]
来源：http://hz.316326.xyz/gtcxsuvipy.html

PHP:  $argv;  $argc;
来源：http://hz.zhengqikj.top/gtcuevelnu.html

JS:   process.argv.slice(2)
来源：http://hz.gogol.net.cn/gtsjmdhydp.html

TS:   process.argv.slice(2)
来源：http://hz.xinyue.icu/gtsqknqzeu.html

Java: args 数组（main 方法参数）
来源：http://hz.redwolf501.top/gtnshblpzs.html

Go:   os.Args[1:]
来源：http://hz.316326.xyz/gtgvflutkq.html

Ruby: ARGV
来源：http://hz.tian-w.cn/gtbagabkik.html

C#:   args 数组（Main 方法参数）
来源：http://hz.daria6918.cn/gtgdohnrsb.html

[M02] 读取环境变量
来源：http://hz.birdmap.top/gtylecuolg.html

Py:   os.environ.get("HOME")
来源：http://hz.chenlongwang.top/gtmfwrhjpu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.svipenyu.cn/gtpvagevmh.html

JS:   process.env.HOME
来源：http://hz.zhengqikj.top/gtkzmjgprd.html

TS:   process.env.HOME
来源：http://hz.cdnleiting.top/gtwaouvnpd.html

Java: System.getenv("HOME")
来源：http://hz.xinyue.icu/gtzdsqhxir.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yanxiufei.cn/gtpczuihju.html

Ruby: ENV["HOME"]
来源：http://hz.chenlongwang.top/gtuetfmivh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhengqikj.top/gtuaqrwity.html

[M03] 执行外部命令
来源：http://hz.smart0.xyz/gtxtweeqgk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhijiandao.cn/gtjmgwgaeb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.fzhhl.top/gtqbxntant.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.havefunace.top/gtkzxigxze.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.meibo888.top/gtjilrgedq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hnxiangtu.top/gtrleahnoh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.gotoacloud.top/gtoobbholo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.tanke756.top/gtoampsyvb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.tanke756.top/gtrxkiynsc.html

[M04] 获取当前工作目录
来源：http://hz.yuxming.cn/gtciybtxra.html

Py:   os.getcwd()
来源：http://hz.hysaishi.cn/gtqooqkjvt.html

PHP:  getcwd();
来源：http://hz.shangyingyoupin.top/gtlbtmthfl.html

JS:   process.cwd()
来源：http://hz.aizwys.cn/gtnigjstfv.html

TS:   process.cwd()
来源：http://hz.jyoumei.cn/gtdnrgaedg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yanxiufei.cn/gtekbjzpyv.html

Go:   os.Getwd()
来源：http://hz.gotoacloud.top/gtkyngaqmt.html

Ruby: Dir.pwd
来源：http://hz.tanke756.top/gtkihmbmox.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shanyushiyangtech.top/gtjjocbjld.html

[M05] 设置退出码
来源：http://hz.chenzaomai.com/gtxrrednum.html

Py:   sys.exit(1)
来源：http://hz.chenlongwang.top/gtimplixxp.html

PHP:  exit(1);
来源：http://hz.bjfxy.top/gtkjveispa.html

JS:   process.exit(1)
来源：http://hz.gaohongyu789.top/gtxccwafze.html

TS:   process.exit(1)
来源：http://hz.smart0.xyz/gtccszirxj.html

Java: System.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtdyailnsf.html

Go:   os.Exit(1)
来源：http://hz.yueranfly.top/gtgwivihgy.html

Ruby: exit 1
来源：http://hz.cqqwz.cn/gtnythrnpm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.haohaochexian.top/gtdqluhngu.html

[M06] 向标准错误输出
来源：http://hz.xuetiantiany.cn/gtisqhlmzw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yuxming.cn/gtvluiamsx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.c1oappe.top/gtbnlrbuil.html

JS:   console.error("err")
来源：http://hz.zhaomingkeji.xyz/gtxnfunnnm.html

TS:   console.error("err")
来源：http://hz.dashuyun.cn/gtrsheqvgc.html

Java: System.err.println("err")
来源：http://hz.shanyushiyangkeji.top/gtcdneippk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jianghu66.top/gtcbktozem.html

Ruby: warn "err"
来源：http://hz.shangyingyoupin.top/gtfvdwlayf.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yuxming.cn/gtgtwrzahi.html

[M07] 判断是否为主入口
来源：http://hz.jinghuilouyu.cn/gttvunfcuf.html

Py:   if __name__ == "__main__":
来源：http://hz.chenzaomai.com/gtovbdhlvq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xingfuxueyuan.xyz/gtjckrfmil.html

JS:   require.main === module
来源：http://hz.andypj.xyz/gtnqqbgdby.html

TS:   require.main === module
来源：http://hz.ywan-chungtsiang.top/gtsjknhukv.html

Java: public static void main(String[] args)
来源：http://hz.nwbrower.top/gtbuokdqzu.html

Go:   func main()
来源：http://hz.jqgfzy.top/gtolirrwou.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yj20258888.top/gtwabojoma.html

C#:   static void Main(string[] args)
来源：http://hz.wangshuangyany.cn/gthpuigkwg.html

[M08] 获取系统与运行时信息
来源：http://hz.yuxming.cn/gtxvykkuia.html

Py:   platform.system();  platform.python_version()
来源：http://hz.daxiang520.top/gtoyroenzf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cucudq.cn/gtvvddsdad.html

JS:   process.platform;  process.version
来源：http://hz.zhijiandao.cn/gtaicrawbu.html

TS:   process.platform;  process.version
来源：http://hz.zdqjudy.top/gtfrsacell.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cdnleiting.top/gtenxkkbae.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.wangshuangyany.cn/gtpkrefsar.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.birdmap.top/gtibfpnuyl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cheryme.top/gtgiylgfsu.html

================================================================================
来源：http://hz.yj20258888.top/gtwmkbngou.html

N. 数据结构与算法
来源：http://hz.cucudq.cn/gtnftpyles.html

================================================================================
来源：http://hz.zdqjudy.top/gtbtiszzjx.html

[N01] 二分查找（有序数组）
来源：http://hz.zycfv.cn/gtnagklcnl.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.pengpengdd.cyou/gtluilkbmg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhaomingkeji.xyz/gtnszvndhj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinghuilouyu.cn/gtyzrivzri.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tianlin.xyz/gtpsjgljgv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jiagoushi.top/gtfqdribeg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zdqjudy.top/gtttmisrka.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jqgufenzy.top/gtgldsdfbg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.kuanghao11.cn/gthpjtgiex.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.fzhhl.top/gtekhljtet.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.aizwys.cn/gtoemtrmub.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.smart0.xyz/gtohelzpuv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jqgufenzy.top/gtdmcjcgjv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangkeji.top/gtjcdxhtne.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.c1oappe.top/gtpnbdaoub.html

Go:   slices.Sort(arr)
来源：http://hz.sufxvd.cn/gtpwztafbl.html

Ruby: arr.sort
来源：http://hz.jianghu66.top/gtcevhymds.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhongyouzk.top/gtcjfvodzq.html

[N03] 快速排序（分治示例）
来源：http://hz.yj20258.top/gtkasgudqj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.havefunace.top/gttmhkzpac.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhiwuduotai.top/gtqxqxpjeu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinghuilouyu.cn/gtjbmhwgzj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gaohongyu789.top/gtxhxlbmpu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shuidangran.top/gtjgcqbpza.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.316326.xyz/gtuvhdpyll.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yuxming.cn/gtwzluqibd.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yanxiufei.cn/gtxripplbq.html

[N04] 斐波那契数列
来源：http://hz.zdqjudy.top/gtzingoryl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.bjfxy.top/gtfkujgxgt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.havefunace.top/gtlnohwsxb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hammf.cn/gtzlzdhhmy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.bjfxy.top/gtdoupfohm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.tanke756.top/gtscezcgdw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yueranfly.top/gtmhukjsvz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shuidangran.top/gtkuukpyyf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jianghu66.top/gtpacwdynv.html

[N05] 最大公约数
来源：http://hz.vqdsnc.cn/gtuynzokyu.html

Py:   math.gcd(a, b)
来源：http://hz.chenzaomai.com/gtauumzlme.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.52xcode.cn/gtrvkhejwy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.9152youxi.cn/gtmjmxhenf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pengpengdd.cyou/gtgpapwzsh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.guannengcc.top/gtffjxxtci.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhongyouzk.top/gtkbsvgyfz.html

Ruby: a.gcd(b)
来源：http://hz.aibaodan.cn/gtfjqnaoey.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.pengpengdd.cyou/gtccctjema.html

[N06] 判断回文字符串
来源：http://hz.c1oappe.top/gtbhvpsats.html

Py:   s == s[::-1]
来源：http://hz.ywan-chungtsiang.top/gtbreolktt.html

PHP:  $s === strrev($s);
来源：http://hz.chenlongwang.top/gtlpnhdpgr.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhixingplan.top/gtccddxetz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtrkrrnejw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yj20258888.top/gtbybjtpjo.html

Go:   // 双指针从两端比较
来源：http://hz.cucudq.cn/gtptsexlcw.html

Ruby: s == s.reverse
来源：http://hz.ydzc1.top/gtesnrhotm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.vqdsnc.cn/gthzeibcfp.html

[N07] 两数之和（返回下标）
来源：http://hz.cdnleiting.top/gtipeuoban.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yj20258888.top/gtdjkmixuo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ydzc1.top/gtlfdwylxd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.fzhhl.top/gtyjdzlbzl.html

TS:   // 手写 Map<string, number>
来源：http://hz.andypj.xyz/gtwzpxbwnu.html

Java: // 手写 HashMap
来源：http://hz.quarkkingdee.top/gtpjhlklfp.html

Go:   // 手写 map[int]int
来源：http://hz.ydzc1.top/gtdqkxtngd.html

Ruby: // 手写 Hash
来源：http://hz.jinyuanbaomall.cn/gtvmmlhakb.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ivvv.top/gtlnmarmju.html

[N08] 生成全排列
来源：http://hz.kuanghao11.cn/gtfezzsavv.html

Py:   itertools.permutations(arr)
来源：http://hz.chenzaomai.com/gtpultnxkp.html

PHP:  // 手写递归交换
来源：http://hz.yuanzhike.top/gtypgyzlmz.html

JS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtnnvcskiz.html

TS:   // 手写回溯递归
来源：http://hz.daxiang520.top/gtsldgfgxs.html

Java: // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtaszuocbv.html

Go:   // 手写回溯递归
来源：http://hz.pycfn.com/gtqmcydwgp.html

Ruby: arr.permutation.to_a
来源：http://hz.9152youxi.cn/gtdveevtil.html

C#:   // 手写回溯递归
来源：http://hz.cdnleiting.top/gtnlwnfgeq.html

[N09] 栈与队列
来源：http://hz.feifeiyinyue.top/gtxaesnxlk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jqgfzy.top/gtxjujzaun.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hnqzz.top/gtnogpbmpk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.nanxinkj.top/gtlesnqujo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.havefunace.top/gtrexxdrur.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hnxiangtu.top/gtpsynnnfa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cqqwz.cn/gtaggtfpio.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yj20258.top/gtasykactx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yuxming.cn/gttabhknkt.html

[N10] 链表节点定义
来源：http://hz.xinyue.icu/gtzrkntern.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jqgfzy.top/gtjdbloqcq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.birdmap.top/gteslalmws.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.havefunace.top/gteydcfsit.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.havefunace.top/gtxrzyixfb.html

Java: class Node { int v; Node next; }
来源：http://hz.gogol.net.cn/gtgqvaujgl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.dashuyun.cn/gtklcltbqp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.feifeiyinyue.top/gtoxbryzrc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shuidangran.top/gtbfchqywf.html

[N11] 二叉树中序遍历
来源：http://hz.nanxinkj.top/gtlxuojuej.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shangyingyoupin.top/gtcstfiolw.html

PHP:  // 手写递归函数
来源：http://hz.52xcode.cn/gtefeoitif.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yanxiufei.cn/gtogxnytdm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jyoumei.cn/gtbetssldj.html

Java: // 手写递归
来源：http://hz.andypj.xyz/gtjmgisoup.html

Go:   // 手写递归
来源：http://hz.shuidangran.top/gtmrlxvhul.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jqgfzy.top/gtvqnaqslf.html

C#:   // 手写递归
来源：http://hz.nanxuanxn.top/gtcxbcxsao.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cucudq.cn/gthjivqjck.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhijiandao.cn/gtxmidhuxf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shanyushiyangkeji.top/gtnqmftwwa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dashuyun.cn/gtonoenjnq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhaomingkeji.xyz/gtgihppnax.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jianghu66.top/gtsnbqjrjk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.pengpengdd.cyou/gtfojihfgw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shzxlz.cn/gtcyemwzke.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.haohaochexian.top/gtqvnjmhcz.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtzouxujyk.html

O. 并发与异步
来源：http://hz.aizwys.cn/gtbyivhopk.html

================================================================================
来源：http://hz.pengpengdd.cyou/gthkqwilcf.html

[O01] 启动一个线程
来源：http://hz.ybcxt.top/gtlfmkayio.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.snrcjt.cn/gtambrerik.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ydjk.org.cn/gtaarcckth.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fzhhl.top/gtxkfaogcl.html

TS:   // 同 JS
来源：http://hz.ivvv.top/gtysxpgmad.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhongyouzk.top/gttyijiitx.html

Go:   go f()
来源：http://hz.gzhubu.top/gtzrulmcfu.html

Ruby: Thread.new { f }
来源：http://hz.nanxuanxn.top/gtirznccfh.html

C#:   Task.Run(() => F());
来源：http://hz.hnqzz.top/gthuimpiru.html

[O02] 使用线程池
来源：http://hz.sxryk.cn/gtmxoprbbh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xuetiantiany.cn/gtpcsapdcr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shanyushiyangtech.top/gtlesbghsv.html

JS:   // worker_threads 线程池
来源：http://hz.shuidangran.top/gtfpdyouuu.html

TS:   // worker_threads 线程池
来源：http://hz.gogol.net.cn/gtspjksrwq.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhaomingkeji.xyz/gtakygqqpg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xinyue.icu/gtwpoaqrvj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ydzc1.top/gtjejhhknd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.andypj.xyz/gtgizngmpm.html

[O03] 加锁保护共享数据
来源：http://hz.jqgfzy.top/gtdxpskaak.html

Py:   with lock: shared += 1
来源：http://hz.cdnleiting.top/gtbtxehkeg.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhiwuduotai.top/gtiqrmdrpq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.quarkkingdee.top/gtodmbsttq.html

TS:   // 同 JS
来源：http://hz.fzhhl.top/gtgdhxgfqm.html

Java: synchronized (this) { shared++; }
来源：http://hz.daria6918.cn/gtyvsbzowq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.aibaodan.cn/gtqulhhxzx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.dianchejie.cn/gtinjvksjo.html

C#:   lock (gate) { shared++; }
来源：http://hz.chenzaomai.com/gtcvrozngx.html

[O04] 定义异步函数并等待
来源：http://hz.bjfxy.top/gtnmguvypy.html

Py:   async def f():⏎    await g()
来源：http://hz.jlsjyb.cn/gtfwwkjwrz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gogol.net.cn/gthdlehhrt.html

JS:   async function f() { await g(); }
来源：http://hz.shanyushiyangtech.top/gtegxzcuec.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jinqigufen.top/gtdfmnnyou.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.guannengcc.top/gtaxbclerd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ybcxt.top/gtsigpreos.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gaohongyu789.top/gteufkrkes.html

C#:   async Task F() { await G(); }
来源：http://hz.c1oappe.top/gtbrdaabpq.html

[O05] 并发执行并等待全部完成
来源：http://hz.jianghu66.top/gtoghorqcg.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hongshengwenyu.top/gtmomwszur.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.c1oappe.top/gtgihyxbeo.html

JS:   await Promise.all(tasks)
来源：http://hz.yanxiufei.cn/gtbziegyph.html

TS:   await Promise.all(tasks)
来源：http://hz.xylfe.cn/gtssarnwla.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.smart0.xyz/gtwcsnxxap.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.bjfxy.top/gtnfmlmqrx.html

Ruby: threads.map(&:join)
来源：http://hz.shanyushiyangkeji.top/gthhgymezh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yj20258888.top/gtbiqqmkmd.html

[O06] 使用进程池
来源：http://hz.cucudq.cn/gtxfumwaiq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yvedp.cn/gtyukcdxvq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.quarkkingdee.top/gtdfxzzrpe.html

JS:   // child_process / cluster 模块
来源：http://hz.ydzc1.top/gtiiuogybp.html

TS:   // child_process / cluster 模块
来源：http://hz.gaohongyu789.top/gtaokwnxah.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.guannengcc.top/gtcricgbjx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yj202588.top/gtkhtzfzjh.html

Ruby: // fork 块
来源：http://hz.ybcxt.top/gtgxkepako.html

C#:   Parallel.For
来源：http://hz.316326.xyz/gtuzaazhkb.html

================================================================================
来源：http://hz.daria6918.cn/gttakrbdhk.html

P. 常用工具函数
来源：http://hz.daria6918.cn/gttxpekclu.html

================================================================================
来源：http://hz.ivvv.top/gtxmotgtul.html

[P01] 生成 UUID
来源：http://hz.ybcxt.top/gtqmbdeckt.html

Py:   str(uuid.uuid4())
来源：http://hz.hnqzz.top/gtfvxvftmd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hnxiangtu.top/gtxxailjcq.html

JS:   crypto.randomUUID()
来源：http://hz.gaohongyu789.top/gtjytcdxla.html

TS:   crypto.randomUUID()
来源：http://hz.aizwys.cn/gtmqukjsyb.html

Java: UUID.randomUUID().toString()
来源：http://hz.xinyue.icu/gtlvqhfiqy.html

Go:   // 用 github.com/google/uuid
来源：http://hz.nwbrower.top/gtupqivkel.html

Ruby: SecureRandom.uuid
来源：http://hz.aibaodan.cn/gttussdorr.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhengqikj.top/gtithxenrl.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cqqwz.cn/gtywrnrqhh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhijiandao.cn/gtkqzdfuek.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.chenlongwang.top/gtktdosetd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zdqjudy.top/gtcqjwrbzy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gogol.net.cn/gtpiesjmfx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jinghuilouyu.cn/gtabzflunv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jlsjyb.cn/gtyjgrhtko.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.nwbrower.top/gtqiaxxued.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.sufxvd.cn/gtaxkxrprt.html

[P03] 生成短随机字符串
来源：http://hz.gotoacloud.top/gtfbcxawbu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yangfankeji.com/gtyzpxrzxp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.guowangkeji.top/gtdwykdfvw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.316326.xyz/gtfoggemhg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gotoacloud.top/gtoashbslb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.sysykeji.top/gtgtoetzlq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.fengsongda.top/gtrpmhdlpq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gaohongyu789.top/gtvsfxycwk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gzhubu.top/gtwfdpiwlf.html

[P04] 求长度
来源：http://hz.zhiwuduotai.top/gtkpuioldz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yangfankeji.com/gtgscsrwyk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tanke756.top/gtrsxqlqes.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cdnleiting.top/gtxgolarar.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ywan-chungtsiang.top/gtsomeeanw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hysaishi.cn/gtbbapwwll.html

Go:   len(arr);  len(m)
来源：http://hz.quarkkingdee.top/gtjkvrptww.html

Ruby: x.length;  x.size
来源：http://hz.zycfv.cn/gttucnjtzv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.fengsongda.top/gtamcfbrxz.html


<!-- 参考信息 -->