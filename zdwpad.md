代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.nanxinkj.top/gtpawqpmhd.html

JS:   process.env.HOME
来源：http://hz.cashguo.top/gtmsiatlha.html

TS:   process.env.HOME
来源：http://hz.xingfuxueyuan.xyz/gtbsjkxttj.html

Java: System.getenv("HOME")
来源：http://hz.zhengqikj.top/gtflerwjvt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.guowangkeji.top/gtrvkvfbgg.html

Ruby: ENV["HOME"]
来源：http://hz.meibo888.top/gtymkffidb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.wangdashe.top/gtaymrfqws.html

[M03] 执行外部命令
来源：http://hz.andypj.xyz/gttegrgrvp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cashguo.top/gtxkducqqc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.tian-w.cn/gtvrifjsln.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.gogol.net.cn/gtbpxxtlyd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinghuilouyu.cn/gtycrkmejd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.kuanghao11.cn/gtiwskovxd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hammf.cn/gttrzdkciz.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hfpthk.cn/gtpqxxhykn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.nanxuanxn.top/gtfjhkjwzl.html

[M04] 获取当前工作目录
来源：http://hz.zhoulong.xyz/gtjihmslbz.html

Py:   os.getcwd()
来源：http://hz.sysykeji.top/gtouiwjudl.html

PHP:  getcwd();
来源：http://hz.tian-w.cn/gtmliosooy.html

JS:   process.cwd()
来源：http://hz.c1oappe.top/gtxqpfokxy.html

TS:   process.cwd()
来源：http://hz.yangfankeji.com/gtmpfeqxad.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.aibaodan.cn/gtwedwagtu.html

Go:   os.Getwd()
来源：http://hz.jiagoushi.top/gtsubksnqp.html

Ruby: Dir.pwd
来源：http://hz.ppjwa.cn/gtaxyzmiqg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sufxvd.cn/gtuebnsdrv.html

[M05] 设置退出码
来源：http://hz.mhx1999.top/gtnpijowgi.html

Py:   sys.exit(1)
来源：http://hz.dianchejie.cn/gtsyvuuoax.html

PHP:  exit(1);
来源：http://hz.shuidangran.top/gtvpiczufo.html

JS:   process.exit(1)
来源：http://hz.wangdashe.top/gttjcaexxd.html

TS:   process.exit(1)
来源：http://hz.daxiang520.top/gtfgbpukpc.html

Java: System.exit(1)
来源：http://hz.zycfv.cn/gtygzidzhp.html

Go:   os.Exit(1)
来源：http://hz.hnxiangtu.top/gtrobzpmqg.html

Ruby: exit 1
来源：http://hz.cashguo.top/gtjyykcivp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zdqjudy.top/gtxmqcaefd.html

[M06] 向标准错误输出
来源：http://hz.ivvv.top/gtltmzewpl.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shzxlz.cn/gtxysznyqp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.bjfxy.top/gtrqhyttgd.html

JS:   console.error("err")
来源：http://hz.ydzc1.top/gtyrqdjmvf.html

TS:   console.error("err")
来源：http://hz.daxiang520.top/gtludrbhtv.html

Java: System.err.println("err")
来源：http://hz.cqqwz.cn/gtijhnsmdx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gotoacloud.top/gtabczkgky.html

Ruby: warn "err"
来源：http://hz.zhoulong.xyz/gtsltoyesq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhiwuduotai.top/gtkkgegjhy.html

[M07] 判断是否为主入口
来源：http://hz.sxryk.cn/gtiimskwzk.html

Py:   if __name__ == "__main__":
来源：http://hz.shuidangran.top/gtdyvigfdi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.0kj1m.cn/gtuqfbvuew.html

JS:   require.main === module
来源：http://hz.tianlin.xyz/gtmpkvrxmh.html

TS:   require.main === module
来源：http://hz.jinqigfzy.top/gtppbwaume.html

Java: public static void main(String[] args)
来源：http://hz.shanyushiyangtech.top/gtcmdovobd.html

Go:   func main()
来源：http://hz.zdqjudy.top/gtptllqjkk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sysykeji.top/gtoqbbvaga.html

C#:   static void Main(string[] args)
来源：http://hz.mhx1999.top/gtpxghvcnd.html

