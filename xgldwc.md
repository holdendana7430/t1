代发 wailian999

TS:   resp.ok;  resp.status
来源：http://hz.ydjk.org.cn/gtmnasjpvb.html

Java: resp.statusCode()
来源：http://hz.tianlin.xyz/gtorkqvmqq.html

Go:   resp.StatusCode
来源：http://hz.guannengcc.top/gthvyesqbz.html

Ruby: resp.code.to_i
来源：http://hz.quarkkingdee.top/gthmflogua.html

C#:   (int)resp.StatusCode
来源：http://hz.wangshuangyany.cn/gtssfoflqy.html

[L08] 并发请求多个地址
来源：http://hz.ehwqpu.com/gtflecloxq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.guowangkeji.top/gtvdlcoekm.html

PHP:  curl_multi_init() 系列
来源：http://hz.gzhubu.top/gtqnlshbij.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangshuangyany.cn/gtxixtpajw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtphrirdbw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xziqi.cn/gtshywqxrq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.pycfn.com/gtwitrvgcw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jianghu66.top/gtstqfuqlg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.nwbrower.top/gtxlaqhiij.html

================================================================================
来源：http://hz.andypj.xyz/gtcathdsvc.html

M. 命令行 / 进程 / 环境
来源：http://hz.guowangkeji.top/gtzcwbixpi.html

================================================================================
来源：http://hz.mhx1999.top/gtbeeocqyz.html

[M01] 读取命令行参数
来源：http://hz.jqgufenzy.top/gtlleglygj.html

Py:   sys.argv[1:]
来源：http://hz.zhixingplan.top/gtcebswupj.html

PHP:  $argv;  $argc;
来源：http://hz.cucudq.cn/gthbslxrwo.html

JS:   process.argv.slice(2)
来源：http://hz.hysaishi.cn/gtxstonjfz.html

TS:   process.argv.slice(2)
来源：http://hz.snrcjt.cn/gtcmyxkicn.html

Java: args 数组（main 方法参数）
来源：http://hz.xuanzx.com/gtjfjbfelj.html

Go:   os.Args[1:]
来源：http://hz.jiagoushi.top/gtqjxjcdpp.html

Ruby: ARGV
来源：http://hz.bjfxy.top/gtrkbasgif.html

C#:   args 数组（Main 方法参数）
来源：http://hz.mhx1999.top/gtecgfutur.html

[M02] 读取环境变量
来源：http://hz.wangdashe.top/gtrqgrnzsp.html

Py:   os.environ.get("HOME")
来源：http://hz.zhaomingkeji.xyz/gtclqochew.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.dianchejie.cn/gtdjtkstwp.html

JS:   process.env.HOME
来源：http://hz.shanyushiyangtech.top/gtxippdsfo.html

TS:   process.env.HOME
来源：http://hz.kuanghao11.cn/gtcsfoggij.html

Java: System.getenv("HOME")
来源：http://hz.aizwys.cn/gtudvqykhq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xziqi.cn/gtoxqkojxs.html

Ruby: ENV["HOME"]
来源：http://hz.birdmap.top/gtxcyenvti.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhengqikj.top/gteohocjou.html

[M03] 执行外部命令
来源：http://hz.zhixingplan.top/gtlrxeklzb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cdnleiting.top/gtpkyuparg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shangyingyoupin.top/gtlsmkgfue.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhiwuduotai.top/gtpcyjdanq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhaomingkeji.xyz/gtgvukikez.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.svipenyu.cn/gtcmxawduk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jiagoushi.top/gtfohgwico.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.nanxinkj.top/gtmxlbyjur.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhengqikj.top/gtmsllqyli.html

[M04] 获取当前工作目录
来源：http://hz.vqdsnc.cn/gtobdutrmo.html

Py:   os.getcwd()
来源：http://hz.hywenlv.cn/gtxhsejhsw.html

PHP:  getcwd();
来源：http://hz.shzxlz.cn/gtmvucnleh.html

JS:   process.cwd()
来源：http://hz.vqdsnc.cn/gtnzbuwezm.html

TS:   process.cwd()
来源：http://hz.feifeiyinyue.top/gtuxpqgymw.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.svipenyu.cn/gtxkwffiuj.html

Go:   os.Getwd()
来源：http://hz.shanyushiyangkeji.top/gtsfkaoqql.html

