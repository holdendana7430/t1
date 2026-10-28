代发 wailian999

JS:   process.argv.slice(2)
来源：http://hz.shzxlz.cn/gttddzvloq.html

TS:   process.argv.slice(2)
来源：http://hz.cucudq.cn/gtvkownnbg.html

Java: args 数组（main 方法参数）
来源：http://hz.xinyue.icu/gtmmruhkwq.html

Go:   os.Args[1:]
来源：http://hz.fzhhl.top/gtfmkxedwj.html

Ruby: ARGV
来源：http://hz.hywenlv.cn/gtyrhcnhtu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shzxlz.cn/gtfpkbeiei.html

[M02] 读取环境变量
来源：http://hz.ehwqpu.com/gtqnwmdndc.html

Py:   os.environ.get("HOME")
来源：http://hz.yuanzhike.top/gthlyiwdui.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shuidangran.top/gtudglctdf.html

JS:   process.env.HOME
来源：http://hz.cdnleiting.top/gtqllghncb.html

TS:   process.env.HOME
来源：http://hz.mhx1999.top/gtpbbhayvx.html

Java: System.getenv("HOME")
来源：http://hz.zhijiandao.cn/gtjhqgoltm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shangyingyoupin.top/gtvfjplbuu.html

Ruby: ENV["HOME"]
来源：http://hz.wangdashe.top/gtxheeqemq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ppjwa.cn/gtdfhqznnw.html

[M03] 执行外部命令
来源：http://hz.jianghu66.top/gtlqaeqkxb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.52xcode.cn/gtmanwhmgm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhijiandao.cn/gtweaizrkq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hfpthk.cn/gtayxsdltv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cashguo.top/gtztvmctpj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zycfv.cn/gtpxhplrxl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xinyue.icu/gtaksaztom.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jqgufenzy.top/gtcnwkjqdq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xuetiantiany.cn/gtgfroxryq.html

[M04] 获取当前工作目录
来源：http://hz.zdqjudy.top/gtikpwdorw.html

Py:   os.getcwd()
来源：http://hz.havefunace.top/gtvmvbjenp.html

PHP:  getcwd();
来源：http://hz.shzxlz.cn/gtpvviwpmm.html

JS:   process.cwd()
来源：http://hz.xuanzx.com/gtemgfeodu.html

TS:   process.cwd()
来源：http://hz.xinyue.icu/gtkxayrpyp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yuanzhike.top/gtjvynbzob.html

Go:   os.Getwd()
来源：http://hz.havefunace.top/gtigxqaofo.html

Ruby: Dir.pwd
来源：http://hz.ppjwa.cn/gttrzrfref.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hfpthk.cn/gtatncabuj.html

[M05] 设置退出码
来源：http://hz.yangfankeji.com/gtumrqbijm.html

Py:   sys.exit(1)
来源：http://hz.xinyue.icu/gtojbzoyze.html

PHP:  exit(1);
来源：http://hz.hfpthk.cn/gtllqtwalk.html

JS:   process.exit(1)
来源：http://hz.hfpthk.cn/gtdxkrrgwu.html

TS:   process.exit(1)
来源：http://hz.birdmap.top/gthoxogebu.html

Java: System.exit(1)
来源：http://hz.hnqzz.top/gtuixzyxkq.html

Go:   os.Exit(1)
来源：http://hz.shzxlz.cn/gtdijgwzde.html

Ruby: exit 1
来源：http://hz.svipenyu.cn/gtcvqmhzie.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.kuanghao11.cn/gtageddtsc.html

[M06] 向标准错误输出
来源：http://hz.zhengqikj.top/gtilkchyfl.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hnxiangtu.top/gtsytwqfxv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhoulong.xyz/gtlspfvleo.html

JS:   console.error("err")
来源：http://hz.shanyushiyangkeji.top/gtrlkiyfxu.html

TS:   console.error("err")
来源：http://hz.hywenlv.cn/gtwrcnelav.html

Java: System.err.println("err")
来源：http://hz.shanyushiyangkeji.top/gtvjjyoyim.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.meibo888.top/gtgyowxuik.html

Ruby: warn "err"
来源：http://hz.bjfxy.top/gtoqqtnsnk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.wangshuangyany.cn/gtqhxlkftp.html

[M07] 判断是否为主入口
来源：http://hz.yvedp.cn/gteuhlmiuk.html

