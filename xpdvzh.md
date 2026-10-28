代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://hz.xziqi.cn/gtcccabevh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.pengpengdd.cyou/gtpztbykkt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.pycfn.com/gtnqogqjyy.html

JS:   resp.ok;  resp.status
来源：http://hz.daria6918.cn/gtnneniwag.html

TS:   resp.ok;  resp.status
来源：http://hz.hnxiangtu.top/gtubwoplmg.html

Java: resp.statusCode()
来源：http://hz.yuxming.cn/gtgjbbgkls.html

Go:   resp.StatusCode
来源：http://hz.hfpthk.cn/gtbsrvgxpj.html

Ruby: resp.code.to_i
来源：http://hz.sweek.top/gtpmdumqmp.html

C#:   (int)resp.StatusCode
来源：http://hz.c1oappe.top/gtivocwidg.html

[L08] 并发请求多个地址
来源：http://hz.yonumen.top/gtxmnxetwr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.wangdashe.top/gtzbqtgygc.html

PHP:  curl_multi_init() 系列
来源：http://hz.ybcxt.top/gtsqevpoaq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydjk.org.cn/gtjoudrnva.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hongshengwenyu.top/gtirmccipw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ydjk.org.cn/gtbictqdhn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.snrcjt.cn/gtqofjhyrt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cheryme.top/gteerjudjl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cdnleiting.top/gtmmqlbjmw.html

================================================================================
来源：http://hz.wangdashe.top/gtqxygdcch.html

M. 命令行 / 进程 / 环境
来源：http://hz.meibo888.top/gtcpmxvrhk.html

================================================================================
来源：http://hz.xuanzx.com/gtywczwlgx.html

[M01] 读取命令行参数
来源：http://hz.guannengcc.top/gtljdnndoz.html

Py:   sys.argv[1:]
来源：http://hz.xuanzx.com/gtwxjwpfzc.html

PHP:  $argv;  $argc;
来源：http://hz.zhaomingkeji.xyz/gtzxtbuyns.html

JS:   process.argv.slice(2)
来源：http://hz.zhengqikj.top/gtvbawflfu.html

TS:   process.argv.slice(2)
来源：http://hz.havefunace.top/gtybobsech.html

Java: args 数组（main 方法参数）
来源：http://hz.cqqwz.cn/gtobobglxp.html

Go:   os.Args[1:]
来源：http://hz.9152youxi.cn/gtqvnrrwsx.html

Ruby: ARGV
来源：http://hz.316326.xyz/gtpygomkdv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ehwqpu.com/gtixkmmpwy.html

[M02] 读取环境变量
来源：http://hz.wangshuangyany.cn/gtznrwqsbv.html

Py:   os.environ.get("HOME")
来源：http://hz.ybcxt.top/gtgwsomhhw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xylfe.cn/gtdestzmli.html

JS:   process.env.HOME
来源：http://hz.hammf.cn/gtgrqwrjzt.html

TS:   process.env.HOME
来源：http://hz.aibaodan.cn/gtmwqyrksq.html

Java: System.getenv("HOME")
来源：http://hz.shzxlz.cn/gtylptiuwr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cashguo.top/gttbzxyrhe.html

Ruby: ENV["HOME"]
来源：http://hz.hnxiangtu.top/gtskejaxkj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.daxiang520.top/gtyjmwxcxm.html

[M03] 执行外部命令
来源：http://hz.xziqi.cn/gtndlkdevp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gotoacloud.top/gthnvdbjto.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yongpay.top/gtrauvpbgu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.c1oappe.top/gtgmjecipk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jianghu66.top/gtutlqfrds.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.chenlongwang.top/gthmwiwtrk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.gzhubu.top/gtesntjiwd.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yuxming.cn/gtixhzbmho.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yongpay.top/gtoxxaknmg.html

[M04] 获取当前工作目录
来源：http://hz.haohaochexian.top/gtybefdqmb.html

Py:   os.getcwd()
来源：http://hz.wangdashe.top/gtrgffcsmg.html

PHP:  getcwd();
来源：http://hz.ppjwa.cn/gtzttwndpi.html

JS:   process.cwd()
来源：http://hz.fzhhl.top/gthzxgaggb.html

TS:   process.cwd()
来源：http://hz.shanyushiyangtech.top/gtgpnslmnk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.quarkkingdee.top/gtfpvlbela.html