Ruby: Dir.pwd
来源：http://hz.cdnleiting.top/gtzguhqltf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sweek.top/gtfvfgtgsv.html

[M05] 设置退出码
来源：http://hz.ppjwa.cn/gtfsdbfqhf.html

Py:   sys.exit(1)
来源：http://hz.zhijiandao.cn/gtbfzrrisq.html

PHP:  exit(1);
来源：http://hz.jiagoushi.top/gtmxxgcrxt.html

JS:   process.exit(1)
来源：http://hz.xziqi.cn/gtnjepubcm.html

TS:   process.exit(1)
来源：http://hz.c1oappe.top/gtxkfeuftr.html

Java: System.exit(1)
来源：http://hz.jinghuilouyu.cn/gtwfdcmnsl.html

Go:   os.Exit(1)
来源：http://hz.fzhhl.top/gtpbmykjok.html

Ruby: exit 1
来源：http://hz.svipenyu.cn/gtnyoiszai.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yonumen.top/gtzddjnkfd.html

[M06] 向标准错误输出
来源：http://hz.redwolf501.top/gtfhzqijuq.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sxryk.cn/gteyuukarr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hnqzz.top/gtetuqvhwa.html

JS:   console.error("err")
来源：http://hz.nwbrower.top/gtaahunjkd.html

TS:   console.error("err")
来源：http://hz.tianlin.xyz/gtpyrdblav.html

Java: System.err.println("err")
来源：http://hz.ywan-chungtsiang.top/gtiodweehy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cheryme.top/gtvqlgbrcs.html

Ruby: warn "err"
来源：http://hz.dianchejie.cn/gtfhpkgzfe.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.dashuyun.cn/gtovryphzv.html

[M07] 判断是否为主入口
来源：http://hz.shzxlz.cn/gtmxnrpxnv.html

Py:   if __name__ == "__main__":
来源：http://hz.zhongyouzk.top/gtelenjwuo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.aizwys.cn/gtebjwvcct.html

JS:   require.main === module
来源：http://hz.guannengcc.top/gttoptbeld.html

TS:   require.main === module
来源：http://hz.vqdsnc.cn/gtxsinbacv.html

Java: public static void main(String[] args)
来源：http://hz.dianchejie.cn/gtrcufbyjo.html

Go:   func main()
来源：http://hz.dianchejie.cn/gttsjzwrqp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.chenzaomai.com/gtkpzzhlph.html

C#:   static void Main(string[] args)
来源：http://hz.redwolf501.top/gtcvokmocy.html

[M08] 获取系统与运行时信息
来源：http://hz.yuxming.cn/gtteqgfglj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.nanxuanxn.top/gtfvptdoec.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yuanzhike.top/gtanlotudw.html

JS:   process.platform;  process.version
来源：http://hz.hfpthk.cn/gtwilypsow.html

TS:   process.platform;  process.version
来源：http://hz.andypj.xyz/gtgwqtjhpf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xylfe.cn/gtbbmvkefa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hnqzz.top/gtiofoowwu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zycfv.cn/gtincoxnsp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yongpay.top/gtgkpvyeed.html

================================================================================
来源：http://hz.aibaodan.cn/gtnwlgyyrk.html

N. 数据结构与算法
来源：http://hz.52xcode.cn/gtsulllirh.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtpzshzybc.html

[N01] 二分查找（有序数组）
来源：http://hz.hongshengwenyu.top/gtwkkmqwfl.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ybcxt.top/gtycfkzimx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sweek.top/gtxynfhadw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sxryk.cn/gtvenalxiy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangdashe.top/gtayereoxe.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jlsjyb.cn/gtajwutzls.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhongyouzk.top/gtnvnxmhal.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.meibo888.top/gtyogixojp.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sweek.top/gtfkgtkzbh.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.smart0.xyz/gtwjpxjvhh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gogol.net.cn/gtpxjfvxra.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hnqzz.top/gtufpexnam.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gogol.net.cn/gtwoimnnbl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenlongwang.top/gtjggyitvj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yj20258888.top/gtgzkipjhe.html

Go:   slices.Sort(arr)
来源：http://hz.zhengqikj.top/gtwuqdtvhe.html

Ruby: arr.sort
来源：http://hz.yuxming.cn/gtkgfkjjmv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinqigufen.top/gtqwvwgqoj.html