[M08] 获取系统与运行时信息
来源：http://hz.shzxlz.cn/gtwimnaamg.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jyoumei.cn/gtyafglfhw.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.fzhhl.top/gtjepzqzib.html

JS:   process.platform;  process.version
来源：http://hz.0kj1m.cn/gtebcmnnez.html

TS:   process.platform;  process.version
来源：http://hz.wangdashe.top/gtuqwzggxr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hnqzz.top/gtmsxjkxsy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yanxiufei.cn/gtdgvvletc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinyuanbaomall.cn/gtsqsobnff.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.316326.xyz/gtfmyytsib.html

================================================================================
来源：http://hz.hammf.cn/gtevhittfb.html

N. 数据结构与算法
来源：http://hz.wangdashe.top/gtnqdzrico.html

================================================================================
来源：http://hz.yuxming.cn/gtvxztyhnd.html

[N01] 二分查找（有序数组）
来源：http://hz.tanke756.top/gtaljrvkyi.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gaohongyu789.top/gtrhkfsnvq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.pycfn.com/gtlwnquvkr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gogol.net.cn/gtljdnuoto.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daria6918.cn/gtqsfbntiz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ehwqpu.com/gtaneehrit.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hammf.cn/gtkmhqsjzs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hfpthk.cn/gtndbxjzxw.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.redwolf501.top/gtegztqqyh.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gaohongyu789.top/gtydsrvzig.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangdashe.top/gtwzcpqhbx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.vqdsnc.cn/gtoksbdypb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.bjfxy.top/gtqmlymtmv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhiwuduotai.top/gtjqznszsx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sxryk.cn/gtpmsyehsa.html

Go:   slices.Sort(arr)
来源：http://hz.guannengcc.top/gterxjerhh.html

Ruby: arr.sort
来源：http://hz.yanxiufei.cn/gtiqbezmgy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xylfe.cn/gtqjucfmen.html

[N03] 快速排序（分治示例）
来源：http://hz.ehwqpu.com/gtgxgmuvbu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shangyingyoupin.top/gtnugzppbu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hammf.cn/gtwjkasppg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydjk.org.cn/gtrbidlbdy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.daxiang520.top/gtpjhretzo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yongpay.top/gtlvvptgll.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yj202588.top/gtawmeaznp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.wangshuangyany.cn/gtgwhcyrhp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.birdmap.top/gttnqfsemb.html

[N04] 斐波那契数列
来源：http://hz.sweek.top/gttpdwdedu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhixingplan.top/gtyerphusv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tanke756.top/gtitzvjttx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.smart0.xyz/gthswjoifu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhongyouzk.top/gthkcsjtwl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yuxming.cn/gtzhipnqye.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hammf.cn/gtrlgefngy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigufen.top/gtdgmjxlsu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sxryk.cn/gtqykpkwcp.html

[N05] 最大公约数
来源：http://hz.jianghu66.top/gtykspsigq.html

Py:   math.gcd(a, b)
来源：http://hz.jyoumei.cn/gtquwzogjd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhoulong.xyz/gthnazrqaq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xuanzx.com/gtaeufnvhn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zdqjudy.top/gtzlvcxkfp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xinyue.icu/gthkhmshtt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xuetiantiany.cn/gtvvsngkiw.html

Ruby: a.gcd(b)
来源：http://hz.vqdsnc.cn/gtdzoiprjj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gotoacloud.top/gtuvzqvlst.html

[N06] 判断回文字符串
来源：http://hz.yangfankeji.com/gtvnyztbxf.html

Py:   s == s[::-1]
来源：http://hz.xziqi.cn/gtpcjtsedj.html

PHP:  $s === strrev($s);
来源：http://hz.zhaomingkeji.xyz/gtsvqiuoci.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cheryme.top/gtszucymvl.html

TS:   s === [...s].reverse().join("")
来源：http://hz.iojbl.cn/gtilhwrpxr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shanyushiyangkeji.top/gtpatchsou.html

Go:   // 双指针从两端比较
来源：http://hz.sxryk.cn/gtpxrmxsgf.html

Ruby: s == s.reverse
来源：http://hz.shanyushiyangtech.top/gtkpffnmeo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.smart0.xyz/gtzbednsms.html

