代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xingfuxueyuan.xyz/gtirwbqcdg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cashguo.top/gtbsmffvdy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yangfankeji.com/gtlswhylhi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.nanxuanxn.top/gtsfcexrvu.html

[L07] 处理 HTTP 状态码
来源：http://hz.vqdsnc.cn/gtudmxfdsm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jinqigfzy.top/gtijdepsqn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hammf.cn/gtlmykniny.html

JS:   resp.ok;  resp.status
来源：http://hz.jqgufenzy.top/gtdqddhavc.html

TS:   resp.ok;  resp.status
来源：http://hz.xziqi.cn/gtwvhitfkh.html

Java: resp.statusCode()
来源：http://hz.jinyuanbaomall.cn/gttvucfvux.html

Go:   resp.StatusCode
来源：http://hz.9152youxi.cn/gtwarengez.html

Ruby: resp.code.to_i
来源：http://hz.jinghuilouyu.cn/gtnmevaadm.html

C#:   (int)resp.StatusCode
来源：http://hz.sweek.top/gttwqeetde.html

[L08] 并发请求多个地址
来源：http://hz.yanxiufei.cn/gtvxgfwuha.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.0kj1m.cn/gtsrcyrzog.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhongyouzk.top/gtnwrzbswm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxuanxn.top/gtnrisiyiy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pycfn.com/gtenoqxpik.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.0kj1m.cn/gtfcmfzkfh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xinyue.icu/gtoreuajsv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.daxiang520.top/gtrrpyfkss.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gogol.net.cn/gtaxyuaeil.html

================================================================================
来源：http://hz.9152youxi.cn/gtsjbptdyi.html

M. 命令行 / 进程 / 环境
来源：http://hz.snrcjt.cn/gtfgukzzfd.html

================================================================================
来源：http://hz.shangyingyoupin.top/gttbukhhfi.html

[M01] 读取命令行参数
来源：http://hz.pycfn.com/gtvwpyjeze.html

Py:   sys.argv[1:]
来源：http://hz.tianlin.xyz/gtozuwnwmb.html

PHP:  $argv;  $argc;
来源：http://hz.jqgfzy.top/gtangyqfpe.html

JS:   process.argv.slice(2)
来源：http://hz.xziqi.cn/gttqfpoudc.html

TS:   process.argv.slice(2)
来源：http://hz.vqdsnc.cn/gtsdaddxwe.html

Java: args 数组（main 方法参数）
来源：http://hz.iojbl.cn/gtwmttmjkv.html

Go:   os.Args[1:]
来源：http://hz.sufxvd.cn/gtmkvdrqnd.html

Ruby: ARGV
来源：http://hz.316326.xyz/gtgdeetgkt.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhiwuduotai.top/gtoygezqzg.html

[M02] 读取环境变量
来源：http://hz.ydzc1.top/gtvstkzpgd.html

Py:   os.environ.get("HOME")
来源：http://hz.hongshengwenyu.top/gtvracubmi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xingfuxueyuan.xyz/gtxnmpncpx.html

JS:   process.env.HOME
来源：http://hz.chenlongwang.top/gtatzvjfgd.html

TS:   process.env.HOME
来源：http://hz.cashguo.top/gtzmgtbobg.html

Java: System.getenv("HOME")
来源：http://hz.tanke756.top/gtrexxubfa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.birdmap.top/gtsixbgmnj.html

Ruby: ENV["HOME"]
来源：http://hz.0kj1m.cn/gtatklprca.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shangyingyoupin.top/gtmijtjmzb.html

[M03] 执行外部命令
来源：http://hz.aizwys.cn/gtuidxcxoq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gzhubu.top/gtyvjgsmby.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.guannengcc.top/gtxaggfyei.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.iojbl.cn/gtalmrwkwo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ehwqpu.com/gteceeejaf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhiwuduotai.top/gtyachqanp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.gogol.net.cn/gtblratovi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ivvv.top/gtxwcbltva.html

C#:   Process.Start("ls", "-l");
来源：http://hz.aibaodan.cn/gtrmwjmsmf.html

[M04] 获取当前工作目录
来源：http://hz.nanxinkj.top/gtgdisxirh.html

Py:   os.getcwd()
来源：http://hz.xziqi.cn/gtnzgsuxdf.html