Py:   if __name__ == "__main__":
来源：http://hz.shanyushiyangkeji.top/gtizydamse.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gogol.net.cn/gtxqcciatk.html

JS:   require.main === module
来源：http://hz.gzhubu.top/gtgttvhbsz.html

TS:   require.main === module
来源：http://hz.chenzaomai.com/gtdjnmjhyk.html

Java: public static void main(String[] args)
来源：http://hz.meibo888.top/gttkjnrdzd.html

Go:   func main()
来源：http://hz.chenzaomai.com/gtcfufwlxz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.guannengcc.top/gtroyrxqck.html

C#:   static void Main(string[] args)
来源：http://hz.aibaodan.cn/gtlqpsnhgq.html

[M08] 获取系统与运行时信息
来源：http://hz.mhx1999.top/gtfkiufliy.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xylfe.cn/gthzdbzujq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hammf.cn/gtceexhioq.html

JS:   process.platform;  process.version
来源：http://hz.zhengqikj.top/gtynhqjkut.html

TS:   process.platform;  process.version
来源：http://hz.cheryme.top/gttguopuhc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yj202588.top/gtyaqijldf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ivvv.top/gtiqfeaqyl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ydjk.org.cn/gtukvgmfkk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.nanxuanxn.top/gtuemetdrv.html

================================================================================
来源：http://hz.chenlongwang.top/gtskcelawk.html

N. 数据结构与算法
来源：http://hz.jinyuanbaomall.cn/gtxjmsouoo.html

================================================================================
来源：http://hz.jiagoushi.top/gtgavkmewg.html

[N01] 二分查找（有序数组）
来源：http://hz.ydjk.org.cn/gtqevqchpm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hnxiangtu.top/gtxauwsrdd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shuidangran.top/gtvjlvdgfr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.bjfxy.top/gtwisrpswy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.havefunace.top/gtyckypeqh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.daxiang520.top/gtocznigmz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenlongwang.top/gtbvrqoxmi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yuxming.cn/gtmncxemip.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xuanzx.com/gtwicxsfjs.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.wangshuangyany.cn/gtwolmlcso.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pengpengdd.cyou/gtilhpasjn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tian-w.cn/gtnaxhgnjk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuetiantiany.cn/gtpzgnxvly.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hnqzz.top/gtxestruhr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhaomingkeji.xyz/gtikbrbicr.html

Go:   slices.Sort(arr)
来源：http://hz.dashuyun.cn/gtyvqjbnwn.html

Ruby: arr.sort
来源：http://hz.zdqjudy.top/gtcpvqtvbc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ehwqpu.com/gtpnrudgah.html

[N03] 快速排序（分治示例）
来源：http://hz.fengsongda.top/gthjaeanbw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xuanzx.com/gtbjmiazjj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nanxinkj.top/gtfbcuxfxc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tian-w.cn/gtonwotvgy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgufenzy.top/gtxerkvkro.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.bjfxy.top/gtfxayikgx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.chenlongwang.top/gtbnedssao.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.meibo888.top/gtodjphngo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.svipenyu.cn/gtindlcpjn.html

[N04] 斐波那契数列
来源：http://hz.0kj1m.cn/gtgpucvifz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.fzhhl.top/gtqwsqmsjb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cucudq.cn/gtyyhaemnk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.havefunace.top/gteewchpag.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zycfv.cn/gtdllboyjd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.havefunace.top/gtxvhhdjzl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gaohongyu789.top/gttpttgrpt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sweek.top/gtizmxxsmb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cqqwz.cn/gtshhzsmia.html

[N05] 最大公约数
来源：http://hz.jyoumei.cn/gttuainrir.html

Py:   math.gcd(a, b)
来源：http://hz.hfpthk.cn/gtkmrtpift.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhongyouzk.top/gtdmmgeziq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.svipenyu.cn/gtizhphdka.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gogol.net.cn/gtfycsratr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.quarkkingdee.top/gtnxqepkvo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.haohaochexian.top/gtvsthsuix.html

Ruby: a.gcd(b)
来源：http://hz.jinqigufen.top/gtpxbthtua.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cqqwz.cn/gtrrjyrjhb.html

[N06] 判断回文字符串
来源：http://hz.hnqzz.top/gtyshtijdy.html

