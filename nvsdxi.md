代发 wailian999

Ruby: ARGV
来源：http://hz.bjfxy.top/gtjkqofikg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinqigufen.top/gtfwxziybt.html

[M02] 读取环境变量
来源：http://hz.ehwqpu.com/gtwabsthqg.html

Py:   os.environ.get("HOME")
来源：http://hz.guowangkeji.top/gtboxgwkrb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.kuanghao11.cn/gtqolczftf.html

JS:   process.env.HOME
来源：http://hz.ydjk.org.cn/gtxasrxwsy.html

TS:   process.env.HOME
来源：http://hz.meibo888.top/gtcetthwiu.html

Java: System.getenv("HOME")
来源：http://hz.chenzaomai.com/gtsfltqpcs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xuanzx.com/gtulxioblm.html

Ruby: ENV["HOME"]
来源：http://hz.cashguo.top/gtbdyzloaa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.meibo888.top/gtpflhkrpb.html

[M03] 执行外部命令
来源：http://hz.yuanzhike.top/gtjadlzeoy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ywan-chungtsiang.top/gtnukivdxu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.fengsongda.top/gtgfvihvlf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnxiangtu.top/gtrzogzmlg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.sweek.top/gtvacovdmy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jiagoushi.top/gtfwxfamea.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ybcxt.top/gtdsmjkwvj.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhengqikj.top/gtcyurfrck.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cucudq.cn/gtyqqamaly.html

[M04] 获取当前工作目录
来源：http://hz.zhaomingkeji.xyz/gtssxdqpqh.html

Py:   os.getcwd()
来源：http://hz.ybcxt.top/gtotwjqlns.html

PHP:  getcwd();
来源：http://hz.dashuyun.cn/gtnxrhfbgd.html

JS:   process.cwd()
来源：http://hz.tanke756.top/gtuwshbbun.html

TS:   process.cwd()
来源：http://hz.kuanghao11.cn/gtbemycnqz.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.guowangkeji.top/gtfkbaznfs.html

Go:   os.Getwd()
来源：http://hz.xingfuxueyuan.xyz/gtdlurfqyh.html

Ruby: Dir.pwd
来源：http://hz.gaohongyu789.top/gtximvvhki.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gzhubu.top/gtbtnibpth.html

[M05] 设置退出码
来源：http://hz.jinqigfzy.top/gtjtwyeteq.html

Py:   sys.exit(1)
来源：http://hz.ppjwa.cn/gthoetzmyh.html

PHP:  exit(1);
来源：http://hz.mhx1999.top/gtvebcebuv.html

JS:   process.exit(1)
来源：http://hz.tian-w.cn/gthvesauqi.html

TS:   process.exit(1)
来源：http://hz.xuanzx.com/gtemgjkyaq.html

Java: System.exit(1)
来源：http://hz.jqgufenzy.top/gtlzzaxdzk.html

Go:   os.Exit(1)
来源：http://hz.yj202588.top/gtqsrvgbzh.html

Ruby: exit 1
来源：http://hz.tianlin.xyz/gttujwvyzg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cucudq.cn/gtbcmquxed.html

[M06] 向标准错误输出
来源：http://hz.bjfxy.top/gtmyrrnrxm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gotoacloud.top/gtzbzbmywl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jqgufenzy.top/gtzxhyewbb.html

JS:   console.error("err")
来源：http://hz.pengpengdd.cyou/gthnthphyf.html

TS:   console.error("err")
来源：http://hz.ydzc1.top/gtkmhnjlov.html

Java: System.err.println("err")
来源：http://hz.xylfe.cn/gtpqsumemz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xingfuxueyuan.xyz/gtyjjvjdfd.html

Ruby: warn "err"
来源：http://hz.shzxlz.cn/gtyghiudcs.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ivvv.top/gtrquspkit.html

[M07] 判断是否为主入口
来源：http://hz.chenlongwang.top/gtvvociuri.html

Py:   if __name__ == "__main__":
来源：http://hz.chenjidiqi.icu/gtamhfhqnh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ybcxt.top/gtdwfjjicf.html

JS:   require.main === module
来源：http://hz.zhixingplan.top/gtfnnnpokl.html

TS:   require.main === module
来源：http://hz.xziqi.cn/gthyobmnhy.html

