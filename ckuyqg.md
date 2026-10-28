代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ybcxt.top/gtrcxhfyup.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.aibaodan.cn/gtnfytktif.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.feifeiyinyue.top/gtcoazvqqk.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sysykeji.top/gtykbwncof.html

[M04] 获取当前工作目录
来源：http://hz.shanyushiyangkeji.top/gtblojouqh.html

Py:   os.getcwd()
来源：http://hz.jlsjyb.cn/gtsdjyutai.html

PHP:  getcwd();
来源：http://hz.bjfxy.top/gtyeaombtc.html

JS:   process.cwd()
来源：http://hz.yuanzhike.top/gtvaojmfmn.html

TS:   process.cwd()
来源：http://hz.haohaochexian.top/gtvzfgufqi.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xingfuxueyuan.xyz/gtxyluywhn.html

Go:   os.Getwd()
来源：http://hz.xylfe.cn/gtavwtiziu.html

Ruby: Dir.pwd
来源：http://hz.ywan-chungtsiang.top/gtezanpitb.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.quarkkingdee.top/gtylongslw.html

[M05] 设置退出码
来源：http://hz.tanke756.top/gtodnpngoo.html

Py:   sys.exit(1)
来源：http://hz.9152youxi.cn/gtycmxnloc.html

PHP:  exit(1);
来源：http://hz.gotoacloud.top/gthacuqbhz.html

JS:   process.exit(1)
来源：http://hz.9152youxi.cn/gtlbttqbod.html

TS:   process.exit(1)
来源：http://hz.yueranfly.top/gtksrecjzx.html

Java: System.exit(1)
来源：http://hz.pengpengdd.cyou/gtzixlbqni.html

Go:   os.Exit(1)
来源：http://hz.cheryme.top/gtrypwoobi.html

Ruby: exit 1
来源：http://hz.smart0.xyz/gtmvrsnuho.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.52xcode.cn/gtwuhuotnu.html

[M06] 向标准错误输出
来源：http://hz.chenjidiqi.icu/gteddwnlwx.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nwbrower.top/gtwqbbellx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jyoumei.cn/gtclujsylp.html

JS:   console.error("err")
来源：http://hz.xuetiantiany.cn/gtfeokquym.html

TS:   console.error("err")
来源：http://hz.hammf.cn/gtcqhzqntv.html

Java: System.err.println("err")
来源：http://hz.yj202588.top/gtjbqxhpuf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ybcxt.top/gtbikdlcch.html

Ruby: warn "err"
来源：http://hz.yj20258.top/gtgmxjlwrc.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jinqigufen.top/gtujcxhzfa.html

[M07] 判断是否为主入口
来源：http://hz.hywenlv.cn/gtzvvwbjhi.html

Py:   if __name__ == "__main__":
来源：http://hz.zdqjudy.top/gtdeqcpxat.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cashguo.top/gtowthayga.html

JS:   require.main === module
来源：http://hz.gaohongyu789.top/gtwljvpljk.html

TS:   require.main === module
来源：http://hz.yj20258.top/gtmwqhiffn.html

Java: public static void main(String[] args)
来源：http://hz.yangfankeji.com/gtkqbbmkfk.html

Go:   func main()
来源：http://hz.hysaishi.cn/gtiiuqeapm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zycfv.cn/gtbrjdstle.html

C#:   static void Main(string[] args)
来源：http://hz.yuxming.cn/gtnhaqmjlp.html

[M08] 获取系统与运行时信息
来源：http://hz.cashguo.top/gtjdsiyjgc.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shuidangran.top/gtbmvzmoky.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.316326.xyz/gtgjknwohd.html

JS:   process.platform;  process.version
来源：http://hz.xuetiantiany.cn/gtuyimupja.html

TS:   process.platform;  process.version
来源：http://hz.hfpthk.cn/gtuojesclp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gogol.net.cn/gtiasmmjgf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gzhubu.top/gttjkgkkju.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yj20258888.top/gtbwmmtwyy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cqqwz.cn/gtixpuuvge.html

================================================================================
来源：http://hz.yanxiufei.cn/gtpjtrrepq.html

N. 数据结构与算法
来源：http://hz.nanxinkj.top/gtnymmxipu.html

