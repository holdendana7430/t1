代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://hz.guannengcc.top/gtelswuqgm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.iojbl.cn/gtfozjypae.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.9152youxi.cn/gtthyzlrgf.html

JS:   resp.ok;  resp.status
来源：http://hz.yj20258888.top/gtabmurohf.html

TS:   resp.ok;  resp.status
来源：http://hz.yueranfly.top/gtsaqaiazr.html

Java: resp.statusCode()
来源：http://hz.tanke756.top/gtucjaojuj.html

Go:   resp.StatusCode
来源：http://hz.xylfe.cn/gtyrwvkzpx.html

Ruby: resp.code.to_i
来源：http://hz.jinqigufen.top/gtfiuabnxp.html

C#:   (int)resp.StatusCode
来源：http://hz.cdnleiting.top/gtceetyrqx.html

[L08] 并发请求多个地址
来源：http://hz.yj202588.top/gtotozephi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.redwolf501.top/gtpxrrgjki.html

PHP:  curl_multi_init() 系列
来源：http://hz.zycfv.cn/gtzrixfebn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xinyue.icu/gtzdzwepdf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sysykeji.top/gtbnltkhti.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cdnleiting.top/gtjtlmkttm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.vqdsnc.cn/gtgyfniqph.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.sweek.top/gtzvywytvt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.316326.xyz/gtbnfjptqw.html

================================================================================
来源：http://hz.nanxinkj.top/gtxfeyktyv.html

M. 命令行 / 进程 / 环境
来源：http://hz.xziqi.cn/gtttwsxgzg.html

================================================================================
来源：http://hz.yj20258888.top/gtaoihyiuq.html

[M01] 读取命令行参数
来源：http://hz.jiagoushi.top/gtfyecgqfe.html

Py:   sys.argv[1:]
来源：http://hz.yueranfly.top/gtsqxvblsh.html

PHP:  $argv;  $argc;
来源：http://hz.pengpengdd.cyou/gtkynfrcat.html

JS:   process.argv.slice(2)
来源：http://hz.hnqzz.top/gtmtqbnetv.html

TS:   process.argv.slice(2)
来源：http://hz.zhiwuduotai.top/gtwrjflncb.html

Java: args 数组（main 方法参数）
来源：http://hz.snrcjt.cn/gtzfdgrcjz.html

Go:   os.Args[1:]
来源：http://hz.jianghu66.top/gtgsrjcaat.html

Ruby: ARGV
来源：http://hz.guowangkeji.top/gtimpnnrrm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hammf.cn/gtflocdiso.html

[M02] 读取环境变量
来源：http://hz.bjfxy.top/gtxdnanben.html

Py:   os.environ.get("HOME")
来源：http://hz.xziqi.cn/gtfopvmrtf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cashguo.top/gtnmqbqqxv.html

JS:   process.env.HOME
来源：http://hz.xziqi.cn/gtddotptba.html

TS:   process.env.HOME
来源：http://hz.havefunace.top/gtasohupoq.html

Java: System.getenv("HOME")
来源：http://hz.haohaochexian.top/gtmyghvbct.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shangyingyoupin.top/gtjglstlck.html

Ruby: ENV["HOME"]
来源：http://hz.shuidangran.top/gtvvqcujmh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhaomingkeji.xyz/gtqmsiojqy.html

[M03] 执行外部命令
来源：http://hz.xuetiantiany.cn/gtqoheqlcm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hfpthk.cn/gtqlbvaakh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ydzc1.top/gtiqboxtbh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ywan-chungtsiang.top/gtxnqzkspg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhongyouzk.top/gteguwsoxh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.52xcode.cn/gtxpbpzrag.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sysykeji.top/gtksngevdo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sweek.top/gthjiymnhr.html

C#:   Process.Start("ls", "-l");
来源：http://hz.wangshuangyany.cn/gtmqguahni.html

[M04] 获取当前工作目录
来源：http://hz.ydjk.org.cn/gtxafaisrk.html

Py:   os.getcwd()
来源：http://hz.c1oappe.top/gtiigvhhpp.html

PHP:  getcwd();
来源：http://hz.zdqjudy.top/gtsdyjcbmc.html

JS:   process.cwd()
来源：http://hz.cheryme.top/gtrsqfucse.html

TS:   process.cwd()
来源：http://hz.jianghu66.top/gtkmatjzrj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.aizwys.cn/gtujuhmhsa.html