Go:   os.Getwd()
来源：http://hz.daxiang520.top/gtuxzclhjm.html

Ruby: Dir.pwd
来源：http://hz.jinyuanbaomall.cn/gtwiasvdnx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jinqigufen.top/gtdlagxqls.html

[M05] 设置退出码
来源：http://hz.sweek.top/gttvqitrwj.html

Py:   sys.exit(1)
来源：http://hz.sysykeji.top/gtaxceuyzs.html

PHP:  exit(1);
来源：http://hz.gogol.net.cn/gtycqxfrdl.html

JS:   process.exit(1)
来源：http://hz.xylfe.cn/gtugfmmlga.html

TS:   process.exit(1)
来源：http://hz.chenlongwang.top/gtvbujiapm.html

Java: System.exit(1)
来源：http://hz.ydzc1.top/gtemgsatxa.html

Go:   os.Exit(1)
来源：http://hz.cashguo.top/gtfoywwjmi.html

Ruby: exit 1
来源：http://hz.yj20258.top/gtpofuxysi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yongpay.top/gtlchgvdxr.html

[M06] 向标准错误输出
来源：http://hz.ydzc1.top/gtnlztkxkz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.feifeiyinyue.top/gtbzrbsbwp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenjidiqi.icu/gtjmapesox.html

JS:   console.error("err")
来源：http://hz.gogol.net.cn/gtmfgerpqu.html

TS:   console.error("err")
来源：http://hz.redwolf501.top/gtppykvtqu.html

Java: System.err.println("err")
来源：http://hz.jqgfzy.top/gtpzphwjxl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.wangshuangyany.cn/gtitmalvnz.html

Ruby: warn "err"
来源：http://hz.jinqigfzy.top/gteqgjqasu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yongpay.top/gtafdhdqqr.html

[M07] 判断是否为主入口
来源：http://hz.snrcjt.cn/gttasutnyp.html

Py:   if __name__ == "__main__":
来源：http://hz.hysaishi.cn/gtnkdpbehb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.sxryk.cn/gtkwihfbtx.html

JS:   require.main === module
来源：http://hz.mhx1999.top/gtrkqgdaek.html

TS:   require.main === module
来源：http://hz.tian-w.cn/gtkzldhiqi.html

Java: public static void main(String[] args)
来源：http://hz.hnqzz.top/gtcdzwrxmb.html

Go:   func main()
来源：http://hz.zhengqikj.top/gtwxzikpkt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xziqi.cn/gtqkpgasaj.html

C#:   static void Main(string[] args)
来源：http://hz.sweek.top/gtpmtuaqfe.html

[M08] 获取系统与运行时信息
来源：http://hz.haohaochexian.top/gtapfqaovs.html

Py:   platform.system();  platform.python_version()
来源：http://hz.nanxuanxn.top/gtpoiejbea.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ppjwa.cn/gttlybprsv.html

JS:   process.platform;  process.version
来源：http://hz.yuxming.cn/gtdvvymxal.html

TS:   process.platform;  process.version
来源：http://hz.hfpthk.cn/gtgjcdguut.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shzxlz.cn/gtshzgatgj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.kuanghao11.cn/gtmlaeqswo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.tanke756.top/gtivicanba.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shanyushiyangtech.top/gtrqzkhojj.html

================================================================================
来源：http://hz.sysykeji.top/gtsoqdxcgx.html

N. 数据结构与算法
来源：http://hz.zhaomingkeji.xyz/gtuaawumvp.html

================================================================================
来源：http://hz.zdqjudy.top/gtqhuddsdn.html

[N01] 二分查找（有序数组）
来源：http://hz.0kj1m.cn/gtnbcwctih.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yonumen.top/gtcahqjbxv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.quarkkingdee.top/gtamiqdove.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ehwqpu.com/gtkksjpepj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gaohongyu789.top/gtlegoefcf.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hnxiangtu.top/gtowsfeagw.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhengqikj.top/gtxtdnjcql.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.wangshuangyany.cn/gtvjesgkbi.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sufxvd.cn/gtxibbzmys.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.meibo888.top/gtvgtlqivr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj202588.top/gtrpxjbuuz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.dashuyun.cn/gtnnesktxo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.wangshuangyany.cn/gtboskszzz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gtsqrzdrrp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.gzhubu.top/gttvsywayp.html

Go:   slices.Sort(arr)
来源：http://hz.yj20258888.top/gttgphsduc.html

