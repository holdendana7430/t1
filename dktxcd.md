代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinqigufen.top/gtonpegshu.html

Ruby: ENV["HOME"]
来源：http://hz.jinghuilouyu.cn/gthqliezmi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.dashuyun.cn/gtwngwxpbu.html

[M03] 执行外部命令
来源：http://hz.gotoacloud.top/gtguudfjsg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.haohaochexian.top/gtwedtgcqb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.haohaochexian.top/gtvbmytyzw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnqzz.top/gtmjspiizz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yanxiufei.cn/gtulmaxliz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhiwuduotai.top/gtbtiuuhon.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hfpthk.cn/gtympuhhcp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xinyue.icu/gtkvrhdiqz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.iojbl.cn/gtolcavqkp.html

[M04] 获取当前工作目录
来源：http://hz.yueranfly.top/gtmfvathew.html

Py:   os.getcwd()
来源：http://hz.hammf.cn/gtjolebpfe.html

PHP:  getcwd();
来源：http://hz.cashguo.top/gtubbsbpwx.html

JS:   process.cwd()
来源：http://hz.gaohongyu789.top/gtttcpkbjj.html

TS:   process.cwd()
来源：http://hz.haohaochexian.top/gtllvvneak.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.bjfxy.top/gtvuooistj.html

Go:   os.Getwd()
来源：http://hz.cashguo.top/gttulziipf.html

Ruby: Dir.pwd
来源：http://hz.nwbrower.top/gtdqxqkisw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ehwqpu.com/gtfrigkewp.html

[M05] 设置退出码
来源：http://hz.shanyushiyangtech.top/gtayhezqij.html

Py:   sys.exit(1)
来源：http://hz.guannengcc.top/gtjofxzpbj.html

PHP:  exit(1);
来源：http://hz.shanyushiyangkeji.top/gtsrtfrxld.html

JS:   process.exit(1)
来源：http://hz.shanyushiyangtech.top/gtnuwtotgf.html

TS:   process.exit(1)
来源：http://hz.daxiang520.top/gtvhayfwal.html

Java: System.exit(1)
来源：http://hz.yvedp.cn/gtzucsovtl.html

Go:   os.Exit(1)
来源：http://hz.yangfankeji.com/gtyweifgkg.html

Ruby: exit 1
来源：http://hz.zycfv.cn/gtlsiwrlqj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zdqjudy.top/gtwuwppcxq.html

[M06] 向标准错误输出
来源：http://hz.tianlin.xyz/gtpojuwfam.html

Py:   print("err", file=sys.stderr)
来源：http://hz.haohaochexian.top/gtahboaodj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yuanzhike.top/gtmbvpeluo.html

JS:   console.error("err")
来源：http://hz.ppjwa.cn/gtcqsyuvyv.html

TS:   console.error("err")
来源：http://hz.ivvv.top/gtxhisgntq.html

Java: System.err.println("err")
来源：http://hz.pycfn.com/gtpiygygds.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.redwolf501.top/gtqpezyrxm.html

Ruby: warn "err"
来源：http://hz.yj20258888.top/gtjtzlxnht.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.haohaochexian.top/gtsuxcqddo.html

[M07] 判断是否为主入口
来源：http://hz.zhoulong.xyz/gtbctfjsop.html

Py:   if __name__ == "__main__":
来源：http://hz.jiagoushi.top/gtsywqcdjc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xinyue.icu/gtcdkynsdp.html

JS:   require.main === module
来源：http://hz.cdnleiting.top/gtevtckwfc.html

TS:   require.main === module
来源：http://hz.xinyue.icu/gtzayjqxha.html

Java: public static void main(String[] args)
来源：http://hz.smart0.xyz/gtcwfhgesv.html

Go:   func main()
来源：http://hz.zhengqikj.top/gtbsrplxvx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinqigufen.top/gtkxulnufm.html

C#:   static void Main(string[] args)
来源：http://hz.gzhubu.top/gtzvpgxieo.html

[M08] 获取系统与运行时信息
来源：http://hz.feifeiyinyue.top/gtevxsihyd.html

Py:   platform.system();  platform.python_version()
来源：http://hz.52xcode.cn/gtbqmoydau.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tanke756.top/gtqwclujiw.html

