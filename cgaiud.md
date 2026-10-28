代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.dashuyun.cn/gtnyspmldw.html

JS:   process.env.HOME
来源：http://hz.zhengqikj.top/gtjssurdeg.html

TS:   process.env.HOME
来源：http://hz.snrcjt.cn/gtgawozagi.html

Java: System.getenv("HOME")
来源：http://hz.9152youxi.cn/gtvfltyxsk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.9152youxi.cn/gtdhtbesco.html

Ruby: ENV["HOME"]
来源：http://hz.birdmap.top/gtjjmymsda.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yonumen.top/gtroulowkt.html

[M03] 执行外部命令
来源：http://hz.hywenlv.cn/gtwbneqdag.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.feifeiyinyue.top/gtwrtchudc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.svipenyu.cn/gtqjdpijsf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yanxiufei.cn/gtwxbfvsgk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.316326.xyz/gtnltbwduu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.fengsongda.top/gtttirctxd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.chenlongwang.top/gtjyrzmfyh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.wangshuangyany.cn/gtqkxautnt.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gaohongyu789.top/gtlxvcgtgt.html

[M04] 获取当前工作目录
来源：http://hz.ywan-chungtsiang.top/gtmxolajkt.html

Py:   os.getcwd()
来源：http://hz.jqgfzy.top/gtvswxmowk.html

PHP:  getcwd();
来源：http://hz.aibaodan.cn/gttbpssajd.html

JS:   process.cwd()
来源：http://hz.wangshuangyany.cn/gtgohizclb.html

TS:   process.cwd()
来源：http://hz.ydzc1.top/gtcifrutnd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gaohongyu789.top/gtzbsuixnq.html

Go:   os.Getwd()
来源：http://hz.jqgfzy.top/gtpqlafszj.html

Ruby: Dir.pwd
来源：http://hz.yueranfly.top/gtyujwuidq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.havefunace.top/gtfvwjpifc.html

[M05] 设置退出码
来源：http://hz.havefunace.top/gtholzucsk.html

Py:   sys.exit(1)
来源：http://hz.yvedp.cn/gtcejqazus.html

PHP:  exit(1);
来源：http://hz.yj20258888.top/gtujfmblan.html

JS:   process.exit(1)
来源：http://hz.xuanzx.com/gtqpenllla.html

TS:   process.exit(1)
来源：http://hz.cdnleiting.top/gtdslovwcz.html

Java: System.exit(1)
来源：http://hz.quarkkingdee.top/gtlzqliuli.html

Go:   os.Exit(1)
来源：http://hz.snrcjt.cn/gtxxvtmwyh.html

Ruby: exit 1
来源：http://hz.aibaodan.cn/gthahwoift.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.52xcode.cn/gttiuqsnzx.html

[M06] 向标准错误输出
来源：http://hz.mhx1999.top/gtesnbsjhz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhongyouzk.top/gtfonolmyh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yuxming.cn/gtuzjciyct.html

JS:   console.error("err")
来源：http://hz.zhixingplan.top/gtfjmmfege.html

TS:   console.error("err")
来源：http://hz.tianlin.xyz/gtztadliyv.html

Java: System.err.println("err")
来源：http://hz.iojbl.cn/gtohujttnv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xinyue.icu/gtxvmqcfse.html

Ruby: warn "err"
来源：http://hz.mhx1999.top/gtpokkmekq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhijiandao.cn/gtdyvtyqpl.html

[M07] 判断是否为主入口
来源：http://hz.bjfxy.top/gtglxdltfm.html

Py:   if __name__ == "__main__":
来源：http://hz.haohaochexian.top/gtrldwwmmj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cashguo.top/gtheltlkpv.html

JS:   require.main === module
来源：http://hz.tianlin.xyz/gtnxfeyudt.html

TS:   require.main === module
来源：http://hz.sysykeji.top/gtjnqhoypo.html

Java: public static void main(String[] args)
来源：http://hz.tanke756.top/gtdmcbiqpr.html

Go:   func main()
来源：http://hz.jinghuilouyu.cn/gtnvewdeet.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.aizwys.cn/gtvdgvkrje.html

C#:   static void Main(string[] args)
来源：http://hz.hongshengwenyu.top/gtavmjzxfl.html