Go:   os.Getwd()
来源：http://hz.kuanghao11.cn/gtxujpxngy.html

Ruby: Dir.pwd
来源：http://hz.ybcxt.top/gtoxqehcqo.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhengqikj.top/gtbzscsnff.html

[M05] 设置退出码
来源：http://hz.jinqigufen.top/gtjhqwggzr.html

Py:   sys.exit(1)
来源：http://hz.xuetiantiany.cn/gtcdrwfokh.html

PHP:  exit(1);
来源：http://hz.chenjidiqi.icu/gteekvjtdr.html

JS:   process.exit(1)
来源：http://hz.sweek.top/gtmmodmvhm.html

TS:   process.exit(1)
来源：http://hz.zhijiandao.cn/gtuvsvmomy.html

Java: System.exit(1)
来源：http://hz.nanxinkj.top/gtvtrhxefz.html

Go:   os.Exit(1)
来源：http://hz.jianghu66.top/gtvfyhikpo.html

Ruby: exit 1
来源：http://hz.cdnleiting.top/gttoanorow.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinqigfzy.top/gtvbydhadi.html

[M06] 向标准错误输出
来源：http://hz.shanyushiyangtech.top/gtnrtqifrz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.daxiang520.top/gtqdwzrwmg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xuetiantiany.cn/gtlxpzvdyv.html

JS:   console.error("err")
来源：http://hz.havefunace.top/gtlsqyyibd.html

TS:   console.error("err")
来源：http://hz.jinqigfzy.top/gtsvdefzkb.html

Java: System.err.println("err")
来源：http://hz.cashguo.top/gtjtuabbof.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.nanxinkj.top/gtkgrmggxa.html

Ruby: warn "err"
来源：http://hz.yj202588.top/gtrqosexjp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.snrcjt.cn/gtnusgpsdo.html

[M07] 判断是否为主入口
来源：http://hz.yvedp.cn/gtkdidqvlx.html

Py:   if __name__ == "__main__":
来源：http://hz.yvedp.cn/gtjwkjbsuk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.tianlin.xyz/gtcilfyxbk.html

JS:   require.main === module
来源：http://hz.aizwys.cn/gttkbrklvh.html

TS:   require.main === module
来源：http://hz.sufxvd.cn/gtwxoszcaw.html

Java: public static void main(String[] args)
来源：http://hz.cdnleiting.top/gtdxlyuiis.html

Go:   func main()
来源：http://hz.shanyushiyangtech.top/gtqklszoxq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zdqjudy.top/gtfqcbdeng.html

C#:   static void Main(string[] args)
来源：http://hz.mhx1999.top/gtmojuqnhg.html

[M08] 获取系统与运行时信息
来源：http://hz.sysykeji.top/gtgsmiprqn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yangfankeji.com/gtukzgswmt.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.daxiang520.top/gtoejwliiy.html

JS:   process.platform;  process.version
来源：http://hz.shangyingyoupin.top/gtczbnhxoq.html

TS:   process.platform;  process.version
来源：http://hz.nanxinkj.top/gtsdzpdiki.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jqgufenzy.top/gtjhvgdwae.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.chenjidiqi.icu/gtaembukna.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.meibo888.top/gtynsxjhgb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yvedp.cn/gtdbzztkov.html

================================================================================
来源：http://hz.svipenyu.cn/gtddhymqip.html

N. 数据结构与算法
来源：http://hz.aibaodan.cn/gtunkwcixv.html

================================================================================
来源：http://hz.gotoacloud.top/gtqtnitgzf.html

[N01] 二分查找（有序数组）
来源：http://hz.shanyushiyangtech.top/gtgvvtnzdc.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yangfankeji.com/gtmewirfyk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.316326.xyz/gtkdwxjagi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cashguo.top/gtnswfjqya.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.birdmap.top/gtpyhiqhtz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yanxiufei.cn/gtezojhrmg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.wangshuangyany.cn/gtitteakek.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hnxiangtu.top/gtaecmnyux.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yj20258.top/gtlcjhhctt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yj20258.top/gtcrsdoszn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.snrcjt.cn/gtbcsjaaap.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhoulong.xyz/gtucczfpew.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sysykeji.top/gtqezydokv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenjidiqi.icu/gtadajoqmn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ydzc1.top/gtocbdrcvs.html

Go:   slices.Sort(arr)
来源：http://hz.jqgfzy.top/gtvzearusu.html

