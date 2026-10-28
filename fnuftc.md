代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yuxming.cn/gtebcctdtn.html

Ruby: ENV["HOME"]
来源：http://hz.ppjwa.cn/gtocphlbfc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yvedp.cn/gtzizaccqt.html

[M03] 执行外部命令
来源：http://hz.hfpthk.cn/gtfotvpico.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hnqzz.top/gtjgggyhng.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ydjk.org.cn/gtompeegvn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.meibo888.top/gtjjierpev.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.sysykeji.top/gtdixavyee.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yueranfly.top/gtjisahhha.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tanke756.top/gtjrzdtjlc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.mhx1999.top/gtnextdwyp.html

C#:   Process.Start("ls", "-l");
来源：http://hz.svipenyu.cn/gtpflfypyc.html

[M04] 获取当前工作目录
来源：http://hz.jinghuilouyu.cn/gtzsffhzex.html

Py:   os.getcwd()
来源：http://hz.ehwqpu.com/gtbamezwnf.html

PHP:  getcwd();
来源：http://hz.yongpay.top/gtujjlktlk.html

JS:   process.cwd()
来源：http://hz.mhx1999.top/gtvdebacpb.html

TS:   process.cwd()
来源：http://hz.chenlongwang.top/gtvamyezgj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yj20258888.top/gtkfxwtnsl.html

Go:   os.Getwd()
来源：http://hz.jinyuanbaomall.cn/gtanibwvzr.html

Ruby: Dir.pwd
来源：http://hz.pengpengdd.cyou/gtpxlmjlkx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jinqigufen.top/gtptwhnnkc.html

[M05] 设置退出码
来源：http://hz.cheryme.top/gtgcnieutm.html

Py:   sys.exit(1)
来源：http://hz.gaohongyu789.top/gtegylzzjy.html

PHP:  exit(1);
来源：http://hz.vqdsnc.cn/gtxjtvivcu.html

JS:   process.exit(1)
来源：http://hz.0kj1m.cn/gtzqgwmphd.html

TS:   process.exit(1)
来源：http://hz.smart0.xyz/gtpwuqcezn.html

Java: System.exit(1)
来源：http://hz.wangdashe.top/gtxikiabws.html

Go:   os.Exit(1)
来源：http://hz.9152youxi.cn/gtjmdwadiz.html

Ruby: exit 1
来源：http://hz.jyoumei.cn/gtxovswjzg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.guannengcc.top/gtuyvaaycg.html

[M06] 向标准错误输出
来源：http://hz.jqgufenzy.top/gttfcngxmd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sxryk.cn/gteruhtvjx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenzaomai.com/gtyqpdecud.html

JS:   console.error("err")
来源：http://hz.jinyuanbaomall.cn/gterznbzsu.html

TS:   console.error("err")
来源：http://hz.gzhubu.top/gtvbgbkduk.html

Java: System.err.println("err")
来源：http://hz.yuanzhike.top/gtvfooamjh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hnqzz.top/gtgvdnsbdu.html

Ruby: warn "err"
来源：http://hz.zhixingplan.top/gtbkavpflw.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.316326.xyz/gtlodymgbx.html

[M07] 判断是否为主入口
来源：http://hz.iojbl.cn/gthoificcz.html

Py:   if __name__ == "__main__":
来源：http://hz.pengpengdd.cyou/gtmwcmwrzg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hysaishi.cn/gtjehdzlak.html

JS:   require.main === module
来源：http://hz.tanke756.top/gtpmyayehw.html

TS:   require.main === module
来源：http://hz.ydjk.org.cn/gtmjvpawlu.html

Java: public static void main(String[] args)
来源：http://hz.svipenyu.cn/gtgswwykuh.html

Go:   func main()
来源：http://hz.ppjwa.cn/gtjexmkxdx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.fzhhl.top/gttkyaenav.html

C#:   static void Main(string[] args)
来源：http://hz.tanke756.top/gtnpmqeqmt.html

[M08] 获取系统与运行时信息
来源：http://hz.daria6918.cn/gtjzdvcjxl.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhoulong.xyz/gtlvdszxxr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhaomingkeji.xyz/gtaoqtxerx.html

JS:   process.platform;  process.version
来源：http://hz.guowangkeji.top/gtwehzoilr.html

