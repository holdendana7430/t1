代发 wailian999

JS:   process.argv.slice(2)
来源：http://hz.yj20258888.top/gteiddfzcb.html

TS:   process.argv.slice(2)
来源：http://hz.havefunace.top/gtnpilmvwc.html

Java: args 数组（main 方法参数）
来源：http://hz.gotoacloud.top/gtpexqwrjm.html

Go:   os.Args[1:]
来源：http://hz.meibo888.top/gtwaftikzv.html

Ruby: ARGV
来源：http://hz.guannengcc.top/gttegslmbs.html

C#:   args 数组（Main 方法参数）
来源：http://hz.svipenyu.cn/gtnazmrlci.html

[M02] 读取环境变量
来源：http://hz.0kj1m.cn/gtmklgfblb.html

Py:   os.environ.get("HOME")
来源：http://hz.yueranfly.top/gtlggiegxw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.havefunace.top/gtwqfwrxmk.html

JS:   process.env.HOME
来源：http://hz.hammf.cn/gtnjhtckve.html

TS:   process.env.HOME
来源：http://hz.aizwys.cn/gtxurdbqsb.html

Java: System.getenv("HOME")
来源：http://hz.yj20258888.top/gtokaoulmz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinqigufen.top/gtzleeupzs.html

Ruby: ENV["HOME"]
来源：http://hz.aizwys.cn/gtkjvikfge.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cqqwz.cn/gtgvlxipcd.html

[M03] 执行外部命令
来源：http://hz.yj20258888.top/gtpridkyxx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.daria6918.cn/gtwnwkmiou.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zdqjudy.top/gtlmzsqiwa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yongpay.top/gtqutnnido.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.bjfxy.top/gtqtogzmnr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.nanxinkj.top/gtiykmikvk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yvedp.cn/gtemlyjygk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cucudq.cn/gtxfepvdqd.html

C#:   Process.Start("ls", "-l");
来源：http://hz.pycfn.com/gtosqmzneq.html

[M04] 获取当前工作目录
来源：http://hz.yongpay.top/gtpozmleak.html

Py:   os.getcwd()
来源：http://hz.zhongyouzk.top/gtbjffrptp.html

PHP:  getcwd();
来源：http://hz.tanke756.top/gtzihtsmli.html

JS:   process.cwd()
来源：http://hz.ehwqpu.com/gtsritiktd.html

TS:   process.cwd()
来源：http://hz.gogol.net.cn/gtgjwdpxdx.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhongyouzk.top/gtiecawmnh.html

Go:   os.Getwd()
来源：http://hz.gogol.net.cn/gtbgkqrrff.html

Ruby: Dir.pwd
来源：http://hz.316326.xyz/gtzutrogfu.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gotoacloud.top/gtqgxrnjil.html

[M05] 设置退出码
来源：http://hz.jlsjyb.cn/gtrchyujue.html

Py:   sys.exit(1)
来源：http://hz.chenlongwang.top/gtzqylonho.html

PHP:  exit(1);
来源：http://hz.nanxuanxn.top/gtddfawnny.html

JS:   process.exit(1)
来源：http://hz.smart0.xyz/gtexqmzara.html

TS:   process.exit(1)
来源：http://hz.daxiang520.top/gtckrkujwy.html

Java: System.exit(1)
来源：http://hz.mhx1999.top/gtwbjvlnje.html

Go:   os.Exit(1)
来源：http://hz.chenlongwang.top/gthybjzqqk.html

Ruby: exit 1
来源：http://hz.gzhubu.top/gtqtaojblf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cdnleiting.top/gttoirjakh.html

[M06] 向标准错误输出
来源：http://hz.cdnleiting.top/gtwabasyqz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.tanke756.top/gtmtcnzjsc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinyuanbaomall.cn/gtquazzjtt.html

JS:   console.error("err")
来源：http://hz.jinghuilouyu.cn/gtmlgdjbql.html

TS:   console.error("err")
来源：http://hz.jqgfzy.top/gtbxhnntns.html

Java: System.err.println("err")
来源：http://hz.gzhubu.top/gtazoyhpnb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.pengpengdd.cyou/gtscheoqcs.html

Ruby: warn "err"
来源：http://hz.jqgfzy.top/gtbrmwhnkr.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.daria6918.cn/gteamzuddn.html

