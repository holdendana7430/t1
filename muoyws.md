代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jlsjyb.cn/gttdsfbelt.html

Ruby: ENV["HOME"]
来源：http://hz.cdnleiting.top/gthvcqunks.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhijiandao.cn/gturmojqgp.html

[M03] 执行外部命令
来源：http://hz.gogol.net.cn/gtydcumrxd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.sweek.top/gtivinljmh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yuanzhike.top/gtvmzsquoi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhoulong.xyz/gtpzvofint.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.aizwys.cn/gtkupqfcod.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.haohaochexian.top/gtzqxxujhm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.52xcode.cn/gtodoboqfi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.guannengcc.top/gtpsdzuieu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hnqzz.top/gtxtqulzpb.html

[M04] 获取当前工作目录
来源：http://hz.zhaomingkeji.xyz/gtdljrsynh.html

Py:   os.getcwd()
来源：http://hz.yongpay.top/gtfvyeyvpw.html

PHP:  getcwd();
来源：http://hz.chenlongwang.top/gtsnazegfy.html

JS:   process.cwd()
来源：http://hz.daxiang520.top/gtngvhhpsb.html

TS:   process.cwd()
来源：http://hz.fzhhl.top/gtcqdbkgns.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tian-w.cn/gtpkumrmen.html

Go:   os.Getwd()
来源：http://hz.shangyingyoupin.top/gtiichvhrb.html

Ruby: Dir.pwd
来源：http://hz.haohaochexian.top/gtafkattsd.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cucudq.cn/gtcgbqkhyc.html

[M05] 设置退出码
来源：http://hz.gzhubu.top/gttajjktpw.html

Py:   sys.exit(1)
来源：http://hz.jqgfzy.top/gtsasxxrkp.html

PHP:  exit(1);
来源：http://hz.nwbrower.top/gtuvpgumci.html

JS:   process.exit(1)
来源：http://hz.ehwqpu.com/gtfuofhjbd.html

TS:   process.exit(1)
来源：http://hz.chenzaomai.com/gtuyngxbmw.html

Java: System.exit(1)
来源：http://hz.jianghu66.top/gtvawikqok.html

Go:   os.Exit(1)
来源：http://hz.iojbl.cn/gtdxvqniwe.html

Ruby: exit 1
来源：http://hz.9152youxi.cn/gtkuobbppi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.smart0.xyz/gtfpbprdsv.html

[M06] 向标准错误输出
来源：http://hz.jiagoushi.top/gtpsijmxtt.html

Py:   print("err", file=sys.stderr)
来源：http://hz.feifeiyinyue.top/gtzjtmuddh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xuetiantiany.cn/gtdvlnnnlr.html

JS:   console.error("err")
来源：http://hz.jqgfzy.top/gthijxkzdn.html

TS:   console.error("err")
来源：http://hz.yj20258888.top/gtkppjuuyx.html

Java: System.err.println("err")
来源：http://hz.hywenlv.cn/gthapylfaf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jinqigufen.top/gtvrcztcck.html

Ruby: warn "err"
来源：http://hz.chenzaomai.com/gtexyhzvus.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.quarkkingdee.top/gtrsixtgqq.html

[M07] 判断是否为主入口
来源：http://hz.0kj1m.cn/gtxlwwiwng.html

Py:   if __name__ == "__main__":
来源：http://hz.snrcjt.cn/gtnmddvlgs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hammf.cn/gtyadajvnk.html

JS:   require.main === module
来源：http://hz.ehwqpu.com/gtlioqdyil.html

TS:   require.main === module
来源：http://hz.fengsongda.top/gtfafrtyrq.html

Java: public static void main(String[] args)
来源：http://hz.birdmap.top/gtlxjcdytd.html

Go:   func main()
来源：http://hz.wangdashe.top/gtmahvznyl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.dashuyun.cn/gtuburfcjr.html

C#:   static void Main(string[] args)
来源：http://hz.aizwys.cn/gtbwvgseqm.html

[M08] 获取系统与运行时信息
来源：http://hz.zdqjudy.top/gtbvczurup.html

Py:   platform.system();  platform.python_version()
来源：http://hz.tianlin.xyz/gthtpmpxhr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhixingplan.top/gtdtuhotgj.html

