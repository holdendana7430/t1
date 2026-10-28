代发 wailian999

JS:   process.argv.slice(2)
来源：http://hz.yvedp.cn/gtipoibaar.html

TS:   process.argv.slice(2)
来源：http://hz.redwolf501.top/gteqirvqxz.html

Java: args 数组（main 方法参数）
来源：http://hz.zhiwuduotai.top/gtpvnktpxx.html

Go:   os.Args[1:]
来源：http://hz.hnqzz.top/gtebttfryv.html

Ruby: ARGV
来源：http://hz.xuetiantiany.cn/gtgvrbpjmy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jianghu66.top/gtsvlkwwic.html

[M02] 读取环境变量
来源：http://hz.0kj1m.cn/gteaygmuin.html

Py:   os.environ.get("HOME")
来源：http://hz.zhoulong.xyz/gtjjxxcbfz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ydjk.org.cn/gtzwohwtzy.html

JS:   process.env.HOME
来源：http://hz.cheryme.top/gtvwpiuvwh.html

TS:   process.env.HOME
来源：http://hz.shanyushiyangkeji.top/gtpiuheydt.html

Java: System.getenv("HOME")
来源：http://hz.yuxming.cn/gtvygcborh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.chenjidiqi.icu/gtkezhidiv.html

Ruby: ENV["HOME"]
来源：http://hz.shuidangran.top/gtpyflddxj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shanyushiyangtech.top/gtvtfjzkxk.html

[M03] 执行外部命令
来源：http://hz.svipenyu.cn/gtyabickva.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yvedp.cn/gtdllaqpzw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yonumen.top/gttyprbtuw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgfzy.top/gtqeriwrvg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydjk.org.cn/gtikqhmbka.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhijiandao.cn/gtfwfbeosb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.redwolf501.top/gtvgqwmxtg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hammf.cn/gtbwvfcidh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.52xcode.cn/gthklvslhb.html

[M04] 获取当前工作目录
来源：http://hz.ydjk.org.cn/gtwpppzvdv.html

Py:   os.getcwd()
来源：http://hz.xylfe.cn/gtgreneres.html

PHP:  getcwd();
来源：http://hz.shzxlz.cn/gtuopgvakn.html

JS:   process.cwd()
来源：http://hz.dashuyun.cn/gtocvwqqxz.html

TS:   process.cwd()
来源：http://hz.ehwqpu.com/gtuwdiedev.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ywan-chungtsiang.top/gtepnwnqib.html

Go:   os.Getwd()
来源：http://hz.yangfankeji.com/gtmeuiexhy.html

Ruby: Dir.pwd
来源：http://hz.jiagoushi.top/gtgdctjrss.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.quarkkingdee.top/gtxygxhyfw.html

[M05] 设置退出码
来源：http://hz.0kj1m.cn/gtqeahwzfg.html

Py:   sys.exit(1)
来源：http://hz.jlsjyb.cn/gtvkejardt.html

PHP:  exit(1);
来源：http://hz.cqqwz.cn/gtftgrwwfr.html

JS:   process.exit(1)
来源：http://hz.gzhubu.top/gtjmedszvi.html

TS:   process.exit(1)
来源：http://hz.9152youxi.cn/gtpdhekuif.html

Java: System.exit(1)
来源：http://hz.guowangkeji.top/gtxdjzucsx.html

Go:   os.Exit(1)
来源：http://hz.c1oappe.top/gtwpasysku.html

Ruby: exit 1
来源：http://hz.yuxming.cn/gtyffuvkoh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sweek.top/gtwldsjkik.html

[M06] 向标准错误输出
来源：http://hz.shanyushiyangkeji.top/gtsdypqcsq.html

Py:   print("err", file=sys.stderr)
来源：http://hz.pycfn.com/gtkebrdozc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hnqzz.top/gtrincilmq.html

JS:   console.error("err")
来源：http://hz.hammf.cn/gtymwhzhif.html

TS:   console.error("err")
来源：http://hz.zdqjudy.top/gtwishilkp.html

Java: System.err.println("err")
来源：http://hz.chenzaomai.com/gtmueyzyvf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.redwolf501.top/gtyhvvnvzw.html

Ruby: warn "err"
来源：http://hz.pycfn.com/gtizbhiscu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.wangdashe.top/gtcgeeurzw.html