Ruby: arr.sort
来源：http://hz.cqqwz.cn/gtgzhvpaqm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinyuanbaomall.cn/gtrinsmdcg.html

[N03] 快速排序（分治示例）
来源：http://hz.fengsongda.top/gttcxlmpxd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jianghu66.top/gtjhjikthv.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ivvv.top/gtizziwmjb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.mhx1999.top/gtyekuprrq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cucudq.cn/gtqzuwmmoe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ywan-chungtsiang.top/gtzylefkow.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nanxinkj.top/gthhuovvqs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yonumen.top/gtgfmxjzyq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.birdmap.top/gtezmxzqdp.html

[N04] 斐波那契数列
来源：http://hz.ydjk.org.cn/gtrhgqyvak.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xinyue.icu/gtjvvjibog.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.aizwys.cn/gtwkvljuln.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.redwolf501.top/gtgptvylfk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.wangshuangyany.cn/gtjzsghovb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yvedp.cn/gtbxgnxzfs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jqgufenzy.top/gtukvbjsgs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.bjfxy.top/gtexzcxxcc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.9152youxi.cn/gtlsvkjwag.html

[N05] 最大公约数
来源：http://hz.zhixingplan.top/gtmhgngjkf.html

Py:   math.gcd(a, b)
来源：http://hz.tanke756.top/gtuehrqtto.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.cdnleiting.top/gtgnzqqmnm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hongshengwenyu.top/gtuvomoiwr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.mhx1999.top/gtigyekclg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.tianlin.xyz/gthwvufdrw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.vqdsnc.cn/gtsrcggpts.html

Ruby: a.gcd(b)
来源：http://hz.ydzc1.top/gtyhhvlmtp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.mhx1999.top/gtuqwmtiph.html

[N06] 判断回文字符串
来源：http://hz.xuetiantiany.cn/gtjntuxkts.html

Py:   s == s[::-1]
来源：http://hz.vqdsnc.cn/gtrajsigzw.html

PHP:  $s === strrev($s);
来源：http://hz.fzhhl.top/gtsoogfsya.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ybcxt.top/gtrlakxjtc.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gtgytgjxuc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhixingplan.top/gtvircuhxb.html

Go:   // 双指针从两端比较
来源：http://hz.yuxming.cn/gtciaxjgrk.html

Ruby: s == s.reverse
来源：http://hz.svipenyu.cn/gtbsnammqi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.bjfxy.top/gtajpooffj.html

[N07] 两数之和（返回下标）
来源：http://hz.ydjk.org.cn/gtbcctwsjh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cheryme.top/gtkoaiahug.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.birdmap.top/gtlsnjaakr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.9152youxi.cn/gtbrgzxapn.html

TS:   // 手写 Map<string, number>
来源：http://hz.ydzc1.top/gtdvmkovpv.html

Java: // 手写 HashMap
来源：http://hz.kuanghao11.cn/gtzsnkpdvy.html

Go:   // 手写 map[int]int
来源：http://hz.andypj.xyz/gttjqrukuy.html

Ruby: // 手写 Hash
来源：http://hz.dashuyun.cn/gtijxzhkuc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.tanke756.top/gtwlihzjuw.html

[N08] 生成全排列
来源：http://hz.pengpengdd.cyou/gtwenciepl.html

Py:   itertools.permutations(arr)
来源：http://hz.nanxinkj.top/gtdczprfql.html

PHP:  // 手写递归交换
来源：http://hz.hnxiangtu.top/gtkqjlhbjf.html

JS:   // 手写回溯递归
来源：http://hz.ydzc1.top/gtqclhdvqv.html

TS:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtuchcocwb.html

Java: // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtnnyifctj.html

Go:   // 手写回溯递归
来源：http://hz.redwolf501.top/gtitqrgakt.html

Ruby: arr.permutation.to_a
来源：http://hz.cashguo.top/gtxdavygpo.html

C#:   // 手写回溯递归
来源：http://hz.pycfn.com/gtbjlpeqjp.html

[N09] 栈与队列
来源：http://hz.hammf.cn/gtmhyzexam.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.daria6918.cn/gtmzmrzqiu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.andypj.xyz/gtjseytbxo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhiwuduotai.top/gtrtdibkxl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.andypj.xyz/gtgklprhxz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhijiandao.cn/gtymeewpaw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sufxvd.cn/gtuhnfmemh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.tianlin.xyz/gtodkwmgaq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hongshengwenyu.top/gtrwnuyxvd.html