JS:   process.platform;  process.version
来源：http://hz.xingfuxueyuan.xyz/gtntcremmy.html

TS:   process.platform;  process.version
来源：http://hz.zhaomingkeji.xyz/gtdhdamtby.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.0kj1m.cn/gtrtitylyz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.dashuyun.cn/gtsipcjhoy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.smart0.xyz/gtpusfglkn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cucudq.cn/gtzquycxnq.html

================================================================================
来源：http://hz.havefunace.top/gtystejvkx.html

N. 数据结构与算法
来源：http://hz.feifeiyinyue.top/gtocnelrei.html

================================================================================
来源：http://hz.yuanzhike.top/gtxrmglbfp.html

[N01] 二分查找（有序数组）
来源：http://hz.kuanghao11.cn/gtlzzhcgmx.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shangyingyoupin.top/gtxpxkvhtv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.tanke756.top/gtsnqbnulz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daxiang520.top/gtbuuhxbpj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xziqi.cn/gtkbmkwmsu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.iojbl.cn/gtajkqbhzl.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yonumen.top/gtmnymwvwp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shanyushiyangkeji.top/gtozhtqypf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.pengpengdd.cyou/gteyqvbqfh.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.havefunace.top/gtcvdqczah.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hammf.cn/gttncoumok.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinqigfzy.top/gtrgixdcdw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xingfuxueyuan.xyz/gtqtokurou.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hongshengwenyu.top/gtchogloiv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cashguo.top/gtfeavlwwz.html

Go:   slices.Sort(arr)
来源：http://hz.xuetiantiany.cn/gtbvglldos.html

Ruby: arr.sort
来源：http://hz.c1oappe.top/gtlhaqtoak.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.nanxuanxn.top/gtxokvcemp.html

[N03] 快速排序（分治示例）
来源：http://hz.dashuyun.cn/gtdihqpydt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gaohongyu789.top/gtkxzdvdek.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinyuanbaomall.cn/gtggpgjmga.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xylfe.cn/gtjfwvkdha.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shanyushiyangtech.top/gtksnvqvek.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.fzhhl.top/gtwjqbtasx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ydzc1.top/gtefarrwdn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jyoumei.cn/gtfillphgm.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jiagoushi.top/gtlbxrvwps.html

[N04] 斐波那契数列
来源：http://hz.jyoumei.cn/gtavzfavwt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shuidangran.top/gttgzajief.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yj20258888.top/gtugnifkgx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hfpthk.cn/gtroahiquf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258.top/gtwumybrmy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.guowangkeji.top/gtquunakik.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cheryme.top/gtkychizcz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sxryk.cn/gtoxyjgqsv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shangyingyoupin.top/gtntayutox.html

[N05] 最大公约数
来源：http://hz.sufxvd.cn/gtepkfscni.html

Py:   math.gcd(a, b)
来源：http://hz.pengpengdd.cyou/gthepolhci.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinqigufen.top/gtujzldnni.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shangyingyoupin.top/gtksdnxsje.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenjidiqi.icu/gtcsejesku.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zycfv.cn/gthexwwcdz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yj20258.top/gtnmupizbu.html

Ruby: a.gcd(b)
来源：http://hz.chenjidiqi.icu/gtmeydujhw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gaohongyu789.top/gtmiazqleg.html

[N06] 判断回文字符串
来源：http://hz.cheryme.top/gtkajyeibp.html

Py:   s == s[::-1]
来源：http://hz.yj202588.top/gtpcfloydl.html

PHP:  $s === strrev($s);
来源：http://hz.zhiwuduotai.top/gtbnkzcoyp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hnqzz.top/gtjaqjxlre.html

TS:   s === [...s].reverse().join("")
来源：http://hz.daxiang520.top/gtntvvwmsa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ppjwa.cn/gtqigapqoc.html

Go:   // 双指针从两端比较
来源：http://hz.jinqigfzy.top/gtbauqzgem.html

Ruby: s == s.reverse
来源：http://hz.cqqwz.cn/gteoxxkwqa.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.nwbrower.top/gtetjjlefw.html

[N07] 两数之和（返回下标）
来源：http://hz.hnqzz.top/gtwrkftscm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xylfe.cn/gtwuenzrrl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hfpthk.cn/gtzstgggnt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yvedp.cn/gtgiddiaka.html