[M07] 判断是否为主入口
来源：http://hz.bjfxy.top/gtjqgorybs.html

Py:   if __name__ == "__main__":
来源：http://hz.xingfuxueyuan.xyz/gtyhgkbjqd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.9152youxi.cn/gtynzdtgdh.html

JS:   require.main === module
来源：http://hz.cqqwz.cn/gtsjnuhpbt.html

TS:   require.main === module
来源：http://hz.pengpengdd.cyou/gtgcxdlzfy.html

Java: public static void main(String[] args)
来源：http://hz.jinghuilouyu.cn/gtgxajqkcj.html

Go:   func main()
来源：http://hz.hysaishi.cn/gtvcdgrzjn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.tanke756.top/gtlogdifka.html

C#:   static void Main(string[] args)
来源：http://hz.xuetiantiany.cn/gteiyytpis.html

[M08] 获取系统与运行时信息
来源：http://hz.yj202588.top/gtmlrsssbf.html

Py:   platform.system();  platform.python_version()
来源：http://hz.svipenyu.cn/gtehusqijm.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ywan-chungtsiang.top/gtiitoctrt.html

JS:   process.platform;  process.version
来源：http://hz.jlsjyb.cn/gtodydbqbk.html

TS:   process.platform;  process.version
来源：http://hz.tanke756.top/gtgpabnexp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.mhx1999.top/gtllbebsbh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yj20258888.top/gtxtzcsvou.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.mhx1999.top/gthvdkftwn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hywenlv.cn/gtuffdrekp.html

================================================================================
来源：http://hz.nanxuanxn.top/gtazpqfkdf.html

N. 数据结构与算法
来源：http://hz.iojbl.cn/gtigocvscj.html

================================================================================
来源：http://hz.zhongyouzk.top/gtqbyjmrmj.html

[N01] 二分查找（有序数组）
来源：http://hz.zhijiandao.cn/gttpivepvg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gaohongyu789.top/gtyifnwzzu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yonumen.top/gtinxcakib.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydzc1.top/gtjjketfwn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenzaomai.com/gtfzwkxjll.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yj20258.top/gtlpxtclht.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shanyushiyangtech.top/gtcxlobfdk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.birdmap.top/gthnnkbkyf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cheryme.top/gtwtdqrgdi.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.aibaodan.cn/gtxgrvxpai.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.snrcjt.cn/gtsziyvivo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hywenlv.cn/gtijihwona.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ydzc1.top/gtmnkguswa.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cashguo.top/gtzpxjzzax.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.dianchejie.cn/gtvppwdpza.html

Go:   slices.Sort(arr)
来源：http://hz.smart0.xyz/gttffwcvnv.html

Ruby: arr.sort
来源：http://hz.ywan-chungtsiang.top/gtmuklbosc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.gzhubu.top/gtmvkszfdn.html

[N03] 快速排序（分治示例）
来源：http://hz.sxryk.cn/gtwwgfydvw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.bjfxy.top/gtngfnxeal.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yvedp.cn/gtimwabauv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuanzx.com/gtwpheenqi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.snrcjt.cn/gtnkosgzlj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.nwbrower.top/gtttaallih.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ybcxt.top/gtgolyptbe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.pengpengdd.cyou/gtbbljfiih.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yangfankeji.com/gtdacejxdp.html

[N04] 斐波那契数列
来源：http://hz.mhx1999.top/gtqrcmalzd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xuanzx.com/gtzdubshaq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shzxlz.cn/gttrpxiqjq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yueranfly.top/gtwewjcsmw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhaomingkeji.xyz/gthblotjdp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.svipenyu.cn/gtxnbhpkta.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.pycfn.com/gtrswuxyxl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhoulong.xyz/gtvlgorary.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.quarkkingdee.top/gtsekgfpmd.html

[N05] 最大公约数
来源：http://hz.gaohongyu789.top/gtbcbjtixr.html

Py:   math.gcd(a, b)
来源：http://hz.meibo888.top/gtduactmzm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.316326.xyz/gtylachymw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aizwys.cn/gtukmecsop.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgfzy.top/gtpyraajdc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cdnleiting.top/gtchefquvr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hfpthk.cn/gtznptrclk.html

Ruby: a.gcd(b)
来源：http://hz.chenjidiqi.icu/gthybnisel.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.vqdsnc.cn/gtgxesdfqw.html