[M07] 判断是否为主入口
来源：http://hz.jlsjyb.cn/gtsxpcbjot.html

Py:   if __name__ == "__main__":
来源：http://hz.ydjk.org.cn/gtbpuxnumb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hfpthk.cn/gthyymmdgh.html

JS:   require.main === module
来源：http://hz.zhaomingkeji.xyz/gthuhyeczz.html

TS:   require.main === module
来源：http://hz.yueranfly.top/gtyciyxpya.html

Java: public static void main(String[] args)
来源：http://hz.shanyushiyangtech.top/gtnozgboeb.html

Go:   func main()
来源：http://hz.ppjwa.cn/gtortrzihi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shzxlz.cn/gtkhzskyww.html

C#:   static void Main(string[] args)
来源：http://hz.cucudq.cn/gtgowjpyoo.html

[M08] 获取系统与运行时信息
来源：http://hz.zhoulong.xyz/gtdqvfoefk.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yj202588.top/gtlqfngqgg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cqqwz.cn/gtpbdmwkxk.html

JS:   process.platform;  process.version
来源：http://hz.snrcjt.cn/gtjafrabng.html

TS:   process.platform;  process.version
来源：http://hz.jqgfzy.top/gtzvxzarap.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xingfuxueyuan.xyz/gtepfpijwv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinghuilouyu.cn/gtamcgzcvb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yongpay.top/gtetxgrpig.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yvedp.cn/gtdaumjvho.html

================================================================================
来源：http://hz.xinyue.icu/gtpxpwtuac.html

N. 数据结构与算法
来源：http://hz.nanxinkj.top/gtxkwgtzow.html

================================================================================
来源：http://hz.yj202588.top/gthsfgplho.html

[N01] 二分查找（有序数组）
来源：http://hz.aizwys.cn/gtestivlmz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ydzc1.top/gtmbxjelin.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gogol.net.cn/gtkhstizzu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ppjwa.cn/gtolbjyiow.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zycfv.cn/gtduotyzsa.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.haohaochexian.top/gtsgzigjba.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.birdmap.top/gtdlqxjtfn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hywenlv.cn/gtaykzfego.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shanyushiyangtech.top/gtyybsuhlj.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.daxiang520.top/gtqnzyzciv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gotoacloud.top/gtwzcbrvpi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhengqikj.top/gtnzaybuvy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jlsjyb.cn/gtveuzykbc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sxryk.cn/gtqnpicxwj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zycfv.cn/gtqufohxsd.html

Go:   slices.Sort(arr)
来源：http://hz.ydzc1.top/gtawbwfmor.html

Ruby: arr.sort
来源：http://hz.jlsjyb.cn/gtsuagfarl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.chenlongwang.top/gtyssljdsk.html

[N03] 快速排序（分治示例）
来源：http://hz.feifeiyinyue.top/gtmeyapegw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shzxlz.cn/gtbapadloz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.redwolf501.top/gtbynxtgim.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhiwuduotai.top/gtksuateag.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dianchejie.cn/gtcqfxbaog.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj20258.top/gtgfgiioua.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jianghu66.top/gtzerlvlgc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.0kj1m.cn/gtwqwaxhdf.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.9152youxi.cn/gthniexrfd.html

[N04] 斐波那契数列
来源：http://hz.andypj.xyz/gtgzghpdyj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.daxiang520.top/gtdbpshbkw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.snrcjt.cn/gttgztbthc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sysykeji.top/gtmdoylvne.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yangfankeji.com/gtsubuffvl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.fengsongda.top/gtqnxumyay.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yuanzhike.top/gtlzoduwqk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.nanxinkj.top/gtlqdjqvuz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gotoacloud.top/gtgnynruxs.html

[N05] 最大公约数
来源：http://hz.tanke756.top/gtjwqcfrwe.html

Py:   math.gcd(a, b)
来源：http://hz.jqgfzy.top/gtbcrvcnsu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xuanzx.com/gtkccibvia.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.quarkkingdee.top/gtymmtdwpy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangdashe.top/gtxmpivljj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.svipenyu.cn/gtjzflvpej.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhaomingkeji.xyz/gtwfelwkdb.html

Ruby: a.gcd(b)
来源：http://hz.jlsjyb.cn/gtqgcexowa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gogol.net.cn/gtdduonomr.html

[N06] 判断回文字符串
来源：http://hz.sysykeji.top/gtmirmukoc.html

