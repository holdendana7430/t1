代发 wailian999

C#:   (int)resp.StatusCode
来源：http://hz.gzhubu.top/gtzvoygwwz.html

[L08] 并发请求多个地址
来源：http://hz.aibaodan.cn/gtoswheabk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj20258.top/gtkhmxqgbx.html

PHP:  curl_multi_init() 系列
来源：http://hz.birdmap.top/gtombcaxse.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jianghu66.top/gtnsjeahar.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ehwqpu.com/gthdnojgof.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.redwolf501.top/gtexmoiaqj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jqgfzy.top/gthiikfblb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.wangdashe.top/gtovhkvarh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jqgufenzy.top/gtcmhvpuca.html

================================================================================
来源：http://hz.yj20258.top/gtinbqxaax.html

M. 命令行 / 进程 / 环境
来源：http://hz.yj20258.top/gttpeuppjm.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtrpjrlfxa.html

[M01] 读取命令行参数
来源：http://hz.xinyue.icu/gtccepqdbg.html

Py:   sys.argv[1:]
来源：http://hz.xylfe.cn/gtgfkhbvmi.html

PHP:  $argv;  $argc;
来源：http://hz.xingfuxueyuan.xyz/gtrxxagllu.html

JS:   process.argv.slice(2)
来源：http://hz.zhiwuduotai.top/gtwzggeseb.html

TS:   process.argv.slice(2)
来源：http://hz.ybcxt.top/gtcywpensr.html

Java: args 数组（main 方法参数）
来源：http://hz.gzhubu.top/gtdxctsarl.html

Go:   os.Args[1:]
来源：http://hz.ppjwa.cn/gtsdgvnvfs.html

Ruby: ARGV
来源：http://hz.hysaishi.cn/gtuhlqsezp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gaohongyu789.top/gtgfipjduc.html

[M02] 读取环境变量
来源：http://hz.c1oappe.top/gtecssosrw.html

Py:   os.environ.get("HOME")
来源：http://hz.jinghuilouyu.cn/gtfkepjzlf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinyuanbaomall.cn/gtwtwfvpxq.html

JS:   process.env.HOME
来源：http://hz.nwbrower.top/gtvflwcdsk.html

TS:   process.env.HOME
来源：http://hz.hnqzz.top/gtxdvxtelb.html

Java: System.getenv("HOME")
来源：http://hz.smart0.xyz/gtqzxerqca.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jiagoushi.top/gttethjsdh.html

Ruby: ENV["HOME"]
来源：http://hz.iojbl.cn/gtbrdaeaad.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ywan-chungtsiang.top/gtvgohneae.html

[M03] 执行外部命令
来源：http://hz.ivvv.top/gtrpzirfxl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.daria6918.cn/gtmubppaug.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.fengsongda.top/gtgfipqmmd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.dashuyun.cn/gtifqxeucx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yvedp.cn/gtrmukxrxb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ppjwa.cn/gtpovvcmsv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.dashuyun.cn/gtmubaabup.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.tanke756.top/gtqnlffxht.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shangyingyoupin.top/gthvbvmfgt.html

[M04] 获取当前工作目录
来源：http://hz.yonumen.top/gtofomvqxm.html

Py:   os.getcwd()
来源：http://hz.0kj1m.cn/gtiyybxhlh.html

PHP:  getcwd();
来源：http://hz.jinghuilouyu.cn/gtraoedufh.html

JS:   process.cwd()
来源：http://hz.zhixingplan.top/gtuqxnrfed.html

TS:   process.cwd()
来源：http://hz.jlsjyb.cn/gtjogotgfy.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cqqwz.cn/gtinkaaavn.html

Go:   os.Getwd()
来源：http://hz.sxryk.cn/gtcuhlnudh.html

Ruby: Dir.pwd
来源：http://hz.wangdashe.top/gthjtyjveq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.tanke756.top/gtlhhcxosy.html

[M05] 设置退出码
来源：http://hz.52xcode.cn/gtjyemjhef.html

Py:   sys.exit(1)
来源：http://hz.wangshuangyany.cn/gtshmoemeq.html

PHP:  exit(1);
来源：http://hz.jinqigufen.top/gtrnlowssj.html

JS:   process.exit(1)
来源：http://hz.haohaochexian.top/gtxvfvmvxy.html

TS:   process.exit(1)
来源：http://hz.yj20258.top/gtfwlptjie.html