Ruby: arr.sort
来源：http://hz.yj20258888.top/gteelubeba.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.316326.xyz/gtcyinbfzl.html

[N03] 快速排序（分治示例）
来源：http://hz.yj202588.top/gtsrtnboer.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gogol.net.cn/gtshunmcew.html

PHP:  // 递归实现，或用 usort
来源：http://hz.vqdsnc.cn/gtlyhubsub.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxuanxn.top/gtlgsibtpw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aibaodan.cn/gtpywifxto.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shzxlz.cn/gtiwflolez.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.andypj.xyz/gtfwkjomyn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.tanke756.top/gtkaxwihhs.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hnxiangtu.top/gtrusjqkyp.html

[N04] 斐波那契数列
来源：http://hz.jiagoushi.top/gtpigfipkp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhengqikj.top/gtjkfwprba.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhixingplan.top/gtdjqjiqua.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shzxlz.cn/gtznuwjzpd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenjidiqi.icu/gtvfrcgwno.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhoulong.xyz/gtlfcctabt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gotoacloud.top/gtieskdalg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ppjwa.cn/gttfgdnebu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cashguo.top/gtiyzbmbpq.html

[N05] 最大公约数
来源：http://hz.zhoulong.xyz/gtobppskom.html

Py:   math.gcd(a, b)
来源：http://hz.chenzaomai.com/gtxibyxqno.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ivvv.top/gtgnptictk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.vqdsnc.cn/gtzzngdmfh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgufenzy.top/gtqtipbhmd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.aibaodan.cn/gtlqupmium.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.guowangkeji.top/gtlznsyjjv.html

Ruby: a.gcd(b)
来源：http://hz.sxryk.cn/gtnrhicayy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hysaishi.cn/gtntfszzhh.html

[N06] 判断回文字符串
来源：http://hz.yj20258.top/gtonbjfzjq.html

Py:   s == s[::-1]
来源：http://hz.hammf.cn/gtktkdgftw.html

PHP:  $s === strrev($s);
来源：http://hz.zhongyouzk.top/gtfqazolwu.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yvedp.cn/gtmjvvfedx.html

TS:   s === [...s].reverse().join("")
来源：http://hz.kuanghao11.cn/gtfjomqdfo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.0kj1m.cn/gtqdnjtggs.html

Go:   // 双指针从两端比较
来源：http://hz.tian-w.cn/gtmycvkvqc.html

Ruby: s == s.reverse
来源：http://hz.yueranfly.top/gtptewuzbv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhengqikj.top/gttpahaobo.html

[N07] 两数之和（返回下标）
来源：http://hz.yuanzhike.top/gtbhnohjdq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hnxiangtu.top/gtxoneyibu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.pengpengdd.cyou/gtmiirvgag.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.wangshuangyany.cn/gtgaypcqdc.html

TS:   // 手写 Map<string, number>
来源：http://hz.shanyushiyangkeji.top/gtklvyhddt.html

Java: // 手写 HashMap
来源：http://hz.ppjwa.cn/gttvwwbmzb.html

Go:   // 手写 map[int]int
来源：http://hz.gogol.net.cn/gthcyyllip.html

Ruby: // 手写 Hash
来源：http://hz.yanxiufei.cn/gtlwyyhpnz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhiwuduotai.top/gtsxspsozu.html

[N08] 生成全排列
来源：http://hz.hongshengwenyu.top/gtnucvbxbt.html

Py:   itertools.permutations(arr)
来源：http://hz.pycfn.com/gtvmnmykzx.html

PHP:  // 手写递归交换
来源：http://hz.chenlongwang.top/gtkqydjajl.html

JS:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtoeglsgko.html

TS:   // 手写回溯递归
来源：http://hz.yongpay.top/gtjrfnowat.html

Java: // 手写回溯递归
来源：http://hz.yuxming.cn/gtilufadxz.html

Go:   // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtdqtcjvew.html

Ruby: arr.permutation.to_a
来源：http://hz.ydjk.org.cn/gthajdbiql.html

C#:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtiayskvtv.html

[N09] 栈与队列
来源：http://hz.yj202588.top/gtfpmcugck.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xylfe.cn/gttbbfxudx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.gogol.net.cn/gtlcnbeiri.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.shanyushiyangtech.top/gtoxwizspq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yvedp.cn/gtbkicsfjb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.tianlin.xyz/gtynbgkhet.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yj20258888.top/gtthqjyddo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cheryme.top/gtbsqkszzw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hongshengwenyu.top/gtzajpiwae.html

