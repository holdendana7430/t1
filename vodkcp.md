代发 wailian999

Ruby: ARGV
来源：http://hz.zhengqikj.top/gtqpjgaojh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinyuanbaomall.cn/gtbaptnjun.html

[M02] 读取环境变量
来源：http://hz.dashuyun.cn/gtfketrvox.html

Py:   os.environ.get("HOME")
来源：http://hz.hysaishi.cn/gteihmxtoy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cucudq.cn/gtlntkmbix.html

JS:   process.env.HOME
来源：http://hz.cucudq.cn/gtvmnbwiao.html

TS:   process.env.HOME
来源：http://hz.mhx1999.top/gtbiixbqbv.html

Java: System.getenv("HOME")
来源：http://hz.yongpay.top/gtldmsghle.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gogol.net.cn/gteabbozgr.html

Ruby: ENV["HOME"]
来源：http://hz.hnqzz.top/gtxaagvgtx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jqgfzy.top/gtnhnkrigl.html

[M03] 执行外部命令
来源：http://hz.xinyue.icu/gtayfsxeve.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xziqi.cn/gthmkyehcx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.52xcode.cn/gtudabxjvf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cdnleiting.top/gtmszfcnzq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ybcxt.top/gtmuzymcoq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.svipenyu.cn/gtsilhxeil.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yonumen.top/gtjyrggeje.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cheryme.top/gtotdlzqrp.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinyuanbaomall.cn/gtryttldva.html

[M04] 获取当前工作目录
来源：http://hz.xinyue.icu/gtoclscwgk.html

Py:   os.getcwd()
来源：http://hz.daria6918.cn/gtkxtwtxot.html

PHP:  getcwd();
来源：http://hz.svipenyu.cn/gthvvwjjkr.html

JS:   process.cwd()
来源：http://hz.jiagoushi.top/gtvblewpgx.html

TS:   process.cwd()
来源：http://hz.xinyue.icu/gtfdgopbwy.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.wangshuangyany.cn/gtcklnbblc.html

Go:   os.Getwd()
来源：http://hz.jqgufenzy.top/gtpdclfupz.html

Ruby: Dir.pwd
来源：http://hz.hnqzz.top/gttjairunt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.bjfxy.top/gthwtcttfa.html

[M05] 设置退出码
来源：http://hz.ehwqpu.com/gtrlyokawv.html

Py:   sys.exit(1)
来源：http://hz.nanxinkj.top/gtwqoyzbug.html

PHP:  exit(1);
来源：http://hz.birdmap.top/gtgvrbrwig.html

JS:   process.exit(1)
来源：http://hz.meibo888.top/gthjrytuot.html

TS:   process.exit(1)
来源：http://hz.wangshuangyany.cn/gthvszejne.html

Java: System.exit(1)
来源：http://hz.tian-w.cn/gtwrdwofrh.html

Go:   os.Exit(1)
来源：http://hz.9152youxi.cn/gtpdvblimy.html

Ruby: exit 1
来源：http://hz.zhongyouzk.top/gtoszvvlpd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sysykeji.top/gtwpfbzbin.html

[M06] 向标准错误输出
来源：http://hz.shanyushiyangkeji.top/gtanpbovah.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gaohongyu789.top/gtgdfvqovu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.dianchejie.cn/gttomkjakv.html

JS:   console.error("err")
来源：http://hz.zhijiandao.cn/gtrrbaewlo.html

TS:   console.error("err")
来源：http://hz.jyoumei.cn/gtqcqaclso.html

Java: System.err.println("err")
来源：http://hz.ywan-chungtsiang.top/gtwsjcpnbh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jinqigufen.top/gtibeitrbi.html

Ruby: warn "err"
来源：http://hz.yuxming.cn/gtrnhqpjch.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hywenlv.cn/gthggocucg.html

[M07] 判断是否为主入口
来源：http://hz.yuxming.cn/gtliivsbhv.html

Py:   if __name__ == "__main__":
来源：http://hz.jianghu66.top/gtvlsirycl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shuidangran.top/gtuufcqtfu.html

JS:   require.main === module
来源：http://hz.zhengqikj.top/gtuecihbne.html

TS:   require.main === module
来源：http://hz.xylfe.cn/gtzjlwlset.html