PHP:  getcwd();
来源：http://hz.zhiwuduotai.top/gtnmuwttbk.html

JS:   process.cwd()
来源：http://hz.yonumen.top/gtukeodspp.html

TS:   process.cwd()
来源：http://hz.ivvv.top/gtuzouvhvz.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shangyingyoupin.top/gtbljonujq.html

Go:   os.Getwd()
来源：http://hz.jiagoushi.top/gtllnopgly.html

Ruby: Dir.pwd
来源：http://hz.jinqigfzy.top/gtulmaujuf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.dianchejie.cn/gtwqmnssrx.html

[M05] 设置退出码
来源：http://hz.ybcxt.top/gtrqrqnevc.html

Py:   sys.exit(1)
来源：http://hz.zhengqikj.top/gtkdnyduzs.html

PHP:  exit(1);
来源：http://hz.vqdsnc.cn/gtqceevabw.html

JS:   process.exit(1)
来源：http://hz.shzxlz.cn/gtxzcwwhsa.html

TS:   process.exit(1)
来源：http://hz.meibo888.top/gttavskopv.html

Java: System.exit(1)
来源：http://hz.zhijiandao.cn/gtjiblxrkf.html

Go:   os.Exit(1)
来源：http://hz.chenzaomai.com/gttylkqjvi.html

Ruby: exit 1
来源：http://hz.cqqwz.cn/gtcjfflomd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nanxuanxn.top/gtaqkwhrjv.html

[M06] 向标准错误输出
来源：http://hz.52xcode.cn/gtswfpyiae.html

Py:   print("err", file=sys.stderr)
来源：http://hz.316326.xyz/gtqiulovbc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cucudq.cn/gtudyahtjp.html

JS:   console.error("err")
来源：http://hz.ybcxt.top/gtjrnxexuy.html

TS:   console.error("err")
来源：http://hz.jinqigfzy.top/gttqfcgvun.html

Java: System.err.println("err")
来源：http://hz.zhiwuduotai.top/gtsorhdwey.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhiwuduotai.top/gtvltrbdje.html

Ruby: warn "err"
来源：http://hz.wangshuangyany.cn/gtgzglgkkq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhongyouzk.top/gtoicyzpba.html

[M07] 判断是否为主入口
来源：http://hz.gotoacloud.top/gtasdkhqlp.html

Py:   if __name__ == "__main__":
来源：http://hz.xinyue.icu/gtlksdhxfe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xinyue.icu/gtggmfyjtl.html

JS:   require.main === module
来源：http://hz.jqgfzy.top/gtuywoyspu.html

TS:   require.main === module
来源：http://hz.9152youxi.cn/gtuxdquarw.html

Java: public static void main(String[] args)
来源：http://hz.316326.xyz/gtxchqcowl.html

Go:   func main()
来源：http://hz.guannengcc.top/gtucyrgpzc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ivvv.top/gtolbpcgoi.html

C#:   static void Main(string[] args)
来源：http://hz.sweek.top/gtdepkwavv.html

[M08] 获取系统与运行时信息
来源：http://hz.yj202588.top/gtxrhmzkkg.html

Py:   platform.system();  platform.python_version()
来源：http://hz.dianchejie.cn/gtxfrgozuv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.dashuyun.cn/gtkxmkitkf.html

JS:   process.platform;  process.version
来源：http://hz.yongpay.top/gtafrqzraw.html

TS:   process.platform;  process.version
来源：http://hz.zdqjudy.top/gtcrxyuwye.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xingfuxueyuan.xyz/gtbjkkrqaa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yvedp.cn/gtvtsdyqhd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.snrcjt.cn/gtulargrrf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinqigufen.top/gtvxvvcued.html

================================================================================
来源：http://hz.jqgufenzy.top/gtvvjgirqp.html

N. 数据结构与算法
来源：http://hz.pengpengdd.cyou/gtvqanuozo.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtywuetwkj.html

[N01] 二分查找（有序数组）
来源：http://hz.cdnleiting.top/gtrxpuhcrw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj20258.top/gtrigvkwki.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yangfankeji.com/gtceodogle.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dashuyun.cn/gtgmscljjd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cdnleiting.top/gtxjpcwtvi.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.vqdsnc.cn/gtqaveinhz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cdnleiting.top/gtczlflkxs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yj20258.top/gtopopekvz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sufxvd.cn/gtestfzzma.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.wangshuangyany.cn/gtdzrfqcag.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.havefunace.top/gtyovtqoua.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yuxming.cn/gtaghqrexk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.dianchejie.cn/gtxeewfzmy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sufxvd.cn/gtzglzggek.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.52xcode.cn/gturisbwux.html

