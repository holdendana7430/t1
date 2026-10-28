代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.meibo888.top/gtdqygdbkh.html

JS:   process.env.HOME
来源：http://hz.wangshuangyany.cn/gtamhrbnse.html

TS:   process.env.HOME
来源：http://hz.zhiwuduotai.top/gtzqhkgsfs.html

Java: System.getenv("HOME")
来源：http://hz.havefunace.top/gtcvyhtvrz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hysaishi.cn/gtvojsvren.html

Ruby: ENV["HOME"]
来源：http://hz.jianghu66.top/gtftvwttnb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yongpay.top/gtjkxuksjy.html

[M03] 执行外部命令
来源：http://hz.fzhhl.top/gtkkhkokqh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zdqjudy.top/gtgqoedwqp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jqgufenzy.top/gtiegkweme.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.aibaodan.cn/gtncbdpmlo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gaohongyu789.top/gtukdfnnnf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.guannengcc.top/gtvzqcevuk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ehwqpu.com/gtldzrxemk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jyoumei.cn/gteqeoemdw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.aizwys.cn/gtzrozfubr.html

[M04] 获取当前工作目录
来源：http://hz.dianchejie.cn/gtaohudxea.html

Py:   os.getcwd()
来源：http://hz.shzxlz.cn/gtslzblkah.html

PHP:  getcwd();
来源：http://hz.hammf.cn/gtjwrhhftq.html

JS:   process.cwd()
来源：http://hz.zhaomingkeji.xyz/gtqynvxawa.html

TS:   process.cwd()
来源：http://hz.shanyushiyangkeji.top/gtwukjyege.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hnqzz.top/gtpjexwunu.html

Go:   os.Getwd()
来源：http://hz.hnqzz.top/gthawwzisp.html

Ruby: Dir.pwd
来源：http://hz.mhx1999.top/gtyjwvxrfs.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhongyouzk.top/gtskgfztcc.html

[M05] 设置退出码
来源：http://hz.jqgfzy.top/gtdobdkori.html

Py:   sys.exit(1)
来源：http://hz.jiagoushi.top/gtzurvhvoj.html

PHP:  exit(1);
来源：http://hz.yongpay.top/gtmjcfwkbu.html

JS:   process.exit(1)
来源：http://hz.hnqzz.top/gtrltdubyt.html

TS:   process.exit(1)
来源：http://hz.xuetiantiany.cn/gteynwyexq.html

Java: System.exit(1)
来源：http://hz.hnqzz.top/gtmcjtihee.html

Go:   os.Exit(1)
来源：http://hz.tanke756.top/gtjixscxrs.html

Ruby: exit 1
来源：http://hz.jinghuilouyu.cn/gtsretuiba.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.redwolf501.top/gtbmfgrzxg.html

[M06] 向标准错误输出
来源：http://hz.andypj.xyz/gtptalivfg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xingfuxueyuan.xyz/gtgppzwpje.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shuidangran.top/gtgzvloead.html

JS:   console.error("err")
来源：http://hz.zdqjudy.top/gtxjyofcrk.html

TS:   console.error("err")
来源：http://hz.hysaishi.cn/gtwnfbybfd.html

Java: System.err.println("err")
来源：http://hz.andypj.xyz/gtlckifjvw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.chenzaomai.com/gttutzglvk.html

Ruby: warn "err"
来源：http://hz.9152youxi.cn/gtqjioqhva.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.havefunace.top/gtyhyoqnan.html

[M07] 判断是否为主入口
来源：http://hz.iojbl.cn/gtovcvftnv.html

Py:   if __name__ == "__main__":
来源：http://hz.xingfuxueyuan.xyz/gtdrzxxgje.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yuxming.cn/gtjovlrqbr.html

JS:   require.main === module
来源：http://hz.shangyingyoupin.top/gtgdonfbhi.html

TS:   require.main === module
来源：http://hz.aizwys.cn/gtjrfvhlje.html

Java: public static void main(String[] args)
来源：http://hz.sweek.top/gtvtpizuyi.html

Go:   func main()
来源：http://hz.shangyingyoupin.top/gtwhimnnoe.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.tian-w.cn/gtixajzeul.html

