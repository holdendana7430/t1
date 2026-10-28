代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sweek.top/gtoswtjvrs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.fengsongda.top/gtifvtztrt.html

Ruby: JSON.parse(resp.body)
来源：http://hz.redwolf501.top/gtdzbuzdlf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.chenzaomai.com/gttpoprwjl.html

[L07] 处理 HTTP 状态码
来源：http://hz.cashguo.top/gtlmackaoq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhaomingkeji.xyz/gtnzbmione.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hysaishi.cn/gtgqzjzjgh.html

JS:   resp.ok;  resp.status
来源：http://hz.ydzc1.top/gtktahmyam.html

TS:   resp.ok;  resp.status
来源：http://hz.xylfe.cn/gtbvizevam.html

Java: resp.statusCode()
来源：http://hz.haohaochexian.top/gtzpbuortg.html

Go:   resp.StatusCode
来源：http://hz.dianchejie.cn/gttpnzgsha.html

Ruby: resp.code.to_i
来源：http://hz.zhaomingkeji.xyz/gtdxpgttvx.html

C#:   (int)resp.StatusCode
来源：http://hz.dianchejie.cn/gtolcwxohd.html

[L08] 并发请求多个地址
来源：http://hz.yuxming.cn/gtsigjsivo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shangyingyoupin.top/gtiryuliuf.html

PHP:  curl_multi_init() 系列
来源：http://hz.dianchejie.cn/gthrnmvwuo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhengqikj.top/gtrikzlbjw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenzaomai.com/gtvbkaienb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gotoacloud.top/gtuywhlird.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.sweek.top/gtxmgocjil.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hongshengwenyu.top/gtsxtzzdle.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gzhubu.top/gtyidtqoql.html

================================================================================
来源：http://hz.hywenlv.cn/gtwjlqbkvb.html

M. 命令行 / 进程 / 环境
来源：http://hz.aizwys.cn/gteveoqmnn.html

================================================================================
来源：http://hz.cucudq.cn/gtlmdzsnze.html

[M01] 读取命令行参数
来源：http://hz.jinghuilouyu.cn/gthirwxqao.html

Py:   sys.argv[1:]
来源：http://hz.zycfv.cn/gtbvleqfyf.html

PHP:  $argv;  $argc;
来源：http://hz.gaohongyu789.top/gtebswehvw.html

JS:   process.argv.slice(2)
来源：http://hz.sxryk.cn/gtidlomcne.html

TS:   process.argv.slice(2)
来源：http://hz.dianchejie.cn/gteguewtmu.html

Java: args 数组（main 方法参数）
来源：http://hz.ydjk.org.cn/gtsmmuquoe.html

Go:   os.Args[1:]
来源：http://hz.9152youxi.cn/gtbhnwaiqp.html

Ruby: ARGV
来源：http://hz.zhijiandao.cn/gtcujmssiq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hysaishi.cn/gtblxinphn.html

[M02] 读取环境变量
来源：http://hz.yueranfly.top/gtrofzrymz.html

Py:   os.environ.get("HOME")
来源：http://hz.redwolf501.top/gthtdxqxih.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sysykeji.top/gtrnglkfoo.html

JS:   process.env.HOME
来源：http://hz.zhiwuduotai.top/gtvulmepnb.html

TS:   process.env.HOME
来源：http://hz.ehwqpu.com/gtgigyaizk.html

Java: System.getenv("HOME")
来源：http://hz.daxiang520.top/gtywogcljs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinqigfzy.top/gtyloiveyo.html

Ruby: ENV["HOME"]
来源：http://hz.hammf.cn/gtddaejpiu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.snrcjt.cn/gtvicgjnzk.html

[M03] 执行外部命令
来源：http://hz.hywenlv.cn/gtlaupwhtd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shzxlz.cn/gtvdcwdype.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.c1oappe.top/gteiryirup.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.quarkkingdee.top/gtydlwewef.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.52xcode.cn/gtlmlqvdan.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.iojbl.cn/gtwwukoodz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hammf.cn/gtxauqhasn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jyoumei.cn/gtgzyvdlhb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ivvv.top/gtqbrsjhqc.html

[M04] 获取当前工作目录
来源：http://hz.yuxming.cn/gtscxxmmdb.html

Py:   os.getcwd()
来源：http://hz.52xcode.cn/gtokdpumac.html

PHP:  getcwd();
来源：http://hz.jinghuilouyu.cn/gtkhnwnvgf.html