Py:   s == s[::-1]
来源：http://hz.sufxvd.cn/gtavnvjmhb.html

PHP:  $s === strrev($s);
来源：http://hz.jinyuanbaomall.cn/gtrwhjarim.html

JS:   s === [...s].reverse().join("")
来源：http://hz.andypj.xyz/gthosnhpmi.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ehwqpu.com/gtlqpvnxgv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.tian-w.cn/gtuviwiech.html

Go:   // 双指针从两端比较
来源：http://hz.guannengcc.top/gtkenjicof.html

Ruby: s == s.reverse
来源：http://hz.haohaochexian.top/gtifrtdwtp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.0kj1m.cn/gthmnyxmqq.html

[N07] 两数之和（返回下标）
来源：http://hz.tian-w.cn/gtgshotprb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.sweek.top/gtqwkjrjsj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sysykeji.top/gtennxihux.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.meibo888.top/gtsafxfljv.html

TS:   // 手写 Map<string, number>
来源：http://hz.shanyushiyangkeji.top/gtcmvgnele.html

Java: // 手写 HashMap
来源：http://hz.sxryk.cn/gtjhmnpcyw.html

Go:   // 手写 map[int]int
来源：http://hz.cashguo.top/gtlppqbfsv.html

Ruby: // 手写 Hash
来源：http://hz.sufxvd.cn/gtwmmyghgt.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.chenzaomai.com/gtpijmldqt.html

[N08] 生成全排列
来源：http://hz.yonumen.top/gtljpcchrb.html

Py:   itertools.permutations(arr)
来源：http://hz.9152youxi.cn/gthfoejjdx.html

PHP:  // 手写递归交换
来源：http://hz.jinqigufen.top/gtazkpibyf.html

JS:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtrjughuqr.html

TS:   // 手写回溯递归
来源：http://hz.hfpthk.cn/gtgezmtwbj.html

Java: // 手写回溯递归
来源：http://hz.xziqi.cn/gtlhfhwjdf.html

Go:   // 手写回溯递归
来源：http://hz.cashguo.top/gtfiehapnh.html

Ruby: arr.permutation.to_a
来源：http://hz.zhaomingkeji.xyz/gtmdoeqzqp.html

C#:   // 手写回溯递归
来源：http://hz.sweek.top/gtscjjljzw.html

[N09] 栈与队列
来源：http://hz.cashguo.top/gtzellhoyn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.daria6918.cn/gtpylbjsgc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.quarkkingdee.top/gtthghnfea.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hnqzz.top/gtbrpzbzkh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cashguo.top/gtxmxhushq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gaohongyu789.top/gtqgnkhanx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.vqdsnc.cn/gtkxdsdhcf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.kuanghao11.cn/gtiwhvtpmh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hfpthk.cn/gtcpclpqer.html

[N10] 链表节点定义
来源：http://hz.chenlongwang.top/gtlhgvggkv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.guannengcc.top/gttbjjzhhi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.iojbl.cn/gtpaufszhn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj202588.top/gtwiksiiom.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.316326.xyz/gttlztjrok.html

Java: class Node { int v; Node next; }
来源：http://hz.zhijiandao.cn/gthnnafpjs.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhongyouzk.top/gtogxfccmv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sufxvd.cn/gtuupljfnw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.316326.xyz/gtcbmjajzr.html

[N11] 二叉树中序遍历
来源：http://hz.xylfe.cn/gtfsbtwykz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cdnleiting.top/gtjelrojhc.html

PHP:  // 手写递归函数
来源：http://hz.fzhhl.top/gtlabnffyu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.redwolf501.top/gtyydrofqv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.c1oappe.top/gtdnizenmw.html

Java: // 手写递归
来源：http://hz.jlsjyb.cn/gttiwcgkyd.html

Go:   // 手写递归
来源：http://hz.shzxlz.cn/gteyaoldys.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ydjk.org.cn/gtqzqxjtbu.html

C#:   // 手写递归
来源：http://hz.hysaishi.cn/gtmqljusfh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ehwqpu.com/gtmoympbro.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.nwbrower.top/gtayocimkh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xingfuxueyuan.xyz/gtaqdowrwe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.feifeiyinyue.top/gtnathpbns.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jianghu66.top/gthvxlurav.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hywenlv.cn/gtnpmjvuel.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.cqqwz.cn/gtozogthjd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.iojbl.cn/gtaczmelja.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.birdmap.top/gtfcjhwdql.html