[N07] 两数之和（返回下标）
来源：http://hz.cqqwz.cn/gtvmhzbxvr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cdnleiting.top/gtaebmiive.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ppjwa.cn/gtdwnvffhy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ehwqpu.com/gtszcmrqwl.html

TS:   // 手写 Map<string, number>
来源：http://hz.xinyue.icu/gtikgblxjg.html

Java: // 手写 HashMap
来源：http://hz.jinghuilouyu.cn/gtbeivsobd.html

Go:   // 手写 map[int]int
来源：http://hz.jqgufenzy.top/gtbhmhbqun.html

Ruby: // 手写 Hash
来源：http://hz.vqdsnc.cn/gtcvieftjg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xuetiantiany.cn/gteqekvuhq.html

[N08] 生成全排列
来源：http://hz.haohaochexian.top/gtjgsjrgjl.html

Py:   itertools.permutations(arr)
来源：http://hz.tian-w.cn/gtgrurqjef.html

PHP:  // 手写递归交换
来源：http://hz.shanyushiyangkeji.top/gtrveuvcce.html

JS:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtraichoat.html

TS:   // 手写回溯递归
来源：http://hz.tianlin.xyz/gtizjbmuob.html

Java: // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtsvfyffml.html

Go:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtvtezfmim.html

Ruby: arr.permutation.to_a
来源：http://hz.zhongyouzk.top/gtzsqulxfu.html

C#:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtbunzotab.html

[N09] 栈与队列
来源：http://hz.hfpthk.cn/gturmgbotc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xinyue.icu/gtlkufurqa.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zdqjudy.top/gtbzaaapcn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.pengpengdd.cyou/gtwycvftpf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.svipenyu.cn/gtifpbhevr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.316326.xyz/gteexqqvir.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cqqwz.cn/gtgpqpbboo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hysaishi.cn/gtjlkvzvoo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.vqdsnc.cn/gtlqlwdgpv.html

[N10] 链表节点定义
来源：http://hz.dashuyun.cn/gtnplrvjrl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hnqzz.top/gtrfbyjtdd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hywenlv.cn/gtsrzuxjmq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.nwbrower.top/gtfatuntlk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jyoumei.cn/gtxozucfto.html

Java: class Node { int v; Node next; }
来源：http://hz.dashuyun.cn/gttwobuenk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhixingplan.top/gtwdafvblo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xinyue.icu/gtzoginama.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yuxming.cn/gttwoaeecr.html

[N11] 二叉树中序遍历
来源：http://hz.yuanzhike.top/gttohevjcg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.aibaodan.cn/gtypemzprw.html

PHP:  // 手写递归函数
来源：http://hz.aibaodan.cn/gtuxfmedlo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ivvv.top/gtsitffhuj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.9152youxi.cn/gttprpejev.html

Java: // 手写递归
来源：http://hz.sufxvd.cn/gtfqcylzjb.html

Go:   // 手写递归
来源：http://hz.ywan-chungtsiang.top/gtwshquqed.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xziqi.cn/gtsrwadmga.html

C#:   // 手写递归
来源：http://hz.yangfankeji.com/gtxaeokasy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.birdmap.top/gtmptdplua.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.sweek.top/gtqcgkzbxt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.9152youxi.cn/gtpteebaki.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ppjwa.cn/gtgwqevxcn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.snrcjt.cn/gtrtmvinsz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fengsongda.top/gtepqgtagx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yuanzhike.top/gtyeentrhx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xylfe.cn/gtqyfihdxc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenzaomai.com/gtrarrqodp.html

================================================================================
来源：http://hz.birdmap.top/gtbwrslmsw.html

O. 并发与异步
来源：http://hz.iojbl.cn/gtcdwvqjjd.html

================================================================================
来源：http://hz.xuanzx.com/gthwbqbknf.html

[O01] 启动一个线程
来源：http://hz.yvedp.cn/gtmuqshejx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hammf.cn/gtartezkji.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jlsjyb.cn/gtaostwcrd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.shanyushiyangkeji.top/gtgoviqfpe.html

TS:   // 同 JS
来源：http://hz.hysaishi.cn/gtsutqxjnn.html