[N10] 链表节点定义
来源：http://hz.yvedp.cn/gtscemeypt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhijiandao.cn/gtqkuifcgc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sysykeji.top/gtgmrgnsoy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cucudq.cn/gtvxfqhyxj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hywenlv.cn/gtcsazjiyf.html

Java: class Node { int v; Node next; }
来源：http://hz.gzhubu.top/gtmeljvjee.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinqigfzy.top/gtmvtevcvd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.andypj.xyz/gttdyogckn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cucudq.cn/gtuawefbzx.html

[N11] 二叉树中序遍历
来源：http://hz.zhiwuduotai.top/gtyrhryasq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinqigufen.top/gtcpenjmbm.html

PHP:  // 手写递归函数
来源：http://hz.zhengqikj.top/gtxewlxeir.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tian-w.cn/gttgczbngb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.mhx1999.top/gtgnzaxeon.html

Java: // 手写递归
来源：http://hz.wangshuangyany.cn/gtnhwtoqgw.html

Go:   // 手写递归
来源：http://hz.tian-w.cn/gtecyufzxm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tian-w.cn/gtrhhivwhs.html

C#:   // 手写递归
来源：http://hz.c1oappe.top/gtwholyzcs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yangfankeji.com/gtgyibyvph.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhaomingkeji.xyz/gtuzvifkye.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.316326.xyz/gtmcnywhgl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cqqwz.cn/gtsneptoik.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zdqjudy.top/gtntrpjebi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yueranfly.top/gtzbhdixzo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.feifeiyinyue.top/gtlsumvfhv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yuanzhike.top/gtyqxdysfy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xylfe.cn/gtmsiunaor.html

================================================================================
来源：http://hz.jianghu66.top/gtltlioevr.html

O. 并发与异步
来源：http://hz.yongpay.top/gtyvrbtjyu.html

================================================================================
来源：http://hz.tanke756.top/gthqfvyuob.html

[O01] 启动一个线程
来源：http://hz.yonumen.top/gtjzocmgqu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.52xcode.cn/gtobgicuxa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.chenlongwang.top/gtwqpixicn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.pengpengdd.cyou/gteitoshdg.html

TS:   // 同 JS
来源：http://hz.zhaomingkeji.xyz/gtswymxolp.html

Java: new Thread(() -> f()).start()
来源：http://hz.chenzaomai.com/gthdikwarn.html

Go:   go f()
来源：http://hz.xylfe.cn/gtcfkpbnes.html

Ruby: Thread.new { f }
来源：http://hz.yanxiufei.cn/gtsngdneqg.html

C#:   Task.Run(() => F());
来源：http://hz.yangfankeji.com/gtuyllwlzr.html

[O02] 使用线程池
来源：http://hz.zhaomingkeji.xyz/gtmgdxolzr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhijiandao.cn/gtozftaeku.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.bjfxy.top/gtsnwefgbf.html

JS:   // worker_threads 线程池
来源：http://hz.feifeiyinyue.top/gtrmoumdut.html

TS:   // worker_threads 线程池
来源：http://hz.kuanghao11.cn/gtbxuwpiyh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xuetiantiany.cn/gtropzlhza.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cdnleiting.top/gtypydpxfq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinghuilouyu.cn/gtlsksegsf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cheryme.top/gtdodijagi.html

[O03] 加锁保护共享数据
来源：http://hz.hammf.cn/gtfqonucxq.html

Py:   with lock: shared += 1
来源：http://hz.fzhhl.top/gtgofvcvds.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.haohaochexian.top/gtqxzmcpuy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gotoacloud.top/gtyoaijdtw.html

TS:   // 同 JS
来源：http://hz.jlsjyb.cn/gtlxgrrhak.html

Java: synchronized (this) { shared++; }
来源：http://hz.ybcxt.top/gtfziwxvnt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xuetiantiany.cn/gtdqkxvtjc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.mhx1999.top/gtsnikwggb.html

C#:   lock (gate) { shared++; }
来源：http://hz.yangfankeji.com/gtismylfae.html

[O04] 定义异步函数并等待
来源：http://hz.kuanghao11.cn/gtunknrwiw.html

Py:   async def f():⏎    await g()
来源：http://hz.zhengqikj.top/gttvzmgbgf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.feifeiyinyue.top/gtubgjlkhf.html

