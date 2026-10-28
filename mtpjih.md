代发 wailian999

Ruby: ARGV
来源：http://hz.birdmap.top/gtlfblgshu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.52xcode.cn/gtwrdtdppq.html

[M02] 读取环境变量
来源：http://hz.shanyushiyangkeji.top/gteykptonp.html

Py:   os.environ.get("HOME")
来源：http://hz.yonumen.top/gtuydfwzom.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ivvv.top/gtqyctwaip.html

JS:   process.env.HOME
来源：http://hz.yuanzhike.top/gthfsthqzd.html

TS:   process.env.HOME
来源：http://hz.nanxuanxn.top/gtlcdxdged.html

Java: System.getenv("HOME")
来源：http://hz.mhx1999.top/gtlyduhdaz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gogol.net.cn/gtcsoobfkt.html

Ruby: ENV["HOME"]
来源：http://hz.hysaishi.cn/gtzzyzefuj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xuanzx.com/gtivcahstf.html

[M03] 执行外部命令
来源：http://hz.dashuyun.cn/gtdfbrirkp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jqgufenzy.top/gtsgivnizh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yj202588.top/gtktuftotx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.nanxuanxn.top/gttpmojdfh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ywan-chungtsiang.top/gtqnlyjsgi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.chenzaomai.com/gtrwalccgp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.fzhhl.top/gtehjmbulj.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shuidangran.top/gtobsxkdai.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhengqikj.top/gtuvxbahnf.html

[M04] 获取当前工作目录
来源：http://hz.bjfxy.top/gtehfofawu.html

Py:   os.getcwd()
来源：http://hz.birdmap.top/gtvzgljshp.html

PHP:  getcwd();
来源：http://hz.chenjidiqi.icu/gtnstscumc.html

JS:   process.cwd()
来源：http://hz.xinyue.icu/gtmclwlqog.html

TS:   process.cwd()
来源：http://hz.smart0.xyz/gtktjykdjr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cucudq.cn/gtmpflojiu.html

Go:   os.Getwd()
来源：http://hz.meibo888.top/gtalkuzipf.html

Ruby: Dir.pwd
来源：http://hz.nanxinkj.top/gtrbbkemco.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.feifeiyinyue.top/gtxnuexahc.html

[M05] 设置退出码
来源：http://hz.cucudq.cn/gtxmolshlu.html

Py:   sys.exit(1)
来源：http://hz.sxryk.cn/gtvxnefvsl.html

PHP:  exit(1);
来源：http://hz.feifeiyinyue.top/gtfgeaolps.html

JS:   process.exit(1)
来源：http://hz.hysaishi.cn/gtpomlsznq.html

TS:   process.exit(1)
来源：http://hz.redwolf501.top/gtmvkluxjn.html

Java: System.exit(1)
来源：http://hz.chenjidiqi.icu/gtxmfzkiiy.html

Go:   os.Exit(1)
来源：http://hz.jianghu66.top/gtpptaduyr.html

Ruby: exit 1
来源：http://hz.316326.xyz/gtxkjejiac.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xuetiantiany.cn/gtrzcopzit.html

[M06] 向标准错误输出
来源：http://hz.zhengqikj.top/gtjsttujfd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yanxiufei.cn/gtqpnyyumu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.wangshuangyany.cn/gthmxldcyg.html

JS:   console.error("err")
来源：http://hz.jlsjyb.cn/gtfrfzbojn.html

TS:   console.error("err")
来源：http://hz.yangfankeji.com/gtbmcwnwwx.html

Java: System.err.println("err")
来源：http://hz.guannengcc.top/gtefauusnq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yonumen.top/gtvesvtrfd.html

Ruby: warn "err"
来源：http://hz.sufxvd.cn/gtfsbtlexv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.fengsongda.top/gtyqfvipjb.html

[M07] 判断是否为主入口
来源：http://hz.jinyuanbaomall.cn/gtwlktxlod.html

Py:   if __name__ == "__main__":
来源：http://hz.hywenlv.cn/gtyscacktt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhengqikj.top/gtzwshbfds.html

JS:   require.main === module
来源：http://hz.pycfn.com/gtpvnntpow.html

TS:   require.main === module
来源：http://hz.nwbrower.top/gtirtajhrp.html