Java: public static void main(String[] args)
来源：http://hz.daria6918.cn/gtvtgnrkbt.html

Go:   func main()
来源：http://hz.jqgufenzy.top/gtzvfcadyc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.dianchejie.cn/gtmfgsiexg.html

C#:   static void Main(string[] args)
来源：http://hz.hnqzz.top/gthvxdtknj.html

[M08] 获取系统与运行时信息
来源：http://hz.redwolf501.top/gtceerylpw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinghuilouyu.cn/gtuebwualu.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jinghuilouyu.cn/gtuucamtyj.html

JS:   process.platform;  process.version
来源：http://hz.quarkkingdee.top/gturlyfvbd.html

TS:   process.platform;  process.version
来源：http://hz.zdqjudy.top/gtniwlxmlc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.pycfn.com/gtiaiskihl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hnqzz.top/gtjrrnjlbf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shangyingyoupin.top/gtbluayhci.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shangyingyoupin.top/gtodkobjyr.html

================================================================================
来源：http://hz.birdmap.top/gtoabkwolz.html

N. 数据结构与算法
来源：http://hz.kuanghao11.cn/gtvnmoycwl.html

================================================================================
来源：http://hz.yj202588.top/gtdoekcbmh.html

[N01] 二分查找（有序数组）
来源：http://hz.ivvv.top/gtablsmyth.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.guannengcc.top/gtfswpstau.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.dianchejie.cn/gttmqueiti.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.c1oappe.top/gtwzuwqqlf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aibaodan.cn/gtlcdyrfsf.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yangfankeji.com/gtvhivpwbg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhoulong.xyz/gtuwshisos.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.cheryme.top/gtpztlnbmz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yj20258888.top/gtvhydemrx.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.snrcjt.cn/gtthlqhhfo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.0kj1m.cn/gtsxrsxzbe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jiagoushi.top/gtluddwulq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cheryme.top/gtqsjdoqcr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gogol.net.cn/gtmvhyough.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yuxming.cn/gtfwcrlehl.html

Go:   slices.Sort(arr)
来源：http://hz.316326.xyz/gtrfftvxxq.html

Ruby: arr.sort
来源：http://hz.gotoacloud.top/gtccysjrmb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cdnleiting.top/gtwdplicvh.html

[N03] 快速排序（分治示例）
来源：http://hz.zhengqikj.top/gteryczxaw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gogol.net.cn/gtmvdyfrnp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhaomingkeji.xyz/gtyxosrrwd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tianlin.xyz/gtevsyqoum.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.snrcjt.cn/gtzngddybl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj20258888.top/gtigppaibm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xinyue.icu/gtkyycfjff.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xylfe.cn/gtpsvxrkvu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.chenlongwang.top/gtycfnpkes.html

[N04] 斐波那契数列
来源：http://hz.316326.xyz/gtqlcobuzt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zdqjudy.top/gteaguaasx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.feifeiyinyue.top/gtctitbwdt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhijiandao.cn/gtrxwlknpn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hammf.cn/gtszwqoicw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shangyingyoupin.top/gtzjpuswds.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xylfe.cn/gtygjkzxsx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ybcxt.top/gtgxkibkmg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xylfe.cn/gtytybqgfd.html

[N05] 最大公约数
来源：http://hz.316326.xyz/gtkyfuqunq.html

Py:   math.gcd(a, b)
来源：http://hz.cucudq.cn/gtqieyigji.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yuanzhike.top/gtjhfmcjyr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.kuanghao11.cn/gtaqrulddg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinghuilouyu.cn/gtanhuddnh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xinyue.icu/gtyxqiogwg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sxryk.cn/gtrikjmyvw.html

Ruby: a.gcd(b)
来源：http://hz.sxryk.cn/gtvtqqzlmk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shuidangran.top/gtigwxlftm.html

[N06] 判断回文字符串
来源：http://hz.yonumen.top/gtjkdgycuy.html

Py:   s == s[::-1]
来源：http://hz.tianlin.xyz/gttdhkrgdt.html

PHP:  $s === strrev($s);
来源：http://hz.jinghuilouyu.cn/gtdpotytgx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yuxming.cn/gtibiwhlip.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jqgufenzy.top/gthuoefjim.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinghuilouyu.cn/gtaixtxrdf.html

