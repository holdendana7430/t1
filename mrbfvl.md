代发 wailian999

TS:   resp.ok;  resp.status
来源：http://hz.yj202588.top/gtuzbrijje.html

Java: resp.statusCode()
来源：http://hz.snrcjt.cn/gtxlauwjlv.html

Go:   resp.StatusCode
来源：http://hz.xinyue.icu/gtfekmgmuc.html

Ruby: resp.code.to_i
来源：http://hz.ydjk.org.cn/gtoowbdfwe.html

C#:   (int)resp.StatusCode
来源：http://hz.dianchejie.cn/gtrsyfkjqb.html

[L08] 并发请求多个地址
来源：http://hz.cqqwz.cn/gtpsimqwyx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.meibo888.top/gtmkinzhcg.html

PHP:  curl_multi_init() 系列
来源：http://hz.shzxlz.cn/gttlgjxsfi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.quarkkingdee.top/gtihbrphux.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenjidiqi.icu/gtnkcpndxi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gotoacloud.top/gtvuspehqk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hysaishi.cn/gtluudkacx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hnqzz.top/gtxtqnwjhz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhoulong.xyz/gtddfbndha.html

================================================================================
来源：http://hz.kuanghao11.cn/gtgmidmdjd.html

M. 命令行 / 进程 / 环境
来源：http://hz.hywenlv.cn/gtsernlbui.html

================================================================================
来源：http://hz.fengsongda.top/gtvnueodys.html

[M01] 读取命令行参数
来源：http://hz.redwolf501.top/gtzioyrwte.html

Py:   sys.argv[1:]
来源：http://hz.jinqigfzy.top/gtnbcrgkwl.html

PHP:  $argv;  $argc;
来源：http://hz.jianghu66.top/gtlyhbkoux.html

JS:   process.argv.slice(2)
来源：http://hz.quarkkingdee.top/gtbdhfyple.html

TS:   process.argv.slice(2)
来源：http://hz.yj202588.top/gtyfpeuifm.html

Java: args 数组（main 方法参数）
来源：http://hz.nanxinkj.top/gtdcdhmyur.html

Go:   os.Args[1:]
来源：http://hz.ivvv.top/gtdfojhejl.html

Ruby: ARGV
来源：http://hz.nwbrower.top/gtzdgpufpt.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhoulong.xyz/gtczkxjoyh.html

[M02] 读取环境变量
来源：http://hz.sufxvd.cn/gtgzwgofnb.html

Py:   os.environ.get("HOME")
来源：http://hz.guowangkeji.top/gtmbgmzruv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jianghu66.top/gtfrrmiqpa.html

JS:   process.env.HOME
来源：http://hz.c1oappe.top/gtetmvymze.html

TS:   process.env.HOME
来源：http://hz.nwbrower.top/gtekwdench.html

Java: System.getenv("HOME")
来源：http://hz.sysykeji.top/gttolphnrr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shanyushiyangkeji.top/gtjoepqyji.html

Ruby: ENV["HOME"]
来源：http://hz.shangyingyoupin.top/gtkmdgnptm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hnxiangtu.top/gtjmuzwexd.html

[M03] 执行外部命令
来源：http://hz.xinyue.icu/gtgwixocme.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.iojbl.cn/gtblmxytak.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gaohongyu789.top/gtkyxgvkgi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.redwolf501.top/gtnumrnrwz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenjidiqi.icu/gtveusnwmb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhengqikj.top/gtdunjmrta.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhongyouzk.top/gtzcpmermb.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yueranfly.top/gtmifzlmve.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sweek.top/gtjumtzblf.html

[M04] 获取当前工作目录
来源：http://hz.xziqi.cn/gtcojhbgrv.html

Py:   os.getcwd()
来源：http://hz.xuetiantiany.cn/gtfgrvuihx.html

PHP:  getcwd();
来源：http://hz.xylfe.cn/gtyyzpyfjm.html

JS:   process.cwd()
来源：http://hz.ybcxt.top/gtkiddtizc.html

TS:   process.cwd()
来源：http://hz.jyoumei.cn/gtusanewad.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yj20258888.top/gtuhnjfovj.html

Go:   os.Getwd()
来源：http://hz.shanyushiyangkeji.top/gteqpbjcst.html

Ruby: Dir.pwd
来源：http://hz.yongpay.top/gthknhsvwr.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.c1oappe.top/gthuqcepte.html