Go:   slices.Sort(arr)
来源：http://hz.cdnleiting.top/gtbkterqgs.html

Ruby: arr.sort
来源：http://hz.jiagoushi.top/gtajkutdnu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.fzhhl.top/gtnoziavjc.html

[N03] 快速排序（分治示例）
来源：http://hz.hnxiangtu.top/gtkmfgpbcx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hywenlv.cn/gtlnvwlykz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.fengsongda.top/gtxayhfzhi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dashuyun.cn/gtfvvmtlrm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jianghu66.top/gtowcsqtto.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yueranfly.top/gtcwlxeelc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.haohaochexian.top/gtfftwdnpn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yj20258888.top/gtdydtbibr.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hongshengwenyu.top/gtuilueapw.html

[N04] 斐波那契数列
来源：http://hz.jianghu66.top/gtmalflxme.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.mhx1999.top/gtiiivhbhu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.chenjidiqi.icu/gtvkwdwyon.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cashguo.top/gtumksyaap.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnqzz.top/gtbivdcqyv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gaohongyu789.top/gtmglduxkm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhiwuduotai.top/gtyutwaonh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zycfv.cn/gthibjcvjd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shanyushiyangtech.top/gtcirpjcxa.html

[N05] 最大公约数
来源：http://hz.tian-w.cn/gtqeqxrydk.html

Py:   math.gcd(a, b)
来源：http://hz.zycfv.cn/gtpqdjyalt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xylfe.cn/gtvucydbdq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cashguo.top/gtrzomyanb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dashuyun.cn/gtukjryqft.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shanyushiyangkeji.top/gtcsfwxbai.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.0kj1m.cn/gtbhkovbnj.html

Ruby: a.gcd(b)
来源：http://hz.hnqzz.top/gtyyjoqqhi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cucudq.cn/gtlhwcgcwf.html

[N06] 判断回文字符串
来源：http://hz.dianchejie.cn/gthbvpynga.html

Py:   s == s[::-1]
来源：http://hz.xylfe.cn/gtrseyzksk.html

PHP:  $s === strrev($s);
来源：http://hz.yueranfly.top/gtvmmpvirx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sysykeji.top/gtdznfympy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtunsxlics.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhongyouzk.top/gttunhlqpo.html

Go:   // 双指针从两端比较
来源：http://hz.jyoumei.cn/gtyosjynut.html

Ruby: s == s.reverse
来源：http://hz.dianchejie.cn/gtvfqkckku.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.52xcode.cn/gthzfaegzh.html

[N07] 两数之和（返回下标）
来源：http://hz.jlsjyb.cn/gtbxwgoird.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xylfe.cn/gtickgzxki.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.chenlongwang.top/gtuhohxlun.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zycfv.cn/gtarkxtvjl.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinyuanbaomall.cn/gtcbshpwje.html

Java: // 手写 HashMap
来源：http://hz.tanke756.top/gtwqfjxdcr.html

Go:   // 手写 map[int]int
来源：http://hz.cqqwz.cn/gttcdbeani.html

Ruby: // 手写 Hash
来源：http://hz.yonumen.top/gtixzhkzym.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yj20258888.top/gtlethpcul.html

[N08] 生成全排列
来源：http://hz.52xcode.cn/gtxfjwajae.html

Py:   itertools.permutations(arr)
来源：http://hz.jiagoushi.top/gtxzvlrojn.html

PHP:  // 手写递归交换
来源：http://hz.guowangkeji.top/gtvgznhbzu.html

JS:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtgijoqgug.html

TS:   // 手写回溯递归
来源：http://hz.hysaishi.cn/gtsycxxevg.html

Java: // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtsjwygczt.html

Go:   // 手写回溯递归
来源：http://hz.ehwqpu.com/gtlydjorjg.html

Ruby: arr.permutation.to_a
来源：http://hz.ehwqpu.com/gthvquhskm.html

C#:   // 手写回溯递归
来源：http://hz.nwbrower.top/gtsdkltyyf.html