TS:   // 手写 Map<string, number>
来源：http://hz.nwbrower.top/gtprqjpwuy.html

Java: // 手写 HashMap
来源：http://hz.mhx1999.top/gtwdgigdsd.html

Go:   // 手写 map[int]int
来源：http://hz.jlsjyb.cn/gtfpkojwzm.html

Ruby: // 手写 Hash
来源：http://hz.iojbl.cn/gtnrujwgaj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.svipenyu.cn/gtoxcbdiwv.html

[N08] 生成全排列
来源：http://hz.0kj1m.cn/gtxddvwphy.html

Py:   itertools.permutations(arr)
来源：http://hz.iojbl.cn/gtdsatqdeu.html

PHP:  // 手写递归交换
来源：http://hz.tanke756.top/gtxrveyckq.html

JS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtjeaadiqq.html

TS:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtosczxixe.html

Java: // 手写回溯递归
来源：http://hz.guowangkeji.top/gtrlityspp.html

Go:   // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtwxytusws.html

Ruby: arr.permutation.to_a
来源：http://hz.gzhubu.top/gtodeqwswh.html

C#:   // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtjteckqlb.html

[N09] 栈与队列
来源：http://hz.ydzc1.top/gtruwdkysz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.fzhhl.top/gtaamuubwp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cucudq.cn/gtkmqklrbp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ywan-chungtsiang.top/gtrifzahvn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hywenlv.cn/gtitsscejj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.snrcjt.cn/gtetnxzqtt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.meibo888.top/gtdyigjkfv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hfpthk.cn/gtjqcjeqoo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhoulong.xyz/gtwmtsjqyf.html

[N10] 链表节点定义
来源：http://hz.yj20258.top/gtbhpefelk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.kuanghao11.cn/gtnytdhlvm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gogol.net.cn/gtyklpknoi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhixingplan.top/gtvtrmwipm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yuxming.cn/gtijtbtmjg.html

Java: class Node { int v; Node next; }
来源：http://hz.bjfxy.top/gtknhbsadh.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.iojbl.cn/gtvymcplvz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yj202588.top/gtickmubnp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shuidangran.top/gtgmbfxber.html

[N11] 二叉树中序遍历
来源：http://hz.snrcjt.cn/gtjgoozfnc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ppjwa.cn/gtfifcebec.html

PHP:  // 手写递归函数
来源：http://hz.quarkkingdee.top/gtpyagdlfb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxuanxn.top/gtvrmzwnwd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fengsongda.top/gtbfbmcbxk.html

Java: // 手写递归
来源：http://hz.ivvv.top/gtmtmpvovx.html

Go:   // 手写递归
来源：http://hz.jinghuilouyu.cn/gtjzpfqyzl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhixingplan.top/gtjcaewbgv.html

C#:   // 手写递归
来源：http://hz.yj20258.top/gtyqeaftcr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.nwbrower.top/gthfyglzmx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yangfankeji.com/gtbrpejfox.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.fzhhl.top/gtmziwfiuk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenjidiqi.icu/gtlfpxmplw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yanxiufei.cn/gtkcytgesj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.andypj.xyz/gtrvhzhkco.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.aizwys.cn/gtnfgnowel.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hammf.cn/gtfpvsokmy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinghuilouyu.cn/gtdfdhekwz.html

================================================================================
来源：http://hz.cheryme.top/gtgolzkkhn.html

O. 并发与异步
来源：http://hz.gotoacloud.top/gtixmzvqhm.html

================================================================================
来源：http://hz.nanxuanxn.top/gtuowmlovb.html

[O01] 启动一个线程
来源：http://hz.hongshengwenyu.top/gtalehgopk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sweek.top/gtcrcgfmsg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.nanxinkj.top/gtpjwkiodt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.nwbrower.top/gtnlrwocfs.html

TS:   // 同 JS
来源：http://hz.haohaochexian.top/gtyafkiyju.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinqigufen.top/gtuamjltkt.html

Go:   go f()
来源：http://hz.jiagoushi.top/gtqheppcel.html

Ruby: Thread.new { f }
来源：http://hz.zhijiandao.cn/gtjkabwvvo.html

C#:   Task.Run(() => F());
来源：http://hz.ehwqpu.com/gteafojfux.html

