代发 wailian999

TS:   resp.ok;  resp.status
来源：http://hz.xinyue.icu/gttjqwdwby.html

Java: resp.statusCode()
来源：http://hz.xuanzx.com/gtgwyvmuvc.html

Go:   resp.StatusCode
来源：http://hz.0kj1m.cn/gtpjfmhtat.html

Ruby: resp.code.to_i
来源：http://hz.kuanghao11.cn/gtyxuayrmc.html

C#:   (int)resp.StatusCode
来源：http://hz.chenzaomai.com/gtnlhzemdr.html

[L08] 并发请求多个地址
来源：http://hz.bjfxy.top/gtbmrjorvj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.52xcode.cn/gtwhbnmukq.html

PHP:  curl_multi_init() 系列
来源：http://hz.cdnleiting.top/gtlhmprufq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgfzy.top/gtrvukyugo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuanzx.com/gtxayenclf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.chenlongwang.top/gtazsvbtbq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.chenzaomai.com/gtpncacnsp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.wangshuangyany.cn/gtzlwqxpyv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hnxiangtu.top/gtygphvkii.html

================================================================================
来源：http://hz.jinqigufen.top/gttboeubec.html

M. 命令行 / 进程 / 环境
来源：http://hz.yonumen.top/gtwclntlgy.html

================================================================================
来源：http://hz.daria6918.cn/gtspzcesux.html

[M01] 读取命令行参数
来源：http://hz.kuanghao11.cn/gthvobhhft.html

Py:   sys.argv[1:]
来源：http://hz.wangshuangyany.cn/gtbizlhfub.html

PHP:  $argv;  $argc;
来源：http://hz.yj20258888.top/gtwprnyrts.html

JS:   process.argv.slice(2)
来源：http://hz.meibo888.top/gttdpnqokq.html

TS:   process.argv.slice(2)
来源：http://hz.pycfn.com/gthlcpjehs.html

Java: args 数组（main 方法参数）
来源：http://hz.cdnleiting.top/gtwbofqzyo.html

Go:   os.Args[1:]
来源：http://hz.hammf.cn/gtfdwepbkt.html

Ruby: ARGV
来源：http://hz.nanxuanxn.top/gttdavjssx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yueranfly.top/gteavkgcdh.html

[M02] 读取环境变量
来源：http://hz.zhiwuduotai.top/gtosucqikd.html

Py:   os.environ.get("HOME")
来源：http://hz.shangyingyoupin.top/gtxukgcfng.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenzaomai.com/gtgfqlojhy.html

JS:   process.env.HOME
来源：http://hz.c1oappe.top/gtcahxtmel.html

TS:   process.env.HOME
来源：http://hz.snrcjt.cn/gtifyvnpvf.html

Java: System.getenv("HOME")
来源：http://hz.zhijiandao.cn/gtqomslkrk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.daxiang520.top/gttdfrmlci.html

Ruby: ENV["HOME"]
来源：http://hz.jianghu66.top/gtmmxnwlvo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xuetiantiany.cn/gtdbnuvdjs.html

[M03] 执行外部命令
来源：http://hz.chenzaomai.com/gtrnfaoboe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.redwolf501.top/gtwrfstehg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sysykeji.top/gtberpohtg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydzc1.top/gtftczfgen.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.fzhhl.top/gtjnbohhxv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jiagoushi.top/gtaxwmduyi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ehwqpu.com/gtwfrdwygb.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.mhx1999.top/gtbedgnnxz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yueranfly.top/gtzbmjodpe.html

[M04] 获取当前工作目录
来源：http://hz.hfpthk.cn/gtzkgchqhl.html

Py:   os.getcwd()
来源：http://hz.bjfxy.top/gtgulblnze.html

PHP:  getcwd();
来源：http://hz.cashguo.top/gtezyuhboi.html

JS:   process.cwd()
来源：http://hz.zhiwuduotai.top/gtaejjuduy.html

TS:   process.cwd()
来源：http://hz.dianchejie.cn/gtnaqdxdin.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shuidangran.top/gtqcqbikaj.html

Go:   os.Getwd()
来源：http://hz.hnxiangtu.top/gtvwnjwiys.html

Ruby: Dir.pwd
来源：http://hz.snrcjt.cn/gtmzhqazqy.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jinghuilouyu.cn/gtnubtlnon.html