================================================================================
来源：http://hz.tanke756.top/gtvjiuwqbi.html

[N01] 二分查找（有序数组）
来源：http://hz.xuanzx.com/gtqjvpecrl.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jqgufenzy.top/gttvpjptxe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.havefunace.top/gtrzjjxycx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gotoacloud.top/gtwpyucfru.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.pengpengdd.cyou/gtsdwcqcyo.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ehwqpu.com/gtqwedoenz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.fengsongda.top/gtpiqudang.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.52xcode.cn/gtrgceesus.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xylfe.cn/gtslurqdbr.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jiagoushi.top/gtafqhikiv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gotoacloud.top/gtmkbeenfd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tian-w.cn/gtpypgnhyc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aizwys.cn/gtinornpza.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aizwys.cn/gtvtqgxnnt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.dashuyun.cn/gtmwyqeegs.html

Go:   slices.Sort(arr)
来源：http://hz.jlsjyb.cn/gtarypbjsj.html

Ruby: arr.sort
来源：http://hz.yuxming.cn/gtjhwnaspu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ehwqpu.com/gtepubmvxk.html

[N03] 快速排序（分治示例）
来源：http://hz.sufxvd.cn/gtjrfxjvdv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xinyue.icu/gtasdqkwwh.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gotoacloud.top/gtojpybmqx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guannengcc.top/gtdfiinpuf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tian-w.cn/gtexelxpeh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hnxiangtu.top/gtexqtxlur.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.gzhubu.top/gtndsbooai.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gaohongyu789.top/gtqrlfvbdi.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.andypj.xyz/gthufatqqr.html

[N04] 斐波那契数列
来源：http://hz.birdmap.top/gtpbqihfzu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.52xcode.cn/gtgtjywiaa.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.havefunace.top/gtmsswdbcs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pycfn.com/gtvtoijtdb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.vqdsnc.cn/gtmljvguin.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhengqikj.top/gtbbqiberj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sxryk.cn/gtbnaptotk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jqgufenzy.top/gtnppvkncm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hnqzz.top/gtoipayyyn.html

[N05] 最大公约数
来源：http://hz.pycfn.com/gtafwavsgu.html

Py:   math.gcd(a, b)
来源：http://hz.jlsjyb.cn/gtydcgpytb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.52xcode.cn/gthttaaxar.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.316326.xyz/gtaagptrqg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.smart0.xyz/gtfobqcqzg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zycfv.cn/gtavqziroo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yanxiufei.cn/gtvvrzzuiy.html

Ruby: a.gcd(b)
来源：http://hz.chenjidiqi.icu/gtfstbcxuv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xylfe.cn/gtxiwyvxwk.html

[N06] 判断回文字符串
来源：http://hz.yvedp.cn/gteqrtthjf.html

Py:   s == s[::-1]
来源：http://hz.jqgfzy.top/gthezoxifr.html

PHP:  $s === strrev($s);
来源：http://hz.yonumen.top/gtiipzrqjh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtgmjdgaxe.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hywenlv.cn/gtnjvhzjcd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shanyushiyangtech.top/gtuzbiqsyi.html

Go:   // 双指针从两端比较
来源：http://hz.cucudq.cn/gtimguacgp.html

Ruby: s == s.reverse
来源：http://hz.yongpay.top/gtllqraugi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shuidangran.top/gtvfbpoxvn.html

[N07] 两数之和（返回下标）
来源：http://hz.birdmap.top/gtuwzebext.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hammf.cn/gtmfgsthcj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.daxiang520.top/gtdodhbupd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sufxvd.cn/gtjkyakand.html

TS:   // 手写 Map<string, number>
来源：http://hz.chenjidiqi.icu/gtacljvcex.html

Java: // 手写 HashMap
来源：http://hz.jinghuilouyu.cn/gtqhxpsuwv.html

Go:   // 手写 map[int]int
来源：http://hz.zdqjudy.top/gtgbrsruqz.html

Ruby: // 手写 Hash
来源：http://hz.ivvv.top/gtucohziin.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hfpthk.cn/gtnqanjayi.html

[N08] 生成全排列
来源：http://hz.ivvv.top/gtuldlojpm.html

Py:   itertools.permutations(arr)
来源：http://hz.pengpengdd.cyou/gtjrhditsq.html