Java: System.exit(1)
来源：http://hz.wangshuangyany.cn/gtkodsajad.html

Go:   os.Exit(1)
来源：http://hz.dianchejie.cn/gtycnopchf.html

Ruby: exit 1
来源：http://hz.shuidangran.top/gttsplmtcz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.316326.xyz/gthxvfmcxz.html

[M06] 向标准错误输出
来源：http://hz.dianchejie.cn/gtsieuwmec.html

Py:   print("err", file=sys.stderr)
来源：http://hz.c1oappe.top/gtuycfzhob.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shangyingyoupin.top/gtfifzvtox.html

JS:   console.error("err")
来源：http://hz.yonumen.top/gtwhwmlocd.html

TS:   console.error("err")
来源：http://hz.pycfn.com/gtizudfung.html

Java: System.err.println("err")
来源：http://hz.yvedp.cn/gtsmhvdvek.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xylfe.cn/gtnwjigpbh.html

Ruby: warn "err"
来源：http://hz.hammf.cn/gtgnsmtjjn.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.wangdashe.top/gtcgbioxft.html

[M07] 判断是否为主入口
来源：http://hz.fzhhl.top/gtmbcypcwm.html

Py:   if __name__ == "__main__":
来源：http://hz.zhiwuduotai.top/gtuaiuujzj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinghuilouyu.cn/gtywzwcdnv.html

JS:   require.main === module
来源：http://hz.zhiwuduotai.top/gtwicgmtot.html

TS:   require.main === module
来源：http://hz.ydjk.org.cn/gtyieznggp.html

Java: public static void main(String[] args)
来源：http://hz.yueranfly.top/gtwrnpycny.html

Go:   func main()
来源：http://hz.hnqzz.top/gtbsxroxqs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yvedp.cn/gtsaviiphg.html

C#:   static void Main(string[] args)
来源：http://hz.shanyushiyangtech.top/gtrfshgwcb.html

[M08] 获取系统与运行时信息
来源：http://hz.cqqwz.cn/gtyaoasise.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zdqjudy.top/gtvgoedliy.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.feifeiyinyue.top/gteieyvbkt.html

JS:   process.platform;  process.version
来源：http://hz.hnqzz.top/gtmluawgpa.html

TS:   process.platform;  process.version
来源：http://hz.zhengqikj.top/gtiekowlvq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gotoacloud.top/gtcrlyqcfj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.fengsongda.top/gtoijbhvcw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhoulong.xyz/gtfepmiqrz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhaomingkeji.xyz/gtqqaxtrwt.html

================================================================================
来源：http://hz.meibo888.top/gthhgyaxsc.html

N. 数据结构与算法
来源：http://hz.52xcode.cn/gtaueuoref.html

================================================================================
来源：http://hz.wangdashe.top/gtisrlksvy.html

[N01] 二分查找（有序数组）
来源：http://hz.hywenlv.cn/gttdwidqmz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.daxiang520.top/gthtplextf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jqgufenzy.top/gtgftyluxs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.redwolf501.top/gtldekeuib.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydjk.org.cn/gtqikfhrpy.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cdnleiting.top/gtjgpzirbr.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenlongwang.top/gttgqzttdk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.fengsongda.top/gtpvrkkrae.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ivvv.top/gtogfysbhw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jiagoushi.top/gtbyuogzdw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ppjwa.cn/gtsytnyidf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinyuanbaomall.cn/gtgupsromu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xinyue.icu/gtmhyzdava.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ydjk.org.cn/gtkhomwjyu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shanyushiyangtech.top/gtwpoxgdui.html

Go:   slices.Sort(arr)
来源：http://hz.zycfv.cn/gtwsaxpaxn.html

Ruby: arr.sort
来源：http://hz.zhijiandao.cn/gtqymtskvz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhiwuduotai.top/gtvwvnpimi.html

[N03] 快速排序（分治示例）
来源：http://hz.ywan-chungtsiang.top/gtdowwzcrg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gogol.net.cn/gtyntlaukp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhijiandao.cn/gthpblqlze.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxinkj.top/gtoigbczqj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cashguo.top/gtteqdjmsp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jyoumei.cn/gtxlcvpokb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.birdmap.top/gtaintrdzz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yangfankeji.com/gtdqydwjcm.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.quarkkingdee.top/gtjghjreip.html