[N06] 判断回文字符串
来源：http://hz.c1oappe.top/gtuiorfrsj.html

Py:   s == s[::-1]
来源：http://hz.ydjk.org.cn/gtcblbusvi.html

PHP:  $s === strrev($s);
来源：http://hz.ydzc1.top/gtenwqlzki.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtvkqgrpcl.html

TS:   s === [...s].reverse().join("")
来源：http://hz.guannengcc.top/gthccdkvch.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.nanxinkj.top/gteeiasgou.html

Go:   // 双指针从两端比较
来源：http://hz.hammf.cn/gteovrwxry.html

Ruby: s == s.reverse
来源：http://hz.fzhhl.top/gtklornink.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.sysykeji.top/gtnztvwfaq.html

[N07] 两数之和（返回下标）
来源：http://hz.fzhhl.top/gtidbabhtx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xylfe.cn/gtvtpihwyo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cqqwz.cn/gtizybxzha.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yanxiufei.cn/gtrquyudxq.html

TS:   // 手写 Map<string, number>
来源：http://hz.hnxiangtu.top/gtkiipbzkb.html

Java: // 手写 HashMap
来源：http://hz.yanxiufei.cn/gtzuuyrxkw.html

Go:   // 手写 map[int]int
来源：http://hz.cdnleiting.top/gtgazbjxvw.html

Ruby: // 手写 Hash
来源：http://hz.gaohongyu789.top/gtsyixzsja.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ydjk.org.cn/gtxazezckl.html

[N08] 生成全排列
来源：http://hz.ppjwa.cn/gtwiuftlso.html

Py:   itertools.permutations(arr)
来源：http://hz.redwolf501.top/gtsmgxapeh.html

PHP:  // 手写递归交换
来源：http://hz.sxryk.cn/gtrspwwjvu.html

JS:   // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtrgncvsjl.html

TS:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtgnmtapot.html

Java: // 手写回溯递归
来源：http://hz.fzhhl.top/gtlabsirqz.html

Go:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtnmichjml.html

Ruby: arr.permutation.to_a
来源：http://hz.tian-w.cn/gtxfylongh.html

C#:   // 手写回溯递归
来源：http://hz.jqgfzy.top/gtadslvbrw.html

[N09] 栈与队列
来源：http://hz.redwolf501.top/gtckcokuqn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.0kj1m.cn/gtdvsnriie.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ehwqpu.com/gtfeallzcg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.smart0.xyz/gtlchfctbo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shzxlz.cn/gttprohmpi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ivvv.top/gtqkcbxuhz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yuanzhike.top/gtpztqkqnd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.daria6918.cn/gtqpqdpxsk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cashguo.top/gtucvecdzl.html

[N10] 链表节点定义
来源：http://hz.kuanghao11.cn/gtdbwmezhh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jinqigfzy.top/gtqfhivamb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.havefunace.top/gtzpwevypj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hywenlv.cn/gtrpklwccx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenlongwang.top/gtuutpiqtr.html

Java: class Node { int v; Node next; }
来源：http://hz.ywan-chungtsiang.top/gtqdyufbqc.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinyuanbaomall.cn/gtruciwwvi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhoulong.xyz/gtxzevzboa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.chenlongwang.top/gtwrrcsxej.html

[N11] 二叉树中序遍历
来源：http://hz.havefunace.top/gtzovkaywa.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhiwuduotai.top/gtblwlbhsf.html

PHP:  // 手写递归函数
来源：http://hz.sufxvd.cn/gtjfnmmwmx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pengpengdd.cyou/gtomxjrpel.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj202588.top/gtkobudynw.html

Java: // 手写递归
来源：http://hz.ybcxt.top/gtjrywnphd.html

Go:   // 手写递归
来源：http://hz.wangshuangyany.cn/gtbcdzizjv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shuidangran.top/gtftuvqxix.html

C#:   // 手写递归
来源：http://hz.xziqi.cn/gtvmqgbvrd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gaohongyu789.top/gtfimwflxm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhiwuduotai.top/gtazogwbxx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sysykeji.top/gtvshzehbi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.daxiang520.top/gthdwhtzeo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258888.top/gtlapgczly.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.aizwys.cn/gtubncstpp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ppjwa.cn/gtaerjderk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhijiandao.cn/gtijhkvbay.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pycfn.com/gtqfzdnjbu.html