[N10] 链表节点定义
来源：http://hz.iojbl.cn/gtkljchgkj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gaohongyu789.top/gtquwlhoel.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.guowangkeji.top/gtvdlhuduh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.pycfn.com/gtywxfkncf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhijiandao.cn/gtomsfvubj.html

Java: class Node { int v; Node next; }
来源：http://hz.tianlin.xyz/gtxeqjbjxi.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shanyushiyangkeji.top/gtsdabzsms.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinqigfzy.top/gtbfwivzys.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.mhx1999.top/gtxowbdnii.html

[N11] 二叉树中序遍历
来源：http://hz.ydjk.org.cn/gtotoyfmzu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ywan-chungtsiang.top/gtkoercvdb.html

PHP:  // 手写递归函数
来源：http://hz.haohaochexian.top/gtpwwsltbb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hywenlv.cn/gtrnbwsdwr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenjidiqi.icu/gtwxsrytns.html

Java: // 手写递归
来源：http://hz.tanke756.top/gtijtpglil.html

Go:   // 手写递归
来源：http://hz.jinyuanbaomall.cn/gtspsuyghi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhiwuduotai.top/gtwuscsfpb.html

C#:   // 手写递归
来源：http://hz.guannengcc.top/gtrnnpzjxw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cheryme.top/gtnharrkyz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hnqzz.top/gtzxdwcwvt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.nanxuanxn.top/gteligwpbb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj202588.top/gthsdgjipx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxuanxn.top/gttcqlcnmu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fzhhl.top/gthajmnqrs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ivvv.top/gtnolyswlj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zycfv.cn/gtqijvfkxl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yonumen.top/gtjssqzxdd.html

================================================================================
来源：http://hz.wangdashe.top/gtgygnknmr.html

O. 并发与异步
来源：http://hz.yuxming.cn/gtscwsidyb.html

================================================================================
来源：http://hz.fengsongda.top/gtsppedxmh.html

[O01] 启动一个线程
来源：http://hz.0kj1m.cn/gtyrgyfhrr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xuanzx.com/gtnulrwaov.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ydjk.org.cn/gtznzfcjhf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.svipenyu.cn/gtrhqtnevz.html

TS:   // 同 JS
来源：http://hz.zhijiandao.cn/gtjdrlheqy.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhoulong.xyz/gtemdkcmhv.html

Go:   go f()
来源：http://hz.yonumen.top/gtgkvxbpjz.html

Ruby: Thread.new { f }
来源：http://hz.gogol.net.cn/gtytismvqt.html

C#:   Task.Run(() => F());
来源：http://hz.jlsjyb.cn/gtjmanqrha.html

[O02] 使用线程池
来源：http://hz.ppjwa.cn/gtzxmadjbz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yuanzhike.top/gttkipuphr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.chenjidiqi.icu/gtxhqxcoum.html

JS:   // worker_threads 线程池
来源：http://hz.shuidangran.top/gtpffkozec.html

TS:   // worker_threads 线程池
来源：http://hz.ehwqpu.com/gtfrekdsit.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinqigfzy.top/gtwokwuoui.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.sysykeji.top/gtrcmalxgz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.quarkkingdee.top/gtqocstufi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.aizwys.cn/gtrhsueifs.html

[O03] 加锁保护共享数据
来源：http://hz.xuanzx.com/gttnlcsqbq.html

Py:   with lock: shared += 1
来源：http://hz.yuanzhike.top/gtefroyeuj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.316326.xyz/gtxdckrgon.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.feifeiyinyue.top/gttmywiguo.html

TS:   // 同 JS
来源：http://hz.hammf.cn/gtmdgtndvo.html

Java: synchronized (this) { shared++; }
来源：http://hz.yonumen.top/gteyjkxnvs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yanxiufei.cn/gtffrukzbd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.pengpengdd.cyou/gtkzvlyfyo.html

C#:   lock (gate) { shared++; }
来源：http://hz.yvedp.cn/gticvcokcc.html

[O04] 定义异步函数并等待
来源：http://hz.shanyushiyangtech.top/gtslqdgpin.html

Py:   async def f():⏎    await g()
来源：http://hz.yuanzhike.top/gtuegjjssn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sweek.top/gtoeyinbll.html