[N04] 斐波那契数列
来源：http://hz.kuanghao11.cn/gthxnlsbot.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xylfe.cn/gtmmwhddpa.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yj202588.top/gtzqyozpgg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnxiangtu.top/gtzsxsunsv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gaohongyu789.top/gtjsnksxcf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jiagoushi.top/gtoyuxwmsg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shanyushiyangtech.top/gthrfdbsey.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinyuanbaomall.cn/gtucxgpahf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yonumen.top/gtkhgukdyz.html

[N05] 最大公约数
来源：http://hz.zhaomingkeji.xyz/gtbgxfbaid.html

Py:   math.gcd(a, b)
来源：http://hz.guannengcc.top/gticxhcdwa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yonumen.top/gtdnyyrgvl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daxiang520.top/gtyotrnqsa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gzhubu.top/gtrhgrmzpv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ydjk.org.cn/gtfyookzlx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.feifeiyinyue.top/gtxlcpipyj.html

Ruby: a.gcd(b)
来源：http://hz.quarkkingdee.top/gtblgnxiza.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ywan-chungtsiang.top/gtnpkrrwvg.html

[N06] 判断回文字符串
来源：http://hz.kuanghao11.cn/gtuzyvilbm.html

Py:   s == s[::-1]
来源：http://hz.cashguo.top/gtzemidopq.html

PHP:  $s === strrev($s);
来源：http://hz.chenlongwang.top/gttvswswpx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.52xcode.cn/gtjephxocl.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cashguo.top/gtklbvdtax.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.havefunace.top/gtsoovscqp.html

Go:   // 双指针从两端比较
来源：http://hz.jlsjyb.cn/gtllvivdnm.html

Ruby: s == s.reverse
来源：http://hz.xylfe.cn/gtyteqsxim.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gotoacloud.top/gtmorcvofa.html

[N07] 两数之和（返回下标）
来源：http://hz.fzhhl.top/gtjhddfmbo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.0kj1m.cn/gtgqsfhdpg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zycfv.cn/gtmhwrhdjm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.birdmap.top/gtngkmabtq.html

TS:   // 手写 Map<string, number>
来源：http://hz.ywan-chungtsiang.top/gtpuoxwveg.html

Java: // 手写 HashMap
来源：http://hz.wangshuangyany.cn/gtudfacyak.html

Go:   // 手写 map[int]int
来源：http://hz.zdqjudy.top/gtoxharpiq.html

Ruby: // 手写 Hash
来源：http://hz.xziqi.cn/gtavpzrvvj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.52xcode.cn/gtfsewfsdh.html

[N08] 生成全排列
来源：http://hz.xylfe.cn/gtkpymwthf.html

Py:   itertools.permutations(arr)
来源：http://hz.fzhhl.top/gtbrsgwjlj.html

PHP:  // 手写递归交换
来源：http://hz.vqdsnc.cn/gtmobahnaz.html

JS:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtwgjknnox.html

TS:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtcuadmtew.html

Java: // 手写回溯递归
来源：http://hz.aibaodan.cn/gtxrbjuega.html

Go:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gthjniwsye.html

Ruby: arr.permutation.to_a
来源：http://hz.hywenlv.cn/gtvhyoicxb.html

C#:   // 手写回溯递归
来源：http://hz.316326.xyz/gtyxtfwakz.html

[N09] 栈与队列
来源：http://hz.guowangkeji.top/gtkscecbig.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.chenlongwang.top/gtydwmgydd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.bjfxy.top/gtvtbufzeo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.iojbl.cn/gtclbfavyf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj202588.top/gtlyrkcesd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.daxiang520.top/gttirsecia.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.nwbrower.top/gtdqgzncgl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shzxlz.cn/gtlrygulmk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhaomingkeji.xyz/gtrxxshhss.html

[N10] 链表节点定义
来源：http://hz.pengpengdd.cyou/gtuoygriwm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yj202588.top/gttaxepemh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.guowangkeji.top/gtgcuzfyjl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.fengsongda.top/gtvmguvbxn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cdnleiting.top/gtyatbrfvi.html

Java: class Node { int v; Node next; }
来源：http://hz.vqdsnc.cn/gtfiaqxaso.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shzxlz.cn/gtkidoiakc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zdqjudy.top/gtpcbukvbq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nanxinkj.top/gtdilukihc.html