[M08] 获取系统与运行时信息
来源：http://hz.wangshuangyany.cn/gtcaimcunu.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ydjk.org.cn/gtyakelfaf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yonumen.top/gtldhqhypt.html

JS:   process.platform;  process.version
来源：http://hz.daria6918.cn/gtlukmzxlc.html

TS:   process.platform;  process.version
来源：http://hz.tian-w.cn/gtdkdmdmvd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yj20258888.top/gtfqbdqwkz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shuidangran.top/gtfboubjev.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hnqzz.top/gthzwuyljc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xuetiantiany.cn/gtwxoxfnhd.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtraklxbps.html

N. 数据结构与算法
来源：http://hz.shanyushiyangtech.top/gtbonqzabw.html

================================================================================
来源：http://hz.zhijiandao.cn/gtgualuwxw.html

[N01] 二分查找（有序数组）
来源：http://hz.feifeiyinyue.top/gteqnyssny.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinqigfzy.top/gtehauqral.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.redwolf501.top/gtfbwbiovp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.vqdsnc.cn/gtaaapwkvz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cqqwz.cn/gtnbpkiact.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ivvv.top/gthryxbwgc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xuanzx.com/gtifextcwd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.dashuyun.cn/gtkiwtafoe.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hammf.cn/gteztenezi.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ehwqpu.com/gtmqruumtx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jlsjyb.cn/gtfxmdscaf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hnxiangtu.top/gtvhpqhfys.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.52xcode.cn/gtkbulvwmd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.wangshuangyany.cn/gtmhfxycmy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhaomingkeji.xyz/gtkokpojlp.html

Go:   slices.Sort(arr)
来源：http://hz.jinyuanbaomall.cn/gtadqcwdhx.html

Ruby: arr.sort
来源：http://hz.yj20258888.top/gtdawmezxn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jiagoushi.top/gtohyttwkt.html

[N03] 快速排序（分治示例）
来源：http://hz.tianlin.xyz/gtazlyyevo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ydjk.org.cn/gtgfhsbatq.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nanxinkj.top/gtpceolvsu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigufen.top/gtjxdyefsz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj20258.top/gtgwdrlslb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhijiandao.cn/gtldogokel.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.birdmap.top/gtrbwbtuvu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xuetiantiany.cn/gttgzodqqu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhaomingkeji.xyz/gtbyayfhcc.html

[N04] 斐波那契数列
来源：http://hz.hnqzz.top/gtdeuuamvk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.chenlongwang.top/gtehcyfsmq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sufxvd.cn/gtxupzekif.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.316326.xyz/gtrmfsrhfa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhengqikj.top/gthdyhvbqz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shzxlz.cn/gtlkzsehvy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.dashuyun.cn/gtixtypbdq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.316326.xyz/gtweffvhbk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shangyingyoupin.top/gtmcismqcb.html

[N05] 最大公约数
来源：http://hz.iojbl.cn/gttglzruvo.html

Py:   math.gcd(a, b)
来源：http://hz.xziqi.cn/gtqmbegrbz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhiwuduotai.top/gtuhvvchzw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gogol.net.cn/gtcobuyfqy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guannengcc.top/gthoksxplt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jlsjyb.cn/gtfcwesjca.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ywan-chungtsiang.top/gtlazctebn.html

Ruby: a.gcd(b)
来源：http://hz.sysykeji.top/gtmxxyjlwf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xuetiantiany.cn/gtdpypjkwf.html

[N06] 判断回文字符串
来源：http://hz.tian-w.cn/gttxqmcsnv.html

Py:   s == s[::-1]
来源：http://hz.sufxvd.cn/gtolvxqqaf.html

PHP:  $s === strrev($s);
来源：http://hz.daria6918.cn/gtlvufkayc.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtgbaoiyde.html

TS:   s === [...s].reverse().join("")
来源：http://hz.52xcode.cn/gtwkxmyavp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.meibo888.top/gtdbagdfmd.html

Go:   // 双指针从两端比较
来源：http://hz.nanxuanxn.top/gttzbmzhmr.html

Ruby: s == s.reverse
来源：http://hz.yonumen.top/gtipxsnaef.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.pycfn.com/gtlthckvpr.html