Java: new Thread(() -> f()).start()
来源：http://hz.hnqzz.top/gtmaxkvhtw.html

Go:   go f()
来源：http://hz.dashuyun.cn/gtqaiftlyk.html

Ruby: Thread.new { f }
来源：http://hz.yonumen.top/gtgsqtsvcr.html

C#:   Task.Run(() => F());
来源：http://hz.sweek.top/gtpjuejpio.html

[O02] 使用线程池
来源：http://hz.ywan-chungtsiang.top/gtpjyzayfm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.316326.xyz/gthvmzprek.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.chenlongwang.top/gtguergpyt.html

JS:   // worker_threads 线程池
来源：http://hz.sysykeji.top/gtdzwoabfp.html

TS:   // worker_threads 线程池
来源：http://hz.kuanghao11.cn/gtpurlayoz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.aibaodan.cn/gtizyoegcg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yonumen.top/gtkpkdvqbl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shanyushiyangtech.top/gtgrulcssj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jqgfzy.top/gtwmehozcq.html

[O03] 加锁保护共享数据
来源：http://hz.shuidangran.top/gtucigbkiu.html

Py:   with lock: shared += 1
来源：http://hz.hammf.cn/gtkpmqwnts.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.fengsongda.top/gtfswjqrog.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.nwbrower.top/gthofdsjcv.html

TS:   // 同 JS
来源：http://hz.yvedp.cn/gtdirciijy.html

Java: synchronized (this) { shared++; }
来源：http://hz.yj20258.top/gtucsqoheo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.smart0.xyz/gtwmwslvnw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jqgufenzy.top/gtewhelxdo.html

C#:   lock (gate) { shared++; }
来源：http://hz.hammf.cn/gtdqicbesy.html

[O04] 定义异步函数并等待
来源：http://hz.0kj1m.cn/gtcjpcspyr.html

Py:   async def f():⏎    await g()
来源：http://hz.zhijiandao.cn/gtnjikfdio.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hywenlv.cn/gtnwghhhph.html

JS:   async function f() { await g(); }
来源：http://hz.hammf.cn/gtigmazaid.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.aibaodan.cn/gtfwnwumaa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.meibo888.top/gtzagflnut.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.nanxuanxn.top/gtqyfrmkuc.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.smart0.xyz/gtfsndhcom.html

C#:   async Task F() { await G(); }
来源：http://hz.9152youxi.cn/gtzobbgbil.html

[O05] 并发执行并等待全部完成
来源：http://hz.ydzc1.top/gtuxfhkglk.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jqgfzy.top/gtdgbbolut.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.chenjidiqi.icu/gtpokfvstt.html

JS:   await Promise.all(tasks)
来源：http://hz.xingfuxueyuan.xyz/gtgjxhawpz.html

TS:   await Promise.all(tasks)
来源：http://hz.zhijiandao.cn/gteragdsty.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.0kj1m.cn/gtaxuxkabk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.dianchejie.cn/gtolwrckmf.html

Ruby: threads.map(&:join)
来源：http://hz.aizwys.cn/gtoendanfq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yongpay.top/gtysreeret.html

[O06] 使用进程池
来源：http://hz.ppjwa.cn/gtzrxicxgt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jinqigfzy.top/gtkthhhugh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jyoumei.cn/gtoohrzsce.html

JS:   // child_process / cluster 模块
来源：http://hz.iojbl.cn/gthcdkceox.html

TS:   // child_process / cluster 模块
来源：http://hz.tian-w.cn/gtookmnqsr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.snrcjt.cn/gtgfxaowlm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.chenlongwang.top/gtsudnetwf.html

Ruby: // fork 块
来源：http://hz.cashguo.top/gtkldpcqlf.html

C#:   Parallel.For
来源：http://hz.sufxvd.cn/gtiifwsqsg.html

================================================================================
来源：http://hz.aizwys.cn/gtukevezic.html

P. 常用工具函数
来源：http://hz.c1oappe.top/gtmopxmbda.html

================================================================================
来源：http://hz.yvedp.cn/gtusajmecc.html

[P01] 生成 UUID
来源：http://hz.nanxinkj.top/gttbrwjpcz.html