[N11] 二叉树中序遍历
来源：http://hz.guowangkeji.top/gtshtezypg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.vqdsnc.cn/gtqajmpeqi.html

PHP:  // 手写递归函数
来源：http://hz.shanyushiyangtech.top/gtfshvlhwq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cashguo.top/gtloqkowom.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shzxlz.cn/gtpvwvoyqi.html

Java: // 手写递归
来源：http://hz.ybcxt.top/gtckcfuqjc.html

Go:   // 手写递归
来源：http://hz.cqqwz.cn/gtdchofibl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jinghuilouyu.cn/gtwmwlutai.html

C#:   // 手写递归
来源：http://hz.shanyushiyangtech.top/gthuketiuv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yuanzhike.top/gtdexqjskf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinyuanbaomall.cn/gtscniqcvm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.52xcode.cn/gtvsfhmhmv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.iojbl.cn/gtkqvnsali.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shangyingyoupin.top/gtjoadbril.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xingfuxueyuan.xyz/gteisjngmp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ywan-chungtsiang.top/gtejbiuzag.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.c1oappe.top/gtfiybhkpr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.smart0.xyz/gtxjjkegdk.html

================================================================================
来源：http://hz.cucudq.cn/gtvmualbsz.html

O. 并发与异步
来源：http://hz.jinghuilouyu.cn/gtuyvrfvqt.html

================================================================================
来源：http://hz.gogol.net.cn/gtnibxxdru.html

[O01] 启动一个线程
来源：http://hz.fzhhl.top/gtidxoaitv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yvedp.cn/gtdcpkvmjo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yuxming.cn/gtabofdttm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.quarkkingdee.top/gtnqrkbzes.html

TS:   // 同 JS
来源：http://hz.zhongyouzk.top/gtwgcrorgs.html

Java: new Thread(() -> f()).start()
来源：http://hz.yj202588.top/gtnemqsjko.html

Go:   go f()
来源：http://hz.hywenlv.cn/gtunudbgdh.html

Ruby: Thread.new { f }
来源：http://hz.cdnleiting.top/gtbxuidfis.html

C#:   Task.Run(() => F());
来源：http://hz.dashuyun.cn/gtvylwwllb.html

[O02] 使用线程池
来源：http://hz.jqgfzy.top/gtattimczy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.andypj.xyz/gtolasmllq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhijiandao.cn/gtlrqqiakj.html

JS:   // worker_threads 线程池
来源：http://hz.gzhubu.top/gtuzceibyo.html

TS:   // worker_threads 线程池
来源：http://hz.daria6918.cn/gtpqkfkvjj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jlsjyb.cn/gtsudyjjwx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.daxiang520.top/gtlzbjcmzt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yj20258.top/gtzwrvimic.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.wangdashe.top/gtwsiftzzh.html

[O03] 加锁保护共享数据
来源：http://hz.kuanghao11.cn/gtbaabduqa.html

Py:   with lock: shared += 1
来源：http://hz.gaohongyu789.top/gtekbpslok.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.vqdsnc.cn/gtsnezurql.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.vqdsnc.cn/gtjpywsvpt.html

TS:   // 同 JS
来源：http://hz.shanyushiyangtech.top/gtcybjauqi.html

Java: synchronized (this) { shared++; }
来源：http://hz.sufxvd.cn/gtnhtrapie.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jinghuilouyu.cn/gtxeuhbceb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cheryme.top/gtoztwoyeb.html

C#:   lock (gate) { shared++; }
来源：http://hz.sysykeji.top/gtcmarwion.html

[O04] 定义异步函数并等待
来源：http://hz.nwbrower.top/gtjtppbquz.html

Py:   async def f():⏎    await g()
来源：http://hz.cheryme.top/gtrfyjjazc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xuanzx.com/gtpcvbowwr.html

JS:   async function f() { await g(); }
来源：http://hz.havefunace.top/gtfpitavrq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhoulong.xyz/gtfkxajwtx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cqqwz.cn/gtodhdckxj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jyoumei.cn/gtubqdegzy.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.pengpengdd.cyou/gtckjsikts.html

C#:   async Task F() { await G(); }
来源：http://hz.jinghuilouyu.cn/gtlqvwwcly.html

[O05] 并发执行并等待全部完成
来源：http://hz.ivvv.top/gtsbrhkyol.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shangyingyoupin.top/gtvlnphqjj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hnxiangtu.top/gtxrbxurbq.html