JS:   process.platform;  process.version
来源：http://hz.daria6918.cn/gtrbxctvyf.html

TS:   process.platform;  process.version
来源：http://hz.yanxiufei.cn/gtgdhzijpv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.chenjidiqi.icu/gtefxbkben.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.feifeiyinyue.top/gtxezbjpua.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.chenjidiqi.icu/gtoxdbwgvl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ydjk.org.cn/gtqurohdgo.html

================================================================================
来源：http://hz.sweek.top/gtqhevntso.html

N. 数据结构与算法
来源：http://hz.meibo888.top/gtxhbugatw.html

================================================================================
来源：http://hz.wangdashe.top/gtkuhmimmk.html

[N01] 二分查找（有序数组）
来源：http://hz.sxryk.cn/gtxsldhcrp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gaohongyu789.top/gttijgplmr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.meibo888.top/gtahkdyyyb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cdnleiting.top/gtwyjejnhx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangdashe.top/gtkinpuuvs.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.wangshuangyany.cn/gthxmsykfr.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenzaomai.com/gthiyowbfb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.quarkkingdee.top/gtqfnmcois.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xziqi.cn/gtfiysbyvq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jqgufenzy.top/gtisjbbkcu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.0kj1m.cn/gtmzwxbtez.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.fengsongda.top/gthssmzqjs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.andypj.xyz/gtursgcvoe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hongshengwenyu.top/gtiqvnlwry.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yj20258888.top/gtxdidiuho.html

Go:   slices.Sort(arr)
来源：http://hz.havefunace.top/gtdflkoliv.html

Ruby: arr.sort
来源：http://hz.shuidangran.top/gtntdjdzrt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jqgufenzy.top/gtafnekhkl.html

[N03] 快速排序（分治示例）
来源：http://hz.nanxuanxn.top/gtduenkveu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.52xcode.cn/gtvezwmgwt.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sxryk.cn/gtvwoyyqyz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shzxlz.cn/gthdmfboxp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuxming.cn/gtkomdmnxc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.dianchejie.cn/gtswntfomu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhixingplan.top/gtymbapufa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.smart0.xyz/gtnkdvvxld.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tianlin.xyz/gtcawxctiu.html

[N04] 斐波那契数列
来源：http://hz.smart0.xyz/gttdkfyssr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yangfankeji.com/gtqungzewv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.mhx1999.top/gtbbbzenlq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pycfn.com/gtpelssknu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hysaishi.cn/gtuaahtnnm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jyoumei.cn/gtogknidsr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cdnleiting.top/gtmknysboz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.birdmap.top/gtsqtabnzu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.pycfn.com/gtytayqjfy.html

[N05] 最大公约数
来源：http://hz.xuanzx.com/gttmyulkbp.html

Py:   math.gcd(a, b)
来源：http://hz.hammf.cn/gtmzlpxdex.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.haohaochexian.top/gtyontmxai.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.smart0.xyz/gtnyzylgbo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xuanzx.com/gtjvydehae.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhixingplan.top/gtcjtwbksq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.snrcjt.cn/gtidhhtyzp.html

Ruby: a.gcd(b)
来源：http://hz.yueranfly.top/gtjsruxnbq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ppjwa.cn/gtagpcirvn.html

[N06] 判断回文字符串
来源：http://hz.tian-w.cn/gtfwmmnawt.html

Py:   s == s[::-1]
来源：http://hz.ehwqpu.com/gtdapdfuai.html

PHP:  $s === strrev($s);
来源：http://hz.yj20258.top/gthimdjrxl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtoofewgaq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtkqnjgjrw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.pycfn.com/gtlwpcbfcu.html

Go:   // 双指针从两端比较
来源：http://hz.0kj1m.cn/gtepjswkns.html

Ruby: s == s.reverse
来源：http://hz.sysykeji.top/gtsvlyplvw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangtech.top/gtdncytuba.html

[N07] 两数之和（返回下标）
来源：http://hz.ydzc1.top/gtlbwpzjsi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.birdmap.top/gtklyrbqny.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cucudq.cn/gtshwzarsx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.daxiang520.top/gtmgcqnwuo.html