[N03] 快速排序（分治示例）
来源：http://hz.xuanzx.com/gtjfrerddn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.sufxvd.cn/gtazkhtkwn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhiwuduotai.top/gtykyerdav.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinghuilouyu.cn/gtdtwduuer.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhengqikj.top/gtthhwckpc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.mhx1999.top/gtxppoksvd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cdnleiting.top/gtndnbuoxy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.dashuyun.cn/gtqzrduzwy.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yuanzhike.top/gtfkmmeoww.html

[N04] 斐波那契数列
来源：http://hz.xinyue.icu/gtfgjeqlbj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ywan-chungtsiang.top/gtqzukzynm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tanke756.top/gtxtlinfjm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenjidiqi.icu/gtqcqahpit.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gzhubu.top/gtckkyezbb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.havefunace.top/gtdgmtmrxl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yangfankeji.com/gtsuvfdsai.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.tian-w.cn/gthmuvcrlp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhengqikj.top/gtedcudchk.html

[N05] 最大公约数
来源：http://hz.tianlin.xyz/gttqrmsvbb.html

Py:   math.gcd(a, b)
来源：http://hz.mhx1999.top/gtobyriozh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.havefunace.top/gtgqewaxny.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhixingplan.top/gtnknfhfxf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.feifeiyinyue.top/gtzdkizijp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shuidangran.top/gtgvgyluyf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ivvv.top/gthgrnynew.html

Ruby: a.gcd(b)
来源：http://hz.hongshengwenyu.top/gtivcpxtja.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.nwbrower.top/gtstbqpnfz.html

[N06] 判断回文字符串
来源：http://hz.jqgufenzy.top/gthtbfxqtr.html

Py:   s == s[::-1]
来源：http://hz.0kj1m.cn/gtbwtoshng.html

PHP:  $s === strrev($s);
来源：http://hz.guowangkeji.top/gtjwbqgcsz.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ydjk.org.cn/gttrcfvhas.html

TS:   s === [...s].reverse().join("")
来源：http://hz.pycfn.com/gttkeqdlxz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.c1oappe.top/gtgfqpsjlr.html

Go:   // 双指针从两端比较
来源：http://hz.fengsongda.top/gtrirrpgvb.html

Ruby: s == s.reverse
来源：http://hz.daria6918.cn/gtcktbndya.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ppjwa.cn/gtttpxxkgh.html

[N07] 两数之和（返回下标）
来源：http://hz.0kj1m.cn/gtfdzunkfv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinqigufen.top/gtumovohji.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yueranfly.top/gtzjdeyzcv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.9152youxi.cn/gtlpjshclb.html

TS:   // 手写 Map<string, number>
来源：http://hz.ydzc1.top/gtfugrsexp.html

Java: // 手写 HashMap
来源：http://hz.meibo888.top/gtafyfrzpn.html

Go:   // 手写 map[int]int
来源：http://hz.chenjidiqi.icu/gtnxcsgedy.html

Ruby: // 手写 Hash
来源：http://hz.gotoacloud.top/gtlmltshmk.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhoulong.xyz/gtrzgpryzv.html

[N08] 生成全排列
来源：http://hz.yj202588.top/gtrbtdikut.html

Py:   itertools.permutations(arr)
来源：http://hz.tian-w.cn/gtmvciebvz.html

PHP:  // 手写递归交换
来源：http://hz.snrcjt.cn/gtiprmtwsi.html

JS:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtbiphlyla.html

TS:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gthuzcknfs.html

Java: // 手写回溯递归
来源：http://hz.yuxming.cn/gtlvaqedxm.html

Go:   // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtfbfqpjiq.html

Ruby: arr.permutation.to_a
来源：http://hz.zhixingplan.top/gtrtwjoetg.html

C#:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtxpohlgns.html

[N09] 栈与队列
来源：http://hz.zdqjudy.top/gtpuvealpe.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.daria6918.cn/gttjmaocrw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.wangshuangyany.cn/gteixkhlyb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhiwuduotai.top/gtuufohnuk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shangyingyoupin.top/gtmgzwgufz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zycfv.cn/gtiaifjspo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yvedp.cn/gthbgppakm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ywan-chungtsiang.top/gtuxggkpkm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xylfe.cn/gtysavmjam.html

[N10] 链表节点定义
来源：http://hz.redwolf501.top/gtuyailjsp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cqqwz.cn/gtsmzemoql.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.fzhhl.top/gtmkpvlysh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.fzhhl.top/gtvnhmmvnd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.wangdashe.top/gtgxjoeqeh.html