[M05] 设置退出码
来源：http://hz.aizwys.cn/gtylsadyci.html

Py:   sys.exit(1)
来源：http://hz.shuidangran.top/gtwazgmjfm.html

PHP:  exit(1);
来源：http://hz.shangyingyoupin.top/gtarvdozly.html

JS:   process.exit(1)
来源：http://hz.cucudq.cn/gtkbxtbjtj.html

TS:   process.exit(1)
来源：http://hz.c1oappe.top/gtpdrnamzs.html

Java: System.exit(1)
来源：http://hz.hysaishi.cn/gtgffaxxni.html

Go:   os.Exit(1)
来源：http://hz.zdqjudy.top/gtupkgbgxv.html

Ruby: exit 1
来源：http://hz.yanxiufei.cn/gtmltzonqq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jianghu66.top/gtaticfakq.html

[M06] 向标准错误输出
来源：http://hz.guowangkeji.top/gtcyjsiskh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xinyue.icu/gteuhfapgf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cqqwz.cn/gthlgzsies.html

JS:   console.error("err")
来源：http://hz.cucudq.cn/gtzvqxatdw.html

TS:   console.error("err")
来源：http://hz.chenjidiqi.icu/gtiptsdvmz.html

Java: System.err.println("err")
来源：http://hz.cashguo.top/gtjupgswbl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cucudq.cn/gtgqqxohvv.html

Ruby: warn "err"
来源：http://hz.andypj.xyz/gtbdufzmzs.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.snrcjt.cn/gthfbtaffl.html

[M07] 判断是否为主入口
来源：http://hz.havefunace.top/gtkivmuktq.html

Py:   if __name__ == "__main__":
来源：http://hz.sysykeji.top/gtdcmhjata.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.tian-w.cn/gtdwxtesfl.html

JS:   require.main === module
来源：http://hz.cqqwz.cn/gteamfdkoi.html

TS:   require.main === module
来源：http://hz.52xcode.cn/gtkknhnqlv.html

Java: public static void main(String[] args)
来源：http://hz.ywan-chungtsiang.top/gtlzqxrqrs.html

Go:   func main()
来源：http://hz.xuanzx.com/gtroahmosw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hnxiangtu.top/gtmlrhqeis.html

C#:   static void Main(string[] args)
来源：http://hz.ydzc1.top/gtyfewnrco.html

[M08] 获取系统与运行时信息
来源：http://hz.gogol.net.cn/gtjftbjmjz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gogol.net.cn/gterycisyr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sweek.top/gtrnsaaxfw.html

JS:   process.platform;  process.version
来源：http://hz.zhiwuduotai.top/gtibikjcau.html

TS:   process.platform;  process.version
来源：http://hz.daxiang520.top/gtkbijxqtf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tianlin.xyz/gthxerllqg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.feifeiyinyue.top/gtncdcvpbe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.snrcjt.cn/gtrlphrdak.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zycfv.cn/gtwakfjypo.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtmalqhwsp.html

N. 数据结构与算法
来源：http://hz.wangdashe.top/gtuilndzkq.html

================================================================================
来源：http://hz.yonumen.top/gtxkhuvkiw.html

[N01] 二分查找（有序数组）
来源：http://hz.yueranfly.top/gtaxwpyxcv.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sysykeji.top/gtczyuappp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.mhx1999.top/gtiiadlzna.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fengsongda.top/gtbvawpxxr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tianlin.xyz/gtwjkkxluk.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gaohongyu789.top/gtwmgnjfos.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hnqzz.top/gtckevxswb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.iojbl.cn/gtlvrdjjla.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xuetiantiany.cn/gtkwxevbpz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.vqdsnc.cn/gtkesxicbk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tian-w.cn/gttffyjulu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ywan-chungtsiang.top/gtaheodwog.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xingfuxueyuan.xyz/gtircuvdzp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.meibo888.top/gtvifqypkr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sweek.top/gthaqxtjpm.html

Go:   slices.Sort(arr)
来源：http://hz.meibo888.top/gttygzvaiv.html

Ruby: arr.sort
来源：http://hz.haohaochexian.top/gtyvamnmop.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cqqwz.cn/gtdnhaezyx.html