Java: public static void main(String[] args)
来源：http://hz.ehwqpu.com/gtpeiaymro.html

Go:   func main()
来源：http://hz.cashguo.top/gtimysazid.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sysykeji.top/gtzjtxcwdg.html

C#:   static void Main(string[] args)
来源：http://hz.hnqzz.top/gtrmybehpm.html

[M08] 获取系统与运行时信息
来源：http://hz.pengpengdd.cyou/gticdlssbc.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shanyushiyangkeji.top/gtyyafkgyw.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.52xcode.cn/gteunlvbfl.html

JS:   process.platform;  process.version
来源：http://hz.ppjwa.cn/gtjxjsxffh.html

TS:   process.platform;  process.version
来源：http://hz.ppjwa.cn/gttppgotry.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gzhubu.top/gtgygcqnfe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ppjwa.cn/gtngjimqtf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.aizwys.cn/gtanmukvnq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.316326.xyz/gtwehqotrd.html

================================================================================
来源：http://hz.jyoumei.cn/gtqedowmfo.html

N. 数据结构与算法
来源：http://hz.gogol.net.cn/gtagteofsu.html

================================================================================
来源：http://hz.cqqwz.cn/gtwcaffczv.html

[N01] 二分查找（有序数组）
来源：http://hz.yongpay.top/gtelmjtkqz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hongshengwenyu.top/gtvegnbruf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ehwqpu.com/gtowsjpvhs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xingfuxueyuan.xyz/gtekvqzznb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jiagoushi.top/gtqhmpxojh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.sweek.top/gtmhdhprcf.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.sysykeji.top/gtkwoykwut.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yonumen.top/gtxzthvvcz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.pycfn.com/gtndchojcy.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ppjwa.cn/gtarncbrpo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tianlin.xyz/gtgtntkosh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhixingplan.top/gtlmhbtbyi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yonumen.top/gtawqjdafd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.pycfn.com/gtlppbyfyd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.feifeiyinyue.top/gtfwvrdanw.html

Go:   slices.Sort(arr)
来源：http://hz.zhoulong.xyz/gtvgurgybr.html

Ruby: arr.sort
来源：http://hz.gaohongyu789.top/gttouaeuwu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.pycfn.com/gtunsyzlgx.html

[N03] 快速排序（分治示例）
来源：http://hz.feifeiyinyue.top/gtocckufjt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yvedp.cn/gtctbhumgu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ivvv.top/gtaaeiogww.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.feifeiyinyue.top/gtorrfkqgk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.316326.xyz/gtzscqpphk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinqigfzy.top/gtbeleingy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.feifeiyinyue.top/gtdebhpxem.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sweek.top/gtavjopfem.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.0kj1m.cn/gtikdrancz.html

[N04] 斐波那契数列
来源：http://hz.jlsjyb.cn/gtdozluonr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sufxvd.cn/gtjetdzxbv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cucudq.cn/gtiisofmmk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.9152youxi.cn/gtixxuifqp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gotoacloud.top/gtdabnvfew.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhoulong.xyz/gtnizmugzd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jyoumei.cn/gtqxgkudyx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258.top/gtjappmrvu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.daria6918.cn/gtojlyxwne.html

[N05] 最大公约数
来源：http://hz.svipenyu.cn/gtcnbwvpnl.html

Py:   math.gcd(a, b)
来源：http://hz.jinqigfzy.top/gtvuboagjh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.cucudq.cn/gtpssjtfyk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tianlin.xyz/gtgvpbhdos.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gtahcykpcf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sufxvd.cn/gttvasyrol.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.316326.xyz/gtvadqcbhp.html

Ruby: a.gcd(b)
来源：http://hz.shangyingyoupin.top/gtaaynmcri.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gzhubu.top/gtjvzpfids.html

[N06] 判断回文字符串
来源：http://hz.birdmap.top/gtpyjnqstw.html

Py:   s == s[::-1]
来源：http://hz.cashguo.top/gtibxhptzs.html

PHP:  $s === strrev($s);
来源：http://hz.yj20258888.top/gtnpxwktat.html

JS:   s === [...s].reverse().join("")
来源：http://hz.daria6918.cn/gtzbqvcptg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gtvxsbhtbr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yongpay.top/gtfgfpphog.html