================================================================================
来源：http://hz.chenzaomai.com/gtwumfoxyv.html

O. 并发与异步
来源：http://hz.zhiwuduotai.top/gttirdkvtl.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtdmhecdte.html

[O01] 启动一个线程
来源：http://hz.sysykeji.top/gtsbiesqfd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhengqikj.top/gtuuothnor.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yanxiufei.cn/gtbiiryntk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fengsongda.top/gtbpfvoflf.html

TS:   // 同 JS
来源：http://hz.zhengqikj.top/gtjkxgvilf.html

Java: new Thread(() -> f()).start()
来源：http://hz.havefunace.top/gtddaomado.html

Go:   go f()
来源：http://hz.feifeiyinyue.top/gtszakcuwo.html

Ruby: Thread.new { f }
来源：http://hz.yanxiufei.cn/gtkvswfmpa.html

C#:   Task.Run(() => F());
来源：http://hz.hnxiangtu.top/gthqrfxtzg.html

[O02] 使用线程池
来源：http://hz.xziqi.cn/gtrfxncnio.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hfpthk.cn/gtaaagobou.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hnqzz.top/gtktyrnyfv.html

JS:   // worker_threads 线程池
来源：http://hz.cheryme.top/gtxuwcvrfk.html

TS:   // worker_threads 线程池
来源：http://hz.redwolf501.top/gtbyspolpf.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.vqdsnc.cn/gtzpialilh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.aizwys.cn/gtbvmkwuda.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.havefunace.top/gtowtzimpz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhoulong.xyz/gteymyslpx.html

[O03] 加锁保护共享数据
来源：http://hz.shangyingyoupin.top/gtjzxddlno.html

Py:   with lock: shared += 1
来源：http://hz.tanke756.top/gthiwkfkvc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.gotoacloud.top/gtbwmbhlpo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cashguo.top/gtugvbdohj.html

TS:   // 同 JS
来源：http://hz.xylfe.cn/gthdfwxtyc.html

Java: synchronized (this) { shared++; }
来源：http://hz.9152youxi.cn/gtaketifie.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.nanxuanxn.top/gtpozsbufk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yongpay.top/gtxjeonzuf.html

C#:   lock (gate) { shared++; }
来源：http://hz.jqgfzy.top/gtyfhjayxt.html

[O04] 定义异步函数并等待
来源：http://hz.316326.xyz/gtbjwhqnef.html

Py:   async def f():⏎    await g()
来源：http://hz.hywenlv.cn/gtkbyyydhd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sweek.top/gttywnjhdh.html

JS:   async function f() { await g(); }
来源：http://hz.hywenlv.cn/gtzpwtejfv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shangyingyoupin.top/gtjggedjbb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.bjfxy.top/gtotksamss.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.gaohongyu789.top/gtylpyocxu.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.nanxinkj.top/gtagizvfny.html

C#:   async Task F() { await G(); }
来源：http://hz.52xcode.cn/gtlfmfrrxo.html

[O05] 并发执行并等待全部完成
来源：http://hz.svipenyu.cn/gtsnlfzjfi.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yj202588.top/gtpneseomh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hnxiangtu.top/gtgcebchyo.html

JS:   await Promise.all(tasks)
来源：http://hz.jlsjyb.cn/gtwtirdqyq.html

TS:   await Promise.all(tasks)
来源：http://hz.pycfn.com/gtzucihjop.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinqigufen.top/gtjjwovhvz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.daxiang520.top/gtzvguntex.html

Ruby: threads.map(&:join)
来源：http://hz.cdnleiting.top/gtyaysrrwm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xziqi.cn/gtvgihviwx.html

[O06] 使用进程池
来源：http://hz.zhaomingkeji.xyz/gtndzjofqi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shanyushiyangkeji.top/gtnckmfuta.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.sweek.top/gtxhzfhtww.html

JS:   // child_process / cluster 模块
来源：http://hz.guannengcc.top/gtvmjgbwkj.html

TS:   // child_process / cluster 模块
来源：http://hz.jyoumei.cn/gtqigrjesd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jiagoushi.top/gtmkdwclym.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shanyushiyangtech.top/gtlnyqsxcm.html

Ruby: // fork 块
来源：http://hz.yanxiufei.cn/gtokatyvmf.html