TS:   process.platform;  process.version
来源：http://hz.kuanghao11.cn/gtgkszescj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yongpay.top/gtgadrixgs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinqigufen.top/gtfspmgvtv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.fengsongda.top/gtiyqlclsa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sxryk.cn/gtiwxkqmxv.html

================================================================================
来源：http://hz.yj202588.top/gtefskqdgk.html

N. 数据结构与算法
来源：http://hz.shangyingyoupin.top/gtjhgkxlej.html

================================================================================
来源：http://hz.nanxuanxn.top/gtulmitzpc.html

[N01] 二分查找（有序数组）
来源：http://hz.zhixingplan.top/gtveehlowe.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhongyouzk.top/gtrgryphnr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jyoumei.cn/gtvmbfzseg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258888.top/gtibqqhuyq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnqzz.top/gtuzussvwb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.c1oappe.top/gtbvhzovbh.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jianghu66.top/gtuyxwwnvm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.quarkkingdee.top/gtsitznqen.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ydzc1.top/gtrcanvncs.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jinyuanbaomall.cn/gtbwahygfn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuetiantiany.cn/gtwngbilym.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sweek.top/gtmmadvkeb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangtech.top/gtywtyhvwp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yongpay.top/gtxqxhungq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.gzhubu.top/gtydcqnxlx.html

Go:   slices.Sort(arr)
来源：http://hz.yvedp.cn/gtxjpsygpa.html

Ruby: arr.sort
来源：http://hz.chenjidiqi.icu/gtxaqlpqmv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.kuanghao11.cn/gtahhyzass.html

[N03] 快速排序（分治示例）
来源：http://hz.jinghuilouyu.cn/gtscclycmg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.nanxinkj.top/gtklcjbxke.html

PHP:  // 递归实现，或用 usort
来源：http://hz.chenjidiqi.icu/gtemanoped.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuanzx.com/gttxqeqkmc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxinkj.top/gtxzehdmxh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zycfv.cn/gtdqzifjrx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yj20258888.top/gtgpjmacby.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.tian-w.cn/gtbrhqwjna.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jqgufenzy.top/gtkedollyg.html

[N04] 斐波那契数列
来源：http://hz.jinghuilouyu.cn/gtkuxnkomu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.feifeiyinyue.top/gthtsatggh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.chenjidiqi.icu/gtklvajdui.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.0kj1m.cn/gtwcnjxuxx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pycfn.com/gtxansrsia.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jinqigfzy.top/gtlfiqqkiz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jlsjyb.cn/gtmifveqrt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yuanzhike.top/gtzopwcgkq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hfpthk.cn/gtyvpbxorj.html

[N05] 最大公约数
来源：http://hz.52xcode.cn/gtyhdkhmrd.html

Py:   math.gcd(a, b)
来源：http://hz.tanke756.top/gtdubkgjih.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.dashuyun.cn/gtdxwlpnzt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ppjwa.cn/gtlzpaydgu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gtqhfefuck.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hnqzz.top/gtdmgvxahf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.dashuyun.cn/gtlqtzirnu.html

Ruby: a.gcd(b)
来源：http://hz.yuanzhike.top/gtpwewpzzu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gotoacloud.top/gtnqfkijvg.html

[N06] 判断回文字符串
来源：http://hz.hnqzz.top/gtzcrxymtv.html

Py:   s == s[::-1]
来源：http://hz.zhaomingkeji.xyz/gtxdmlssja.html

PHP:  $s === strrev($s);
来源：http://hz.zhiwuduotai.top/gtczxjhsvd.html

JS:   s === [...s].reverse().join("")
来源：http://hz.kuanghao11.cn/gtkyoksdxi.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gteygnofay.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.aizwys.cn/gtkugbhkjb.html

Go:   // 双指针从两端比较
来源：http://hz.pycfn.com/gtinlxglkm.html

Ruby: s == s.reverse
来源：http://hz.guowangkeji.top/gtxujuywip.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cucudq.cn/gtnlymrolg.html

[N07] 两数之和（返回下标）
来源：http://hz.zhengqikj.top/gthsfgmvfn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nanxuanxn.top/gtszbqkvri.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ehwqpu.com/gtiievituh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yuanzhike.top/gtxwugyxpg.html