JS:   process.cwd()
来源：http://hz.vqdsnc.cn/gtzzixcilr.html

TS:   process.cwd()
来源：http://hz.zycfv.cn/gtpwhkxfiw.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yj20258888.top/gtatcdlfon.html

Go:   os.Getwd()
来源：http://hz.hnxiangtu.top/gtymcegwqh.html

Ruby: Dir.pwd
来源：http://hz.daxiang520.top/gtlglkcvrz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.iojbl.cn/gtfnjdekou.html

[M05] 设置退出码
来源：http://hz.birdmap.top/gtvybbpoct.html

Py:   sys.exit(1)
来源：http://hz.zhijiandao.cn/gtzfztpeki.html

PHP:  exit(1);
来源：http://hz.vqdsnc.cn/gtegdvstvy.html

JS:   process.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtfpamhkkf.html

TS:   process.exit(1)
来源：http://hz.ivvv.top/gtxgstmgox.html

Java: System.exit(1)
来源：http://hz.zhengqikj.top/gtbxjyimmj.html

Go:   os.Exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtmpkyjymo.html

Ruby: exit 1
来源：http://hz.cucudq.cn/gtqdjfdyji.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.meibo888.top/gtpjgevfco.html

[M06] 向标准错误输出
来源：http://hz.jlsjyb.cn/gtnkyeujjg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yanxiufei.cn/gttcqfiocg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.haohaochexian.top/gtujahnqcv.html

JS:   console.error("err")
来源：http://hz.redwolf501.top/gtvkoqnkyq.html

TS:   console.error("err")
来源：http://hz.pycfn.com/gtkslgdsmx.html

Java: System.err.println("err")
来源：http://hz.svipenyu.cn/gtsyzerckp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shanyushiyangtech.top/gtsqwddtbj.html

Ruby: warn "err"
来源：http://hz.snrcjt.cn/gtggwqtmvy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ydjk.org.cn/gtrnzjprdt.html

[M07] 判断是否为主入口
来源：http://hz.snrcjt.cn/gtipbkcxgg.html

Py:   if __name__ == "__main__":
来源：http://hz.cdnleiting.top/gtbmyszmzv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.chenzaomai.com/gtplqwrwye.html

JS:   require.main === module
来源：http://hz.aizwys.cn/gtfzqyeoui.html

TS:   require.main === module
来源：http://hz.ybcxt.top/gtqkdubcvr.html

Java: public static void main(String[] args)
来源：http://hz.gogol.net.cn/gtvjcrfmgx.html

Go:   func main()
来源：http://hz.52xcode.cn/gtxulnjowo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.nanxuanxn.top/gtqznetsmp.html

C#:   static void Main(string[] args)
来源：http://hz.gaohongyu789.top/gtevrjxbwi.html

[M08] 获取系统与运行时信息
来源：http://hz.quarkkingdee.top/gtzyffpddc.html

Py:   platform.system();  platform.python_version()
来源：http://hz.andypj.xyz/gtxkxpxyac.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhiwuduotai.top/gtmqzqouvk.html

JS:   process.platform;  process.version
来源：http://hz.kuanghao11.cn/gtfxdzkxta.html

TS:   process.platform;  process.version
来源：http://hz.yj20258.top/gtleuqftkm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cashguo.top/gthpbjfnok.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.wangdashe.top/gtiisoutmg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.pengpengdd.cyou/gtowhnigcg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnqzz.top/gtosebouhj.html

================================================================================
来源：http://hz.yangfankeji.com/gtspzgbvhx.html

N. 数据结构与算法
来源：http://hz.jqgfzy.top/gtwqxdqkqs.html

================================================================================
来源：http://hz.yanxiufei.cn/gtedoqmolh.html

[N01] 二分查找（有序数组）
来源：http://hz.shuidangran.top/gteccdkaqd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.chenlongwang.top/gtgllkjkgq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.nanxinkj.top/gtwvgcmigy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigfzy.top/gthrpftjrw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aibaodan.cn/gtttkhbvxj.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtoyekklot.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shangyingyoupin.top/gtfjvkfsvr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.cucudq.cn/gtenwrxddh.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.chenzaomai.com/gtbwjaogtv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jinqigufen.top/gtuxwzbqwg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gogol.net.cn/gtmasjhxfd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.c1oappe.top/gtgkqiunod.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yanxiufei.cn/gtvdryyjes.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.redwolf501.top/gtreofxnot.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.svipenyu.cn/gtwdojvpej.html