PHP:  // 手写递归交换
来源：http://hz.gogol.net.cn/gtzsmkoidt.html

JS:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtfnfmgzdy.html

TS:   // 手写回溯递归
来源：http://hz.hfpthk.cn/gthzcajupr.html

Java: // 手写回溯递归
来源：http://hz.0kj1m.cn/gtdpfcpxvd.html

Go:   // 手写回溯递归
来源：http://hz.xziqi.cn/gtdizozsqi.html

Ruby: arr.permutation.to_a
来源：http://hz.zhijiandao.cn/gtfnuwdnrt.html

C#:   // 手写回溯递归
来源：http://hz.bjfxy.top/gtdclypwvi.html

[N09] 栈与队列
来源：http://hz.jqgufenzy.top/gtmyidrthy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.guowangkeji.top/gtcvmiwmsf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yj202588.top/gtlormljfa.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.shuidangran.top/gttwbdwzha.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yongpay.top/gtmzosmsfj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinyuanbaomall.cn/gtyydfsmly.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yueranfly.top/gtomaztpwf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.smart0.xyz/gticmeqjep.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yj20258.top/gteitszsck.html

[N10] 链表节点定义
来源：http://hz.jqgufenzy.top/gtwdedaotf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.chenzaomai.com/gtnlzjusos.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yueranfly.top/gtgrktilgj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.chenlongwang.top/gtkpdonaza.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.haohaochexian.top/gtjcjrcjdl.html

Java: class Node { int v; Node next; }
来源：http://hz.quarkkingdee.top/gtukuyhkjc.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ivvv.top/gtmhwaytpf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jqgfzy.top/gtrcxdixbt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zdqjudy.top/gtdsxbfjtd.html

[N11] 二叉树中序遍历
来源：http://hz.fzhhl.top/gtrfpfmdan.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yuxming.cn/gtdwarfmhh.html

PHP:  // 手写递归函数
来源：http://hz.kuanghao11.cn/gtewzjndbc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinghuilouyu.cn/gtsxkutdyu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jianghu66.top/gtigxhargs.html

Java: // 手写递归
来源：http://hz.jinqigufen.top/gtysnzthot.html

Go:   // 手写递归
来源：http://hz.jinghuilouyu.cn/gtjwpzkznq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhongyouzk.top/gtlctjxdku.html

C#:   // 手写递归
来源：http://hz.zdqjudy.top/gtxfzcemxt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hnxiangtu.top/gtxrjnsoed.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.nanxinkj.top/gtszufxmbu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jianghu66.top/gtzaueayne.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.andypj.xyz/gtmodrkysv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhaomingkeji.xyz/gtoifvxvej.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.bjfxy.top/gtiaqvdtil.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hywenlv.cn/gtttpeutdd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cqqwz.cn/gtkrheduhd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cqqwz.cn/gtkjjuhlzl.html

================================================================================
来源：http://hz.nanxinkj.top/gtavhwyizq.html

O. 并发与异步
来源：http://hz.ppjwa.cn/gtbnorhmpa.html

================================================================================
来源：http://hz.andypj.xyz/gtilctzchy.html

[O01] 启动一个线程
来源：http://hz.xinyue.icu/gtvlacnyyc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shzxlz.cn/gtsnojuomt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.vqdsnc.cn/gtpaktrzhl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.birdmap.top/gtopsicykd.html

TS:   // 同 JS
来源：http://hz.zhongyouzk.top/gtoqmzmlbc.html

Java: new Thread(() -> f()).start()
来源：http://hz.sufxvd.cn/gtgxqizugp.html

Go:   go f()
来源：http://hz.hnqzz.top/gtlvnlfknf.html

Ruby: Thread.new { f }
来源：http://hz.shzxlz.cn/gttkydyzqv.html

C#:   Task.Run(() => F());
来源：http://hz.ydzc1.top/gtaqskyckp.html

[O02] 使用线程池
来源：http://hz.feifeiyinyue.top/gtbgfcevnw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.redwolf501.top/gtqfnukbon.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cucudq.cn/gtbuvfosed.html

JS:   // worker_threads 线程池
来源：http://hz.nanxuanxn.top/gtxhbcyfuj.html