Py:   s == s[::-1]
来源：http://hz.316326.xyz/gtbractnoa.html

PHP:  $s === strrev($s);
来源：http://hz.zhoulong.xyz/gtmvqniuka.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtrezvffwf.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yuxming.cn/gttquqmhqr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zdqjudy.top/gthxaszebu.html

Go:   // 双指针从两端比较
来源：http://hz.dianchejie.cn/gtcyzsynfe.html

Ruby: s == s.reverse
来源：http://hz.chenlongwang.top/gtmksaqama.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.feifeiyinyue.top/gtdornyssg.html

[N07] 两数之和（返回下标）
来源：http://hz.jinghuilouyu.cn/gtdowkxkze.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.svipenyu.cn/gtlgvdwshs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hywenlv.cn/gtzdgvrplj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shzxlz.cn/gtpdpktpqw.html

TS:   // 手写 Map<string, number>
来源：http://hz.vqdsnc.cn/gtsmneqiku.html

Java: // 手写 HashMap
来源：http://hz.jyoumei.cn/gtgaaqetkn.html

Go:   // 手写 map[int]int
来源：http://hz.ywan-chungtsiang.top/gtwkzpgaks.html

Ruby: // 手写 Hash
来源：http://hz.andypj.xyz/gtbcgyglwy.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinqigufen.top/gtleaxwjiy.html

[N08] 生成全排列
来源：http://hz.aibaodan.cn/gtxwzigpvq.html

Py:   itertools.permutations(arr)
来源：http://hz.dashuyun.cn/gtgrbfapjc.html

PHP:  // 手写递归交换
来源：http://hz.fzhhl.top/gttvdfbatd.html

JS:   // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtdervmxqs.html

TS:   // 手写回溯递归
来源：http://hz.hfpthk.cn/gtwjlujanf.html

Java: // 手写回溯递归
来源：http://hz.ydzc1.top/gtqqdybjtv.html

Go:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtekcmekuh.html

Ruby: arr.permutation.to_a
来源：http://hz.ehwqpu.com/gtlyqwjyjw.html

C#:   // 手写回溯递归
来源：http://hz.yuxming.cn/gthsoeqvbv.html

[N09] 栈与队列
来源：http://hz.shangyingyoupin.top/gtrnnjeyvm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.tianlin.xyz/gtwteiykbx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinqigufen.top/gtvvaoqmfp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yonumen.top/gtoizqrtzs.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hywenlv.cn/gtjmnjcvvd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.9152youxi.cn/gtucwwuzmx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.pycfn.com/gtfeiyryva.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hywenlv.cn/gttqfpzkgv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.fengsongda.top/gtyprewopu.html

[N10] 链表节点定义
来源：http://hz.jiagoushi.top/gtqfrhdufv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xinyue.icu/gtalrokosb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cqqwz.cn/gtysehkbsy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.shanyushiyangtech.top/gtgtcjfdxe.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hfpthk.cn/gtvagvyjuo.html

Java: class Node { int v; Node next; }
来源：http://hz.chenzaomai.com/gtbierlzpc.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.quarkkingdee.top/gtbqlrvtuu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhixingplan.top/gtuhvobmly.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xuanzx.com/gtvhvuphbf.html

[N11] 二叉树中序遍历
来源：http://hz.316326.xyz/gttedwbjub.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.guowangkeji.top/gtdbpybxfs.html

PHP:  // 手写递归函数
来源：http://hz.svipenyu.cn/gtnprdzoro.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.snrcjt.cn/gtjhwwtkvo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tanke756.top/gtyjmkfomz.html

Java: // 手写递归
来源：http://hz.andypj.xyz/gttbeahwej.html

Go:   // 手写递归
来源：http://hz.xinyue.icu/gttakunztp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ydjk.org.cn/gtjzujttje.html

C#:   // 手写递归
来源：http://hz.jyoumei.cn/gtafqxvvja.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinqigfzy.top/gtqvkcrtgs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shuidangran.top/gtvgsfpmoe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ehwqpu.com/gtlqfzhlad.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.fengsongda.top/gtemkdaxxb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shzxlz.cn/gthledtqpk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cdnleiting.top/gtsxojxrzp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.aibaodan.cn/gtwytxubkm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.fengsongda.top/gtjcjhazcs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hnqzz.top/gtzgamxysz.html