[N09] 栈与队列
来源：http://hz.xuanzx.com/gtjlzircxw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.chenzaomai.com/gtxrcxowee.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.nanxuanxn.top/gtvrpxidrn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.meibo888.top/gtaoqkvpzx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shanyushiyangkeji.top/gtsdgwhrpp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shzxlz.cn/gtbsnznfgx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yvedp.cn/gtjqmxlpik.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yuxming.cn/gtekmcyxbp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.52xcode.cn/gtgghktzmc.html

[N10] 链表节点定义
来源：http://hz.cheryme.top/gtrlgijmzt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.guowangkeji.top/gtsjmmfpyg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.haohaochexian.top/gtfvjtcjud.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sysykeji.top/gtrpbvzwro.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jqgufenzy.top/gttqhbtdzl.html

Java: class Node { int v; Node next; }
来源：http://hz.sweek.top/gtwxuyxvnj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.bjfxy.top/gtclthlqke.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cdnleiting.top/gtzmumgqrq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hnqzz.top/gtnovvhckj.html

[N11] 二叉树中序遍历
来源：http://hz.dianchejie.cn/gtdumydtia.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.mhx1999.top/gtgbzmtldb.html

PHP:  // 手写递归函数
来源：http://hz.jqgufenzy.top/gtxsvytsvu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ppjwa.cn/gtcccxvswa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj202588.top/gteiezgdju.html

Java: // 手写递归
来源：http://hz.c1oappe.top/gtqygaoypk.html

Go:   // 手写递归
来源：http://hz.cqqwz.cn/gtaijewbug.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.52xcode.cn/gtrfvdlmag.html

C#:   // 手写递归
来源：http://hz.yangfankeji.com/gtfglrjrvu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yuxming.cn/gttptethmk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yangfankeji.com/gtxtlzacfs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cashguo.top/gtjojfmvdb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ehwqpu.com/gtzeniedpf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.kuanghao11.cn/gtghefkvjb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sweek.top/gtxuobmwie.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yj20258888.top/gtmeriylrb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.52xcode.cn/gtgnxgxaes.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgfzy.top/gtiemvmwfi.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtrnhbmdkk.html

O. 并发与异步
来源：http://hz.shanyushiyangtech.top/gtneobxomb.html

================================================================================
来源：http://hz.chenlongwang.top/gtmkgkknbv.html

[O01] 启动一个线程
来源：http://hz.birdmap.top/gtwzoiynnw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.quarkkingdee.top/gtbfzmjrau.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.smart0.xyz/gtdgxfasee.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cqqwz.cn/gtjfxcfppg.html

TS:   // 同 JS
来源：http://hz.shanyushiyangkeji.top/gturxzwife.html

Java: new Thread(() -> f()).start()
来源：http://hz.jqgufenzy.top/gtqqwxwkol.html

Go:   go f()
来源：http://hz.jqgufenzy.top/gtwygogmdq.html

Ruby: Thread.new { f }
来源：http://hz.jlsjyb.cn/gtkabjzpcr.html

C#:   Task.Run(() => F());
来源：http://hz.316326.xyz/gteiopzlja.html

[O02] 使用线程池
来源：http://hz.jqgufenzy.top/gtyjdljqee.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.52xcode.cn/gtizfrsntb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinqigufen.top/gtswbcpnwd.html

JS:   // worker_threads 线程池
来源：http://hz.jinqigufen.top/gtfeqgchsf.html

TS:   // worker_threads 线程池
来源：http://hz.dianchejie.cn/gtossnrjgs.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.vqdsnc.cn/gthyfgyjxl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xuanzx.com/gttveprlbo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.nanxinkj.top/gtcmvxgxff.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xylfe.cn/gtdhusqqld.html

[O03] 加锁保护共享数据
来源：http://hz.fzhhl.top/gtofztsqvb.html

Py:   with lock: shared += 1
来源：http://hz.zhiwuduotai.top/gtxwlmkuda.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.kuanghao11.cn/gtbxoohqqx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xziqi.cn/gtowmvxdga.html

TS:   // 同 JS
来源：http://hz.gzhubu.top/gteqpvltkp.html

Java: synchronized (this) { shared++; }
来源：http://hz.ydjk.org.cn/gtmxndnocz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cucudq.cn/gtlieidpaw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinyuanbaomall.cn/gthiyikilk.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj20258888.top/gtvqptkwet.html