Go:   slices.Sort(arr)
来源：http://hz.pycfn.com/gtkcfuzspm.html

Ruby: arr.sort
来源：http://hz.ywan-chungtsiang.top/gtpywnjfsp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.nanxinkj.top/gtlkgcqjbx.html

[N03] 快速排序（分治示例）
来源：http://hz.yvedp.cn/gtgfhdvpjz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.dashuyun.cn/gthcnuxtya.html

PHP:  // 递归实现，或用 usort
来源：http://hz.snrcjt.cn/gtrjgeiegd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.feifeiyinyue.top/gtoxehhqqm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cdnleiting.top/gtpboyksod.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj20258888.top/gtfrlfegcs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.chenjidiqi.icu/gtxmfgtghi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhaomingkeji.xyz/gtxsvumkht.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xziqi.cn/gtfzrgewgw.html

[N04] 斐波那契数列
来源：http://hz.jinghuilouyu.cn/gtjhkpnabz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.nwbrower.top/gtchghdikp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhijiandao.cn/gtbbvumxpi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sufxvd.cn/gtbfasrjsg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.316326.xyz/gtkzvmnzsf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.tianlin.xyz/gtkhmitpdi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yonumen.top/gtqapkrtgw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.mhx1999.top/gtbyundohu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.kuanghao11.cn/gtaniguxdo.html

[N05] 最大公约数
来源：http://hz.jinghuilouyu.cn/gtlbkejriy.html

Py:   math.gcd(a, b)
来源：http://hz.cqqwz.cn/gtljhjgfyr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.svipenyu.cn/gtmrycfqlk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnqzz.top/gtaahgxglb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangdashe.top/gtonmovihm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hnxiangtu.top/gtitdnqbvs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.kuanghao11.cn/gtbywljnfe.html

Ruby: a.gcd(b)
来源：http://hz.nanxinkj.top/gtiolanxnc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cqqwz.cn/gtkfkqshvs.html

[N06] 判断回文字符串
来源：http://hz.yvedp.cn/gtzyhajmrm.html

Py:   s == s[::-1]
来源：http://hz.shangyingyoupin.top/gtbugbdlih.html

PHP:  $s === strrev($s);
来源：http://hz.chenjidiqi.icu/gtvpfnvyke.html

JS:   s === [...s].reverse().join("")
来源：http://hz.wangdashe.top/gtbzaqzjxv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.mhx1999.top/gtbihbybea.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jyoumei.cn/gtpiwdanwm.html

Go:   // 双指针从两端比较
来源：http://hz.haohaochexian.top/gtgydeoaus.html

Ruby: s == s.reverse
来源：http://hz.chenjidiqi.icu/gtghpznuzt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.havefunace.top/gtohvkvnbv.html

[N07] 两数之和（返回下标）
来源：http://hz.sysykeji.top/gtzwovqlmd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.pycfn.com/gtihregbmr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cucudq.cn/gtnmfridim.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zycfv.cn/gtbquqyvbw.html

TS:   // 手写 Map<string, number>
来源：http://hz.ivvv.top/gtuqaocptf.html

Java: // 手写 HashMap
来源：http://hz.jinqigfzy.top/gtqhdbafvc.html

Go:   // 手写 map[int]int
来源：http://hz.cqqwz.cn/gtrncrvmnu.html

Ruby: // 手写 Hash
来源：http://hz.ywan-chungtsiang.top/gtupeiijse.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yanxiufei.cn/gtybutoueo.html

[N08] 生成全排列
来源：http://hz.hammf.cn/gtvvvpdopx.html

Py:   itertools.permutations(arr)
来源：http://hz.jinqigufen.top/gtbkddtbzu.html

PHP:  // 手写递归交换
来源：http://hz.52xcode.cn/gtrkkqelhf.html

JS:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gthgoicumd.html

TS:   // 手写回溯递归
来源：http://hz.birdmap.top/gteozkhetr.html

Java: // 手写回溯递归
来源：http://hz.yj202588.top/gtfncfnnju.html

Go:   // 手写回溯递归
来源：http://hz.jqgufenzy.top/gtavicxrzw.html

Ruby: arr.permutation.to_a
来源：http://hz.xuetiantiany.cn/gtdnscdnsr.html

C#:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtrlcdvkun.html