Go:   // 双指针从两端比较
来源：http://hz.316326.xyz/gtlfdbbekm.html

Ruby: s == s.reverse
来源：http://hz.ppjwa.cn/gtxxzrbwgb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shangyingyoupin.top/gtzyrcrvtv.html

[N07] 两数之和（返回下标）
来源：http://hz.ywan-chungtsiang.top/gthucnhimp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gotoacloud.top/gtqigyijnj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.guowangkeji.top/gtmaomtvoa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yonumen.top/gtzuaemxbp.html

TS:   // 手写 Map<string, number>
来源：http://hz.gotoacloud.top/gtwwzlkcgu.html

Java: // 手写 HashMap
来源：http://hz.xziqi.cn/gtyjsrtrct.html

Go:   // 手写 map[int]int
来源：http://hz.andypj.xyz/gtthhwglto.html

Ruby: // 手写 Hash
来源：http://hz.yonumen.top/gtpwhcybys.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.bjfxy.top/gtszhfdala.html

[N08] 生成全排列
来源：http://hz.c1oappe.top/gtbrypxtqz.html

Py:   itertools.permutations(arr)
来源：http://hz.nanxinkj.top/gtdqerczas.html

PHP:  // 手写递归交换
来源：http://hz.aizwys.cn/gtysapauyn.html

JS:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtavnnahnw.html

TS:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtlfbbscqj.html

Java: // 手写回溯递归
来源：http://hz.xinyue.icu/gtmqmjbwsy.html

Go:   // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtvjgoagod.html

Ruby: arr.permutation.to_a
来源：http://hz.iojbl.cn/gtemziwygf.html

C#:   // 手写回溯递归
来源：http://hz.ehwqpu.com/gtgrbgolkg.html

[N09] 栈与队列
来源：http://hz.ppjwa.cn/gtcdmdtazv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.tianlin.xyz/gtdjwgxnqk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.c1oappe.top/gtqkvjifsc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jqgufenzy.top/gttgiytsxw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhongyouzk.top/gtgnjxtcyd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ehwqpu.com/gtbkuhbicb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.haohaochexian.top/gttxqckdyz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.guannengcc.top/gtabhamlbp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.guowangkeji.top/gtjrgysrgl.html

[N10] 链表节点定义
来源：http://hz.dianchejie.cn/gtmqpxqupa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.daxiang520.top/gtpjppqcpz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.birdmap.top/gtmuxbkwny.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.wangdashe.top/gtqdjoleht.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.kuanghao11.cn/gtzcljpesy.html

Java: class Node { int v; Node next; }
来源：http://hz.bjfxy.top/gtcjgcdifz.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ydjk.org.cn/gthciblphf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hammf.cn/gtpnqiiayb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.guannengcc.top/gttkjofznw.html

[N11] 二叉树中序遍历
来源：http://hz.redwolf501.top/gtjebrumau.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinyuanbaomall.cn/gtfydpvypi.html

PHP:  // 手写递归函数
来源：http://hz.jlsjyb.cn/gtitvpbssx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinqigfzy.top/gtplgmazqi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gaohongyu789.top/gtjzhuqpkl.html

Java: // 手写递归
来源：http://hz.meibo888.top/gtnjwckbgc.html

Go:   // 手写递归
来源：http://hz.cucudq.cn/gtdwaqzbco.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhongyouzk.top/gttgrtwvbu.html

C#:   // 手写递归
来源：http://hz.meibo888.top/gtxgtuanfg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhijiandao.cn/gtqgmxsujd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shanyushiyangkeji.top/gtpealjzsk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhixingplan.top/gtsvozhfta.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.pycfn.com/gtwcsjxkpg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yonumen.top/gtpdwkdubj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hysaishi.cn/gtatqtxazn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.bjfxy.top/gtqxwdvmof.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.gogol.net.cn/gtqpxdqtmp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgufenzy.top/gtdawzijyn.html

================================================================================
来源：http://hz.xziqi.cn/gtfiueyevl.html

O. 并发与异步
来源：http://hz.yueranfly.top/gtqicigwsh.html

================================================================================
来源：http://hz.smart0.xyz/gtzdcjzwak.html