C#:   static void Main(string[] args)
来源：http://hz.hnqzz.top/gtfoyrhenm.html

[M08] 获取系统与运行时信息
来源：http://hz.9152youxi.cn/gtdspgcduj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinyuanbaomall.cn/gtfbwipttw.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gaohongyu789.top/gtjersnupx.html

JS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtwtrcalwu.html

TS:   process.platform;  process.version
来源：http://hz.hysaishi.cn/gtysterxli.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ywan-chungtsiang.top/gtpbpsomlu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yueranfly.top/gtuagcenyi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.c1oappe.top/gtrvxywwog.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.andypj.xyz/gtefyygtzs.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtihijhrkn.html

N. 数据结构与算法
来源：http://hz.hammf.cn/gtbmuxferg.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtexuozpmy.html

[N01] 二分查找（有序数组）
来源：http://hz.bjfxy.top/gtvjdxoeyz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sysykeji.top/gtahkmwolm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.c1oappe.top/gtqoncgdgs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daxiang520.top/gtamzcfvyg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daxiang520.top/gtnpeovslq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jinqigufen.top/gtqrwotbzy.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.havefunace.top/gtvgralvfp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jqgufenzy.top/gtalfjbpmn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sufxvd.cn/gttvfnjelm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.nanxinkj.top/gtfftbrape.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cdnleiting.top/gtiufiohng.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ivvv.top/gtdayiqvaw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.mhx1999.top/gtbczyqdnw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cashguo.top/gtbotzzuxv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.feifeiyinyue.top/gtkxtgdqca.html

Go:   slices.Sort(arr)
来源：http://hz.wangdashe.top/gtgqcubbzl.html

Ruby: arr.sort
来源：http://hz.ybcxt.top/gtghkafylk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shzxlz.cn/gtvlcxntkp.html

[N03] 快速排序（分治示例）
来源：http://hz.sweek.top/gtugsplomm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.chenlongwang.top/gtsktmgury.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shanyushiyangtech.top/gtrapcgzss.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.smart0.xyz/gtyvoruqqn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuxming.cn/gtqaxgjtsd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj20258.top/gtuaqwtqml.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.guowangkeji.top/gtbaabnvjd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yongpay.top/gtaojpnisl.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.pengpengdd.cyou/gtykhapzmv.html

[N04] 斐波那契数列
来源：http://hz.smart0.xyz/gtymhcwrky.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.guannengcc.top/gtebdbskqw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.guannengcc.top/gtnjbofciw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xziqi.cn/gtshwsqypv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shuidangran.top/gtyimftkrm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cdnleiting.top/gtipqhmhfh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ybcxt.top/gtcddnslek.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ydzc1.top/gtdjotkejw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hongshengwenyu.top/gtixhditae.html

[N05] 最大公约数
来源：http://hz.ehwqpu.com/gtruufsrcr.html

Py:   math.gcd(a, b)
来源：http://hz.wangshuangyany.cn/gtwkncpawf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hnxiangtu.top/gtujiqslwv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aizwys.cn/gtteopycnt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guannengcc.top/gtkmocyksb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenzaomai.com/gtrchopufz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.daria6918.cn/gtwgjfrxbn.html

Ruby: a.gcd(b)
来源：http://hz.ivvv.top/gtkjtulnfx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.wangshuangyany.cn/gtwnfqxvku.html

[N06] 判断回文字符串
来源：http://hz.hongshengwenyu.top/gtlpyetxcp.html

Py:   s == s[::-1]
来源：http://hz.dianchejie.cn/gtpszzjhpx.html

PHP:  $s === strrev($s);
来源：http://hz.daria6918.cn/gtgsllhizc.html

JS:   s === [...s].reverse().join("")
来源：http://hz.havefunace.top/gtvsgvyqhz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtvsfvdfnu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.snrcjt.cn/gtoejpouro.html

Go:   // 双指针从两端比较
来源：http://hz.tanke756.top/gtegpdgglc.html

Ruby: s == s.reverse
来源：http://hz.hysaishi.cn/gtzmjpphpp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinyuanbaomall.cn/gtduovrfvx.html

[N07] 两数之和（返回下标）
来源：http://hz.sufxvd.cn/gtzqodayvn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.redwolf501.top/gtdefarjof.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yueranfly.top/gtpgdelcaa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shuidangran.top/gtdvgiqjfs.html