JS:   async function f() { await g(); }
来源：http://hz.yuxming.cn/gthplvobzm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhoulong.xyz/gtfwfwoiko.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ybcxt.top/gtvjdyeqtd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cdnleiting.top/gtwycrnsoj.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.feifeiyinyue.top/gtfeetasni.html

C#:   async Task F() { await G(); }
来源：http://hz.havefunace.top/gtnsuyibzh.html

[O05] 并发执行并等待全部完成
来源：http://hz.haohaochexian.top/gtvgazwpbp.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhoulong.xyz/gtfmvjzrml.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.snrcjt.cn/gteqcwahmm.html

JS:   await Promise.all(tasks)
来源：http://hz.sysykeji.top/gtavrubjnj.html

TS:   await Promise.all(tasks)
来源：http://hz.aibaodan.cn/gtqgzceueu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jianghu66.top/gtkgbhymhh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yj20258.top/gtoxjvigrc.html

Ruby: threads.map(&:join)
来源：http://hz.sysykeji.top/gtzcopqsxn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinqigufen.top/gtelfgzdoh.html

[O06] 使用进程池
来源：http://hz.yanxiufei.cn/gtdefzxwdp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shangyingyoupin.top/gtytwuesmx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhongyouzk.top/gtpkmxjiwd.html

JS:   // child_process / cluster 模块
来源：http://hz.xylfe.cn/gtykwbjrrs.html

TS:   // child_process / cluster 模块
来源：http://hz.aizwys.cn/gtpuicabop.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.tian-w.cn/gtnqkurtww.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.svipenyu.cn/gtkxlkpxkf.html

Ruby: // fork 块
来源：http://hz.ywan-chungtsiang.top/gtlbkowwsi.html

C#:   Parallel.For
来源：http://hz.tian-w.cn/gtadueosxb.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtbtpsudkb.html

P. 常用工具函数
来源：http://hz.jqgufenzy.top/gtjzkuccbp.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtxdhzwyol.html

[P01] 生成 UUID
来源：http://hz.jyoumei.cn/gtonslnecp.html

Py:   str(uuid.uuid4())
来源：http://hz.52xcode.cn/gtiwmefwnp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jqgufenzy.top/gthvsseuyz.html

JS:   crypto.randomUUID()
来源：http://hz.sxryk.cn/gtnfbocrtx.html

TS:   crypto.randomUUID()
来源：http://hz.havefunace.top/gtgsgwxugk.html

Java: UUID.randomUUID().toString()
来源：http://hz.zycfv.cn/gtlgscmavu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jinghuilouyu.cn/gtecbrfxpm.html

Ruby: SecureRandom.uuid
来源：http://hz.ivvv.top/gtcmwquahc.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.fengsongda.top/gtxrxghesi.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yanxiufei.cn/gtbydqrazw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jianghu66.top/gttnasmsfr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.0kj1m.cn/gtozvhqioz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinghuilouyu.cn/gtjptrqeyg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xinyue.icu/gtfqhedsnu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cqqwz.cn/gtmopnsquc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.birdmap.top/gtrmbqwblr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.wangdashe.top/gtfmwggtjl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.aizwys.cn/gtcpqrxxlr.html

[P03] 生成短随机字符串
来源：http://hz.jinghuilouyu.cn/gtiutgzpvy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hywenlv.cn/gtljixryxk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jianghu66.top/gtqliblkdj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hysaishi.cn/gtvwpvpfku.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.fengsongda.top/gtpvrizchc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.c1oappe.top/gtpduxwotg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhongyouzk.top/gtedwggnui.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.bjfxy.top/gtjyghqljp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hnxiangtu.top/gtdlvcnnjj.html

[P04] 求长度
来源：http://hz.redwolf501.top/gtnaeecfuj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shangyingyoupin.top/gtmrgtzqcw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aizwys.cn/gtsstwcqeq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.aizwys.cn/gtiyjohqpw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinqigufen.top/gtlnfwudgp.html

Java: list.size();  map.size();  s.length()
来源：http://hz.andypj.xyz/gtwzxmmrvf.html

Go:   len(arr);  len(m)
来源：http://hz.sxryk.cn/gtumhvaaxl.html

Ruby: x.length;  x.size
来源：http://hz.xylfe.cn/gtrioozaoy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ppjwa.cn/gtwryhdfpr.html


<!-- 参考信息 -->