================================================================================
来源：http://hz.andypj.xyz/gtjcacgnhp.html

O. 并发与异步
来源：http://hz.ehwqpu.com/gtzalzmsjj.html

================================================================================
来源：http://hz.smart0.xyz/gtlkhmjeqq.html

[O01] 启动一个线程
来源：http://hz.pengpengdd.cyou/gtwginbmje.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.redwolf501.top/gtdnglyyyy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yj20258.top/gtshatseka.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenzaomai.com/gtzrlkgzwn.html

TS:   // 同 JS
来源：http://hz.daria6918.cn/gtdfinrhtn.html

Java: new Thread(() -> f()).start()
来源：http://hz.guannengcc.top/gtcqckhjtx.html

Go:   go f()
来源：http://hz.hfpthk.cn/gtuxpdkglx.html

Ruby: Thread.new { f }
来源：http://hz.52xcode.cn/gtizijdhnl.html

C#:   Task.Run(() => F());
来源：http://hz.ybcxt.top/gtgkuqxekt.html

[O02] 使用线程池
来源：http://hz.jyoumei.cn/gtuyxmqoov.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.chenzaomai.com/gtuuemfehx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shanyushiyangkeji.top/gtmgslkvnp.html

JS:   // worker_threads 线程池
来源：http://hz.birdmap.top/gtnhamqwaz.html

TS:   // worker_threads 线程池
来源：http://hz.zhiwuduotai.top/gtivbmpqxk.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.smart0.xyz/gtwpblzufw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yj20258888.top/gtzkkkpvqf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhaomingkeji.xyz/gtcpmqguzx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.sweek.top/gtrlegxphx.html

[O03] 加锁保护共享数据
来源：http://hz.0kj1m.cn/gtfdzymajl.html

Py:   with lock: shared += 1
来源：http://hz.chenzaomai.com/gtobovjkso.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.daxiang520.top/gtstssmbsp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.wangdashe.top/gtvjibhhpn.html

TS:   // 同 JS
来源：http://hz.jyoumei.cn/gtndgkhmut.html

Java: synchronized (this) { shared++; }
来源：http://hz.9152youxi.cn/gtapqyshwx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.dianchejie.cn/gtmevibzzq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yuanzhike.top/gtxuiplyco.html

C#:   lock (gate) { shared++; }
来源：http://hz.shzxlz.cn/gtzkgcfyqa.html

[O04] 定义异步函数并等待
来源：http://hz.52xcode.cn/gteljhnvrf.html

Py:   async def f():⏎    await g()
来源：http://hz.hnqzz.top/gtbxucyney.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.52xcode.cn/gtmwgpecfe.html

JS:   async function f() { await g(); }
来源：http://hz.yonumen.top/gtqxbgzrxu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cdnleiting.top/gtnpcukevi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hysaishi.cn/gtmxedqepa.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.wangdashe.top/gtflsuyitf.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.nanxuanxn.top/gtpbqffnvt.html

C#:   async Task F() { await G(); }
来源：http://hz.aizwys.cn/gtbcmkkuhu.html

[O05] 并发执行并等待全部完成
来源：http://hz.316326.xyz/gtiifsdkos.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenlongwang.top/gtwwbknyrs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jlsjyb.cn/gtvjoabtiv.html

JS:   await Promise.all(tasks)
来源：http://hz.xuanzx.com/gtmmkraqcz.html

TS:   await Promise.all(tasks)
来源：http://hz.nanxinkj.top/gtoqybnqxx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.daxiang520.top/gtnvuvpirk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yj20258888.top/gtzcteyecs.html

Ruby: threads.map(&:join)
来源：http://hz.yueranfly.top/gtusrdsxim.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xuetiantiany.cn/gtxqwusvhb.html

[O06] 使用进程池
来源：http://hz.meibo888.top/gtnleeqhky.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yj20258.top/gticcbldcu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxinkj.top/gtdkxsnlrf.html

JS:   // child_process / cluster 模块
来源：http://hz.redwolf501.top/gtrlmysvxs.html

TS:   // child_process / cluster 模块
来源：http://hz.yuxming.cn/gtraxummrq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hfpthk.cn/gtlqbuphtg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xylfe.cn/gtnxqbeqol.html

Ruby: // fork 块
来源：http://hz.guannengcc.top/gtvynbarwr.html