TS:   // 手写 Map<string, number>
来源：http://hz.daria6918.cn/gtgajchbao.html

Java: // 手写 HashMap
来源：http://hz.zhiwuduotai.top/gtalcbiqmc.html

Go:   // 手写 map[int]int
来源：http://hz.zycfv.cn/gtjrdatjas.html

Ruby: // 手写 Hash
来源：http://hz.cucudq.cn/gtpivdkiyi.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.iojbl.cn/gtcgsmxbxj.html

[N08] 生成全排列
来源：http://hz.wangshuangyany.cn/gtrtssbbkn.html

Py:   itertools.permutations(arr)
来源：http://hz.sweek.top/gtxocluwhn.html

PHP:  // 手写递归交换
来源：http://hz.nanxuanxn.top/gtkucilonx.html

JS:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtpqfuozju.html

TS:   // 手写回溯递归
来源：http://hz.ivvv.top/gtzpuggdou.html

Java: // 手写回溯递归
来源：http://hz.tianlin.xyz/gtdnamrcex.html

Go:   // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtvwaigknb.html

Ruby: arr.permutation.to_a
来源：http://hz.fengsongda.top/gtadmmojzm.html

C#:   // 手写回溯递归
来源：http://hz.cdnleiting.top/gtptixmzzc.html

[N09] 栈与队列
来源：http://hz.yueranfly.top/gtqtxvveei.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hongshengwenyu.top/gtnmwpivyv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.quarkkingdee.top/gtcqxcuomg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.fzhhl.top/gtgmwxgogg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jlsjyb.cn/gtqxnasmtp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.daxiang520.top/gtswxzgocb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.c1oappe.top/gtuaehyqhs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shanyushiyangtech.top/gttzvqtoum.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xingfuxueyuan.xyz/gtniwppark.html

[N10] 链表节点定义
来源：http://hz.cheryme.top/gtokghyacc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ehwqpu.com/gtwcsblfao.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhengqikj.top/gtjtbpmojp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.0kj1m.cn/gtavmtjgpp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.bjfxy.top/gtvrbgidgg.html

Java: class Node { int v; Node next; }
来源：http://hz.quarkkingdee.top/gtihibbway.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.guannengcc.top/gtbxxkskdn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jlsjyb.cn/gtsbilosnz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.sufxvd.cn/gtvwyowbmz.html

[N11] 二叉树中序遍历
来源：http://hz.zhengqikj.top/gteacrozvn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.mhx1999.top/gtesrsflku.html

PHP:  // 手写递归函数
来源：http://hz.guannengcc.top/gtsnohdguc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.52xcode.cn/gtebdaaemx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gaohongyu789.top/gtbfnbiidl.html

Java: // 手写递归
来源：http://hz.yj202588.top/gtbggmmiwy.html

Go:   // 手写递归
来源：http://hz.yuxming.cn/gtcrudinmt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.c1oappe.top/gtkpbljjrl.html

C#:   // 手写递归
来源：http://hz.yanxiufei.cn/gtixyqkdon.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.nanxinkj.top/gtlaiqarlw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.nanxuanxn.top/gtuszflbgh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.bjfxy.top/gtttxevcuh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sysykeji.top/gtczgkilua.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.svipenyu.cn/gtwwrxxpvm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xylfe.cn/gtswugzits.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.aizwys.cn/gtbybwacor.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xuetiantiany.cn/gtfbknzowl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.bjfxy.top/gtojomwpfi.html

================================================================================
来源：http://hz.9152youxi.cn/gtmoycdkfu.html

O. 并发与异步
来源：http://hz.guannengcc.top/gtzlceikpw.html

================================================================================
来源：http://hz.xziqi.cn/gtxognthuu.html

[O01] 启动一个线程
来源：http://hz.cheryme.top/gtsmzqdtjc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinqigfzy.top/gtzybduuuf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jqgfzy.top/gtsiuxvvfm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yueranfly.top/gtazfbvllq.html

TS:   // 同 JS
来源：http://hz.fengsongda.top/gthnzjauau.html

Java: new Thread(() -> f()).start()
来源：http://hz.yj20258888.top/gtbnppeqjp.html