Java: class Node { int v; Node next; }
来源：http://hz.cqqwz.cn/gthakauocx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.pycfn.com/gtxaerzmye.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ivvv.top/gtlaarjxsq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.quarkkingdee.top/gtnmyalffx.html

[N11] 二叉树中序遍历
来源：http://hz.ybcxt.top/gtxvxadhwt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xziqi.cn/gtbfslhand.html

PHP:  // 手写递归函数
来源：http://hz.zycfv.cn/gtrdytawha.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hysaishi.cn/gtbdnetqfx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jiagoushi.top/gtcepfeceh.html

Java: // 手写递归
来源：http://hz.zhiwuduotai.top/gtldaebuuv.html

Go:   // 手写递归
来源：http://hz.hfpthk.cn/gtwhftxfbl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.smart0.xyz/gthebynvrx.html

C#:   // 手写递归
来源：http://hz.iojbl.cn/gtvztzyyqw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.wangdashe.top/gtphvidgfv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.feifeiyinyue.top/gtxhwdopiq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yj20258.top/gtwjeqdbfu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xinyue.icu/gtwhkdjirt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yvedp.cn/gtczqgillp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gtlttubyjb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.andypj.xyz/gtxwtumfin.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yongpay.top/gtooevespd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cucudq.cn/gtjcicekal.html

================================================================================
来源：http://hz.sxryk.cn/gtchykwtwv.html

O. 并发与异步
来源：http://hz.yongpay.top/gtzjqzcjcw.html

================================================================================
来源：http://hz.zhixingplan.top/gtagmoxsnz.html

[O01] 启动一个线程
来源：http://hz.yongpay.top/gtnpxdzmwk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gzhubu.top/gtgsncztvo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.smart0.xyz/gtnczxfudv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.9152youxi.cn/gthmqvgyxg.html

TS:   // 同 JS
来源：http://hz.feifeiyinyue.top/gtgstwnbtr.html

Java: new Thread(() -> f()).start()
来源：http://hz.sufxvd.cn/gtzsnzyjre.html

Go:   go f()
来源：http://hz.zdqjudy.top/gtgicjmgwn.html

Ruby: Thread.new { f }
来源：http://hz.yuxming.cn/gtlkqogsze.html

C#:   Task.Run(() => F());
来源：http://hz.redwolf501.top/gtxpcpuusn.html

[O02] 使用线程池
来源：http://hz.redwolf501.top/gtflvgrtyl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hysaishi.cn/gtqxughajk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jianghu66.top/gtohftpeti.html

JS:   // worker_threads 线程池
来源：http://hz.jinqigufen.top/gtfbznrcwc.html

TS:   // worker_threads 线程池
来源：http://hz.316326.xyz/gtowxbsqau.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hywenlv.cn/gtwpoqooxk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zdqjudy.top/gtfjjcgzzv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ivvv.top/gtwbmykjky.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ydjk.org.cn/gtumeogukj.html

[O03] 加锁保护共享数据
来源：http://hz.shuidangran.top/gtdtixvlsx.html

Py:   with lock: shared += 1
来源：http://hz.feifeiyinyue.top/gtlbwffnxz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.chenzaomai.com/gtmxvidohn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.daxiang520.top/gtzcizzzwf.html

TS:   // 同 JS
来源：http://hz.bjfxy.top/gtmelupamb.html

Java: synchronized (this) { shared++; }
来源：http://hz.c1oappe.top/gtkitbizsx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jqgufenzy.top/gtjhsayfiv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yj202588.top/gthzkkiiym.html

C#:   lock (gate) { shared++; }
来源：http://hz.yanxiufei.cn/gtjpmvsrkl.html

[O04] 定义异步函数并等待
来源：http://hz.tanke756.top/gtphbcxedc.html

Py:   async def f():⏎    await g()
来源：http://hz.shzxlz.cn/gtekqhhbfp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinghuilouyu.cn/gtzifytehe.html

JS:   async function f() { await g(); }
来源：http://hz.yuanzhike.top/gtyandjuho.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xinyue.icu/gtytyvvunq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.smart0.xyz/gtzqgxvfbi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shzxlz.cn/gtqnetensn.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.tianlin.xyz/gtlyajwzdk.html