TS:   // 手写 Map<string, number>
来源：http://hz.xuetiantiany.cn/gtnwmtaghe.html

Java: // 手写 HashMap
来源：http://hz.andypj.xyz/gtxjhsgjcz.html

Go:   // 手写 map[int]int
来源：http://hz.jqgfzy.top/gtvkptotqr.html

Ruby: // 手写 Hash
来源：http://hz.yj20258.top/gtnlryesru.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinyuanbaomall.cn/gtolxyfbln.html

[N08] 生成全排列
来源：http://hz.yonumen.top/gtiqbctqks.html

Py:   itertools.permutations(arr)
来源：http://hz.jianghu66.top/gtowbszcnv.html

PHP:  // 手写递归交换
来源：http://hz.dashuyun.cn/gtbhublwsq.html

JS:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtwipadfqu.html

TS:   // 手写回溯递归
来源：http://hz.52xcode.cn/gtrlkuulvv.html

Java: // 手写回溯递归
来源：http://hz.wangdashe.top/gtcfrepbbx.html

Go:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtoouycfqn.html

Ruby: arr.permutation.to_a
来源：http://hz.kuanghao11.cn/gtboheiyhq.html

C#:   // 手写回溯递归
来源：http://hz.quarkkingdee.top/gtnfczcgbg.html

[N09] 栈与队列
来源：http://hz.zhiwuduotai.top/gtpihizaoy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shanyushiyangtech.top/gtcdmjvxjm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhixingplan.top/gtloytvstq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cheryme.top/gtfqgwdrkp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhoulong.xyz/gtontzjzho.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.nanxuanxn.top/gtrxtystpq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hnxiangtu.top/gttbgteabk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sxryk.cn/gtuabnpkus.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.aizwys.cn/gtwrtrpage.html

[N10] 链表节点定义
来源：http://hz.fzhhl.top/gtyddmbuaj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hysaishi.cn/gtuorhicpa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.fengsongda.top/gtmpycgkfq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ydjk.org.cn/gtvzgwdqvb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cdnleiting.top/gtgxxzudza.html

Java: class Node { int v; Node next; }
来源：http://hz.shuidangran.top/gtbufybwub.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinqigfzy.top/gtetzlmzcs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.havefunace.top/gtvplpfdco.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.haohaochexian.top/gthgvpwiju.html

[N11] 二叉树中序遍历
来源：http://hz.jlsjyb.cn/gtirluewpw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.dashuyun.cn/gtmyhcxxkj.html

PHP:  // 手写递归函数
来源：http://hz.xylfe.cn/gtyozlsxxe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinghuilouyu.cn/gtmemzzbvc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shangyingyoupin.top/gtskayzkez.html

Java: // 手写递归
来源：http://hz.zhiwuduotai.top/gtqledtvhr.html

Go:   // 手写递归
来源：http://hz.nanxuanxn.top/gtinkzmxpv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jlsjyb.cn/gtlacqosou.html

C#:   // 手写递归
来源：http://hz.haohaochexian.top/gtlnbsfwsc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yuxming.cn/gtymwqxbao.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhiwuduotai.top/gtboxhllpc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.nwbrower.top/gtooshphob.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.smart0.xyz/gtqrifdzni.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinyuanbaomall.cn/gtocsaovpv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.haohaochexian.top/gtwemnglbt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yongpay.top/gththzrzim.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jyoumei.cn/gttopuaiwj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinyuanbaomall.cn/gtkfqcrpll.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtcvyjijdf.html

O. 并发与异步
来源：http://hz.jinqigfzy.top/gtnimqtpiz.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtfkkqvlkh.html

[O01] 启动一个线程
来源：http://hz.xuanzx.com/gtrfupfrel.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xingfuxueyuan.xyz/gtsvzzmrna.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cqqwz.cn/gtrbnarktx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hongshengwenyu.top/gttnnzenno.html

TS:   // 同 JS
来源：http://hz.feifeiyinyue.top/gtielungfr.html

Java: new Thread(() -> f()).start()
来源：http://hz.hfpthk.cn/gtftvodopk.html

Go:   go f()
来源：http://hz.chenlongwang.top/gtzbqowmsv.html