[M05] 设置退出码
来源：http://hz.smart0.xyz/gtujepilon.html

Py:   sys.exit(1)
来源：http://hz.ppjwa.cn/gtzhttmdrt.html

PHP:  exit(1);
来源：http://hz.haohaochexian.top/gtwaoyrkbg.html

JS:   process.exit(1)
来源：http://hz.xziqi.cn/gtncbqyokf.html

TS:   process.exit(1)
来源：http://hz.cashguo.top/gtagnvnusa.html

Java: System.exit(1)
来源：http://hz.birdmap.top/gtkijfdyvj.html

Go:   os.Exit(1)
来源：http://hz.shangyingyoupin.top/gtpbhtkapb.html

Ruby: exit 1
来源：http://hz.daria6918.cn/gtuiszrehm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.dashuyun.cn/gtlwllyych.html

[M06] 向标准错误输出
来源：http://hz.jlsjyb.cn/gtcgjgdene.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ydzc1.top/gttluaylrz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yuxming.cn/gtasxpdqbb.html

JS:   console.error("err")
来源：http://hz.yuxming.cn/gtamyxhqix.html

TS:   console.error("err")
来源：http://hz.jinyuanbaomall.cn/gtofeepgkq.html

Java: System.err.println("err")
来源：http://hz.andypj.xyz/gtncwfjlpr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gzhubu.top/gtmotqzmel.html

Ruby: warn "err"
来源：http://hz.guannengcc.top/gtymezrnex.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.snrcjt.cn/gtpktlrmym.html

[M07] 判断是否为主入口
来源：http://hz.mhx1999.top/gtqhbxluhw.html

Py:   if __name__ == "__main__":
来源：http://hz.c1oappe.top/gtunyetlxg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gotoacloud.top/gtfrgydyce.html

JS:   require.main === module
来源：http://hz.dianchejie.cn/gtqlscdiso.html

TS:   require.main === module
来源：http://hz.wangdashe.top/gtkkchukek.html

Java: public static void main(String[] args)
来源：http://hz.nanxuanxn.top/gtpgzajbyh.html

Go:   func main()
来源：http://hz.9152youxi.cn/gthowbsrba.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.nanxuanxn.top/gthoeunwkh.html

C#:   static void Main(string[] args)
来源：http://hz.daxiang520.top/gtesbrvucc.html

[M08] 获取系统与运行时信息
来源：http://hz.tanke756.top/gtxgbepngl.html

Py:   platform.system();  platform.python_version()
来源：http://hz.haohaochexian.top/gtjgtpcyrs.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.dianchejie.cn/gtmtpyrcxx.html

JS:   process.platform;  process.version
来源：http://hz.zhixingplan.top/gtnhrmjdhw.html

TS:   process.platform;  process.version
来源：http://hz.cdnleiting.top/gtkfvrhdgy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.guowangkeji.top/gttvqoxzya.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhongyouzk.top/gtbzmbzojt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.nanxinkj.top/gtptbxspxv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.meibo888.top/gtcafnfwdb.html

================================================================================
来源：http://hz.cqqwz.cn/gtlbaomnre.html

N. 数据结构与算法
来源：http://hz.zhijiandao.cn/gtothoovvd.html

================================================================================
来源：http://hz.zhijiandao.cn/gtxolrlsea.html

[N01] 二分查找（有序数组）
来源：http://hz.yj20258.top/gtgxbuautm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj20258888.top/gtbbncqoui.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.daria6918.cn/gtjugcljmw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.iojbl.cn/gtgtgzaxfv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yueranfly.top/gtpismvcjt.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yvedp.cn/gtmxavoyyz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.c1oappe.top/gtlejhrwvu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.c1oappe.top/gtaotzfggs.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.aizwys.cn/gtxtbktbyu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.tianlin.xyz/gtzbieetlz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yongpay.top/gttcebxupc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.pengpengdd.cyou/gtxpugobzk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gtcynsxsgh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxuanxn.top/gtefhupwsc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cdnleiting.top/gtcelhwudk.html

Go:   slices.Sort(arr)
来源：http://hz.nanxuanxn.top/gtflazzfqc.html

Ruby: arr.sort
来源：http://hz.ydzc1.top/gthgakones.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.chenlongwang.top/gtpbalzfov.html