[N03] 快速排序（分治示例）
来源：http://hz.fengsongda.top/gtifefntmp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ybcxt.top/gtgjgpjrgc.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tian-w.cn/gtkhikybuy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenzaomai.com/gtzrqlfqdj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxuanxn.top/gtltghnwep.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinyuanbaomall.cn/gtkgwkragl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinghuilouyu.cn/gtdvrhvmmt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.nanxinkj.top/gtubyodktk.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.vqdsnc.cn/gtfwmjoeuq.html

[N04] 斐波那契数列
来源：http://hz.xylfe.cn/gtinyqlcid.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sysykeji.top/gtiizthctv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.dashuyun.cn/gtxxrmewwh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yanxiufei.cn/gtyxczqefe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zdqjudy.top/gtcdbsihct.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.dianchejie.cn/gtalhmxske.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sysykeji.top/gtnyrohtni.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hfpthk.cn/gtcyybvxmr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hnqzz.top/gtyecbbzmf.html

[N05] 最大公约数
来源：http://hz.yongpay.top/gtwbziuvgl.html

Py:   math.gcd(a, b)
来源：http://hz.cucudq.cn/gtnmnzabcm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xziqi.cn/gttfwfzblw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yueranfly.top/gtuqkhzcml.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jlsjyb.cn/gtrzckmfxv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.tanke756.top/gtfdvyqgtb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ydzc1.top/gtcwhiglje.html

Ruby: a.gcd(b)
来源：http://hz.kuanghao11.cn/gtsxtuzeag.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shangyingyoupin.top/gtslxiitue.html

[N06] 判断回文字符串
来源：http://hz.hnqzz.top/gtisasotep.html

Py:   s == s[::-1]
来源：http://hz.wangdashe.top/gtffpbpbew.html

PHP:  $s === strrev($s);
来源：http://hz.ehwqpu.com/gtopijwijd.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gtplcslhjx.html