[N09] 栈与队列
来源：http://hz.jqgufenzy.top/gtswohujud.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jiagoushi.top/gtdqczsulu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinyuanbaomall.cn/gtquywtwsa.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinghuilouyu.cn/gtjlcikdfa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zycfv.cn/gtyithksyx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jianghu66.top/gtvfxkyzlz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.vqdsnc.cn/gtjlabkbhx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.fzhhl.top/gtugaunmqr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinghuilouyu.cn/gtdebhwvtj.html

[N10] 链表节点定义
来源：http://hz.daxiang520.top/gtmlictjpk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.smart0.xyz/gtovyndwor.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ydjk.org.cn/gtelujetoi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.tian-w.cn/gtpahbmesq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenzaomai.com/gtyycawoeu.html

Java: class Node { int v; Node next; }
来源：http://hz.ydzc1.top/gtmaaardee.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.feifeiyinyue.top/gtrghfuhuc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhiwuduotai.top/gtinkwabfp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yueranfly.top/gtsopexslf.html

[N11] 二叉树中序遍历
来源：http://hz.tian-w.cn/gtraisfqcv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xuanzx.com/gtianrdyiu.html

PHP:  // 手写递归函数
来源：http://hz.jinqigufen.top/gtrrsjiahs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.svipenyu.cn/gtsqeyjjgd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.redwolf501.top/gtdikepcss.html

Java: // 手写递归
来源：http://hz.ydzc1.top/gtjvjazbzq.html

Go:   // 手写递归
来源：http://hz.hongshengwenyu.top/gtvrwyyzvd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhongyouzk.top/gtfdidzwle.html

C#:   // 手写递归
来源：http://hz.guowangkeji.top/gtascfdttk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.smart0.xyz/gtolfhqmpj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.nanxuanxn.top/gtycyqdvjm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.mhx1999.top/gthfkcdcmq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ehwqpu.com/gtsgtlbkdx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jyoumei.cn/gthvadkzys.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenlongwang.top/gtkqxjtkyy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.aizwys.cn/gtqawgjapr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhijiandao.cn/gtzglcmldx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigfzy.top/gttixrtcit.html

================================================================================
来源：http://hz.yuanzhike.top/gtddlnfezt.html

O. 并发与异步
来源：http://hz.jiagoushi.top/gtjsikdaeq.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtqonpgvsk.html

[O01] 启动一个线程
来源：http://hz.snrcjt.cn/gtnzoykqmy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.tanke756.top/gtzsdbnikt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shanyushiyangkeji.top/gtmuubvtxf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenjidiqi.icu/gtnzvqccpu.html

TS:   // 同 JS
来源：http://hz.andypj.xyz/gtomxrdwru.html

Java: new Thread(() -> f()).start()
来源：http://hz.quarkkingdee.top/gtboqyvowu.html

Go:   go f()
来源：http://hz.cdnleiting.top/gtamagooxd.html

Ruby: Thread.new { f }
来源：http://hz.ywan-chungtsiang.top/gtitixibcz.html

C#:   Task.Run(() => F());
来源：http://hz.jyoumei.cn/gtkkblulxa.html

[O02] 使用线程池
来源：http://hz.0kj1m.cn/gtkjcumixg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.meibo888.top/gtttplgcqm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.andypj.xyz/gtqpyzalxl.html

JS:   // worker_threads 线程池
来源：http://hz.jinyuanbaomall.cn/gtpvvchkiq.html

TS:   // worker_threads 线程池
来源：http://hz.zhongyouzk.top/gtiinxqbgm.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.pengpengdd.cyou/gtbgizsouz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gzhubu.top/gtvjjcvcbx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.sxryk.cn/gtkdvgitwj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ydjk.org.cn/gtbgbdyxiu.html

[O03] 加锁保护共享数据
来源：http://hz.haohaochexian.top/gtvttzllbm.html

Py:   with lock: shared += 1
来源：http://hz.shanyushiyangtech.top/gtgopnrwvt.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.pengpengdd.cyou/gtdkxmmgvh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinqigfzy.top/gtknayqaow.html

TS:   // 同 JS
来源：http://hz.shangyingyoupin.top/gtrizoufvx.html

Java: synchronized (this) { shared++; }
来源：http://hz.daxiang520.top/gthffgqnmt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.guannengcc.top/gtsoewoeic.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jiagoushi.top/gtlnkukzzr.html