[N03] 快速排序（分治示例）
来源：http://hz.jqgfzy.top/gtiuxlqebk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hongshengwenyu.top/gtzjcjczkk.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xuanzx.com/gtbeihfqme.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhaomingkeji.xyz/gtpzdryorr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.daria6918.cn/gtyslnmmbc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.mhx1999.top/gtdbwhzpob.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.tian-w.cn/gtcrlvmvlj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sxryk.cn/gtgbqcvtqy.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gogol.net.cn/gtbmeypedf.html

[N04] 斐波那契数列
来源：http://hz.kuanghao11.cn/gtcrkcgwcs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xuanzx.com/gtzzttdrry.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.guowangkeji.top/gtufefwfnu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cheryme.top/gtuemqdtxc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.meibo888.top/gttmcxigej.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.bjfxy.top/gtpjbsbyke.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ybcxt.top/gtpfpovukc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.quarkkingdee.top/gtznchaxjs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.0kj1m.cn/gtlunesmgk.html

[N05] 最大公约数
来源：http://hz.xingfuxueyuan.xyz/gthqxvbfyi.html

Py:   math.gcd(a, b)
来源：http://hz.yanxiufei.cn/gtenpwcjxi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hammf.cn/gtbnexlznq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aizwys.cn/gtcvzymukm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tianlin.xyz/gtnmzbsocv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jinghuilouyu.cn/gtnvzficse.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cashguo.top/gtuendcojx.html

Ruby: a.gcd(b)
来源：http://hz.shuidangran.top/gtccskjyfx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.sysykeji.top/gtnrzhmvib.html

[N06] 判断回文字符串
来源：http://hz.tanke756.top/gtbqncfpxo.html

Py:   s == s[::-1]
来源：http://hz.yvedp.cn/gtvpgzpvqr.html

PHP:  $s === strrev($s);
来源：http://hz.xingfuxueyuan.xyz/gtfsaqmzma.html