Java: public static void main(String[] args)
来源：http://hz.guowangkeji.top/gtevbfnsyh.html

Go:   func main()
来源：http://hz.tian-w.cn/gtsnftcflx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.wangshuangyany.cn/gtapbloxfp.html

C#:   static void Main(string[] args)
来源：http://hz.nwbrower.top/gtlzjpsluc.html

[M08] 获取系统与运行时信息
来源：http://hz.svipenyu.cn/gtnzdlspkm.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinqigfzy.top/gtcpnlmegx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ppjwa.cn/gtykyvmswy.html

JS:   process.platform;  process.version
来源：http://hz.haohaochexian.top/gtbpdtfomz.html

TS:   process.platform;  process.version
来源：http://hz.bjfxy.top/gtmwlvxeyt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.wangdashe.top/gtxiexmuxt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yangfankeji.com/gtlehqocsi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.aibaodan.cn/gtmljaiqrc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ehwqpu.com/gtfjltwaqd.html

================================================================================
来源：http://hz.bjfxy.top/gtctkdfzwx.html

N. 数据结构与算法
来源：http://hz.xziqi.cn/gtpwqhkzmx.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtddkbxxnj.html

[N01] 二分查找（有序数组）
来源：http://hz.c1oappe.top/gtqvvmtque.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.wangdashe.top/gtxuqyvoaz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.pycfn.com/gtfdmpxpuq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhengqikj.top/gtlmimgcbk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aizwys.cn/gtbubbebmx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gzhubu.top/gthbgomucx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shuidangran.top/gtwkmiikto.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhiwuduotai.top/gtxglehsqb.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hnqzz.top/gtueppleti.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.redwolf501.top/gtjhglrajg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jqgufenzy.top/gtesbkvbbo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jiagoushi.top/gtgusfdeop.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinyuanbaomall.cn/gtswudppth.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtvinavbnv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.birdmap.top/gtwnefapkx.html

Go:   slices.Sort(arr)
来源：http://hz.tian-w.cn/gtmaruljah.html

Ruby: arr.sort
来源：http://hz.gzhubu.top/gtquxcvmnb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.0kj1m.cn/gtqpzbzzom.html

[N03] 快速排序（分治示例）
来源：http://hz.jlsjyb.cn/gtxzclwvmt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hnqzz.top/gtopfivmqi.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gzhubu.top/gtgphjoliy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shzxlz.cn/gtwymhmpus.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenzaomai.com/gtvznanifq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinqigufen.top/gtlbvplzpr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.wangdashe.top/gtdumakgkp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zdqjudy.top/gtxsndubxa.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cucudq.cn/gtazyeneeu.html

[N04] 斐波那契数列
来源：http://hz.zhaomingkeji.xyz/gtxgrzlmgu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258.top/gtckopgroo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhixingplan.top/gtroiccqyr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ydjk.org.cn/gtvhuksuhy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ydjk.org.cn/gtyaojjfws.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ivvv.top/gtrbdulvky.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.redwolf501.top/gtrgtecbci.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.chenjidiqi.icu/gtrlbhpnwm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.smart0.xyz/gtiyfaucro.html

[N05] 最大公约数
来源：http://hz.gaohongyu789.top/gtfzdvuwwz.html

Py:   math.gcd(a, b)
来源：http://hz.c1oappe.top/gtmkdqlaka.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.c1oappe.top/gtkmlyimrn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhengqikj.top/gtlhuaigff.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.c1oappe.top/gtlgctkiny.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jianghu66.top/gtrpktixlw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.gaohongyu789.top/gtaaxecmhj.html

Ruby: a.gcd(b)
来源：http://hz.cqqwz.cn/gtyphplbxb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.mhx1999.top/gtjjinesnl.html

[N06] 判断回文字符串
来源：http://hz.hfpthk.cn/gtiduxajbh.html

Py:   s == s[::-1]
来源：http://hz.yueranfly.top/gtbbgizydu.html

PHP:  $s === strrev($s);
来源：http://hz.yuxming.cn/gtkipvwfpt.html