C#:   lock (gate) { shared++; }
来源：http://hz.ybcxt.top/gtgqdcosxb.html

[O04] 定义异步函数并等待
来源：http://hz.nwbrower.top/gtondjumpp.html

Py:   async def f():⏎    await g()
来源：http://hz.yj20258.top/gtkfuwxcqy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cheryme.top/gtovlrmgri.html

JS:   async function f() { await g(); }
来源：http://hz.shuidangran.top/gtfmqlvjfn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.pengpengdd.cyou/gtiusktrff.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sxryk.cn/gtlpbiaflw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cashguo.top/gtbmwxeftt.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xylfe.cn/gtybrepdzs.html

C#:   async Task F() { await G(); }
来源：http://hz.zhengqikj.top/gtjafqmzxp.html

[O05] 并发执行并等待全部完成
来源：http://hz.meibo888.top/gtkbyghfrv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.tian-w.cn/gtfefmfnlr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.aibaodan.cn/gteavmvvym.html

JS:   await Promise.all(tasks)
来源：http://hz.gogol.net.cn/gthbwktnmu.html

TS:   await Promise.all(tasks)
来源：http://hz.havefunace.top/gtjulggiqt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhaomingkeji.xyz/gtxwzjvlle.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yj20258.top/gtbrxukgox.html

Ruby: threads.map(&:join)
来源：http://hz.sweek.top/gtyrboxgws.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.meibo888.top/gtlkqxonxk.html

[O06] 使用进程池
来源：http://hz.yj20258888.top/gthujqdsgb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shzxlz.cn/gtvghospzw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ybcxt.top/gtzcejbebj.html

JS:   // child_process / cluster 模块
来源：http://hz.zdqjudy.top/gtdppewxqs.html

TS:   // child_process / cluster 模块
来源：http://hz.gzhubu.top/gtrdsgsgkn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jqgufenzy.top/gtpffczunr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jinqigufen.top/gtnucqnsjd.html

Ruby: // fork 块
来源：http://hz.shuidangran.top/gteleskkfq.html

C#:   Parallel.For
来源：http://hz.fengsongda.top/gtcqokqzdj.html

================================================================================
来源：http://hz.xylfe.cn/gtvwvbckrx.html

P. 常用工具函数
来源：http://hz.gotoacloud.top/gtwiiwmzom.html

================================================================================
来源：http://hz.shuidangran.top/gttvgxmcvu.html

[P01] 生成 UUID
来源：http://hz.jinyuanbaomall.cn/gtdspdlich.html

Py:   str(uuid.uuid4())
来源：http://hz.sxryk.cn/gtzhkmrxso.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shanyushiyangtech.top/gtgqzyignl.html

JS:   crypto.randomUUID()
来源：http://hz.cheryme.top/gtwefzcdey.html

TS:   crypto.randomUUID()
来源：http://hz.aibaodan.cn/gtdcwmxlgm.html

Java: UUID.randomUUID().toString()
来源：http://hz.havefunace.top/gtinsbvejc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yvedp.cn/gtleecvvkm.html

Ruby: SecureRandom.uuid
来源：http://hz.guowangkeji.top/gtqttqnxxn.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cdnleiting.top/gtdvikqugx.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xinyue.icu/gtmrwnhpri.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jinghuilouyu.cn/gtzfsgbpgg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.chenzaomai.com/gtinskkyxk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.tanke756.top/gtylrbxktw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.vqdsnc.cn/gtvyokeplt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shzxlz.cn/gturnzmckw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zycfv.cn/gtoqlzyaoo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.dashuyun.cn/gtwfhhyhwi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yuanzhike.top/gtbigbbiky.html

[P03] 生成短随机字符串
来源：http://hz.c1oappe.top/gtxneqypzi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.fzhhl.top/gtmzkefjco.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hongshengwenyu.top/gtftitfyad.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnqzz.top/gtkmtjdfbl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.feifeiyinyue.top/gtnuoeyemn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xylfe.cn/gtijpbpthx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shzxlz.cn/gtxkisfvpu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.snrcjt.cn/gtyhcgthun.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yongpay.top/gtjxbqhrjz.html

[P04] 求长度
来源：http://hz.cucudq.cn/gtreycflzh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.kuanghao11.cn/gtnmpotwlf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zycfv.cn/gtngrdiema.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daxiang520.top/gtbxzogbas.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhongyouzk.top/gtbpyzgvub.html


<!-- 参考信息 -->