C#:   Parallel.For
来源：http://hz.gogol.net.cn/gturabggps.html

================================================================================
来源：http://hz.0kj1m.cn/gtmruphmdc.html

P. 常用工具函数
来源：http://hz.yangfankeji.com/gtdjqumlqv.html

================================================================================
来源：http://hz.jiagoushi.top/gtthwbknqr.html

[P01] 生成 UUID
来源：http://hz.jyoumei.cn/gtibbkwujh.html

Py:   str(uuid.uuid4())
来源：http://hz.guowangkeji.top/gtanksyhtq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.nanxinkj.top/gtpbhxzfss.html

JS:   crypto.randomUUID()
来源：http://hz.gotoacloud.top/gtxzpyltxx.html

TS:   crypto.randomUUID()
来源：http://hz.nwbrower.top/gtbgnsngvz.html

Java: UUID.randomUUID().toString()
来源：http://hz.jianghu66.top/gtublfdbej.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj20258.top/gttfrfbwii.html

Ruby: SecureRandom.uuid
来源：http://hz.shanyushiyangkeji.top/gtgwmdfxjb.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhiwuduotai.top/gtuqcfkmcz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.redwolf501.top/gtamkxprua.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xuanzx.com/gtjoaqjelv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.cucudq.cn/gtwglpzdam.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ywan-chungtsiang.top/gtjxnzyqps.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.kuanghao11.cn/gtgoigslbv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zycfv.cn/gtiztpexwn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hfpthk.cn/gtlrwmkvxr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xuanzx.com/gtrdokmavi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ppjwa.cn/gtinslxhqv.html

[P03] 生成短随机字符串
来源：http://hz.tanke756.top/gtlvebypsj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jqgufenzy.top/gtsroezlqr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.chenlongwang.top/gtnqlegxjs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinghuilouyu.cn/gtkfnymisf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cqqwz.cn/gtomjtzuyj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.snrcjt.cn/gtfklrrrup.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.iojbl.cn/gthleairia.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.smart0.xyz/gtoilzvjry.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shuidangran.top/gtdayiupwt.html

[P04] 求长度
来源：http://hz.smart0.xyz/gtumldagwt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhengqikj.top/gtdwadeouv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.mhx1999.top/gtdoxaxhyr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.redwolf501.top/gtakjotpao.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ybcxt.top/gtrakrzkkd.html

Java: list.size();  map.size();  s.length()
来源：http://hz.dianchejie.cn/gtlahrezdo.html

Go:   len(arr);  len(m)
来源：http://hz.andypj.xyz/gtoknwgbzf.html

Ruby: x.length;  x.size
来源：http://hz.svipenyu.cn/gtdfvcsybl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hnxiangtu.top/gtznleqrzc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hysaishi.cn/gthjfvwboi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.52xcode.cn/gtppihcuuh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jlsjyb.cn/gtksolaqpe.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nanxinkj.top/gtdsrjzbal.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jiagoushi.top/gtqzgunetr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cdnleiting.top/gtvimjqert.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xylfe.cn/gtchibbajo.html

Ruby: a == b
来源：http://hz.daria6918.cn/gtqwlrrtdk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cheryme.top/gtbowrqzep.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ywan-chungtsiang.top/gtexetothr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shangyingyoupin.top/gtpredrhxg.html

PHP:  if (empty($x)) {}
来源：http://hz.xingfuxueyuan.xyz/gttwjgmxka.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.havefunace.top/gtnzcezhrb.html

TS:   if (x == null) {}
来源：http://hz.daxiang520.top/gtpmrxjtcy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.cqqwz.cn/gtzrldcvgm.html

Go:   if x == nil {}
来源：http://hz.cashguo.top/gtvoxecahy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hongshengwenyu.top/gtssnbckpd.html

C#:   if (x is null) {}
来源：http://hz.pycfn.com/gteifrrlzp.html

[P07] 防抖与节流
来源：http://hz.cheryme.top/gtcqyrkcmt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cdnleiting.top/gtphyvqswf.html

PHP:  // 手写时间戳比较
来源：http://hz.jinqigfzy.top/gtbgmunbck.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuanzhike.top/gtdxoqgfuy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hysaishi.cn/gtxifmaayh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zdqjudy.top/gtuzrtlurd.html


<!-- 参考信息 -->