C#:   Parallel.For
来源：http://hz.bjfxy.top/gtpgzomepe.html

================================================================================
来源：http://hz.xylfe.cn/gtmyxrvfka.html

P. 常用工具函数
来源：http://hz.xinyue.icu/gtvbkzbyqy.html

================================================================================
来源：http://hz.guannengcc.top/gtxuahrmel.html

[P01] 生成 UUID
来源：http://hz.jlsjyb.cn/gtywlaopom.html

Py:   str(uuid.uuid4())
来源：http://hz.tian-w.cn/gtjmllwncw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cheryme.top/gtgfthomcw.html

JS:   crypto.randomUUID()
来源：http://hz.yueranfly.top/gtwzwyvhyr.html

TS:   crypto.randomUUID()
来源：http://hz.zhongyouzk.top/gtmemzpkpo.html

Java: UUID.randomUUID().toString()
来源：http://hz.yuanzhike.top/gtrvkstsbs.html

Go:   // 用 github.com/google/uuid
来源：http://hz.chenjidiqi.icu/gtovsrbybw.html

Ruby: SecureRandom.uuid
来源：http://hz.jinqigfzy.top/gtdnzbuegd.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sxryk.cn/gtbvsosivs.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yanxiufei.cn/gtsqeysqxg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.vqdsnc.cn/gtjntdvpcx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ehwqpu.com/gtdggmbynb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.andypj.xyz/gtpowpaguy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shuidangran.top/gtqdzqlbmt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cheryme.top/gtrnhdvcyy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.dashuyun.cn/gttpdvtwqi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.aizwys.cn/gtchdngcup.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.sxryk.cn/gtyjzuotse.html

[P03] 生成短随机字符串
来源：http://hz.jinyuanbaomall.cn/gttewwpxnb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jqgufenzy.top/gtznoqbabp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.fengsongda.top/gtcylzrqmq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.316326.xyz/gtlfvrmldu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xingfuxueyuan.xyz/gtkeucaahc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hnqzz.top/gtukrdgaol.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yongpay.top/gtrlfbahbs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ydjk.org.cn/gtztvmoyhz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.sufxvd.cn/gtzjlvmasn.html

[P04] 求长度
来源：http://hz.hnqzz.top/gtbwcnurii.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hammf.cn/gtgrwehoaa.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zdqjudy.top/gtlcwhpwic.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fengsongda.top/gtyerjbqvc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shzxlz.cn/gtarmlkeaj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.pycfn.com/gtzkpdxwsz.html

Go:   len(arr);  len(m)
来源：http://hz.0kj1m.cn/gtzslhlatv.html

Ruby: x.length;  x.size
来源：http://hz.zycfv.cn/gtfnshcvsx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hammf.cn/gttecebnwq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ybcxt.top/gtwqzaxreq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.haohaochexian.top/gtntxxkwvz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.wangshuangyany.cn/gtxxlwpoxh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.pycfn.com/gtsxtarhek.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhixingplan.top/gtzqisoggp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhongyouzk.top/gtscanomad.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenlongwang.top/gtmglwcsln.html

Ruby: a == b
来源：http://hz.aibaodan.cn/gthpkpfyqy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yangfankeji.com/gttspwyika.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.pycfn.com/gtcyrieqrq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ydjk.org.cn/gtdaddgdgt.html

PHP:  if (empty($x)) {}
来源：http://hz.pengpengdd.cyou/gthwzqmqjn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.kuanghao11.cn/gtnbrrucsa.html

TS:   if (x == null) {}
来源：http://hz.yvedp.cn/gtzhglswos.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.52xcode.cn/gthugmirie.html

Go:   if x == nil {}
来源：http://hz.shangyingyoupin.top/gtmmrkznri.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shangyingyoupin.top/gtuhaubstk.html

C#:   if (x is null) {}
来源：http://hz.gotoacloud.top/gtjbmqzhik.html

[P07] 防抖与节流
来源：http://hz.xuetiantiany.cn/gtofzypsvg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.aibaodan.cn/gtewaqvted.html

PHP:  // 手写时间戳比较
来源：http://hz.zycfv.cn/gtlrencusy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuetiantiany.cn/gtjgphyupw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hysaishi.cn/gtfmvamgvk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhongyouzk.top/gtjsxfjwlr.html


<!-- 参考信息 -->