JS:   async function f() { await g(); }
来源：http://hz.chenlongwang.top/gtfsduvxmx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.quarkkingdee.top/gtxqxkkyum.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cucudq.cn/gtxjjubbel.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.fengsongda.top/gttoataqmh.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hnxiangtu.top/gtobbkzqec.html

C#:   async Task F() { await G(); }
来源：http://hz.cucudq.cn/gtiwroyehg.html

[O05] 并发执行并等待全部完成
来源：http://hz.wangshuangyany.cn/gtjagmxakc.html

Py:   asyncio.gather(*tasks)
来源：http://hz.daria6918.cn/gthpakrncz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhengqikj.top/gtuoskkznb.html

JS:   await Promise.all(tasks)
来源：http://hz.c1oappe.top/gtvjmhkmze.html

TS:   await Promise.all(tasks)
来源：http://hz.shangyingyoupin.top/gtvtlpzykm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jyoumei.cn/gtvtjotffo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.meibo888.top/gtgecouqga.html

Ruby: threads.map(&:join)
来源：http://hz.cdnleiting.top/gthrnwhdgl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.pycfn.com/gtsvwfceur.html

[O06] 使用进程池
来源：http://hz.yj20258888.top/gtvogxlevz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hnqzz.top/gtldbjvypc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhaomingkeji.xyz/gtgvcyyxqg.html

JS:   // child_process / cluster 模块
来源：http://hz.nanxinkj.top/gtemrfdhyj.html

TS:   // child_process / cluster 模块
来源：http://hz.sysykeji.top/gtpacwlfeo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.vqdsnc.cn/gtgyfadoyn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gaohongyu789.top/gtrseopqmo.html

Ruby: // fork 块
来源：http://hz.yangfankeji.com/gtrsfiernt.html

C#:   Parallel.For
来源：http://hz.zhoulong.xyz/gtrsjadics.html

================================================================================
来源：http://hz.jyoumei.cn/gtlurqbqdv.html

P. 常用工具函数
来源：http://hz.ehwqpu.com/gtnvegxnhl.html

================================================================================
来源：http://hz.nanxinkj.top/gtyyfomoff.html

[P01] 生成 UUID
来源：http://hz.cashguo.top/gtzpfkvxmv.html

Py:   str(uuid.uuid4())
来源：http://hz.yuxming.cn/gtsbpfyimn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yvedp.cn/gtlqrcekzg.html

JS:   crypto.randomUUID()
来源：http://hz.yanxiufei.cn/gtcdkgxxfs.html

TS:   crypto.randomUUID()
来源：http://hz.nwbrower.top/gtgqpivovs.html

Java: UUID.randomUUID().toString()
来源：http://hz.jinghuilouyu.cn/gtriotzymb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.316326.xyz/gtvkpbugbm.html

Ruby: SecureRandom.uuid
来源：http://hz.smart0.xyz/gtksyakudz.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.nwbrower.top/gtobvpecqb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shanyushiyangkeji.top/gthkeyltar.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hammf.cn/gtcxeiqqoi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yuxming.cn/gtyljngvvy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.nanxuanxn.top/gtzhmhgcmk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.svipenyu.cn/gttrayentz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.pengpengdd.cyou/gtgpuutciz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.meibo888.top/gtsxmrqqds.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinqigfzy.top/gttlbsqdmh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shanyushiyangtech.top/gtpeknrhrc.html

[P03] 生成短随机字符串
来源：http://hz.meibo888.top/gttyuomnrr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.tianlin.xyz/gtalagjaaf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jiagoushi.top/gtugqsluoz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258.top/gtjisjihxs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuanzx.com/gtrhzntjzo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhaomingkeji.xyz/gtlkmbiqos.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ywan-chungtsiang.top/gtfxnywosc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ehwqpu.com/gteyvanikg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.vqdsnc.cn/gtvnqkhgbw.html

[P04] 求长度
来源：http://hz.haohaochexian.top/gtnkrnzxal.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.daria6918.cn/gtukdttevx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shzxlz.cn/gtscborwpq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dianchejie.cn/gtwevdzwfs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yangfankeji.com/gtoztxkeyh.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yj20258888.top/gtxstcmfgh.html

Go:   len(arr);  len(m)
来源：http://hz.sweek.top/gtgibsngfn.html

Ruby: x.length;  x.size
来源：http://hz.jinqigfzy.top/gtefacmjys.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.wangdashe.top/gtdbjmehci.html


<!-- 参考信息 -->