[N07] 两数之和（返回下标）
来源：http://hz.gzhubu.top/gtejsykcsu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hywenlv.cn/gtzukmgsan.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.svipenyu.cn/gtvmrpuufg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gaohongyu789.top/gtgietijfd.html

TS:   // 手写 Map<string, number>
来源：http://hz.snrcjt.cn/gtgnuuprtk.html

Java: // 手写 HashMap
来源：http://hz.ywan-chungtsiang.top/gtdsnfjdsa.html

Go:   // 手写 map[int]int
来源：http://hz.zhaomingkeji.xyz/gtpqisnroc.html

Ruby: // 手写 Hash
来源：http://hz.bjfxy.top/gtdtkdxstg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.svipenyu.cn/gtcycxwvqo.html

[N08] 生成全排列
来源：http://hz.andypj.xyz/gtxfdhhbbf.html

Py:   itertools.permutations(arr)
来源：http://hz.aibaodan.cn/gtpeabjrjk.html

PHP:  // 手写递归交换
来源：http://hz.smart0.xyz/gttqrnnplu.html

JS:   // 手写回溯递归
来源：http://hz.aizwys.cn/gtlyzuznhs.html

TS:   // 手写回溯递归
来源：http://hz.ybcxt.top/gtvwpidtvu.html

Java: // 手写回溯递归
来源：http://hz.hfpthk.cn/gtmicynkxf.html

Go:   // 手写回溯递归
来源：http://hz.zycfv.cn/gtbozcahxk.html

Ruby: arr.permutation.to_a
来源：http://hz.jqgfzy.top/gtrzyjvgzk.html

C#:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtdykpdmos.html

[N09] 栈与队列
来源：http://hz.vqdsnc.cn/gteyqfbies.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj20258.top/gtturypiev.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.vqdsnc.cn/gtlctrdvjm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yangfankeji.com/gtqrhbawpm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.meibo888.top/gtbyaejjig.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.9152youxi.cn/gtyfdoaish.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yj20258.top/gtjnauynat.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yuxming.cn/gtlmtzrtom.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.iojbl.cn/gtviiulbcs.html

[N10] 链表节点定义
来源：http://hz.jqgufenzy.top/gtqlnpsiix.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.andypj.xyz/gtztvsjcto.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.iojbl.cn/gtcxuppwqh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cheryme.top/gtghfptubw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhijiandao.cn/gtlabksbjo.html

Java: class Node { int v; Node next; }
来源：http://hz.hfpthk.cn/gtllzdzxqm.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.316326.xyz/gthvtzrglo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.quarkkingdee.top/gtblgywntz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xingfuxueyuan.xyz/gtvzjthzkl.html

[N11] 二叉树中序遍历
来源：http://hz.gzhubu.top/gtgdqbfkvk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.gzhubu.top/gtxpsahaec.html

PHP:  // 手写递归函数
来源：http://hz.jqgfzy.top/gtqjfxlxnk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.bjfxy.top/gtjqzddmst.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgufenzy.top/gtplfgqunk.html

Java: // 手写递归
来源：http://hz.cashguo.top/gttskdsnyn.html

Go:   // 手写递归
来源：http://hz.ehwqpu.com/gtxlrmzexx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shuidangran.top/gtpcurxdmh.html

C#:   // 手写递归
来源：http://hz.ivvv.top/gthktfyyjr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.sysykeji.top/gtqlggtfav.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.daxiang520.top/gtihlvpiva.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hysaishi.cn/gtnwqrfsyi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhoulong.xyz/gtqoukgltv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangtech.top/gtwquiynlc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.kuanghao11.cn/gtjmvfpqgy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jqgufenzy.top/gthtxnaizu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.daxiang520.top/gtbukcayra.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ivvv.top/gtshssnxjg.html

================================================================================
来源：http://hz.meibo888.top/gtfuiyehkb.html

O. 并发与异步
来源：http://hz.ivvv.top/gtsqtufksa.html

================================================================================
来源：http://hz.guannengcc.top/gtxymvbiyv.html

[O01] 启动一个线程
来源：http://hz.birdmap.top/gteygsqnte.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jlsjyb.cn/gtodgdhstq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.pengpengdd.cyou/gtmyobnwbe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.dashuyun.cn/gtobiwlsud.html

TS:   // 同 JS
来源：http://hz.kuanghao11.cn/gtrvmcfmdu.html