[O04] 定义异步函数并等待
来源：http://hz.zhaomingkeji.xyz/gtyewdeiqh.html

Py:   async def f():⏎    await g()
来源：http://hz.316326.xyz/gtqhyjlaka.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.daria6918.cn/gtjphkbqyh.html

JS:   async function f() { await g(); }
来源：http://hz.redwolf501.top/gtiagbyjdm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zdqjudy.top/gtmlwmxhct.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yanxiufei.cn/gtxsapyger.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cdnleiting.top/gtzaghdwnm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhoulong.xyz/gtxdgeahcm.html

C#:   async Task F() { await G(); }
来源：http://hz.hnqzz.top/gtntfmxaxr.html

[O05] 并发执行并等待全部完成
来源：http://hz.hammf.cn/gtjgznysut.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhongyouzk.top/gthpchqoqf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.daria6918.cn/gtxiofvlat.html

JS:   await Promise.all(tasks)
来源：http://hz.fengsongda.top/gtfuerbbho.html

TS:   await Promise.all(tasks)
来源：http://hz.vqdsnc.cn/gtqfflfxmd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yueranfly.top/gtegdhecvb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yuanzhike.top/gtwkpjdbsu.html

Ruby: threads.map(&:join)
来源：http://hz.iojbl.cn/gtdouiznbk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xinyue.icu/gtkkuqhmud.html

[O06] 使用进程池
来源：http://hz.jlsjyb.cn/gtokkhekkr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhaomingkeji.xyz/gtbllqynge.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.chenjidiqi.icu/gtnblvdxml.html

JS:   // child_process / cluster 模块
来源：http://hz.jlsjyb.cn/gttvdbfmgv.html

TS:   // child_process / cluster 模块
来源：http://hz.yj20258.top/gtsnondeyt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yonumen.top/gtveqktlge.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yongpay.top/gtzzyfghgk.html

Ruby: // fork 块
来源：http://hz.zhijiandao.cn/gtlbwogauu.html

C#:   Parallel.For
来源：http://hz.shanyushiyangkeji.top/gthbswefcb.html

================================================================================
来源：http://hz.smart0.xyz/gtxrbckauv.html

P. 常用工具函数
来源：http://hz.hammf.cn/gtmctvhuld.html

================================================================================
来源：http://hz.yvedp.cn/gtvfngupml.html

[P01] 生成 UUID
来源：http://hz.zhongyouzk.top/gtfpdyddoz.html

Py:   str(uuid.uuid4())
来源：http://hz.fzhhl.top/gtyzivxemb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.birdmap.top/gtgfezcddh.html

JS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtdrivjlhp.html

TS:   crypto.randomUUID()
来源：http://hz.sufxvd.cn/gtplpvtaag.html

Java: UUID.randomUUID().toString()
来源：http://hz.aibaodan.cn/gtlgbatrhu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.birdmap.top/gtufpmvvzi.html

Ruby: SecureRandom.uuid
来源：http://hz.cucudq.cn/gtjngacazy.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.aizwys.cn/gtrwurmcef.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ydjk.org.cn/gtteeisavu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hammf.cn/gtkvdswowq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.nwbrower.top/gtmrzhjbmy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hammf.cn/gtomlbtakq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.wangdashe.top/gthjcrbmig.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.tianlin.xyz/gtyuavxaux.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yangfankeji.com/gtkdysqcfk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yueranfly.top/gtlvbsashn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.tianlin.xyz/gtmktyiebv.html

[P03] 生成短随机字符串
来源：http://hz.tian-w.cn/gtemeiqher.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.snrcjt.cn/gthvzdqrkx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xziqi.cn/gtozspmfzu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xingfuxueyuan.xyz/gtpjqujklj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.haohaochexian.top/gtlepmfwtu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.c1oappe.top/gtmtocaejz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.316326.xyz/gttsbtpunz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.c1oappe.top/gtmamjgcxf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ehwqpu.com/gtqdcjpqni.html

[P04] 求长度
来源：http://hz.jqgfzy.top/gtwzlcgwes.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhaomingkeji.xyz/gtmlxyqoyk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgufenzy.top/gtvwjxcygo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.haohaochexian.top/gtxwotnxzf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.smart0.xyz/gtomdecvuo.html


<!-- 参考信息 -->