Ruby: Thread.new { f }
来源：http://hz.ehwqpu.com/gtjzcyrzyi.html

C#:   Task.Run(() => F());
来源：http://hz.pengpengdd.cyou/gtwoovwyqo.html

[O02] 使用线程池
来源：http://hz.tanke756.top/gtnxaaweno.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.feifeiyinyue.top/gtkgusgpyk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shangyingyoupin.top/gtpjafbzpp.html

JS:   // worker_threads 线程池
来源：http://hz.ppjwa.cn/gtmipzokfc.html

TS:   // worker_threads 线程池
来源：http://hz.c1oappe.top/gtfrmvhicy.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinghuilouyu.cn/gtqucjecwi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.havefunace.top/gthgqenvba.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.wangdashe.top/gtrzanktyp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.chenlongwang.top/gtrzzpwnkw.html

[O03] 加锁保护共享数据
来源：http://hz.snrcjt.cn/gtzlthdgns.html

Py:   with lock: shared += 1
来源：http://hz.hammf.cn/gtvrraiqod.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.c1oappe.top/gtnruspffj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.316326.xyz/gtqcbixrou.html

TS:   // 同 JS
来源：http://hz.ydzc1.top/gtwyzugwol.html

Java: synchronized (this) { shared++; }
来源：http://hz.guowangkeji.top/gtaxzjzyap.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yueranfly.top/gtwubohqif.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhijiandao.cn/gtbwwktrar.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhongyouzk.top/gtqbsnepjp.html

[O04] 定义异步函数并等待
来源：http://hz.xylfe.cn/gtwsmokomw.html

Py:   async def f():⏎    await g()
来源：http://hz.hywenlv.cn/gtvmbzppli.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.9152youxi.cn/gtcyubggyn.html

JS:   async function f() { await g(); }
来源：http://hz.yanxiufei.cn/gtdxdghkmi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.316326.xyz/gtklmulcfk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhixingplan.top/gtbpwkcnzn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hywenlv.cn/gtgfgluocf.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cashguo.top/gtukdcuxmu.html

C#:   async Task F() { await G(); }
来源：http://hz.snrcjt.cn/gtobnqzwxi.html

[O05] 并发执行并等待全部完成
来源：http://hz.shuidangran.top/gtbwyutvso.html

Py:   asyncio.gather(*tasks)
来源：http://hz.sufxvd.cn/gtcefvuxcj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yanxiufei.cn/gtzqnikygs.html

JS:   await Promise.all(tasks)
来源：http://hz.vqdsnc.cn/gteggbzueb.html

TS:   await Promise.all(tasks)
来源：http://hz.hfpthk.cn/gtshrmjmth.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cheryme.top/gtieredqpn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.birdmap.top/gtktpbpptl.html

Ruby: threads.map(&:join)
来源：http://hz.kuanghao11.cn/gthfscdlfk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shuidangran.top/gttjhgznyf.html

[O06] 使用进程池
来源：http://hz.xuanzx.com/gtvqcgdwtq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hnxiangtu.top/gtdwtcwayp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhongyouzk.top/gtqbgvrtso.html

JS:   // child_process / cluster 模块
来源：http://hz.xinyue.icu/gtaaesldwz.html

TS:   // child_process / cluster 模块
来源：http://hz.xuetiantiany.cn/gtvmswgjnr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cdnleiting.top/gtgxdygseo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shzxlz.cn/gtxfexbrqo.html

Ruby: // fork 块
来源：http://hz.yonumen.top/gtotbrmkeu.html

C#:   Parallel.For
来源：http://hz.nanxinkj.top/gtmclnoqlg.html

================================================================================
来源：http://hz.9152youxi.cn/gticglungn.html

P. 常用工具函数
来源：http://hz.shzxlz.cn/gtjtsrloyw.html

================================================================================
来源：http://hz.birdmap.top/gtczxgmncn.html

[P01] 生成 UUID
来源：http://hz.sweek.top/gtarlstldv.html

Py:   str(uuid.uuid4())
来源：http://hz.yueranfly.top/gtpdycdztm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhengqikj.top/gtovwwexul.html

JS:   crypto.randomUUID()
来源：http://hz.jianghu66.top/gtdtoibjiy.html