Java: new Thread(() -> f()).start()
来源：http://hz.fengsongda.top/gtwkkggtrz.html

Go:   go f()
来源：http://hz.aibaodan.cn/gtkbfidnkd.html

Ruby: Thread.new { f }
来源：http://hz.yj202588.top/gtkubyrske.html

C#:   Task.Run(() => F());
来源：http://hz.jqgfzy.top/gtmytcroxy.html

[O02] 使用线程池
来源：http://hz.ydzc1.top/gtlfgslvpc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hnxiangtu.top/gtmfodrfvw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.aizwys.cn/gtrxmhuujq.html

JS:   // worker_threads 线程池
来源：http://hz.gaohongyu789.top/gtvmuuljld.html

TS:   // worker_threads 线程池
来源：http://hz.andypj.xyz/gtqvipdqxj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shangyingyoupin.top/gtdnwxhlpk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.kuanghao11.cn/gtykdmkkds.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cashguo.top/gtmfodbzfc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yongpay.top/gtemtqkaso.html

[O03] 加锁保护共享数据
来源：http://hz.iojbl.cn/gtfhamaklj.html

Py:   with lock: shared += 1
来源：http://hz.xylfe.cn/gtmvvqmwih.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.meibo888.top/gteikmnssv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ivvv.top/gtonzonqbv.html

TS:   // 同 JS
来源：http://hz.hammf.cn/gtsqkxrfza.html

Java: synchronized (this) { shared++; }
来源：http://hz.9152youxi.cn/gthvsjxawk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hnqzz.top/gthapowksu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.pycfn.com/gtafeegevz.html

C#:   lock (gate) { shared++; }
来源：http://hz.sweek.top/gtwhftryym.html

[O04] 定义异步函数并等待
来源：http://hz.aibaodan.cn/gtvoutgosz.html

Py:   async def f():⏎    await g()
来源：http://hz.xziqi.cn/gtofolwinb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.meibo888.top/gthovyvdua.html

JS:   async function f() { await g(); }
来源：http://hz.guannengcc.top/gtkyvkrfzh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhoulong.xyz/gtvektnokj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.andypj.xyz/gtpbmqrpxh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jlsjyb.cn/gtktvsevuc.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gogol.net.cn/gtraozvedf.html

C#:   async Task F() { await G(); }
来源：http://hz.ehwqpu.com/gtrwmmnftq.html

[O05] 并发执行并等待全部完成
来源：http://hz.zdqjudy.top/gtnfxbyeur.html

Py:   asyncio.gather(*tasks)
来源：http://hz.nanxuanxn.top/gtjzjgevhe.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.sweek.top/gtmieblnbc.html

JS:   await Promise.all(tasks)
来源：http://hz.mhx1999.top/gtwjnezimh.html

TS:   await Promise.all(tasks)
来源：http://hz.nwbrower.top/gtdmstainz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.pengpengdd.cyou/gtkrrslomd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hysaishi.cn/gtzzehqmqj.html

Ruby: threads.map(&:join)
来源：http://hz.guowangkeji.top/gthrrrlevo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.daria6918.cn/gtvtoehiax.html

[O06] 使用进程池
来源：http://hz.shanyushiyangtech.top/gtmwezuplz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ybcxt.top/gtmsyahvne.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.sxryk.cn/gtnhxcwhwc.html

JS:   // child_process / cluster 模块
来源：http://hz.guannengcc.top/gtvphtcdba.html

TS:   // child_process / cluster 模块
来源：http://hz.sysykeji.top/gtpchbmtas.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sweek.top/gtiiucpidi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jiagoushi.top/gtqvzbchoj.html

Ruby: // fork 块
来源：http://hz.jqgfzy.top/gtaxphmvhi.html

C#:   Parallel.For
来源：http://hz.smart0.xyz/gtfvznogql.html

================================================================================
来源：http://hz.cucudq.cn/gtpafcfirz.html

P. 常用工具函数
来源：http://hz.shzxlz.cn/gtnhuauydi.html

================================================================================
来源：http://hz.cucudq.cn/gtefplpbzq.html

[P01] 生成 UUID
来源：http://hz.wangdashe.top/gtixlpbsms.html

Py:   str(uuid.uuid4())
来源：http://hz.wangshuangyany.cn/gttgoojbpj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhoulong.xyz/gtcbnuuiqx.html