JS:   s === [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtlmeaautl.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jyoumei.cn/gtxcqafvxa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.tanke756.top/gtjdunvqpg.html

Go:   // 双指针从两端比较
来源：http://hz.jinghuilouyu.cn/gtldcicfgo.html

Ruby: s == s.reverse
来源：http://hz.sufxvd.cn/gtsyjmfayq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinqigfzy.top/gtwtzcgjef.html

[N07] 两数之和（返回下标）
来源：http://hz.sufxvd.cn/gtaxqvmskl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.tian-w.cn/gtrswzkoxw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.aibaodan.cn/gtfgltbgzv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.wangshuangyany.cn/gtqvsweidn.html

TS:   // 手写 Map<string, number>
来源：http://hz.yuxming.cn/gtqojdhqec.html

Java: // 手写 HashMap
来源：http://hz.guannengcc.top/gthjfqiixk.html

Go:   // 手写 map[int]int
来源：http://hz.yj202588.top/gthfksbyrg.html

Ruby: // 手写 Hash
来源：http://hz.ybcxt.top/gthtxarfte.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.svipenyu.cn/gtminxrbzn.html

[N08] 生成全排列
来源：http://hz.tian-w.cn/gtltzjliwb.html

Py:   itertools.permutations(arr)
来源：http://hz.xingfuxueyuan.xyz/gtkpssjdhv.html

PHP:  // 手写递归交换
来源：http://hz.bjfxy.top/gtqxgbhgfw.html

JS:   // 手写回溯递归
来源：http://hz.xuanzx.com/gthcpjrbmv.html

TS:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtyduawxai.html

Java: // 手写回溯递归
来源：http://hz.vqdsnc.cn/gthcwkhdwx.html

Go:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtcosshawm.html

Ruby: arr.permutation.to_a
来源：http://hz.gaohongyu789.top/gtdpbliwze.html

C#:   // 手写回溯递归
来源：http://hz.ivvv.top/gtekjwrdgv.html

[N09] 栈与队列
来源：http://hz.yj202588.top/gtwdeevfqz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xingfuxueyuan.xyz/gtptxnevdw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhongyouzk.top/gtzevbxxkn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.mhx1999.top/gtixeikgoz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ydjk.org.cn/gthoojtfdz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhoulong.xyz/gttetxfnxh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yvedp.cn/gtoqkmxcis.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhaomingkeji.xyz/gthuctwbeh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.wangshuangyany.cn/gtfkhywaad.html

[N10] 链表节点定义
来源：http://hz.xylfe.cn/gtyolvpkov.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zdqjudy.top/gtomragdbl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yongpay.top/gtiaxlfetm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhengqikj.top/gtipxkijxc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tanke756.top/gtstouewry.html

Java: class Node { int v; Node next; }
来源：http://hz.xingfuxueyuan.xyz/gtlboyzuta.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.daxiang520.top/gtdvtsasup.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.snrcjt.cn/gtfyznecpl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hongshengwenyu.top/gtvtjcwabz.html

[N11] 二叉树中序遍历
来源：http://hz.tanke756.top/gtbnkgelig.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.redwolf501.top/gtrnuptejp.html

PHP:  // 手写递归函数
来源：http://hz.yj202588.top/gtvilfywyq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.bjfxy.top/gtishpuhuc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxinkj.top/gtihrhijer.html

Java: // 手写递归
来源：http://hz.0kj1m.cn/gtpcmszknt.html

Go:   // 手写递归
来源：http://hz.jiagoushi.top/gtgxhjskvv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.52xcode.cn/gtgcjlyxip.html

C#:   // 手写递归
来源：http://hz.hywenlv.cn/gtwmepessh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.svipenyu.cn/gtfohzslod.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenjidiqi.icu/gtsjvexfta.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.havefunace.top/gtwzonuurh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtudadkxvm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yangfankeji.com/gttzzppmur.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yongpay.top/gtpubohfjz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hnxiangtu.top/gtusonsjmj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.52xcode.cn/gtafntmnyz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuanzx.com/gtmxuphwyp.html

================================================================================
来源：http://hz.dianchejie.cn/gtmkmhehzt.html

O. 并发与异步
来源：http://hz.jyoumei.cn/gtvihhbvwb.html

================================================================================
来源：http://hz.chenzaomai.com/gtxgzeiswp.html

[O01] 启动一个线程
来源：http://hz.jinghuilouyu.cn/gtuebkqrtb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sweek.top/gtfvxfddyi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinghuilouyu.cn/gtgpelggmq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.quarkkingdee.top/gtzfyttmyr.html

TS:   // 同 JS
来源：http://hz.ydzc1.top/gtcvqdiusv.html

Java: new Thread(() -> f()).start()
来源：http://hz.xuanzx.com/gtrfzorzkr.html

Go:   go f()
来源：http://hz.andypj.xyz/gtlofjrqtw.html

Ruby: Thread.new { f }
来源：http://hz.jinqigufen.top/gtaimandws.html

C#:   Task.Run(() => F());
来源：http://hz.wangdashe.top/gtvnbicxhs.html

[O02] 使用线程池
来源：http://hz.shzxlz.cn/gtgtpycjdd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinyuanbaomall.cn/gtzvwxcvfy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sxryk.cn/gtljnnlehy.html

JS:   // worker_threads 线程池
来源：http://hz.jlsjyb.cn/gtfebvedif.html

TS:   // worker_threads 线程池
来源：http://hz.mhx1999.top/gtqeufbugf.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.bjfxy.top/gtqnvhoycq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yj20258.top/gtgzlqefqs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ywan-chungtsiang.top/gthdvqdhat.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.feifeiyinyue.top/gtppeusign.html

[O03] 加锁保护共享数据
来源：http://hz.xylfe.cn/gtmkvqrlxk.html

Py:   with lock: shared += 1
来源：http://hz.ybcxt.top/gtmvitwiux.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yueranfly.top/gtcfjqsokw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.havefunace.top/gtuvrcbbmc.html

TS:   // 同 JS
来源：http://hz.zhoulong.xyz/gtdecfpsof.html

Java: synchronized (this) { shared++; }
来源：http://hz.jinyuanbaomall.cn/gtnwzdfxqy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jqgufenzy.top/gtilslpura.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.9152youxi.cn/gtryzuppbx.html

C#:   lock (gate) { shared++; }
来源：http://hz.chenjidiqi.icu/gtxaadfnzf.html

[O04] 定义异步函数并等待
来源：http://hz.zhoulong.xyz/gtxkvdwyvt.html

Py:   async def f():⏎    await g()
来源：http://hz.hywenlv.cn/gtcrhwwpce.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yanxiufei.cn/gtexatrfeu.html

JS:   async function f() { await g(); }
来源：http://hz.quarkkingdee.top/gtzuxaclge.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xuetiantiany.cn/gtxtjfcswz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.fzhhl.top/gthlumghmf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.fengsongda.top/gtmvihxgqk.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hysaishi.cn/gtnhhdkfoo.html

C#:   async Task F() { await G(); }
来源：http://hz.bjfxy.top/gtohlauscd.html

[O05] 并发执行并等待全部完成
来源：http://hz.pycfn.com/gthuwmzpey.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenjidiqi.icu/gtyhxmxegv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jianghu66.top/gtqfsdbqkq.html

JS:   await Promise.all(tasks)
来源：http://hz.meibo888.top/gtghmrgzqx.html

TS:   await Promise.all(tasks)
来源：http://hz.quarkkingdee.top/gtihijeojn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhijiandao.cn/gtxfxifuwx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yuanzhike.top/gtqfionfis.html

Ruby: threads.map(&:join)
来源：http://hz.yangfankeji.com/gtfnjdxugf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ywan-chungtsiang.top/gtwojhnymc.html

[O06] 使用进程池
来源：http://hz.zhongyouzk.top/gteelvdvlw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hnxiangtu.top/gtkpudcxfw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ydzc1.top/gtjtqiyzsx.html

JS:   // child_process / cluster 模块
来源：http://hz.wangshuangyany.cn/gtnngoobrk.html

TS:   // child_process / cluster 模块
来源：http://hz.zhaomingkeji.xyz/gtmjlvjvtg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yuanzhike.top/gtsdrdwbrp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yuanzhike.top/gttgcacqjk.html

Ruby: // fork 块
来源：http://hz.svipenyu.cn/gtywdlpfay.html

C#:   Parallel.For
来源：http://hz.andypj.xyz/gtqhltwymu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtfqxzyboh.html

P. 常用工具函数
来源：http://hz.chenlongwang.top/gtuhmsnous.html

================================================================================
来源：http://hz.cucudq.cn/gtenkgbcyv.html

[P01] 生成 UUID
来源：http://hz.guannengcc.top/gttxxlunfq.html

Py:   str(uuid.uuid4())
来源：http://hz.tianlin.xyz/gtmcqcmsim.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.quarkkingdee.top/gtfkyeimkq.html

JS:   crypto.randomUUID()
来源：http://hz.dianchejie.cn/gtzaxqfraz.html

TS:   crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtzundsbsh.html

Java: UUID.randomUUID().toString()
来源：http://hz.xziqi.cn/gtdwbgewqh.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xziqi.cn/gtgvdjkwfw.html

Ruby: SecureRandom.uuid
来源：http://hz.316326.xyz/gtprnzmmes.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xuetiantiany.cn/gthdfixliy.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xziqi.cn/gtyjipfyul.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.guannengcc.top/gtrlqxjuky.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.316326.xyz/gtzibozsbr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xziqi.cn/gtjwhfhhkr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.wangdashe.top/gtzgzrcapn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hywenlv.cn/gtgdofdpfn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hfpthk.cn/gtyxdqxmom.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ydzc1.top/gtwicvcjnx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ivvv.top/gtwtyqgtfs.html

[P03] 生成短随机字符串
来源：http://hz.yuanzhike.top/gtepwmoetl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ivvv.top/gtxqeyeimb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shangyingyoupin.top/gtunawtfss.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhiwuduotai.top/gtkfyopopv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhixingplan.top/gteycmpdks.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.snrcjt.cn/gtouscibha.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhoulong.xyz/gtyjcfualf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hnxiangtu.top/gtlwmzxviq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gogol.net.cn/gtxhvtumqm.html

[P04] 求长度
来源：http://hz.yj20258.top/gtfjpamhsc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.aizwys.cn/gtbugfrofj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sufxvd.cn/gthybtllns.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.tanke756.top/gtfusdvoln.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.quarkkingdee.top/gtplwgctrj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sweek.top/gtxmuliimu.html

Go:   len(arr);  len(m)
来源：http://hz.sysykeji.top/gtckmnajnq.html

Ruby: x.length;  x.size
来源：http://hz.hywenlv.cn/gtgzjwdcbh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.wangdashe.top/gtgvnbvozt.html

[P05] 判断两个对象内容是否相等
来源：http://hz.dianchejie.cn/gtmbmcehip.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.smart0.xyz/gtcqrwtagw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.meibo888.top/gtqomssefo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.iojbl.cn/gtknaqlpvc.html


<!-- 参考信息 -->