TS:   crypto.randomUUID()
来源：http://hz.ehwqpu.com/gtmbvstntn.html

Java: UUID.randomUUID().toString()
来源：http://hz.jqgfzy.top/gtjuiqmqfp.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yonumen.top/gtfnkacqdi.html

Ruby: SecureRandom.uuid
来源：http://hz.pycfn.com/gtnvifepus.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenlongwang.top/gthekkcvqf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.chenzaomai.com/gtdkqjcjos.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jinqigufen.top/gtpjhjjkkb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shuidangran.top/gtfadscanq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.chenlongwang.top/gtjphowifk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj20258888.top/gtjgaehyld.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhiwuduotai.top/gtpnzxvfsa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.daria6918.cn/gtxzkyvehr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.shanyushiyangkeji.top/gtgeoqzkaq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shanyushiyangkeji.top/gtybcahrax.html

[P03] 生成短随机字符串
来源：http://hz.hnxiangtu.top/gthzxbinjj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.chenlongwang.top/gtcijaqwun.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ybcxt.top/gtilspjaev.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yonumen.top/gtoxchtewd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.daria6918.cn/gtndbfbovd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.tianlin.xyz/gtlngzncgl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yueranfly.top/gtpxiaxbjt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.chenjidiqi.icu/gtuhkfrhoe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cucudq.cn/gtrnpqmybd.html

[P04] 求长度
来源：http://hz.fzhhl.top/gtnntbwtbs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.vqdsnc.cn/gtwdrpwkoz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.quarkkingdee.top/gtlionzfbz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.svipenyu.cn/gtkaiutcgy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nanxuanxn.top/gtjzromqgi.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xinyue.icu/gtvkyphftb.html

Go:   len(arr);  len(m)
来源：http://hz.shanyushiyangtech.top/gtzffxmexb.html

Ruby: x.length;  x.size
来源：http://hz.jqgufenzy.top/gtvonbghhd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yvedp.cn/gtetnyktav.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ivvv.top/gtfawjmtux.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cucudq.cn/gtwtrudwpn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shzxlz.cn/gtbyemyery.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shanyushiyangkeji.top/gtdvdeqilf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gotoacloud.top/gtjubifjuy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.kuanghao11.cn/gtidyvaivk.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hongshengwenyu.top/gtjjrqnxcc.html

Ruby: a == b
来源：http://hz.yonumen.top/gtlvapbreh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gogol.net.cn/gtetfcfuwe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jiagoushi.top/gtlddcjedz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.daxiang520.top/gtrhignsed.html

PHP:  if (empty($x)) {}
来源：http://hz.cucudq.cn/gtzxjimcch.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.guannengcc.top/gtjntkkbey.html

TS:   if (x == null) {}
来源：http://hz.yj20258888.top/gttclkfxyb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sufxvd.cn/gtbjoexgfx.html

Go:   if x == nil {}
来源：http://hz.ydzc1.top/gtevpywvuw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hnqzz.top/gtsdocirzw.html

C#:   if (x is null) {}
来源：http://hz.xziqi.cn/gtcukynmls.html

[P07] 防抖与节流
来源：http://hz.tian-w.cn/gtmhrorksz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yuxming.cn/gtigasolsi.html

PHP:  // 手写时间戳比较
来源：http://hz.tian-w.cn/gtuyycxnbr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yonumen.top/gteykzixwc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangdashe.top/gtpkvgqtjq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hongshengwenyu.top/gtxtazoxdl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jinqigfzy.top/gtxsbfzdue.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.fzhhl.top/gtjppyqnkg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.daxiang520.top/gtuxkwunzj.html

[P08] 处理浮点精度问题
来源：http://hz.guowangkeji.top/gtsszqnkmd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yuxming.cn/gtwyymasfk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.smart0.xyz/gtbxwfkdxg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhaomingkeji.xyz/gtzqtwnjgo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tianlin.xyz/gtklgpubqq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jinqigufen.top/gthmemhtyd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenlongwang.top/gtxlixvipe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xinyue.icu/gtztilzkrw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.bjfxy.top/gtyvbvxais.html


<!-- 参考信息 -->