Go:   // 双指针从两端比较
来源：http://hz.sxryk.cn/gtfxhjtqxf.html

Ruby: s == s.reverse
来源：http://hz.chenzaomai.com/gtanstvxym.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yongpay.top/gtphublbhl.html

[N07] 两数之和（返回下标）
来源：http://hz.yuxming.cn/gtvytynqnz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.chenjidiqi.icu/gteemftuiq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.smart0.xyz/gtgvfkikyr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yj20258888.top/gtongvozkf.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhaomingkeji.xyz/gtdvuewlhz.html

Java: // 手写 HashMap
来源：http://hz.zhiwuduotai.top/gtlubzwfct.html

Go:   // 手写 map[int]int
来源：http://hz.jiagoushi.top/gtmauhsrwr.html

Ruby: // 手写 Hash
来源：http://hz.ydjk.org.cn/gtjscrosiw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.chenjidiqi.icu/gtxnrnzcrt.html

[N08] 生成全排列
来源：http://hz.shangyingyoupin.top/gtbmizjkmr.html

Py:   itertools.permutations(arr)
来源：http://hz.bjfxy.top/gtzsmjuyzv.html

PHP:  // 手写递归交换
来源：http://hz.jiagoushi.top/gtaeuawlfr.html

JS:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gthamzlhgj.html

TS:   // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtaydvtohh.html

Java: // 手写回溯递归
来源：http://hz.xinyue.icu/gtdvzoxwlm.html

Go:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtlazonyaf.html

Ruby: arr.permutation.to_a
来源：http://hz.hongshengwenyu.top/gtmozffdit.html

C#:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtgayhxxij.html

[N09] 栈与队列
来源：http://hz.chenzaomai.com/gtbjqdsgbb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jiagoushi.top/gtwuugzgvm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hfpthk.cn/gtewzovjyp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yj202588.top/gtnzyvujhn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yvedp.cn/gtigunsbeq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.daria6918.cn/gtgcqkboco.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.fzhhl.top/gtfaiusmjb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sufxvd.cn/gtmyobnuht.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jianghu66.top/gtinpqhnnp.html

[N10] 链表节点定义
来源：http://hz.hnxiangtu.top/gtaxqhtdja.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.9152youxi.cn/gtxcfmgcth.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinyuanbaomall.cn/gtvvdlvofm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.316326.xyz/gtozopmlma.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.daria6918.cn/gtrrtvrbld.html

Java: class Node { int v; Node next; }
来源：http://hz.hfpthk.cn/gtjsnggzmp.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tanke756.top/gtmfmswmhc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.feifeiyinyue.top/gtwqzvfeiq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hammf.cn/gteonhrjja.html

[N11] 二叉树中序遍历
来源：http://hz.birdmap.top/gtgexiksly.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.feifeiyinyue.top/gtlvdtftog.html

PHP:  // 手写递归函数
来源：http://hz.snrcjt.cn/gtupctnxwp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hongshengwenyu.top/gtzfxmpklb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenzaomai.com/gtkhqtfjbo.html

Java: // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtsovvasjw.html

Go:   // 手写递归
来源：http://hz.xuetiantiany.cn/gtbhncsmbx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.feifeiyinyue.top/gtqhbsyqmw.html

C#:   // 手写递归
来源：http://hz.nanxinkj.top/gtwidabcvx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ydzc1.top/gtuvwqecjx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.52xcode.cn/gtylkrmmac.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.redwolf501.top/gtnperklpt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hammf.cn/gtptwqpmlr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.haohaochexian.top/gtzhralaed.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigufen.top/gtpzzsfras.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.pycfn.com/gtbwmxckoz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xziqi.cn/gtofvagnta.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.bjfxy.top/gtbvfbsfkc.html

================================================================================
来源：http://hz.guowangkeji.top/gtcatgowbc.html

O. 并发与异步
来源：http://hz.jqgufenzy.top/gtdezdxjki.html

================================================================================
来源：http://hz.hnxiangtu.top/gtrqcdbzeh.html

[O01] 启动一个线程
来源：http://hz.dashuyun.cn/gtzbfsrzie.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xinyue.icu/gtdoebpxgh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ywan-chungtsiang.top/gtbljaldwl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.bjfxy.top/gtikslcwzm.html