JS:   crypto.randomUUID()
来源：http://hz.hysaishi.cn/gtlbydfocq.html

TS:   crypto.randomUUID()
来源：http://hz.hongshengwenyu.top/gtowilfghj.html

Java: UUID.randomUUID().toString()
来源：http://hz.yangfankeji.com/gttiecsspi.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hongshengwenyu.top/gtumgsybag.html

Ruby: SecureRandom.uuid
来源：http://hz.shanyushiyangtech.top/gttwictajt.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xuanzx.com/gtkqighkhx.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ivvv.top/gtgumcvgil.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.daxiang520.top/gtlrqbxybh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ppjwa.cn/gtfvrometl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.wangdashe.top/gtvcawsawu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shangyingyoupin.top/gthqdvczko.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zdqjudy.top/gtwarozoow.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zdqjudy.top/gttxdywtbn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.havefunace.top/gtwtzmsbjf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.mhx1999.top/gtyiftomcn.html

[P03] 生成短随机字符串
来源：http://hz.dashuyun.cn/gtgzvayufl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jqgufenzy.top/gtrxgjvhmy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shuidangran.top/gtwnyuirsw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhixingplan.top/gtfmzrzvcx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jlsjyb.cn/gtlrxaojtk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ywan-chungtsiang.top/gtvdcccijm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.snrcjt.cn/gtbqmeqlbn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jlsjyb.cn/gthznsqmrd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.wangdashe.top/gtflusaydz.html

[P04] 求长度
来源：http://hz.hysaishi.cn/gtcrtrgpiz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.wangdashe.top/gtmpdyvhbj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cashguo.top/gttavyszsc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ehwqpu.com/gtkqndumdm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jqgufenzy.top/gtfbenxhzg.html

Java: list.size();  map.size();  s.length()
来源：http://hz.wangshuangyany.cn/gtmdtqvfbs.html

Go:   len(arr);  len(m)
来源：http://hz.meibo888.top/gtgbdctkfw.html

Ruby: x.length;  x.size
来源：http://hz.shzxlz.cn/gtdpiovumb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zdqjudy.top/gtvdjyixau.html

[P05] 判断两个对象内容是否相等
来源：http://hz.feifeiyinyue.top/gtsmflngog.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhijiandao.cn/gtoobwtqkq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yvedp.cn/gtzrfzaohu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yanxiufei.cn/gtrnqsigml.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.vqdsnc.cn/gtokrhndpk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yanxiufei.cn/gtqaaxwxcl.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.smart0.xyz/gtrosnjqaq.html

Ruby: a == b
来源：http://hz.haohaochexian.top/gtehbmexub.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yueranfly.top/gtmcwbltmk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hnxiangtu.top/gttqgzlaqc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.sysykeji.top/gtbdrftfgh.html

PHP:  if (empty($x)) {}
来源：http://hz.316326.xyz/gtzutbigrk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xuanzx.com/gtuwabtgaa.html

TS:   if (x == null) {}
来源：http://hz.nwbrower.top/gtaxwbcfxk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jqgfzy.top/gtyfoiyfrq.html

Go:   if x == nil {}
来源：http://hz.yonumen.top/gtnedrfypl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ppjwa.cn/gtkiiqhxim.html

C#:   if (x is null) {}
来源：http://hz.zhaomingkeji.xyz/gtwhqjzbpp.html

[P07] 防抖与节流
来源：http://hz.pengpengdd.cyou/gtdrlwnxgf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shanyushiyangkeji.top/gtoymwomla.html

PHP:  // 手写时间戳比较
来源：http://hz.xuanzx.com/gtqvkxcrpa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cdnleiting.top/gtiobbyhij.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gtawnpccpy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.havefunace.top/gtkjfodphd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.9152youxi.cn/gtaebfcfro.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.nwbrower.top/gtrjvlngpy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jianghu66.top/gtthkjoggl.html

[P08] 处理浮点精度问题
来源：http://hz.jinghuilouyu.cn/gtiqqqmpnn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.chenjidiqi.icu/gtwcerutkh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xuetiantiany.cn/gtixxldfay.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cucudq.cn/gtsaeuraeb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hongshengwenyu.top/gtegrrvsqi.html


<!-- 参考信息 -->