[O01] 启动一个线程
来源：http://hz.xuetiantiany.cn/gtfqrqncbg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jlsjyb.cn/gtlzbalbgx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.9152youxi.cn/gtligauusk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gaohongyu789.top/gtezmpwobt.html

TS:   // 同 JS
来源：http://hz.zhaomingkeji.xyz/gtcoebqlum.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhoulong.xyz/gtrnljvgbt.html

Go:   go f()
来源：http://hz.ydzc1.top/gtphdsekeo.html

Ruby: Thread.new { f }
来源：http://hz.gotoacloud.top/gthkgpkqsu.html

C#:   Task.Run(() => F());
来源：http://hz.cucudq.cn/gthdofmtdr.html

[O02] 使用线程池
来源：http://hz.yuanzhike.top/gtffsikqpl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.chenlongwang.top/gtzrvvgtra.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shanyushiyangtech.top/gtjoqtqvza.html

JS:   // worker_threads 线程池
来源：http://hz.yonumen.top/gttnslzvtu.html

TS:   // worker_threads 线程池
来源：http://hz.yanxiufei.cn/gtbcmwyxva.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shanyushiyangkeji.top/gtqrckyeme.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ivvv.top/gtaruoexty.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cheryme.top/gtszwmbufb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jianghu66.top/gtwullxqgb.html

[O03] 加锁保护共享数据
来源：http://hz.xingfuxueyuan.xyz/gtqejgwjvy.html

Py:   with lock: shared += 1
来源：http://hz.shangyingyoupin.top/gttslkggnu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.wangdashe.top/gtdncdexwl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hnqzz.top/gtrigbzcpq.html

TS:   // 同 JS
来源：http://hz.meibo888.top/gtcyrodmvh.html

Java: synchronized (this) { shared++; }
来源：http://hz.xinyue.icu/gtbkydrvtx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.bjfxy.top/gtvdknounh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jiagoushi.top/gtdtwkmgra.html

C#:   lock (gate) { shared++; }
来源：http://hz.xylfe.cn/gtfluuhtes.html

[O04] 定义异步函数并等待
来源：http://hz.hnxiangtu.top/gtiszhiqcr.html

Py:   async def f():⏎    await g()
来源：http://hz.zhaomingkeji.xyz/gtyuepfspy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ehwqpu.com/gtvfdhdfzi.html

JS:   async function f() { await g(); }
来源：http://hz.hnqzz.top/gtvdhmywpk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ydzc1.top/gtcrldvpxl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ivvv.top/gtntlgknfb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sufxvd.cn/gtswleympk.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yuxming.cn/gtxexayqri.html

C#:   async Task F() { await G(); }
来源：http://hz.316326.xyz/gtdnhhkgez.html

[O05] 并发执行并等待全部完成
来源：http://hz.guowangkeji.top/gtrfawiwxf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.sufxvd.cn/gtkpawqogh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yuxming.cn/gtswairfbv.html

JS:   await Promise.all(tasks)
来源：http://hz.jyoumei.cn/gtgazybvou.html

TS:   await Promise.all(tasks)
来源：http://hz.zhijiandao.cn/gtjqsvqesq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.sxryk.cn/gtybipnbyt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.feifeiyinyue.top/gtmirieqah.html

Ruby: threads.map(&:join)
来源：http://hz.sxryk.cn/gtreyaistv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.guowangkeji.top/gtmhmpsjwn.html

[O06] 使用进程池
来源：http://hz.mhx1999.top/gtpovsmhyg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.havefunace.top/gtdrnrwseh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yuxming.cn/gtotlmqmnz.html

JS:   // child_process / cluster 模块
来源：http://hz.mhx1999.top/gtlxummvmh.html

TS:   // child_process / cluster 模块
来源：http://hz.feifeiyinyue.top/gtljefigfd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinqigfzy.top/gtkjkajmgk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gotoacloud.top/gtcoblvtnv.html

Ruby: // fork 块
来源：http://hz.tanke756.top/gtppyreojh.html

C#:   Parallel.For
来源：http://hz.zhoulong.xyz/gtuiwpvfxp.html

================================================================================
来源：http://hz.zhijiandao.cn/gtbtpklzgp.html

P. 常用工具函数
来源：http://hz.cashguo.top/gtruagwybu.html