================================================================================
来源：http://hz.ehwqpu.com/gtjwzmyxqh.html

O. 并发与异步
来源：http://hz.tianlin.xyz/gtlifokraa.html

================================================================================
来源：http://hz.zhijiandao.cn/gtjqhrjslw.html

[O01] 启动一个线程
来源：http://hz.shanyushiyangkeji.top/gtsmehsrpk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jiagoushi.top/gtfjwzugid.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gotoacloud.top/gththjpvyc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.quarkkingdee.top/gtinfnvclj.html

TS:   // 同 JS
来源：http://hz.yanxiufei.cn/gtfyvzmrid.html

Java: new Thread(() -> f()).start()
来源：http://hz.pycfn.com/gtzdcysdln.html

Go:   go f()
来源：http://hz.bjfxy.top/gtzbdepdzp.html

Ruby: Thread.new { f }
来源：http://hz.yuxming.cn/gtloddhmtd.html

C#:   Task.Run(() => F());
来源：http://hz.zhijiandao.cn/gtmjgldicb.html

[O02] 使用线程池
来源：http://hz.fzhhl.top/gttxatehpt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hysaishi.cn/gtgjgzguyg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinghuilouyu.cn/gtvhifxxlu.html

JS:   // worker_threads 线程池
来源：http://hz.yongpay.top/gtocsnpoth.html

TS:   // worker_threads 线程池
来源：http://hz.sxryk.cn/gtbruywsqm.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.nanxuanxn.top/gtttnoqeso.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hywenlv.cn/gtackjvlax.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hfpthk.cn/gtgbgmrvyr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yanxiufei.cn/gtfxeepbnb.html

[O03] 加锁保护共享数据
来源：http://hz.xziqi.cn/gtizslmixu.html

Py:   with lock: shared += 1
来源：http://hz.dashuyun.cn/gtnfzszcfn.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ywan-chungtsiang.top/gtlpueefuf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.pengpengdd.cyou/gtokwbmbek.html

TS:   // 同 JS
来源：http://hz.tianlin.xyz/gtetxjqtkp.html

Java: synchronized (this) { shared++; }
来源：http://hz.dashuyun.cn/gtausftukm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.nanxinkj.top/gtutyeohzt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.snrcjt.cn/gtzjmnwpyn.html

C#:   lock (gate) { shared++; }
来源：http://hz.cdnleiting.top/gtvdclnaac.html

[O04] 定义异步函数并等待
来源：http://hz.jinqigfzy.top/gtvzdjrncn.html

Py:   async def f():⏎    await g()
来源：http://hz.jianghu66.top/gtqmepewwz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yvedp.cn/gtfinyoehk.html

JS:   async function f() { await g(); }
来源：http://hz.xuanzx.com/gtnagsccwp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.9152youxi.cn/gtrhhecogq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yj20258888.top/gtmleahclm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jinqigufen.top/gtxwfzokec.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gzhubu.top/gtptdtcsne.html

C#:   async Task F() { await G(); }
来源：http://hz.daria6918.cn/gtqwntczkx.html

[O05] 并发执行并等待全部完成
来源：http://hz.vqdsnc.cn/gtgwjzzzyy.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xylfe.cn/gthvhxtvyc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.nanxinkj.top/gtifgnpxnc.html

JS:   await Promise.all(tasks)
来源：http://hz.ybcxt.top/gtnilyiwci.html

TS:   await Promise.all(tasks)
来源：http://hz.yanxiufei.cn/gtndxownhk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.daxiang520.top/gtktzggjyb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.nanxinkj.top/gthwpcjcvn.html

Ruby: threads.map(&:join)
来源：http://hz.gogol.net.cn/gttdrdkfyc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cashguo.top/gtjoeifcnu.html

[O06] 使用进程池
来源：http://hz.jyoumei.cn/gtmejvkbhf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.sweek.top/gtjbleylha.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shuidangran.top/gtqreopguz.html

JS:   // child_process / cluster 模块
来源：http://hz.fengsongda.top/gtfzukzgat.html

TS:   // child_process / cluster 模块
来源：http://hz.52xcode.cn/gtyzdzdsah.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhiwuduotai.top/gtrwykmbzn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.dashuyun.cn/gtmzrojzmo.html