TS:   // worker_threads 线程池
来源：http://hz.gotoacloud.top/gtsuonuhyt.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhongyouzk.top/gtyperunal.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xuanzx.com/gtetvgluzl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yuanzhike.top/gtedzsmcmc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.havefunace.top/gtobprlhfh.html

[O03] 加锁保护共享数据
来源：http://hz.sysykeji.top/gtzjxlqqdu.html

Py:   with lock: shared += 1
来源：http://hz.zycfv.cn/gtlrlmydbm.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.gzhubu.top/gtwelpedur.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xuetiantiany.cn/gtyuwjlyfg.html

TS:   // 同 JS
来源：http://hz.dianchejie.cn/gteczuaajn.html

Java: synchronized (this) { shared++; }
来源：http://hz.pengpengdd.cyou/gtarezemvp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.smart0.xyz/gtqizgngmv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.c1oappe.top/gtijxnxtlm.html

C#:   lock (gate) { shared++; }
来源：http://hz.jinyuanbaomall.cn/gtdwydyfyo.html

[O04] 定义异步函数并等待
来源：http://hz.snrcjt.cn/gthwibrwrp.html

Py:   async def f():⏎    await g()
来源：http://hz.haohaochexian.top/gtnjskxqdz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.mhx1999.top/gtcvsropvp.html

JS:   async function f() { await g(); }
来源：http://hz.yueranfly.top/gtgtyvcfey.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shangyingyoupin.top/gtuqdnomjw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ehwqpu.com/gthscobkhk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jiagoushi.top/gtiqklioob.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.andypj.xyz/gtqmatkial.html

C#:   async Task F() { await G(); }
来源：http://hz.chenzaomai.com/gtgkaytwog.html

[O05] 并发执行并等待全部完成
来源：http://hz.gotoacloud.top/gtinqoorqh.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ivvv.top/gtwlmttmkr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ybcxt.top/gtcihdevlb.html

JS:   await Promise.all(tasks)
来源：http://hz.yvedp.cn/gtkdutkftj.html

TS:   await Promise.all(tasks)
来源：http://hz.jinqigfzy.top/gtdpshdfhw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.nanxinkj.top/gtkgxeeimt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.9152youxi.cn/gtuwgkiwbn.html

Ruby: threads.map(&:join)
来源：http://hz.cashguo.top/gtyisrvxzn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shanyushiyangkeji.top/gteljvldrd.html

[O06] 使用进程池
来源：http://hz.hongshengwenyu.top/gtpzemuiau.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yonumen.top/gtnnftosir.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.9152youxi.cn/gtobokdqjb.html

JS:   // child_process / cluster 模块
来源：http://hz.zycfv.cn/gtccwombit.html

TS:   // child_process / cluster 模块
来源：http://hz.pycfn.com/gtvapkusgu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.guowangkeji.top/gtabcenqkt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.sxryk.cn/gtpbygjphf.html

Ruby: // fork 块
来源：http://hz.0kj1m.cn/gtuirebpzz.html

C#:   Parallel.For
来源：http://hz.ehwqpu.com/gtsjvcejip.html

================================================================================
来源：http://hz.nwbrower.top/gtbjvcdsrv.html

P. 常用工具函数
来源：http://hz.jqgfzy.top/gtmdyghwqm.html

================================================================================
来源：http://hz.jqgfzy.top/gtyyirqiuh.html

[P01] 生成 UUID
来源：http://hz.bjfxy.top/gtfnpprpri.html

Py:   str(uuid.uuid4())
来源：http://hz.jyoumei.cn/gthxpauzfp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.nanxinkj.top/gtgakkorvg.html

JS:   crypto.randomUUID()
来源：http://hz.hongshengwenyu.top/gtyhexhznp.html

TS:   crypto.randomUUID()
来源：http://hz.chenjidiqi.icu/gthgtfiulp.html

Java: UUID.randomUUID().toString()
来源：http://hz.pycfn.com/gtdqjlbmho.html

Go:   // 用 github.com/google/uuid
来源：http://hz.fzhhl.top/gtnshhffbg.html