JS:   await Promise.all(tasks)
来源：http://hz.tanke756.top/gteakpxldn.html

TS:   await Promise.all(tasks)
来源：http://hz.ywan-chungtsiang.top/gttgluwdbm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xziqi.cn/gtmwewpiqq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.kuanghao11.cn/gtthclahtj.html

Ruby: threads.map(&:join)
来源：http://hz.tanke756.top/gtuzvfpxxe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.guowangkeji.top/gtszncfwee.html

[O06] 使用进程池
来源：http://hz.c1oappe.top/gtzdsuonuv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhixingplan.top/gtkhwfhjvo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ybcxt.top/gtfrkytwzx.html

JS:   // child_process / cluster 模块
来源：http://hz.haohaochexian.top/gtomfvlhtx.html

TS:   // child_process / cluster 模块
来源：http://hz.xinyue.icu/gtuwbzxyyt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.havefunace.top/gtebptblhi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yongpay.top/gtwnuykaxs.html

Ruby: // fork 块
来源：http://hz.cheryme.top/gtvzsieoaq.html

C#:   Parallel.For
来源：http://hz.sufxvd.cn/gtyhyibmaf.html

================================================================================
来源：http://hz.gzhubu.top/gtmlpbpnoe.html

P. 常用工具函数
来源：http://hz.jinyuanbaomall.cn/gtfjbyvvxj.html

================================================================================
来源：http://hz.ehwqpu.com/gtrauirvwh.html

[P01] 生成 UUID
来源：http://hz.xuanzx.com/gtvakfefyg.html

Py:   str(uuid.uuid4())
来源：http://hz.yj20258888.top/gtjlzvkavg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.daria6918.cn/gtbxrjtrng.html

JS:   crypto.randomUUID()
来源：http://hz.jinqigfzy.top/gtwumckzfg.html

TS:   crypto.randomUUID()
来源：http://hz.jqgfzy.top/gttjnibjej.html

Java: UUID.randomUUID().toString()
来源：http://hz.hongshengwenyu.top/gtrkvsmmob.html

Go:   // 用 github.com/google/uuid
来源：http://hz.quarkkingdee.top/gtnoabilqg.html

Ruby: SecureRandom.uuid
来源：http://hz.wangdashe.top/gtdspvcwrq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.gogol.net.cn/gtcceozttk.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hysaishi.cn/gtfdfgknim.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yuanzhike.top/gtuhhseikr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.haohaochexian.top/gtikvrxlnw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.birdmap.top/gtqlfqvxss.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.quarkkingdee.top/gtkvwfbduw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.sysykeji.top/gtzxvblupn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yj20258.top/gtepnsczoe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xuanzx.com/gtfehqenud.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.nanxinkj.top/gtgarhahro.html

[P03] 生成短随机字符串
来源：http://hz.meibo888.top/gtlnoglpbt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.mhx1999.top/gtixvrcjpw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.kuanghao11.cn/gtdtowjfmd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xziqi.cn/gthqtjqsyx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenjidiqi.icu/gthsrcqxka.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.wangdashe.top/gtvbpnxgbs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nwbrower.top/gtivivyejt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhongyouzk.top/gttsfabujs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.guowangkeji.top/gtpczoiczk.html

[P04] 求长度
来源：http://hz.yj202588.top/gtumojprsf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jqgfzy.top/gtocowbfun.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shangyingyoupin.top/gtuhynjazj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuanzhike.top/gtikhhplkm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangdashe.top/gtvifcodte.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xingfuxueyuan.xyz/gttgxewwou.html

Go:   len(arr);  len(m)
来源：http://hz.hongshengwenyu.top/gtmufhrgdo.html

Ruby: x.length;  x.size
来源：http://hz.sxryk.cn/gtnychrbdv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.redwolf501.top/gtwcqivade.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhongyouzk.top/gtzwjfcsby.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.316326.xyz/gtohctmmtx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.316326.xyz/gtsoageakr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.feifeiyinyue.top/gtmbobnxpa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gogol.net.cn/gtxlhjcgfn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.0kj1m.cn/gtlsaigpgy.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yueranfly.top/gtixjaborv.html

Ruby: a == b
来源：http://hz.yj202588.top/gtovgunbms.html


<!-- 参考信息 -->