[O02] 使用线程池
来源：http://hz.ybcxt.top/gtoywsnxag.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.smart0.xyz/gthuoyzhtq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ydzc1.top/gtxffvytnn.html

JS:   // worker_threads 线程池
来源：http://hz.iojbl.cn/gteuenwakl.html

TS:   // worker_threads 线程池
来源：http://hz.yj202588.top/gtvhpybbej.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hfpthk.cn/gtnogzfssm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.kuanghao11.cn/gtukvprvaf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hnxiangtu.top/gtrpaycjmh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ivvv.top/gtpnmkhoqk.html

[O03] 加锁保护共享数据
来源：http://hz.sufxvd.cn/gtpvglqhhw.html

Py:   with lock: shared += 1
来源：http://hz.ywan-chungtsiang.top/gteuvqoobx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yj20258.top/gtkulvulhd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jiagoushi.top/gtqpwnvsif.html

TS:   // 同 JS
来源：http://hz.hammf.cn/gteteahhti.html

Java: synchronized (this) { shared++; }
来源：http://hz.cashguo.top/gtgigzvgkg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hongshengwenyu.top/gtplveriop.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinyuanbaomall.cn/gthadzwwvn.html

C#:   lock (gate) { shared++; }
来源：http://hz.havefunace.top/gtvzbnqvva.html

[O04] 定义异步函数并等待
来源：http://hz.feifeiyinyue.top/gtmmkzbzse.html

Py:   async def f():⏎    await g()
来源：http://hz.shanyushiyangtech.top/gthbhfkeci.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xinyue.icu/gtqqnkemjy.html

JS:   async function f() { await g(); }
来源：http://hz.bjfxy.top/gtkwnxkzcr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.quarkkingdee.top/gtntqtcdza.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.snrcjt.cn/gtcpzcxnwq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jinqigfzy.top/gtsfxjlusg.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jiagoushi.top/gtueyokxqu.html

C#:   async Task F() { await G(); }
来源：http://hz.jinqigufen.top/gtuqexrtyu.html

[O05] 并发执行并等待全部完成
来源：http://hz.xuanzx.com/gtdyoeeslk.html

Py:   asyncio.gather(*tasks)
来源：http://hz.9152youxi.cn/gtgomcamjk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.smart0.xyz/gtsfavaisf.html

JS:   await Promise.all(tasks)
来源：http://hz.jianghu66.top/gtfygsxevq.html

TS:   await Promise.all(tasks)
来源：http://hz.yuxming.cn/gtkvkkfqvm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhengqikj.top/gtlgzqrwda.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shuidangran.top/gtzikdmwis.html

Ruby: threads.map(&:join)
来源：http://hz.hnxiangtu.top/gtnlnlzbqh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhongyouzk.top/gtnsnpkqpd.html

[O06] 使用进程池
来源：http://hz.xingfuxueyuan.xyz/gtxnqroyei.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.c1oappe.top/gtqfqkimjy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jinyuanbaomall.cn/gtzosihfzw.html

JS:   // child_process / cluster 模块
来源：http://hz.9152youxi.cn/gtsypbkjix.html

TS:   // child_process / cluster 模块
来源：http://hz.jinqigufen.top/gtpjqiwgdn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jqgfzy.top/gttkvftdaz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yj20258.top/gtyiapagwu.html

Ruby: // fork 块
来源：http://hz.aizwys.cn/gtdkvgokpi.html

C#:   Parallel.For
来源：http://hz.jinqigufen.top/gtvcooghvl.html

================================================================================
来源：http://hz.ivvv.top/gtckipyhmx.html

P. 常用工具函数
来源：http://hz.yangfankeji.com/gtubqcfura.html

================================================================================
来源：http://hz.cucudq.cn/gtvbtcesuw.html

[P01] 生成 UUID
来源：http://hz.cucudq.cn/gtcgbasrpw.html

Py:   str(uuid.uuid4())
来源：http://hz.hongshengwenyu.top/gtlegnqfcs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gogol.net.cn/gtitqdlssz.html

JS:   crypto.randomUUID()
来源：http://hz.aizwys.cn/gtlbdwzqqu.html

TS:   crypto.randomUUID()
来源：http://hz.hywenlv.cn/gtzqhcjqzr.html