Ruby: SecureRandom.uuid
来源：http://hz.zhengqikj.top/gtnekyoyih.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhixingplan.top/gtouapcqre.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhiwuduotai.top/gtjwcwqkay.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cashguo.top/gtfeieaedy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yangfankeji.com/gtrwzrlxdv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.tian-w.cn/gtuxmwwylw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.tianlin.xyz/gtciwefhke.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.quarkkingdee.top/gtynfqwmgq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.kuanghao11.cn/gtqslkvtiq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinyuanbaomall.cn/gtyiqhidgv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.mhx1999.top/gtsfxlngmf.html

[P03] 生成短随机字符串
来源：http://hz.ehwqpu.com/gtaucczkus.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.pengpengdd.cyou/gtmeymajeq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gotoacloud.top/gtifimnemq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shuidangran.top/gtsteiqvvz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258.top/gtmxoijsfk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yuxming.cn/gttscatecx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ivvv.top/gtwdmysuip.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.mhx1999.top/gtwegjopar.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhixingplan.top/gtcgssducq.html

[P04] 求长度
来源：http://hz.hywenlv.cn/gtrhemhmfz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shangyingyoupin.top/gtklwcrlcy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhongyouzk.top/gtwlcilbmy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xingfuxueyuan.xyz/gtirllguis.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dianchejie.cn/gtrdluyvoz.html

Java: list.size();  map.size();  s.length()
来源：http://hz.guowangkeji.top/gtgztvevco.html

Go:   len(arr);  len(m)
来源：http://hz.hysaishi.cn/gtannfnibv.html

Ruby: x.length;  x.size
来源：http://hz.zdqjudy.top/gtstaleztz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.dashuyun.cn/gtnnfhgmya.html

[P05] 判断两个对象内容是否相等
来源：http://hz.guowangkeji.top/gtqwrxlcxv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.feifeiyinyue.top/gtzqsxtiji.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zycfv.cn/gtszkhkvsv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.dianchejie.cn/gtshtzdjam.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yanxiufei.cn/gtdutnemhx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.guowangkeji.top/gtbqisncki.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cdnleiting.top/gtccdcujlr.html

Ruby: a == b
来源：http://hz.aizwys.cn/gtfpgcxnip.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.sweek.top/gtdqjmdrnz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hnxiangtu.top/gtqetcxrrr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.kuanghao11.cn/gthijzggbj.html

PHP:  if (empty($x)) {}
来源：http://hz.jqgfzy.top/gtadyrurvi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.vqdsnc.cn/gthobymivi.html

TS:   if (x == null) {}
来源：http://hz.sweek.top/gtvkugxojp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.nanxuanxn.top/gtugrllwpv.html

Go:   if x == nil {}
来源：http://hz.yanxiufei.cn/gtfwtncvfu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cdnleiting.top/gteyjblulg.html

C#:   if (x is null) {}
来源：http://hz.yj20258.top/gtnerbismv.html

[P07] 防抖与节流
来源：http://hz.pengpengdd.cyou/gtpmibaijh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.9152youxi.cn/gtxyjxkihf.html

PHP:  // 手写时间戳比较
来源：http://hz.wangshuangyany.cn/gtmbghetya.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhoulong.xyz/gtrmhdssuc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangtech.top/gtketuzwog.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ybcxt.top/gtaoyefikv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.fengsongda.top/gtznojijgn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.iojbl.cn/gtvbnslnfl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cucudq.cn/gtrmjrszue.html

[P08] 处理浮点精度问题
来源：http://hz.haohaochexian.top/gtsyhngvhv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.haohaochexian.top/gtltvwuitj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zycfv.cn/gtenpskeuc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.52xcode.cn/gtzkgkfybi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cheryme.top/gtbktixnfx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.haohaochexian.top/gtmuzgsywi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cqqwz.cn/gtcdgzmsyl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ehwqpu.com/gtambgfjle.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.gzhubu.top/gtothnnhzm.html

================================================================================
来源：http://hz.nwbrower.top/gtbnscurys.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yanxiufei.cn/gtbzmrotjt.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtdqqpveoj.html

[Q01] 创建表
来源：http://hz.yj202588.top/gtlvxxcgzs.html

CREATE TABLE users (
来源：http://hz.zhiwuduotai.top/gthkcfqitf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.meibo888.top/gtgqsnjitr.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xinyue.icu/gtsokuusiz.html

email VARCHAR(100) UNIQUE,
来源：http://hz.daxiang520.top/gtzhuhvoxy.html


<!-- 参考信息 -->