TS:   // 同 JS
来源：http://hz.havefunace.top/gtrevnknhn.html

Java: new Thread(() -> f()).start()
来源：http://hz.shanyushiyangkeji.top/gtworejikj.html

Go:   go f()
来源：http://hz.xziqi.cn/gtoajsshtq.html

Ruby: Thread.new { f }
来源：http://hz.zhengqikj.top/gtdlvswrxp.html

C#:   Task.Run(() => F());
来源：http://hz.sysykeji.top/gtuchndroy.html

[O02] 使用线程池
来源：http://hz.sxryk.cn/gtsngizsxr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yanxiufei.cn/gtrybhopwn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nanxuanxn.top/gtbmhibvbr.html

JS:   // worker_threads 线程池
来源：http://hz.xuanzx.com/gtrilqamzu.html

TS:   // worker_threads 线程池
来源：http://hz.ybcxt.top/gtwjffxmru.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhoulong.xyz/gtybgcsxoz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.tanke756.top/gtnjfsxzvq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jqgfzy.top/gtkpzdnwwc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.dashuyun.cn/gtgciifbfc.html

[O03] 加锁保护共享数据
来源：http://hz.yuxming.cn/gtugjoakrd.html

Py:   with lock: shared += 1
来源：http://hz.xuanzx.com/gtbqtbseov.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yueranfly.top/gtengtonft.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hfpthk.cn/gtglcyhpaj.html

TS:   // 同 JS
来源：http://hz.kuanghao11.cn/gtrrkmgnjv.html

Java: synchronized (this) { shared++; }
来源：http://hz.jyoumei.cn/gtwzxrecmm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.0kj1m.cn/gtygvsfzgp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.9152youxi.cn/gtmzfhntpw.html

C#:   lock (gate) { shared++; }
来源：http://hz.ydjk.org.cn/gtxogcrqbr.html

[O04] 定义异步函数并等待
来源：http://hz.yonumen.top/gtcsymaequ.html

Py:   async def f():⏎    await g()
来源：http://hz.yj202588.top/gttalywnxp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hnqzz.top/gtmaepzhxm.html

JS:   async function f() { await g(); }
来源：http://hz.ydzc1.top/gttknbecvw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shanyushiyangtech.top/gtzpfrabrn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.mhx1999.top/gtousipldp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.wangdashe.top/gtyqklduad.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.nanxinkj.top/gteisvtpuu.html

C#:   async Task F() { await G(); }
来源：http://hz.hfpthk.cn/gtbiocqout.html

[O05] 并发执行并等待全部完成
来源：http://hz.svipenyu.cn/gteukfnbbw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gaohongyu789.top/gtuiemqnuc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hammf.cn/gtkishjepi.html

JS:   await Promise.all(tasks)
来源：http://hz.svipenyu.cn/gtotnvsyql.html

TS:   await Promise.all(tasks)
来源：http://hz.xylfe.cn/gtmeybaiur.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.fzhhl.top/gtxxpfvhqz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sxryk.cn/gtxdlcqlbv.html

Ruby: threads.map(&:join)
来源：http://hz.hysaishi.cn/gtdsaxlvbg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yanxiufei.cn/gtueznaram.html

[O06] 使用进程池
来源：http://hz.gzhubu.top/gtnoeufwgw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhiwuduotai.top/gtghbibgbw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.feifeiyinyue.top/gtsklgybec.html

JS:   // child_process / cluster 模块
来源：http://hz.yangfankeji.com/gtckowuifu.html

TS:   // child_process / cluster 模块
来源：http://hz.redwolf501.top/gtroplmxlr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ehwqpu.com/gtabxkthkw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yj20258888.top/gthyxauklu.html

Ruby: // fork 块
来源：http://hz.ydjk.org.cn/gtgyjypsay.html

C#:   Parallel.For
来源：http://hz.daxiang520.top/gtbqszlifo.html

================================================================================
来源：http://hz.xuanzx.com/gtiutulhrt.html

P. 常用工具函数
来源：http://hz.zhiwuduotai.top/gtaetnsirk.html

================================================================================
来源：http://hz.fengsongda.top/gtjdcdnkfg.html

[P01] 生成 UUID
来源：http://hz.yj20258.top/gtnppzurrf.html