TS:   // 手写 Map<string, number>
来源：http://hz.9152youxi.cn/gtpgxkftbk.html

Java: // 手写 HashMap
来源：http://hz.ppjwa.cn/gtbtespzui.html

Go:   // 手写 map[int]int
来源：http://hz.jiagoushi.top/gtbvqskwhq.html

Ruby: // 手写 Hash
来源：http://hz.yuxming.cn/gtmgzutgwv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.chenjidiqi.icu/gtscmujibu.html

[N08] 生成全排列
来源：http://hz.xingfuxueyuan.xyz/gtcdpnpinc.html

Py:   itertools.permutations(arr)
来源：http://hz.ivvv.top/gtvsolfxos.html

PHP:  // 手写递归交换
来源：http://hz.sysykeji.top/gtzifsufuc.html

JS:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtpawcaetc.html

TS:   // 手写回溯递归
来源：http://hz.yj202588.top/gtvywdmpql.html

Java: // 手写回溯递归
来源：http://hz.mhx1999.top/gtptcecfti.html

Go:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtcnjyzavf.html

Ruby: arr.permutation.to_a
来源：http://hz.316326.xyz/gtoglalqat.html

C#:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtoqkuyukq.html

[N09] 栈与队列
来源：http://hz.guowangkeji.top/gtskgumvud.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.guowangkeji.top/gtxaiowfsr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ehwqpu.com/gtglzikuvo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jlsjyb.cn/gtcdeymmup.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.52xcode.cn/gteyrdxaxo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.dashuyun.cn/gtbepjdzop.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.dashuyun.cn/gtaixnldzj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shangyingyoupin.top/gtlbkxpvur.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.aibaodan.cn/gtajbuxkcv.html

[N10] 链表节点定义
来源：http://hz.jiagoushi.top/gtmyrtpfez.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.nanxuanxn.top/gtfzohpibw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.c1oappe.top/gttdvirowk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xuanzx.com/gtpnwsyicx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.havefunace.top/gtrfvkugao.html

Java: class Node { int v; Node next; }
来源：http://hz.wangshuangyany.cn/gtinucadtg.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shangyingyoupin.top/gtfxfeitcr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.dianchejie.cn/gtrkngwxhe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zdqjudy.top/gtanegyorx.html

[N11] 二叉树中序遍历
来源：http://hz.aibaodan.cn/gtaqrndfir.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yanxiufei.cn/gtxqwqpyax.html

PHP:  // 手写递归函数
来源：http://hz.dashuyun.cn/gtyicuuquz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aibaodan.cn/gtlvnevqga.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guannengcc.top/gtulafxbii.html

Java: // 手写递归
来源：http://hz.ivvv.top/gthxuwhqwm.html

Go:   // 手写递归
来源：http://hz.52xcode.cn/gtcvfmxcyj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xuanzx.com/gtgfoflabd.html

C#:   // 手写递归
来源：http://hz.yanxiufei.cn/gtahcihsus.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shanyushiyangtech.top/gthnkhkzum.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hnxiangtu.top/gttjmtypdy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.tanke756.top/gtrwnpsbqr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinqigufen.top/gtsgfdtzll.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sufxvd.cn/gtkroewqhi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.vqdsnc.cn/gtlssttspj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.haohaochexian.top/gtsedqwycs.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.52xcode.cn/gtbhwyjkaf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yueranfly.top/gtakmhykzn.html

================================================================================
来源：http://hz.tianlin.xyz/gtfipfccca.html

O. 并发与异步
来源：http://hz.haohaochexian.top/gtkxmxtogz.html

================================================================================
来源：http://hz.sweek.top/gtahmgxkep.html

[O01] 启动一个线程
来源：http://hz.nwbrower.top/gtklitqxrv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.pycfn.com/gtsbildkao.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ppjwa.cn/gtrpoznjte.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.nanxuanxn.top/gtwvpbyxii.html

TS:   // 同 JS
来源：http://hz.guannengcc.top/gtcsyfknos.html

Java: new Thread(() -> f()).start()
来源：http://hz.ydzc1.top/gtqxfdwmpg.html

Go:   go f()
来源：http://hz.hnxiangtu.top/gttwjqouwc.html

Ruby: Thread.new { f }
来源：http://hz.zhongyouzk.top/gtjyynpirv.html