C#:   async Task F() { await G(); }
来源：http://hz.meibo888.top/gtcojzipfa.html

[O05] 并发执行并等待全部完成
来源：http://hz.cucudq.cn/gtowuabnpm.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jyoumei.cn/gtsdgtdelk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.nanxuanxn.top/gtfhjmvjvg.html

JS:   await Promise.all(tasks)
来源：http://hz.zdqjudy.top/gtsrctgmsx.html

TS:   await Promise.all(tasks)
来源：http://hz.jianghu66.top/gttquqjqfe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cheryme.top/gtcmvzbcsw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jinghuilouyu.cn/gtayrjgfjv.html

Ruby: threads.map(&:join)
来源：http://hz.svipenyu.cn/gttoivcoba.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.wangdashe.top/gtmsgwpwdj.html

[O06] 使用进程池
来源：http://hz.daria6918.cn/gtyszoczni.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.sufxvd.cn/gtjnojmdgk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hfpthk.cn/gtjmgxjgos.html

JS:   // child_process / cluster 模块
来源：http://hz.ivvv.top/gtpwfjmatr.html

TS:   // child_process / cluster 模块
来源：http://hz.bjfxy.top/gtbrewtcil.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhengqikj.top/gtvjmsurjk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nanxinkj.top/gtgsdsgybs.html

Ruby: // fork 块
来源：http://hz.andypj.xyz/gtrnxwklhj.html

C#:   Parallel.For
来源：http://hz.jiagoushi.top/gtjddguhux.html

================================================================================
来源：http://hz.mhx1999.top/gtzyelrbux.html

P. 常用工具函数
来源：http://hz.daxiang520.top/gtuenotfvm.html

================================================================================
来源：http://hz.bjfxy.top/gtgdtpzabr.html

[P01] 生成 UUID
来源：http://hz.jlsjyb.cn/gtveysevna.html

Py:   str(uuid.uuid4())
来源：http://hz.mhx1999.top/gtxdqlnmgq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ppjwa.cn/gtevnfjooq.html

JS:   crypto.randomUUID()
来源：http://hz.cdnleiting.top/gtgtpoxqxn.html

TS:   crypto.randomUUID()
来源：http://hz.bjfxy.top/gtrbiwfgpc.html

Java: UUID.randomUUID().toString()
来源：http://hz.dianchejie.cn/gtsfclrand.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ywan-chungtsiang.top/gtoaudyeog.html

Ruby: SecureRandom.uuid
来源：http://hz.jinyuanbaomall.cn/gtzlnmcyrn.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sweek.top/gtpdwpcgfw.html

[P02] MD5 / SHA256 摘要
来源：http://hz.feifeiyinyue.top/gtjgybzqqs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shanyushiyangkeji.top/gtisjajumk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.wangdashe.top/gtlarlykvk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hnqzz.top/gtxunkbksx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jlsjyb.cn/gtzjatziqe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhijiandao.cn/gtilibkvae.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.meibo888.top/gtxwbzngna.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.nanxuanxn.top/gtehvhdcqq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.nanxinkj.top/gtnqxeakik.html

[P03] 生成短随机字符串
来源：http://hz.xingfuxueyuan.xyz/gtdhhlmdsk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.fengsongda.top/gtamwxbaqj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jinghuilouyu.cn/gtixbvoxvc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.smart0.xyz/gtkrnvwvox.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj202588.top/gtppmnxcbr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hywenlv.cn/gtoasgixsh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ybcxt.top/gtaqziqqkr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yanxiufei.cn/gtolgkjkse.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xuanzx.com/gtipeonusk.html

[P04] 求长度
来源：http://hz.jinqigfzy.top/gtnwwglnpz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.bjfxy.top/gtcltdjhbi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yanxiufei.cn/gtkhykvohj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.birdmap.top/gtnbygjyby.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dashuyun.cn/gtiggisinw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sufxvd.cn/gtchgylnsd.html

Go:   len(arr);  len(m)
来源：http://hz.jqgufenzy.top/gtaxvxtray.html

Ruby: x.length;  x.size
来源：http://hz.svipenyu.cn/gtpoawtqmq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.smart0.xyz/gtzfsuxsdg.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sufxvd.cn/gtvnvbkrmq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.pycfn.com/gthrgglfyb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhongyouzk.top/gtkpelqcmk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.daria6918.cn/gtrplogckt.html


<!-- 参考信息 -->