Py:   str(uuid.uuid4())
来源：http://hz.jqgufenzy.top/gtswdpgwgm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yj20258.top/gtsyoqskja.html

JS:   crypto.randomUUID()
来源：http://hz.hywenlv.cn/gtbibtxxgf.html

TS:   crypto.randomUUID()
来源：http://hz.sweek.top/gtiisfurgs.html

Java: UUID.randomUUID().toString()
来源：http://hz.jqgfzy.top/gtyiywyygs.html

Go:   // 用 github.com/google/uuid
来源：http://hz.svipenyu.cn/gtbyywiylc.html

Ruby: SecureRandom.uuid
来源：http://hz.dashuyun.cn/gtedfpevyv.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shanyushiyangtech.top/gtxgsnpsxh.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yj20258.top/gtadqrwrds.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gogol.net.cn/gtjlrjxtcq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shzxlz.cn/gtqiyizovi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jyoumei.cn/gtgxjmlacs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhiwuduotai.top/gtkieosctj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.sxryk.cn/gtrolskczg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shuidangran.top/gtvgvlveyp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jyoumei.cn/gtmqrljaeg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jiagoushi.top/gtypennewu.html

[P03] 生成短随机字符串
来源：http://hz.shangyingyoupin.top/gtuwixgcti.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sufxvd.cn/gtuedqgjto.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yuanzhike.top/gtfsrvdfmv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xylfe.cn/gtdmxsvdgf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yangfankeji.com/gtmpjfwktr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinqigfzy.top/gtvilustle.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.0kj1m.cn/gtbamxnito.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.daria6918.cn/gtvolgyhel.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinghuilouyu.cn/gtysymukug.html

[P04] 求长度
来源：http://hz.jqgfzy.top/gtfgsavkqs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.svipenyu.cn/gtslnnjjxj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cheryme.top/gtbkccfkwd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhiwuduotai.top/gtykklzuis.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shzxlz.cn/gtoiroymsj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xuanzx.com/gtnmhazqra.html

Go:   len(arr);  len(m)
来源：http://hz.quarkkingdee.top/gturkfrrkm.html

Ruby: x.length;  x.size
来源：http://hz.jinqigfzy.top/gtpbatcvmh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shzxlz.cn/gtzubyysdx.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yvedp.cn/gtejzenrcb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hnxiangtu.top/gtzvejgezz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.gogol.net.cn/gthwhnpdup.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.havefunace.top/gtnexkbcgt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sysykeji.top/gtedyrgjsy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.fzhhl.top/gttrmzjngf.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shanyushiyangtech.top/gtjurqwnxw.html

Ruby: a == b
来源：http://hz.guowangkeji.top/gtxzurbqxm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yj20258.top/gthhyhbuhb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.birdmap.top/gteolbldpx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.tanke756.top/gthxzbfztk.html

PHP:  if (empty($x)) {}
来源：http://hz.pengpengdd.cyou/gtkdymctwm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sxryk.cn/gtkchfcfbg.html

TS:   if (x == null) {}
来源：http://hz.shanyushiyangtech.top/gtwlhtaifo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.c1oappe.top/gtemqufawn.html

Go:   if x == nil {}
来源：http://hz.hnxiangtu.top/gtnestctha.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.meibo888.top/gtkjsehpal.html

C#:   if (x is null) {}
来源：http://hz.pycfn.com/gtutykvqpi.html

[P07] 防抖与节流
来源：http://hz.zycfv.cn/gtxrlojbsl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinghuilouyu.cn/gtnvdywirj.html

PHP:  // 手写时间戳比较
来源：http://hz.jyoumei.cn/gtjfvrkjmw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hysaishi.cn/gtvvgushrr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigfzy.top/gtfygoequk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sysykeji.top/gtvenyxrwv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.fzhhl.top/gtfaexujrq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yangfankeji.com/gtcmdbgkzy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jqgufenzy.top/gtyslmpvol.html

[P08] 处理浮点精度问题
来源：http://hz.yonumen.top/gtewaxorwh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yuanzhike.top/gtwqyrbfwk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.guannengcc.top/gtaorytmys.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.nwbrower.top/gtxqfplwkb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.aizwys.cn/gtcshkccra.html


<!-- 参考信息 -->