Py:   str(uuid.uuid4())
来源：http://hz.nanxinkj.top/gtdbbpbqcd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhaomingkeji.xyz/gtdxmeqcxs.html

JS:   crypto.randomUUID()
来源：http://hz.chenlongwang.top/gtrlhxzhyh.html

TS:   crypto.randomUUID()
来源：http://hz.52xcode.cn/gttgzjbkaq.html

Java: UUID.randomUUID().toString()
来源：http://hz.xziqi.cn/gtzlyfcspl.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ywan-chungtsiang.top/gthditurrq.html

Ruby: SecureRandom.uuid
来源：http://hz.shanyushiyangkeji.top/gtzsozrisn.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.9152youxi.cn/gtmnpefult.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yongpay.top/gtflcriwcg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xinyue.icu/gtaxgykojg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jyoumei.cn/gtcxjqehan.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jianghu66.top/gtaeawlkbj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.nwbrower.top/gtpzogzizx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yonumen.top/gtjapugjpt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.andypj.xyz/gtucllhyyn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sufxvd.cn/gtzbbtulmp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.haohaochexian.top/gtawcmlbou.html

[P03] 生成短随机字符串
来源：http://hz.jinghuilouyu.cn/gtreffnjgz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sysykeji.top/gtixlbweuv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.kuanghao11.cn/gtkmfapefd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tianlin.xyz/gtydxebith.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gaohongyu789.top/gtnkqwbwkr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.pengpengdd.cyou/gtdbugdscy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ybcxt.top/gtnuszbnfu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.wangdashe.top/gtblfxipue.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhengqikj.top/gttbccunnj.html

[P04] 求长度
来源：http://hz.gogol.net.cn/gtfyuiwsha.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.0kj1m.cn/gtibnptemf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jianghu66.top/gtelexzodu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.kuanghao11.cn/gtmjlflboa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinqigufen.top/gtwihwyqik.html

Java: list.size();  map.size();  s.length()
来源：http://hz.guannengcc.top/gtzqveamwj.html

Go:   len(arr);  len(m)
来源：http://hz.jinyuanbaomall.cn/gtiklekeaf.html

Ruby: x.length;  x.size
来源：http://hz.hywenlv.cn/gtxlhlarzx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.vqdsnc.cn/gtfbdhgazd.html

[P05] 判断两个对象内容是否相等
来源：http://hz.gogol.net.cn/gtunpmapmb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hnxiangtu.top/gtwcrssuul.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.9152youxi.cn/gtarxkbeht.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ydjk.org.cn/gthdtnbqcw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.feifeiyinyue.top/gtsvofysqt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.birdmap.top/gtxtfnzhnc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.wangshuangyany.cn/gtjvfgadpf.html

Ruby: a == b
来源：http://hz.ydzc1.top/gtkluwwzlf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.9152youxi.cn/gtdduacptq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.pycfn.com/gttektderi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hfpthk.cn/gtjoopjnyl.html

PHP:  if (empty($x)) {}
来源：http://hz.chenjidiqi.icu/gtzhpytsei.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.gotoacloud.top/gtgruhqdhc.html

TS:   if (x == null) {}
来源：http://hz.svipenyu.cn/gtkxxgxxma.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yonumen.top/gtanjrhnlb.html

Go:   if x == nil {}
来源：http://hz.yj20258.top/gtggyxjdvm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hnxiangtu.top/gtlmhptffu.html

C#:   if (x is null) {}
来源：http://hz.yj20258888.top/gttfcrjaak.html

[P07] 防抖与节流
来源：http://hz.jinyuanbaomall.cn/gtvssxhbiz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yonumen.top/gtaeomdeik.html

PHP:  // 手写时间戳比较
来源：http://hz.kuanghao11.cn/gtbqpfvfbo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shzxlz.cn/gtxvqjmsoy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hywenlv.cn/gtqprtyqqw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhijiandao.cn/gthzotwwxu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.sxryk.cn/gtjtdaevgw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xingfuxueyuan.xyz/gtxbvcqzld.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hongshengwenyu.top/gtffvqnytz.html

[P08] 处理浮点精度问题
来源：http://hz.fzhhl.top/gtlcpgikfm.html


<!-- 参考信息 -->