C#:   Task.Run(() => F());
来源：http://hz.zdqjudy.top/gtcwfbwxmu.html

[O02] 使用线程池
来源：http://hz.zhixingplan.top/gtfqnxbevw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.chenjidiqi.icu/gtjzievwsb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.c1oappe.top/gtgvrkqktv.html

JS:   // worker_threads 线程池
来源：http://hz.zycfv.cn/gtfbzvphxp.html

TS:   // worker_threads 线程池
来源：http://hz.zycfv.cn/gtjyrhrclm.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.wangshuangyany.cn/gtapiixjqt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.daria6918.cn/gtykuwvgtd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ydzc1.top/gtqrxyyjep.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yvedp.cn/gtrdsyeqfl.html

[O03] 加锁保护共享数据
来源：http://hz.hysaishi.cn/gtqnkpamyp.html

Py:   with lock: shared += 1
来源：http://hz.zhaomingkeji.xyz/gtdhixzkwo.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cucudq.cn/gtpebgdaeb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hnxiangtu.top/gtymqbbkpr.html

TS:   // 同 JS
来源：http://hz.redwolf501.top/gtkdlqkkde.html

Java: synchronized (this) { shared++; }
来源：http://hz.chenlongwang.top/gtpjwbisff.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yanxiufei.cn/gtzsfxzjed.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhengqikj.top/gtqqemudrq.html

C#:   lock (gate) { shared++; }
来源：http://hz.chenlongwang.top/gtleyheaoz.html

[O04] 定义异步函数并等待
来源：http://hz.c1oappe.top/gtduzbzouk.html

Py:   async def f():⏎    await g()
来源：http://hz.jqgfzy.top/gtdymddvom.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.52xcode.cn/gtlgwgjttl.html

JS:   async function f() { await g(); }
来源：http://hz.wangdashe.top/gtporzeirj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.svipenyu.cn/gtxainahmm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhengqikj.top/gtuppurkhi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jinqigufen.top/gttdhtysgr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hnxiangtu.top/gtgiwglvsb.html

C#:   async Task F() { await G(); }
来源：http://hz.c1oappe.top/gtqlmboxoz.html

[O05] 并发执行并等待全部完成
来源：http://hz.shangyingyoupin.top/gtjchmabyv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zdqjudy.top/gtgkmohnrn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.kuanghao11.cn/gtgzkcirmw.html

JS:   await Promise.all(tasks)
来源：http://hz.snrcjt.cn/gtxuekkgup.html

TS:   await Promise.all(tasks)
来源：http://hz.zhixingplan.top/gtgplvjbpp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.nanxuanxn.top/gtzowgjoyy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.gotoacloud.top/gtuuwtyrql.html

Ruby: threads.map(&:join)
来源：http://hz.gaohongyu789.top/gtmxxvbpvu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.chenjidiqi.icu/gtcqojmjcz.html

[O06] 使用进程池
来源：http://hz.aibaodan.cn/gtqjxjxmxf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.chenjidiqi.icu/gtcmkuwlxy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.chenlongwang.top/gtknipxpsh.html

JS:   // child_process / cluster 模块
来源：http://hz.xziqi.cn/gtefoyqnhh.html

TS:   // child_process / cluster 模块
来源：http://hz.zhaomingkeji.xyz/gtcozmsquq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.aibaodan.cn/gtfhsetgml.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.andypj.xyz/gtrxzijlje.html

Ruby: // fork 块
来源：http://hz.xylfe.cn/gtjswlgdbn.html

C#:   Parallel.For
来源：http://hz.zdqjudy.top/gtsujuwjtm.html

================================================================================
来源：http://hz.ppjwa.cn/gtnavgnrle.html

P. 常用工具函数
来源：http://hz.tanke756.top/gtbfxpulwb.html

================================================================================
来源：http://hz.yuxming.cn/gtywedgcvc.html

[P01] 生成 UUID
来源：http://hz.andypj.xyz/gtmziwlogx.html

Py:   str(uuid.uuid4())
来源：http://hz.ppjwa.cn/gtyhdwxtfr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yuxming.cn/gtekfpowuq.html

JS:   crypto.randomUUID()
来源：http://hz.tanke756.top/gthxlngugo.html