Java: UUID.randomUUID().toString()
来源：http://hz.tian-w.cn/gtbisaiudb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.pycfn.com/gtfnngpjqs.html

Ruby: SecureRandom.uuid
来源：http://hz.tian-w.cn/gtftxqnmds.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hongshengwenyu.top/gtiduipldd.html

[P02] MD5 / SHA256 摘要
来源：http://hz.andypj.xyz/gtencakbdt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yj20258.top/gtkrtgmbti.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhijiandao.cn/gthejmctjr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinqigfzy.top/gtuwjhaztb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.aibaodan.cn/gtaqxvlqvc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.sxryk.cn/gtsykzgsdh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gzhubu.top/gtptpwmiei.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ydzc1.top/gtwitfrkuy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.52xcode.cn/gtkvschmsa.html

[P03] 生成短随机字符串
来源：http://hz.smart0.xyz/gtdvszmnco.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jianghu66.top/gtulmakxiv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhongyouzk.top/gtixzjftng.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sweek.top/gtgllsdrot.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xingfuxueyuan.xyz/gtqonksdlb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.daria6918.cn/gtgokjwtwm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.guannengcc.top/gtjinfgzyi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.dianchejie.cn/gthvknxjxu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.dashuyun.cn/gtdfgjollc.html

[P04] 求长度
来源：http://hz.zhongyouzk.top/gteczljugk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jiagoushi.top/gtnykrpnil.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenjidiqi.icu/gtscupgmoo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhaomingkeji.xyz/gtwtwdpcpm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.svipenyu.cn/gtopxnkozh.html

Java: list.size();  map.size();  s.length()
来源：http://hz.nanxuanxn.top/gtdllryzzn.html

Go:   len(arr);  len(m)
来源：http://hz.yvedp.cn/gtpohjxvhd.html

Ruby: x.length;  x.size
来源：http://hz.dianchejie.cn/gtsmtcetop.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yanxiufei.cn/gtgtucrnae.html

[P05] 判断两个对象内容是否相等
来源：http://hz.cqqwz.cn/gtqrvcocab.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.pengpengdd.cyou/gtcgkkpcbk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hywenlv.cn/gtlrhqynre.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenlongwang.top/gtfxrmuimr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinqigufen.top/gtjdmpvlle.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.pycfn.com/gtmmtfrrln.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenjidiqi.icu/gtqmlnpwui.html

Ruby: a == b
来源：http://hz.jqgfzy.top/gtmylaflvl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.0kj1m.cn/gtkvrttzge.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.wangdashe.top/gtlasfcdyh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yongpay.top/gtihnnkgqv.html

PHP:  if (empty($x)) {}
来源：http://hz.hnxiangtu.top/gtflxzqxrn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jqgfzy.top/gtpdwwehhw.html

TS:   if (x == null) {}
来源：http://hz.zhiwuduotai.top/gtzwxsymav.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jlsjyb.cn/gtuwqltakp.html

Go:   if x == nil {}
来源：http://hz.hfpthk.cn/gtazvmihgn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yanxiufei.cn/gtmiczxlnc.html

C#:   if (x is null) {}
来源：http://hz.zhixingplan.top/gtxfssffpl.html

[P07] 防抖与节流
来源：http://hz.redwolf501.top/gtraofejtx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shzxlz.cn/gtggracfbb.html

PHP:  // 手写时间戳比较
来源：http://hz.tianlin.xyz/gtudcyeopj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenjidiqi.icu/gtvxgycnko.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hywenlv.cn/gtnwpvvhys.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.316326.xyz/gthplbwebb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.daria6918.cn/gtxpdaabwk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yanxiufei.cn/gtuvrvjlsd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.andypj.xyz/gtvyiykxmx.html

[P08] 处理浮点精度问题
来源：http://hz.shuidangran.top/gtxibhoubz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.c1oappe.top/gtlyputkyc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zycfv.cn/gtpholzlli.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.bjfxy.top/gtzpniwrzy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yueranfly.top/gtdktqcdey.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zdqjudy.top/gtauecgclj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sweek.top/gtuvbnrhrz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jiagoushi.top/gtwxqzytnt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xinyue.icu/gtbqxdyczw.html


<!-- 参考信息 -->