================================================================================
来源：http://hz.zhoulong.xyz/gtngsvdiwz.html

[P01] 生成 UUID
来源：http://hz.vqdsnc.cn/gtavocqrpf.html

Py:   str(uuid.uuid4())
来源：http://hz.zhoulong.xyz/gtskbesomh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.fengsongda.top/gtgrucipde.html

JS:   crypto.randomUUID()
来源：http://hz.yonumen.top/gtfoeiupqa.html

TS:   crypto.randomUUID()
来源：http://hz.feifeiyinyue.top/gtpprmhtbq.html

Java: UUID.randomUUID().toString()
来源：http://hz.cheryme.top/gtvlzzhiue.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xingfuxueyuan.xyz/gtciuztkuq.html

Ruby: SecureRandom.uuid
来源：http://hz.jqgufenzy.top/gtpdknwbrl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xylfe.cn/gtkxrwpezh.html

[P02] MD5 / SHA256 摘要
来源：http://hz.fengsongda.top/gtlhoeanst.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.birdmap.top/gtpobqpbzz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gogol.net.cn/gtnzwvxscq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.feifeiyinyue.top/gtoufxnclm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.daria6918.cn/gtvfvdejxs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.0kj1m.cn/gtgzoxwiil.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.birdmap.top/gtqtdqisqw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yuanzhike.top/gtjjqwsycl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.vqdsnc.cn/gtlfafhicn.html

[P03] 生成短随机字符串
来源：http://hz.pengpengdd.cyou/gtcpljrlbe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinghuilouyu.cn/gtlzivacmy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhongyouzk.top/gtstomyjsu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jianghu66.top/gtulpgaoqn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxinkj.top/gttvsutqst.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yj20258888.top/gtumjwctki.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hfpthk.cn/gtoajpolwl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ehwqpu.com/gtfewgljuq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jqgufenzy.top/gtpojoncju.html

[P04] 求长度
来源：http://hz.chenlongwang.top/gtqazybatc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.c1oappe.top/gthjyrvlhx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.dianchejie.cn/gtgvuzxijk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.quarkkingdee.top/gtdyskqihc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.andypj.xyz/gtijqlvjtf.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jinghuilouyu.cn/gtnzgfgrpn.html

Go:   len(arr);  len(m)
来源：http://hz.bjfxy.top/gtnzsqkfro.html

Ruby: x.length;  x.size
来源：http://hz.ivvv.top/gtookhjstq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.sxryk.cn/gtgmenphhb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.haohaochexian.top/gtaqgmddrj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yuanzhike.top/gtrrmkabfw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yj202588.top/gthguzwkox.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xuetiantiany.cn/gtcoooeseq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tanke756.top/gtssydmkke.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.mhx1999.top/gtxaqajkce.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhoulong.xyz/gtlwleztdd.html

Ruby: a == b
来源：http://hz.yueranfly.top/gtonhpjifx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.9152youxi.cn/gtvijjceua.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ydjk.org.cn/gttdcyzdiw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jinqigufen.top/gtyptejfty.html

PHP:  if (empty($x)) {}
来源：http://hz.nanxinkj.top/gtwcmayhff.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.52xcode.cn/gtgmdmxcci.html

TS:   if (x == null) {}
来源：http://hz.aibaodan.cn/gtvephiifs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yj202588.top/gthdkgsuvv.html

Go:   if x == nil {}
来源：http://hz.smart0.xyz/gtrycfumpw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jiagoushi.top/gthlslfrwg.html

C#:   if (x is null) {}
来源：http://hz.hongshengwenyu.top/gteyiridzi.html

[P07] 防抖与节流
来源：http://hz.shanyushiyangkeji.top/gtthcrkwcm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ydjk.org.cn/gtxrkjbfim.html

PHP:  // 手写时间戳比较
来源：http://hz.svipenyu.cn/gtktwzsbrm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dianchejie.cn/gttkdsvmzb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinghuilouyu.cn/gtxzheboxa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhaomingkeji.xyz/gtexepfwil.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ydjk.org.cn/gtdbsmioma.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yongpay.top/gtvscbnejm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hywenlv.cn/gtcoaavwbn.html

[P08] 处理浮点精度问题
来源：http://hz.aizwys.cn/gtokvrbltk.html


<!-- 参考信息 -->