Go:   go f()
来源：http://hz.wangdashe.top/gtgbdeavzj.html

Ruby: Thread.new { f }
来源：http://hz.xuetiantiany.cn/gthmtxeiac.html

C#:   Task.Run(() => F());
来源：http://hz.mhx1999.top/gtlognxqeg.html

[O02] 使用线程池
来源：http://hz.zdqjudy.top/gteszhggoy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.bjfxy.top/gtzoxbtwng.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.havefunace.top/gtzeejcsgn.html

JS:   // worker_threads 线程池
来源：http://hz.shanyushiyangkeji.top/gtvkekkyey.html

TS:   // worker_threads 线程池
来源：http://hz.0kj1m.cn/gtipendceb.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.gzhubu.top/gtcvesxbkn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.aibaodan.cn/gtiiddaaac.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hnxiangtu.top/gtclrjwedy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.guowangkeji.top/gtgddrnsss.html

[O03] 加锁保护共享数据
来源：http://hz.yueranfly.top/gtpqezdyyt.html

Py:   with lock: shared += 1
来源：http://hz.hnqzz.top/gtrfpljgsu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yanxiufei.cn/gtryyxdnrg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yonumen.top/gtamhzxhaz.html

TS:   // 同 JS
来源：http://hz.ybcxt.top/gtndruzgtg.html

Java: synchronized (this) { shared++; }
来源：http://hz.ydzc1.top/gtabyovcpj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hysaishi.cn/gtikgcczve.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.nanxinkj.top/gtfvjhimwo.html

C#:   lock (gate) { shared++; }
来源：http://hz.daxiang520.top/gtpxxcyxwl.html

[O04] 定义异步函数并等待
来源：http://hz.hnxiangtu.top/gtseplhucv.html

Py:   async def f():⏎    await g()
来源：http://hz.andypj.xyz/gtcolyzctz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xuanzx.com/gtlbtxcayw.html

JS:   async function f() { await g(); }
来源：http://hz.zhaomingkeji.xyz/gtakxbvkys.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shanyushiyangkeji.top/gtshdiqdjv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shanyushiyangkeji.top/gtrvxugzje.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ivvv.top/gthltkqsyi.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.nwbrower.top/gtryelpzxo.html

C#:   async Task F() { await G(); }
来源：http://hz.jinghuilouyu.cn/gtksvoovjh.html

[O05] 并发执行并等待全部完成
来源：http://hz.daria6918.cn/gtuskbinnz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ywan-chungtsiang.top/gtjkemechq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.haohaochexian.top/gtijcdpktt.html

JS:   await Promise.all(tasks)
来源：http://hz.hywenlv.cn/gtvusxhkjn.html

TS:   await Promise.all(tasks)
来源：http://hz.cdnleiting.top/gtjrpobawk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.pycfn.com/gtnqhmselz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.guannengcc.top/gtisltysve.html

Ruby: threads.map(&:join)
来源：http://hz.hywenlv.cn/gttiqcqdzv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.tanke756.top/gtajkuhlsz.html

[O06] 使用进程池
来源：http://hz.nanxuanxn.top/gthwcwddfg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xinyue.icu/gtspltkhwe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.daxiang520.top/gtbobwoxke.html

JS:   // child_process / cluster 模块
来源：http://hz.feifeiyinyue.top/gtbtwjgnkw.html

TS:   // child_process / cluster 模块
来源：http://hz.ppjwa.cn/gtkxiudino.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jqgufenzy.top/gtetanjpal.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ydzc1.top/gtallafkrd.html

Ruby: // fork 块
来源：http://hz.yangfankeji.com/gtoeaioucx.html

C#:   Parallel.For
来源：http://hz.nanxinkj.top/gtissasnoo.html

================================================================================
来源：http://hz.ppjwa.cn/gtfvemjypb.html

P. 常用工具函数
来源：http://hz.hywenlv.cn/gtnaxpahel.html

================================================================================
来源：http://hz.hnqzz.top/gtpxekknet.html

[P01] 生成 UUID
来源：http://hz.chenjidiqi.icu/gtvlcpubtr.html