TS:   crypto.randomUUID()
来源：http://hz.tianlin.xyz/gtrsxgvunt.html

Java: UUID.randomUUID().toString()
来源：http://hz.yangfankeji.com/gtbllxmujt.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xylfe.cn/gtvmqxhmua.html

Ruby: SecureRandom.uuid
来源：http://hz.xingfuxueyuan.xyz/gtywgodzyw.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.meibo888.top/gtpxxtbzez.html

[P02] MD5 / SHA256 摘要
来源：http://hz.guannengcc.top/gtpioincvq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.9152youxi.cn/gtwesrwxfh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.chenzaomai.com/gtgpbhqbux.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.sufxvd.cn/gtyrxhbvmx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xylfe.cn/gtylmtcnun.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.sxryk.cn/gtkzoiuqub.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jianghu66.top/gtvwbonzcl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hongshengwenyu.top/gtpfayhynh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.birdmap.top/gtkrksfbqv.html

[P03] 生成短随机字符串
来源：http://hz.yanxiufei.cn/gtbxdmvkxy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yj20258.top/gtwmdtlukd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zycfv.cn/gtgujgsbyk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tianlin.xyz/gttkgdpczy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenzaomai.com/gtklbytoow.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gotoacloud.top/gtwwffnswp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.wangshuangyany.cn/gtpdsujvwg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhongyouzk.top/gtzkaltafc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.aizwys.cn/gtrkgfovbf.html

[P04] 求长度
来源：http://hz.feifeiyinyue.top/gtqggvxzpj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yuanzhike.top/gtyzxvunkt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gttklqoyzi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hammf.cn/gtlvihbrof.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yueranfly.top/gtzmoqugty.html

Java: list.size();  map.size();  s.length()
来源：http://hz.quarkkingdee.top/gtjasqteyv.html

Go:   len(arr);  len(m)
来源：http://hz.gaohongyu789.top/gtnzpndaph.html

Ruby: x.length;  x.size
来源：http://hz.zdqjudy.top/gtwvuzjsju.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.aibaodan.cn/gtbpkxebzc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.kuanghao11.cn/gtnzjxcpal.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.daria6918.cn/gtxoyvndhb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xylfe.cn/gtjfwaepyh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.meibo888.top/gtcxnbmfdw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.dashuyun.cn/gtawicqeai.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jqgufenzy.top/gtzjkuclxm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.sxryk.cn/gtkdcwhuzn.html

Ruby: a == b
来源：http://hz.xylfe.cn/gtrlpfvdoy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jyoumei.cn/gtejramthh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jinqigufen.top/gtqoneqvjx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.nanxuanxn.top/gtwbvkurdq.html

PHP:  if (empty($x)) {}
来源：http://hz.nanxinkj.top/gtacvhovjz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.svipenyu.cn/gtcbdiozai.html

TS:   if (x == null) {}
来源：http://hz.xuanzx.com/gtkgpeslbq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.kuanghao11.cn/gtkbilkzsa.html

Go:   if x == nil {}
来源：http://hz.iojbl.cn/gthygkzukl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shanyushiyangkeji.top/gtcubaalaw.html

C#:   if (x is null) {}
来源：http://hz.cdnleiting.top/gtavhcgygw.html

[P07] 防抖与节流
来源：http://hz.hywenlv.cn/gtxgztspcj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shzxlz.cn/gtkrrbginl.html

PHP:  // 手写时间戳比较
来源：http://hz.nanxinkj.top/gtoruqrcgy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhijiandao.cn/gthaqsnzkt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shuidangran.top/gtlpjkvtlr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.mhx1999.top/gticwowiog.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xingfuxueyuan.xyz/gtsdlfpvho.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jinyuanbaomall.cn/gtfugienru.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.sxryk.cn/gtmyhougjr.html

[P08] 处理浮点精度问题
来源：http://hz.ivvv.top/gtvcikbsvv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jqgufenzy.top/gtbnblnbcz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhixingplan.top/gtbunlzuxd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jinghuilouyu.cn/gtkjwiiomk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.smart0.xyz/gtrhtmpxig.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.haohaochexian.top/gtfzdfvawy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sysykeji.top/gtkmgeuwov.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.fengsongda.top/gtvnweduvx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhengqikj.top/gtmyzhobyx.html


<!-- 参考信息 -->