JS:   s === [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gtnydvqkrb.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jiagoushi.top/gtdxiyxxwa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.smart0.xyz/gtbpzjzbuh.html

Go:   // 双指针从两端比较
来源：http://hz.ydjk.org.cn/gtuvfuxwna.html

Ruby: s == s.reverse
来源：http://hz.chenzaomai.com/gtlwjwcvvo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.birdmap.top/gtvgczrfsg.html

[N07] 两数之和（返回下标）
来源：http://hz.yonumen.top/gttijtsiow.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hysaishi.cn/gtleyqgcwr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.chenzaomai.com/gtmlowdjgy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.chenlongwang.top/gtbnzctjue.html

TS:   // 手写 Map<string, number>
来源：http://hz.hnqzz.top/gtpkhhzohn.html

Java: // 手写 HashMap
来源：http://hz.feifeiyinyue.top/gtrjfaxzmk.html

Go:   // 手写 map[int]int
来源：http://hz.xingfuxueyuan.xyz/gttpsisukh.html

Ruby: // 手写 Hash
来源：http://hz.nanxinkj.top/gtfqofncvu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.andypj.xyz/gtyyipvfxf.html

[N08] 生成全排列
来源：http://hz.bjfxy.top/gtsmrfiqcd.html

Py:   itertools.permutations(arr)
来源：http://hz.xingfuxueyuan.xyz/gtxtmhtpir.html

PHP:  // 手写递归交换
来源：http://hz.jinqigufen.top/gtmknjhbgm.html

JS:   // 手写回溯递归
来源：http://hz.bjfxy.top/gtmaoithzw.html

TS:   // 手写回溯递归
来源：http://hz.aibaodan.cn/gtgmhszhes.html

Java: // 手写回溯递归
来源：http://hz.jqgufenzy.top/gtaaxbljzu.html

Go:   // 手写回溯递归
来源：http://hz.yonumen.top/gtexpafngr.html

Ruby: arr.permutation.to_a
来源：http://hz.xinyue.icu/gtvvcvvrzj.html

C#:   // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtjkfkgntv.html

[N09] 栈与队列
来源：http://hz.yj20258888.top/gtheoelmrm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shanyushiyangtech.top/gtolmwuavp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.svipenyu.cn/gtfehgmwrg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zycfv.cn/gtmsvjdnfl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jyoumei.cn/gtwpwuqgoo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sysykeji.top/gtuqblkkvb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ywan-chungtsiang.top/gtvbhcwneh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.fengsongda.top/gtmardkzvz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.0kj1m.cn/gtbnwdecbk.html

[N10] 链表节点定义
来源：http://hz.yuxming.cn/gturduayvd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hammf.cn/gtzmndtqzp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.chenlongwang.top/gtrjzlqlih.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cqqwz.cn/gtnjnumldj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jyoumei.cn/gtnktzlloc.html

Java: class Node { int v; Node next; }
来源：http://hz.hfpthk.cn/gtljmkpsib.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.iojbl.cn/gtclphwigv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.kuanghao11.cn/gttllbtszw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xuetiantiany.cn/gtuoognqcy.html

[N11] 二叉树中序遍历
来源：http://hz.havefunace.top/gtinmqkjaw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.redwolf501.top/gtbmcsmpek.html

PHP:  // 手写递归函数
来源：http://hz.pengpengdd.cyou/gtkddybqqw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.wangshuangyany.cn/gtfizowwwh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.bjfxy.top/gtrbbhzfsm.html

Java: // 手写递归
来源：http://hz.316326.xyz/gtsjtcblrq.html

Go:   // 手写递归
来源：http://hz.nanxinkj.top/gtgwfuzvua.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.aibaodan.cn/gtrfnlgmzm.html

C#:   // 手写递归
来源：http://hz.ydjk.org.cn/gtgjfadojh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jyoumei.cn/gtqrfakfty.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinghuilouyu.cn/gtuoiaqzck.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.nwbrower.top/gtifatmxpe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tian-w.cn/gtgiauhkvn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yangfankeji.com/gtzxbbgrrh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nanxinkj.top/gtbadjwaft.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.cheryme.top/gtethbfrdr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.daria6918.cn/gtaunfleks.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.havefunace.top/gtuoxtwevr.html

================================================================================
来源：http://hz.wangdashe.top/gtlrxmgjqh.html

O. 并发与异步
来源：http://hz.quarkkingdee.top/gtxibdmlff.html

================================================================================
来源：http://hz.yj20258.top/gtekmueqfj.html

[O01] 启动一个线程
来源：http://hz.shzxlz.cn/gtjtektwds.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.birdmap.top/gtsckfpvjt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.aizwys.cn/gtpfghudyz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.meibo888.top/gtxufwhxhq.html

TS:   // 同 JS
来源：http://hz.zhaomingkeji.xyz/gteapeighg.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhaomingkeji.xyz/gtyiadtuuy.html

Go:   go f()
来源：http://hz.hnqzz.top/gtlkkyzdks.html

Ruby: Thread.new { f }
来源：http://hz.yvedp.cn/gtykencxdn.html

C#:   Task.Run(() => F());
来源：http://hz.fengsongda.top/gtbuecihcl.html

[O02] 使用线程池
来源：http://hz.jqgufenzy.top/gtqykobtos.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cashguo.top/gtdmoswtjo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yueranfly.top/gtqeprfznp.html

JS:   // worker_threads 线程池
来源：http://hz.yuanzhike.top/gtygzrgkuq.html

TS:   // worker_threads 线程池
来源：http://hz.feifeiyinyue.top/gtkszjtpud.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.0kj1m.cn/gtguxbzppd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.svipenyu.cn/gtshzkrlxp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yj20258888.top/gtwrnpoewe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.316326.xyz/gtfjrqlsme.html

[O03] 加锁保护共享数据
来源：http://hz.gotoacloud.top/gtellxgksm.html

Py:   with lock: shared += 1
来源：http://hz.hnqzz.top/gtgjwlvmuw.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.nanxuanxn.top/gtvnspovkg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hfpthk.cn/gtjbsgtuak.html

TS:   // 同 JS
来源：http://hz.pengpengdd.cyou/gtmlpekpqu.html

Java: synchronized (this) { shared++; }
来源：http://hz.shangyingyoupin.top/gtppeizayo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.dianchejie.cn/gtozltmqwx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.redwolf501.top/gtnqmndlgb.html

C#:   lock (gate) { shared++; }
来源：http://hz.316326.xyz/gtgjgqwdir.html

[O04] 定义异步函数并等待
来源：http://hz.tianlin.xyz/gtgpbjwhoa.html

Py:   async def f():⏎    await g()
来源：http://hz.jinqigfzy.top/gtcuwwmnkc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yuanzhike.top/gtynygzgyg.html

JS:   async function f() { await g(); }
来源：http://hz.havefunace.top/gtrgvjraqm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.bjfxy.top/gtdwjubcgt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sxryk.cn/gtuvucqmlb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jinghuilouyu.cn/gtmukzyarw.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cheryme.top/gtgoywzovd.html

C#:   async Task F() { await G(); }
来源：http://hz.ppjwa.cn/gtyyqpfvwq.html

[O05] 并发执行并等待全部完成
来源：http://hz.quarkkingdee.top/gthypkoqhd.html

Py:   asyncio.gather(*tasks)
来源：http://hz.guannengcc.top/gtkqxdfcrp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.sysykeji.top/gtfcjyynxv.html

JS:   await Promise.all(tasks)
来源：http://hz.cheryme.top/gtmxwysfxa.html

TS:   await Promise.all(tasks)
来源：http://hz.jianghu66.top/gtfnbnrqrm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.gogol.net.cn/gtysqavsnb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhiwuduotai.top/gtczbwaisc.html

Ruby: threads.map(&:join)
来源：http://hz.svipenyu.cn/gtpcuxiqas.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.9152youxi.cn/gtujbqgslc.html

[O06] 使用进程池
来源：http://hz.chenzaomai.com/gteseakmuu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shanyushiyangtech.top/gtrigwbhes.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ybcxt.top/gtluirotsr.html

JS:   // child_process / cluster 模块
来源：http://hz.ehwqpu.com/gtmzpuhcep.html

TS:   // child_process / cluster 模块
来源：http://hz.bjfxy.top/gtumynjghc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhongyouzk.top/gtzvjyppvs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shangyingyoupin.top/gtgtfokkfq.html

Ruby: // fork 块
来源：http://hz.yongpay.top/gtvqumrtgm.html

C#:   Parallel.For
来源：http://hz.yj202588.top/gtpbaqwlyl.html

================================================================================
来源：http://hz.tanke756.top/gtsijywcbs.html

P. 常用工具函数
来源：http://hz.meibo888.top/gtqjjwxata.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtblbnuazi.html

[P01] 生成 UUID
来源：http://hz.tian-w.cn/gtorrydpou.html

Py:   str(uuid.uuid4())
来源：http://hz.cashguo.top/gtbitegfds.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.fengsongda.top/gtfhmhfkaw.html

JS:   crypto.randomUUID()
来源：http://hz.chenjidiqi.icu/gterfwhpgl.html

TS:   crypto.randomUUID()
来源：http://hz.kuanghao11.cn/gtwktqeljp.html

Java: UUID.randomUUID().toString()
来源：http://hz.shzxlz.cn/gtdrbbynms.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shzxlz.cn/gtxicpadxa.html

Ruby: SecureRandom.uuid
来源：http://hz.zdqjudy.top/gtwnuqtkto.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.gotoacloud.top/gtqnzfjsfu.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xingfuxueyuan.xyz/gtnfkgiqpk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.aizwys.cn/gtvzcpniou.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jyoumei.cn/gtxksgmwsz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gotoacloud.top/gtlgykyhzp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jiagoushi.top/gtvgxgzhqq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhiwuduotai.top/gtqyorvdke.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.bjfxy.top/gtforlaabo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhengqikj.top/gtkwpbiefq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhijiandao.cn/gtbrwlneed.html

[P03] 生成短随机字符串
来源：http://hz.daria6918.cn/gtdiqnmlke.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yanxiufei.cn/gtsasxjwtp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zdqjudy.top/gtycsndayo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.iojbl.cn/gtexuaoqmm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shangyingyoupin.top/gtpjtbsktc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinqigfzy.top/gtsrkmdxkq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.chenlongwang.top/gtkqipppun.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.bjfxy.top/gtprwmjfpt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.aibaodan.cn/gtiglesntg.html

[P04] 求长度
来源：http://hz.cdnleiting.top/gtobkmnkap.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.316326.xyz/gtmdcdvwxk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cdnleiting.top/gtjvoixzqw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hywenlv.cn/gtjqggestd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.bjfxy.top/gtfngammzv.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yuxming.cn/gtfeaueaxo.html

Go:   len(arr);  len(m)
来源：http://hz.sufxvd.cn/gtkatvgbzo.html

Ruby: x.length;  x.size
来源：http://hz.haohaochexian.top/gtoknpvekw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zycfv.cn/gtchapqdne.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hnxiangtu.top/gttvpotcmz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhijiandao.cn/gtlmuuflas.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.chenzaomai.com/gtpjyhckha.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.iojbl.cn/gtvhudjytj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gaohongyu789.top/gtukzlbibl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.feifeiyinyue.top/gtaawdrqzj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.wangshuangyany.cn/gtzvhozsjk.html

Ruby: a == b
来源：http://hz.nanxuanxn.top/gtyrxdiamu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ehwqpu.com/gtesbrhohu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhoulong.xyz/gtpdzajukz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.cdnleiting.top/gtshgptilc.html

PHP:  if (empty($x)) {}
来源：http://hz.chenzaomai.com/gtpvuoqusi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jqgufenzy.top/gtywksqigg.html

TS:   if (x == null) {}
来源：http://hz.yj20258.top/gtlxzjydav.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.gaohongyu789.top/gtvawlylke.html

Go:   if x == nil {}
来源：http://hz.redwolf501.top/gtxpkqmumr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shuidangran.top/gtzbsqalci.html

C#:   if (x is null) {}
来源：http://hz.cdnleiting.top/gtusxtnxdl.html

[P07] 防抖与节流
来源：http://hz.zhengqikj.top/gtjrgubecx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xuanzx.com/gtwmnijwnl.html

PHP:  // 手写时间戳比较
来源：http://hz.yuxming.cn/gtqjrkhira.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gtnkjesrpm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinghuilouyu.cn/gtgdcozfur.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.tianlin.xyz/gtyjolkajd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jyoumei.cn/gtythnvgou.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hongshengwenyu.top/gtflyimynw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yangfankeji.com/gtvotyofoq.html

[P08] 处理浮点精度问题
来源：http://hz.gotoacloud.top/gtktkncuqf.html


<!-- 参考信息 -->