Ruby: // fork 块
来源：http://hz.xuanzx.com/gtvqutuvgd.html

C#:   Parallel.For
来源：http://hz.jqgufenzy.top/gtcjswamsj.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtkjgmgqpw.html

P. 常用工具函数
来源：http://hz.shzxlz.cn/gtyngqqowb.html

================================================================================
来源：http://hz.smart0.xyz/gtuwwfxybl.html

[P01] 生成 UUID
来源：http://hz.cqqwz.cn/gtltiozyke.html

Py:   str(uuid.uuid4())
来源：http://hz.yongpay.top/gtlxqsarcn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhijiandao.cn/gtxbnnrzmf.html

JS:   crypto.randomUUID()
来源：http://hz.shangyingyoupin.top/gtjzulovrl.html

TS:   crypto.randomUUID()
来源：http://hz.chenjidiqi.icu/gtsvkjxdna.html

Java: UUID.randomUUID().toString()
来源：http://hz.redwolf501.top/gtcxtvlgxe.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hfpthk.cn/gtzphwxxyc.html

Ruby: SecureRandom.uuid
来源：http://hz.pycfn.com/gtrnfdodup.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.tian-w.cn/gtwegyvbgf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xylfe.cn/gtldftcjym.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yangfankeji.com/gtlyynekwm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jyoumei.cn/gtkdzyxhej.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhiwuduotai.top/gtbvsqdftv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xylfe.cn/gtjnpquwsz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shangyingyoupin.top/gtapvumvfc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xylfe.cn/gtewuzqryw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.haohaochexian.top/gtuclwomdx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.sxryk.cn/gtrgnsfojj.html

[P03] 生成短随机字符串
来源：http://hz.jlsjyb.cn/gtwmgtpknc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinqigfzy.top/gtapmzkpvv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.kuanghao11.cn/gtcrmqksnv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgufenzy.top/gtiretwfrd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gzhubu.top/gtizvexica.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ydzc1.top/gtytqnlayp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shangyingyoupin.top/gtssuyesmt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sweek.top/gtgazdvkfu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jqgufenzy.top/gtpyhvwhcd.html

[P04] 求长度
来源：http://hz.nwbrower.top/gtspcitizs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.9152youxi.cn/gtpizppmpz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj20258.top/gtqtzaxnat.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.guannengcc.top/gtdswnydsw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinqigufen.top/gtlpbvupyk.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jinqigufen.top/gtizgmdlrh.html

Go:   len(arr);  len(m)
来源：http://hz.c1oappe.top/gtrcgovjih.html

Ruby: x.length;  x.size
来源：http://hz.zycfv.cn/gtvmmgstrd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.nwbrower.top/gtrhrdvpfq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xylfe.cn/gtckdimmoy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.bjfxy.top/gtthrxgcgz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.birdmap.top/gthweiaxjc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhiwuduotai.top/gtimsanpbz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tian-w.cn/gtqknjzqxj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.daxiang520.top/gtorykqguh.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.aibaodan.cn/gtyemuknbp.html

Ruby: a == b
来源：http://hz.yj20258888.top/gtzefuqmxa.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhiwuduotai.top/gtdtyfmkzp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hammf.cn/gtsgsqxtne.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.iojbl.cn/gtkjwxbrek.html

PHP:  if (empty($x)) {}
来源：http://hz.hongshengwenyu.top/gtfgrkcqce.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinqigufen.top/gtbnhtodko.html

TS:   if (x == null) {}
来源：http://hz.havefunace.top/gtmmdbhcih.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yangfankeji.com/gtcjyaittw.html

Go:   if x == nil {}
来源：http://hz.jinqigufen.top/gtilrvgnkm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xuanzx.com/gtkoqabnwb.html

C#:   if (x is null) {}
来源：http://hz.sxryk.cn/gtgofmshbh.html

[P07] 防抖与节流
来源：http://hz.9152youxi.cn/gtxlrlbpzh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.meibo888.top/gtixnpkoni.html

PHP:  // 手写时间戳比较
来源：http://hz.wangshuangyany.cn/gtoyqgtweu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hysaishi.cn/gtutzxbrmy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.haohaochexian.top/gttxzfeymb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinyuanbaomall.cn/gtcuhhqnjl.html


<!-- 参考信息 -->