Py:   str(uuid.uuid4())
来源：http://hz.wangshuangyany.cn/gtemyydvuv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jqgufenzy.top/gtknhkfonl.html

JS:   crypto.randomUUID()
来源：http://hz.cheryme.top/gtgzizddtx.html

TS:   crypto.randomUUID()
来源：http://hz.sufxvd.cn/gtaqdvlfgu.html

Java: UUID.randomUUID().toString()
来源：http://hz.xuetiantiany.cn/gtaudkrxle.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhixingplan.top/gtcjhjidbc.html

Ruby: SecureRandom.uuid
来源：http://hz.quarkkingdee.top/gtbdgpixci.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.nanxinkj.top/gtvivnxguv.html

[P02] MD5 / SHA256 摘要
来源：http://hz.fzhhl.top/gtipavlhcz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.feifeiyinyue.top/gttcwcdeha.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yuanzhike.top/gtmygigquh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hnxiangtu.top/gtkuyuhczd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hywenlv.cn/gtdhjpbvhy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.sysykeji.top/gtjbrhatsj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jinqigfzy.top/gtesalcqca.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.kuanghao11.cn/gtsnusowgp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cdnleiting.top/gtrikicbld.html

[P03] 生成短随机字符串
来源：http://hz.dianchejie.cn/gtwwgtsgbr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhengqikj.top/gtpobwzfpm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.svipenyu.cn/gtjgfxdwvh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.daria6918.cn/gttlmswnku.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.bjfxy.top/gtbezkhudu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yueranfly.top/gtgbmyuoiu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jinqigufen.top/gtxxdvaqcu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shuidangran.top/gtlkekyewz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.daxiang520.top/gtrmznmcem.html

[P04] 求长度
来源：http://hz.cucudq.cn/gtdvvsttln.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.pycfn.com/gtobulqayj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ydzc1.top/gtoaucpzfl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daxiang520.top/gtdpcsbkms.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhiwuduotai.top/gtqmkrywbp.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jinyuanbaomall.cn/gtwmtoxyyj.html

Go:   len(arr);  len(m)
来源：http://hz.hfpthk.cn/gtkvasbsah.html

Ruby: x.length;  x.size
来源：http://hz.sxryk.cn/gtzwqrxefi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yj202588.top/gtkvobbouq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shanyushiyangkeji.top/gtgqbxafta.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zycfv.cn/gtqfnffejv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhijiandao.cn/gtymofbilc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xziqi.cn/gtjijcbroh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.quarkkingdee.top/gtiwluipie.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.daxiang520.top/gtreysrwnn.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yuanzhike.top/gtcsdddqet.html

Ruby: a == b
来源：http://hz.cucudq.cn/gtujveehdc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.feifeiyinyue.top/gtwnftzykj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhixingplan.top/gtyldwowyv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.dianchejie.cn/gtftiirkgy.html

PHP:  if (empty($x)) {}
来源：http://hz.jinqigfzy.top/gtxfvmnnzi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhoulong.xyz/gtcnrithqv.html

TS:   if (x == null) {}
来源：http://hz.feifeiyinyue.top/gtvosgrakk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.mhx1999.top/gtbpkfhqow.html

Go:   if x == nil {}
来源：http://hz.hnxiangtu.top/gtpvewpfqi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jqgfzy.top/gtitnymmsg.html

C#:   if (x is null) {}
来源：http://hz.andypj.xyz/gtsyddodnw.html

[P07] 防抖与节流
来源：http://hz.xziqi.cn/gtkxyzwfql.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.bjfxy.top/gtliygnvpk.html

PHP:  // 手写时间戳比较
来源：http://hz.yuxming.cn/gtsdnxjfio.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zycfv.cn/gtnjbplhhp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.smart0.xyz/gtxocjywhs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jqgufenzy.top/gtgsguyapv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cheryme.top/gtnllpmdqk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.birdmap.top/gtaqyjeysw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cucudq.cn/gtvbojjsjm.html

[P08] 处理浮点精度问题
来源：http://hz.ppjwa.cn/gtxvgcrfbg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.9152youxi.cn/gtoovktiql.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ydzc1.top/gtauhlnqxj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jianghu66.top/gtwcggabhj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.9152youxi.cn/gtmflmljfa.html


<!-- 参考信息 -->