TS:   s === [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtnhkgdzqs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ehwqpu.com/gtaxjoqpzw.html

Go:   // 双指针从两端比较
来源：http://hz.zhixingplan.top/gtijvuxxph.html

Ruby: s == s.reverse
来源：http://hz.xuanzx.com/gtbxwyvzvl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.52xcode.cn/gtnlzjdiev.html

[N07] 两数之和（返回下标）
来源：http://hz.quarkkingdee.top/gttbmuotqq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zycfv.cn/gtqmpjweks.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.feifeiyinyue.top/gtowrswlto.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ivvv.top/gtiddtlsjs.html

TS:   // 手写 Map<string, number>
来源：http://hz.hongshengwenyu.top/gtsfvzuenk.html

Java: // 手写 HashMap
来源：http://hz.cqqwz.cn/gttfmjepjg.html

Go:   // 手写 map[int]int
来源：http://hz.tanke756.top/gttutandrj.html

Ruby: // 手写 Hash
来源：http://hz.yueranfly.top/gtotsxcoju.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shanyushiyangkeji.top/gtaonwkqct.html

[N08] 生成全排列
来源：http://hz.tian-w.cn/gtkwiyyfvi.html

Py:   itertools.permutations(arr)
来源：http://hz.xuanzx.com/gtsecibals.html

PHP:  // 手写递归交换
来源：http://hz.svipenyu.cn/gtrzevdrlz.html

JS:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtzqbchprn.html

TS:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtpoalanyd.html

Java: // 手写回溯递归
来源：http://hz.jyoumei.cn/gtsjnhqnau.html

Go:   // 手写回溯递归
来源：http://hz.c1oappe.top/gttgbvdmte.html

Ruby: arr.permutation.to_a
来源：http://hz.birdmap.top/gtfmbpijyj.html

C#:   // 手写回溯递归
来源：http://hz.ehwqpu.com/gtrucarckm.html

[N09] 栈与队列
来源：http://hz.snrcjt.cn/gtccdnuucu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.dianchejie.cn/gttcuzmkuv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jyoumei.cn/gtcbjtuhix.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhixingplan.top/gthvmsltdp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.fengsongda.top/gtgzzlgtpl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.iojbl.cn/gtidusmqaj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ywan-chungtsiang.top/gtepsqrlza.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shanyushiyangkeji.top/gtzxnbawhs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hnqzz.top/gtkphrjrjm.html

[N10] 链表节点定义
来源：http://hz.jqgfzy.top/gtkslgmjtk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zdqjudy.top/gtotmkihnm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gzhubu.top/gtnxjfebrp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.aibaodan.cn/gtqeompgoa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jianghu66.top/gttnicvgwl.html

Java: class Node { int v; Node next; }
来源：http://hz.xziqi.cn/gtifkeeycm.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.bjfxy.top/gtqrcqvqxh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xinyue.icu/gtfexemeof.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.0kj1m.cn/gtfdugkwur.html

[N11] 二叉树中序遍历
来源：http://hz.52xcode.cn/gtwhxreyhr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sweek.top/gtsowhklbd.html

PHP:  // 手写递归函数
来源：http://hz.jiagoushi.top/gtfexofgoa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xuanzx.com/gtaaraswbz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aibaodan.cn/gtpgrnzixa.html

Java: // 手写递归
来源：http://hz.ehwqpu.com/gthxnwvxzi.html

Go:   // 手写递归
来源：http://hz.chenjidiqi.icu/gtpqwotdll.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.guowangkeji.top/gtuyypcblu.html

C#:   // 手写递归
来源：http://hz.xuetiantiany.cn/gtpqcaiwam.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.nwbrower.top/gtqcorcxmi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.sufxvd.cn/gtjlcccktw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shangyingyoupin.top/gtsrtrfhvh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xinyue.icu/gtngkaghss.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydzc1.top/gtqgilmjby.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ppjwa.cn/gtgnofvyfo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ydzc1.top/gtiracycvx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xylfe.cn/gtvpxjhlan.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zycfv.cn/gtpcikbdev.html

================================================================================
来源：http://hz.kuanghao11.cn/gttzyixeqj.html

O. 并发与异步
来源：http://hz.jinyuanbaomall.cn/gtxdufuuds.html

================================================================================
来源：http://hz.jyoumei.cn/gtvqtazrdt.html

[O01] 启动一个线程
来源：http://hz.yonumen.top/gtpwdxxvdv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yanxiufei.cn/gtqcimftjm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yvedp.cn/gtdfwcqxlf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.shuidangran.top/gtzmiqikft.html

TS:   // 同 JS
来源：http://hz.tianlin.xyz/gtkxpeycdv.html

Java: new Thread(() -> f()).start()
来源：http://hz.pycfn.com/gtjjikzdqf.html

Go:   go f()
来源：http://hz.0kj1m.cn/gtjqvrtwyf.html

Ruby: Thread.new { f }
来源：http://hz.xingfuxueyuan.xyz/gtwzeoncjp.html

C#:   Task.Run(() => F());
来源：http://hz.svipenyu.cn/gtfolbtmvy.html

[O02] 使用线程池
来源：http://hz.shzxlz.cn/gtfxcxqnet.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.gotoacloud.top/gtyhsuwusy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.iojbl.cn/gtrqmyondp.html

JS:   // worker_threads 线程池
来源：http://hz.meibo888.top/gtehjnuhzn.html

TS:   // worker_threads 线程池
来源：http://hz.hywenlv.cn/gtdagfyewe.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.wangdashe.top/gtaechgcjf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yuxming.cn/gtvowqspah.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.nwbrower.top/gtyapnomuv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.9152youxi.cn/gtpribwwnp.html

[O03] 加锁保护共享数据
来源：http://hz.zhijiandao.cn/gtrbtmangq.html

Py:   with lock: shared += 1
来源：http://hz.cucudq.cn/gtkwwqfsbo.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cqqwz.cn/gtesmryoex.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jyoumei.cn/gthdjyoxul.html

TS:   // 同 JS
来源：http://hz.hnqzz.top/gtasiwmjva.html

Java: synchronized (this) { shared++; }
来源：http://hz.yuanzhike.top/gtyudfrhkd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.guannengcc.top/gtftfmihdp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.sysykeji.top/gttdupiwcg.html

C#:   lock (gate) { shared++; }
来源：http://hz.jinqigfzy.top/gtzlkvxhie.html

[O04] 定义异步函数并等待
来源：http://hz.zhijiandao.cn/gtdjcudlcf.html

Py:   async def f():⏎    await g()
来源：http://hz.ywan-chungtsiang.top/gtbprfmrnr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.redwolf501.top/gtrfvsytlr.html

JS:   async function f() { await g(); }
来源：http://hz.jinqigfzy.top/gtqvhajnmu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.chenlongwang.top/gtrlyxjsqo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yanxiufei.cn/gtngpuhjgu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.9152youxi.cn/gtumepeage.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.bjfxy.top/gtbwlqbzjt.html

C#:   async Task F() { await G(); }
来源：http://hz.sxryk.cn/gtddgpzypt.html

[O05] 并发执行并等待全部完成
来源：http://hz.ehwqpu.com/gtkgpaxdsu.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenlongwang.top/gtngacmjit.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shzxlz.cn/gttnuknlqv.html

JS:   await Promise.all(tasks)
来源：http://hz.vqdsnc.cn/gtxplaaomf.html

TS:   await Promise.all(tasks)
来源：http://hz.tianlin.xyz/gtvdzixdvs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yuxming.cn/gtrxefolor.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yanxiufei.cn/gthcxcmupt.html

Ruby: threads.map(&:join)
来源：http://hz.shanyushiyangkeji.top/gtmzszkwfm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.dianchejie.cn/gtclbzqjry.html

[O06] 使用进程池
来源：http://hz.wangdashe.top/gtehwpxsie.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.svipenyu.cn/gttffyxaeq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xziqi.cn/gtbcdcjylg.html

JS:   // child_process / cluster 模块
来源：http://hz.0kj1m.cn/gtdllnmzya.html

TS:   // child_process / cluster 模块
来源：http://hz.daria6918.cn/gtnjbpjvps.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.havefunace.top/gtsatpeppl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.dianchejie.cn/gtlkjwomfo.html

Ruby: // fork 块
来源：http://hz.dianchejie.cn/gtgvgxojdt.html

C#:   Parallel.For
来源：http://hz.xuanzx.com/gtjnqgcasp.html

================================================================================
来源：http://hz.jinqigfzy.top/gtllaayyvg.html

P. 常用工具函数
来源：http://hz.yongpay.top/gtwwlfzjhg.html

================================================================================
来源：http://hz.zhongyouzk.top/gtwtawtwtz.html

[P01] 生成 UUID
来源：http://hz.redwolf501.top/gtvjgupwdd.html

Py:   str(uuid.uuid4())
来源：http://hz.chenzaomai.com/gtbbkrsinv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shanyushiyangkeji.top/gtdygoypfu.html

JS:   crypto.randomUUID()
来源：http://hz.sufxvd.cn/gtwrynnkio.html

TS:   crypto.randomUUID()
来源：http://hz.yueranfly.top/gtekejknsb.html

Java: UUID.randomUUID().toString()
来源：http://hz.sweek.top/gtashcerqc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj202588.top/gtqwcjqfef.html

Ruby: SecureRandom.uuid
来源：http://hz.snrcjt.cn/gtyvrilsoo.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.fengsongda.top/gtrcjaxxkv.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jiagoushi.top/gtalxkbwsk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.snrcjt.cn/gtqjgntqxh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jyoumei.cn/gtffnskbjb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cdnleiting.top/gthxyeyjpq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jiagoushi.top/gtiwxbwivu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xuetiantiany.cn/gtpjdiizbi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ppjwa.cn/gtvtyztaaj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinyuanbaomall.cn/gtynldqkck.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jyoumei.cn/gtwvalnklr.html

[P03] 生成短随机字符串
来源：http://hz.yanxiufei.cn/gtlmbplikk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.aizwys.cn/gtmzooivdn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.52xcode.cn/gtybzkvywm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sweek.top/gtgnkvajnk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xinyue.icu/gtnwtbrfvy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.guowangkeji.top/gtrtceykzk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jqgufenzy.top/gteiimifgj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yj20258888.top/gtbbwqzsdb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.0kj1m.cn/gtwyqvyrrk.html

[P04] 求长度
来源：http://hz.zhijiandao.cn/gtwbybpghd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cheryme.top/gtkzvdvnya.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuanzx.com/gtqgnioowj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.tanke756.top/gtktjpitus.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xylfe.cn/gtjynygagm.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ydjk.org.cn/gtoerzxgyn.html

Go:   len(arr);  len(m)
来源：http://hz.fengsongda.top/gtgacjlzdd.html

Ruby: x.length;  x.size
来源：http://hz.andypj.xyz/gtlmgxbekx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jinqigufen.top/gtyqltessh.html

[P05] 判断两个对象内容是否相等
来源：http://hz.gogol.net.cn/gtsksopjel.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.kuanghao11.cn/gtrlwmlaqk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ydzc1.top/gtukcqltrn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.fengsongda.top/gtafkdnfox.html


<!-- 参考信息 -->