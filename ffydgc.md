代发 wailian999

JS:   process.argv.slice(2)
来源：http://hz.c1oappe.top/gtehcwewzy.html

TS:   process.argv.slice(2)
来源：http://hz.chenjidiqi.icu/gtljjjqbke.html

Java: args 数组（main 方法参数）
来源：http://hz.tian-w.cn/gtpzjoxwtt.html

Go:   os.Args[1:]
来源：http://hz.zhoulong.xyz/gtetqlbnlp.html

Ruby: ARGV
来源：http://hz.iojbl.cn/gtkgmcphcg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.guowangkeji.top/gtqntgqlhm.html

[M02] 读取环境变量
来源：http://hz.0kj1m.cn/gternreret.html

Py:   os.environ.get("HOME")
来源：http://hz.zhixingplan.top/gtzgbrvhyb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ydjk.org.cn/gtzwwpjtwq.html

JS:   process.env.HOME
来源：http://hz.yuxming.cn/gtutpadgsq.html

TS:   process.env.HOME
来源：http://hz.sxryk.cn/gtnybkjqbc.html

Java: System.getenv("HOME")
来源：http://hz.aibaodan.cn/gtrgqbhikg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yonumen.top/gtxkmwsbwy.html

Ruby: ENV["HOME"]
来源：http://hz.mhx1999.top/gtjpzhnfox.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shanyushiyangtech.top/gtycywbmmz.html

[M03] 执行外部命令
来源：http://hz.redwolf501.top/gtzyzlgmha.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.bjfxy.top/gtekoyowma.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hywenlv.cn/gtgqvawyif.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenlongwang.top/gtvarcljqw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yanxiufei.cn/gtagjuylvh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.tanke756.top/gtgzmjbqrc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hammf.cn/gthuawvubj.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.nanxinkj.top/gtgjgbxwzd.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ydzc1.top/gtsnitgmnl.html

[M04] 获取当前工作目录
来源：http://hz.jinghuilouyu.cn/gtmaxafggu.html

Py:   os.getcwd()
来源：http://hz.hfpthk.cn/gtkcktqtvp.html

PHP:  getcwd();
来源：http://hz.xuetiantiany.cn/gtxdackaur.html

JS:   process.cwd()
来源：http://hz.birdmap.top/gtypdswtmg.html

TS:   process.cwd()
来源：http://hz.jlsjyb.cn/gtmrymxklo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hongshengwenyu.top/gtfqhyycxv.html

Go:   os.Getwd()
来源：http://hz.yj202588.top/gtcxzeatgl.html

Ruby: Dir.pwd
来源：http://hz.nanxuanxn.top/gtglhwiybg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yanxiufei.cn/gtapyhkgna.html

[M05] 设置退出码
来源：http://hz.zhongyouzk.top/gtbdkpfoca.html

Py:   sys.exit(1)
来源：http://hz.aizwys.cn/gtnkzntqlu.html

PHP:  exit(1);
来源：http://hz.andypj.xyz/gtotsnrzfp.html

JS:   process.exit(1)
来源：http://hz.yj20258.top/gtrrlldffh.html

TS:   process.exit(1)
来源：http://hz.cqqwz.cn/gtuacrgojt.html

Java: System.exit(1)
来源：http://hz.gzhubu.top/gtbrqfoomp.html

Go:   os.Exit(1)
来源：http://hz.sxryk.cn/gtzjvzwxbx.html

Ruby: exit 1
来源：http://hz.guannengcc.top/gtvwzkrpyk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.316326.xyz/gtgdrsscuw.html

[M06] 向标准错误输出
来源：http://hz.tian-w.cn/gtvdayqgvx.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gotoacloud.top/gtawixsynx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jyoumei.cn/gtgagkhyil.html

JS:   console.error("err")
来源：http://hz.yuanzhike.top/gtfnoeoptc.html

TS:   console.error("err")
来源：http://hz.ppjwa.cn/gthniwkovr.html

Java: System.err.println("err")
来源：http://hz.ybcxt.top/gtxmbnsich.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.316326.xyz/gtagiypnkn.html

Ruby: warn "err"
来源：http://hz.fzhhl.top/gtkexyhwsx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.wangshuangyany.cn/gtdcyvaeyi.html

[M07] 判断是否为主入口
来源：http://hz.ehwqpu.com/gttbjixlue.html

Py:   if __name__ == "__main__":
来源：http://hz.nanxinkj.top/gtbcasgmyu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shangyingyoupin.top/gtisclmriw.html

JS:   require.main === module
来源：http://hz.jinqigfzy.top/gtazlzedoa.html

TS:   require.main === module
来源：http://hz.zhongyouzk.top/gtuebvlicf.html

Java: public static void main(String[] args)
来源：http://hz.ppjwa.cn/gtdhdommec.html

Go:   func main()
来源：http://hz.cdnleiting.top/gtktvwykan.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.wangdashe.top/gtslungibp.html

C#:   static void Main(string[] args)
来源：http://hz.gogol.net.cn/gtooahrtil.html

[M08] 获取系统与运行时信息
来源：http://hz.feifeiyinyue.top/gtngjspmbk.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xylfe.cn/gtokgwthal.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xziqi.cn/gtnkmcpfrv.html

JS:   process.platform;  process.version
来源：http://hz.nanxuanxn.top/gtltbxxsru.html

TS:   process.platform;  process.version
来源：http://hz.aibaodan.cn/gtpfdqgbqg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hammf.cn/gttbnmpnju.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinqigfzy.top/gtaiemihzz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.redwolf501.top/gtuhplgwxe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yuanzhike.top/gtgymvmlfm.html

================================================================================
来源：http://hz.hnqzz.top/gtyctuweeh.html

N. 数据结构与算法
来源：http://hz.hnxiangtu.top/gtpggekdgr.html

================================================================================
来源：http://hz.cdnleiting.top/gtybhuedgt.html

[N01] 二分查找（有序数组）
来源：http://hz.ybcxt.top/gtovmymaxm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yonumen.top/gthvjtkgnk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.52xcode.cn/gtezoeqzzn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxuanxn.top/gtfvwrktui.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cucudq.cn/gtktfbzqqi.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.tanke756.top/gtnlqbxinq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhengqikj.top/gtimpxzpvq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.dianchejie.cn/gtbhhbqzxr.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.dianchejie.cn/gtzjpttfnz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.daria6918.cn/gtscqrlmdj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yueranfly.top/gttximvxtj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shuidangran.top/gtdqavntum.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cqqwz.cn/gtovvqakvv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nwbrower.top/gtvcwvofwu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ehwqpu.com/gtjksssejb.html

Go:   slices.Sort(arr)
来源：http://hz.yj202588.top/gtywzlicph.html

Ruby: arr.sort
来源：http://hz.sxryk.cn/gtxlursjeh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinyuanbaomall.cn/gtyzvuzekq.html

[N03] 快速排序（分治示例）
来源：http://hz.jinqigfzy.top/gtobgeokou.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.c1oappe.top/gtymrxhwsi.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sysykeji.top/gtyhcdniph.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xziqi.cn/gtphvbqlwx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gtwallrrim.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shanyushiyangtech.top/gtqypcrqgt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.chenlongwang.top/gtbxxfrlzu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xuanzx.com/gtzgauvrxc.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.svipenyu.cn/gtrubxvzul.html

[N04] 斐波那契数列
来源：http://hz.ydjk.org.cn/gtlulorqet.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jqgfzy.top/gtvfjsbpcj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ppjwa.cn/gtysfztrpd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sxryk.cn/gtobicrzrv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shangyingyoupin.top/gtxgyxlqrz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shzxlz.cn/gthgyeuhji.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.quarkkingdee.top/gtvvdjzmex.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zycfv.cn/gtqgptiisc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.aizwys.cn/gtngrtqbai.html

[N05] 最大公约数
来源：http://hz.tianlin.xyz/gtnudaacka.html

Py:   math.gcd(a, b)
来源：http://hz.ehwqpu.com/gtlncuwony.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinqigfzy.top/gtcpvgpwlv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yongpay.top/gtrbcdffzy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.kuanghao11.cn/gtcronygvc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.fengsongda.top/gtlkwevyti.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.fengsongda.top/gtpxrklycw.html

Ruby: a.gcd(b)
来源：http://hz.pengpengdd.cyou/gtjekbouvw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hnqzz.top/gtvddgnvmt.html

[N06] 判断回文字符串
来源：http://hz.xuetiantiany.cn/gtqlyfuwzz.html

Py:   s == s[::-1]
来源：http://hz.yuanzhike.top/gtlaooydcf.html

PHP:  $s === strrev($s);
来源：http://hz.meibo888.top/gtmvbnqpkj.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sysykeji.top/gtwilywbhc.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtgokyltzq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cdnleiting.top/gthofmiipe.html

Go:   // 双指针从两端比较
来源：http://hz.meibo888.top/gtptnscnry.html

Ruby: s == s.reverse
来源：http://hz.nwbrower.top/gtsrhpdora.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.fzhhl.top/gtzaglaxao.html

[N07] 两数之和（返回下标）
来源：http://hz.chenjidiqi.icu/gtiabnngmw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zdqjudy.top/gtzihhjbqi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhijiandao.cn/gtlmmvbdsh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gogol.net.cn/gtdltxurbk.html

TS:   // 手写 Map<string, number>
来源：http://hz.cqqwz.cn/gtunfpfyke.html

Java: // 手写 HashMap
来源：http://hz.jyoumei.cn/gtaiatwzxl.html

Go:   // 手写 map[int]int
来源：http://hz.jinghuilouyu.cn/gtihjvfliw.html

Ruby: // 手写 Hash
来源：http://hz.nanxuanxn.top/gtvnwcewjq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.havefunace.top/gthhrvgoqd.html

[N08] 生成全排列
来源：http://hz.zhoulong.xyz/gtytwlqayq.html

Py:   itertools.permutations(arr)
来源：http://hz.snrcjt.cn/gtfshthwlz.html

PHP:  // 手写递归交换
来源：http://hz.guowangkeji.top/gtajvkmufc.html

JS:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtvfvlloqn.html

TS:   // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gtfyanlcjg.html

Java: // 手写回溯递归
来源：http://hz.snrcjt.cn/gtqzeifslk.html

Go:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtadaqrqzz.html

Ruby: arr.permutation.to_a
来源：http://hz.xuanzx.com/gttdjutuzq.html

C#:   // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gtsjemehoq.html

[N09] 栈与队列
来源：http://hz.snrcjt.cn/gtwydnymon.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.aibaodan.cn/gttmgkxwig.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.vqdsnc.cn/gtimmdsqak.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.daxiang520.top/gtbsfainri.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.tianlin.xyz/gtevlrgnnm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shanyushiyangkeji.top/gtxvyzaggd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.pengpengdd.cyou/gtknsiugax.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.quarkkingdee.top/gtnnutwqon.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.aibaodan.cn/gtzokibutd.html

[N10] 链表节点定义
来源：http://hz.9152youxi.cn/gthvwjlfgk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.aizwys.cn/gtjyfepldg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yvedp.cn/gtqnlxhrea.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cdnleiting.top/gtoarqbpsa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.nanxuanxn.top/gtgoznicww.html

Java: class Node { int v; Node next; }
来源：http://hz.shanyushiyangtech.top/gttuewbmgi.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.guannengcc.top/gtmxglqixd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shzxlz.cn/gtbfwnssjd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hongshengwenyu.top/gthdgsuyls.html

[N11] 二叉树中序遍历
来源：http://hz.yj20258888.top/gtxlejuhfp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shzxlz.cn/gtxkkpptmc.html

PHP:  // 手写递归函数
来源：http://hz.zhongyouzk.top/gtmongwlbk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fzhhl.top/gtrmudiamx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.svipenyu.cn/gtzrlikkxt.html

Java: // 手写递归
来源：http://hz.0kj1m.cn/gtkwbfnjih.html

Go:   // 手写递归
来源：http://hz.aibaodan.cn/gtgywtvtob.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.chenjidiqi.icu/gtchlumacv.html

C#:   // 手写递归
来源：http://hz.jinqigufen.top/gtiepmyfxl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.fengsongda.top/gtwgjhdnia.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yangfankeji.com/gtfzbphfci.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.tanke756.top/gtsgitvzgc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.316326.xyz/gtsxbmskmv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yanxiufei.cn/gtscptvbvc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenzaomai.com/gteogvxvwg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yj20258888.top/gtviebwxnv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhoulong.xyz/gtpebtbkit.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gzhubu.top/gtzqunslfm.html

================================================================================
来源：http://hz.jyoumei.cn/gtnxjmayqs.html

O. 并发与异步
来源：http://hz.zhixingplan.top/gtaakxfvds.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtmkxwedfy.html

[O01] 启动一个线程
来源：http://hz.jiagoushi.top/gttwjastaf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.aizwys.cn/gthbsmcqtg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gotoacloud.top/gtrmxepctx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gogol.net.cn/gtvleghqqk.html

TS:   // 同 JS
来源：http://hz.svipenyu.cn/gtjtejwefm.html

Java: new Thread(() -> f()).start()
来源：http://hz.kuanghao11.cn/gtgwgyhqjd.html

Go:   go f()
来源：http://hz.cashguo.top/gtdjsqcdte.html

Ruby: Thread.new { f }
来源：http://hz.zhengqikj.top/gtgdaypcyp.html

C#:   Task.Run(() => F());
来源：http://hz.xingfuxueyuan.xyz/gtbnrdevin.html

[O02] 使用线程池
来源：http://hz.zhengqikj.top/gtavqtfupl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sufxvd.cn/gtpjchwpzt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jqgfzy.top/gtpipcfwts.html

JS:   // worker_threads 线程池
来源：http://hz.snrcjt.cn/gtfqbrlazo.html

TS:   // worker_threads 线程池
来源：http://hz.nanxinkj.top/gtyalmgqva.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.birdmap.top/gtphfoerou.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yj20258888.top/gtovcizara.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.iojbl.cn/gtrtbchsde.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ydjk.org.cn/gtsrrqrzgh.html

[O03] 加锁保护共享数据
来源：http://hz.yonumen.top/gtgwjktqbb.html

Py:   with lock: shared += 1
来源：http://hz.haohaochexian.top/gtjrzxjlsj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.vqdsnc.cn/gtabxxbqhs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yonumen.top/gtpkjwcnzy.html

TS:   // 同 JS
来源：http://hz.xingfuxueyuan.xyz/gtnuveaboq.html

Java: synchronized (this) { shared++; }
来源：http://hz.zdqjudy.top/gtqhuvvhxe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.guowangkeji.top/gtgrdusxre.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhiwuduotai.top/gtausfkalb.html

C#:   lock (gate) { shared++; }
来源：http://hz.wangdashe.top/gtvcpsiyyb.html

[O04] 定义异步函数并等待
来源：http://hz.9152youxi.cn/gtizzseici.html

Py:   async def f():⏎    await g()
来源：http://hz.shanyushiyangtech.top/gtzvjwyryx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.fengsongda.top/gtnnhozcwh.html

JS:   async function f() { await g(); }
来源：http://hz.aibaodan.cn/gtcsfzwoeg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.gotoacloud.top/gtfeqokwka.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sweek.top/gtqkhzagka.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.daria6918.cn/gtoxokojbt.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gzhubu.top/gtiocqvopm.html

C#:   async Task F() { await G(); }
来源：http://hz.sxryk.cn/gteewtrpqw.html

[O05] 并发执行并等待全部完成
来源：http://hz.ywan-chungtsiang.top/gtkxxxesqy.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ydjk.org.cn/gtgsrohzwx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gotoacloud.top/gtgwzobljy.html

JS:   await Promise.all(tasks)
来源：http://hz.smart0.xyz/gtaogeypxb.html

TS:   await Promise.all(tasks)
来源：http://hz.ybcxt.top/gtdszxkroi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cheryme.top/gtpqdabdtz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xuetiantiany.cn/gtnzageftz.html

Ruby: threads.map(&:join)
来源：http://hz.quarkkingdee.top/gtlodjnzrj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.pengpengdd.cyou/gtkmvvtfoa.html

[O06] 使用进程池
来源：http://hz.redwolf501.top/gtkccawahq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hammf.cn/gtmgmkbgoo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hongshengwenyu.top/gtkkiygteu.html

JS:   // child_process / cluster 模块
来源：http://hz.yonumen.top/gtcltdrurb.html

TS:   // child_process / cluster 模块
来源：http://hz.xziqi.cn/gtpegpqjtk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhaomingkeji.xyz/gtyivqaluh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.daxiang520.top/gtrebpyuop.html

Ruby: // fork 块
来源：http://hz.chenzaomai.com/gtxpgbewgt.html

C#:   Parallel.For
来源：http://hz.gogol.net.cn/gtpqxuhvph.html

================================================================================
来源：http://hz.tian-w.cn/gtmrcjjjzl.html

P. 常用工具函数
来源：http://hz.yanxiufei.cn/gtbsvfcayv.html

================================================================================
来源：http://hz.tian-w.cn/gtxxzgibzb.html

[P01] 生成 UUID
来源：http://hz.c1oappe.top/gtpzkuauka.html

Py:   str(uuid.uuid4())
来源：http://hz.jqgfzy.top/gtilsbkvsi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.52xcode.cn/gtbmsfsuna.html

JS:   crypto.randomUUID()
来源：http://hz.pengpengdd.cyou/gtsmjqcezi.html

TS:   crypto.randomUUID()
来源：http://hz.yuxming.cn/gtvtwiyopz.html

Java: UUID.randomUUID().toString()
来源：http://hz.andypj.xyz/gtmttgxvzx.html

Go:   // 用 github.com/google/uuid
来源：http://hz.iojbl.cn/gtzajfzxbv.html

Ruby: SecureRandom.uuid
来源：http://hz.sweek.top/gtbtrgwozm.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yuxming.cn/gtmudutcny.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yangfankeji.com/gthrtfyiiz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zdqjudy.top/gtastbcxdy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.pycfn.com/gtdvibwaqt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yangfankeji.com/gtnfhzenob.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cdnleiting.top/gtooalatsy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cheryme.top/gtcxioiwms.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shanyushiyangtech.top/gtsyariqcu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.0kj1m.cn/gtupnrghvi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jlsjyb.cn/gttaclsfgh.html

[P03] 生成短随机字符串
来源：http://hz.xingfuxueyuan.xyz/gtdtsmhfna.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cdnleiting.top/gtilxnmyzp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cqqwz.cn/gthtcogeyg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.52xcode.cn/gtxudwtzlv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.9152youxi.cn/gtvyquthxw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jlsjyb.cn/gtbtiyztcq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.svipenyu.cn/gtqxyiggpo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.aizwys.cn/gthronkwed.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yuxming.cn/gtsqebousa.html

[P04] 求长度
来源：http://hz.haohaochexian.top/gttnnyclhz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jqgufenzy.top/gthlblfdia.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aizwys.cn/gtufzhatvw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gaohongyu789.top/gtdtmohcjd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.guowangkeji.top/gtllhqxysk.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yj20258888.top/gtjniculch.html

Go:   len(arr);  len(m)
来源：http://hz.xingfuxueyuan.xyz/gthfddremm.html

Ruby: x.length;  x.size
来源：http://hz.andypj.xyz/gtranbxwcf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jinqigufen.top/gtdmcobnuw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jyoumei.cn/gtooqvcoxt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xuetiantiany.cn/gtqhxacyzg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.aizwys.cn/gtcuqimzqf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.guowangkeji.top/gtlnaruaqe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.fzhhl.top/gtysngajgq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinqigufen.top/gtzigxwmek.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.dashuyun.cn/gtmvhnykxd.html

Ruby: a == b
来源：http://hz.zhixingplan.top/gtyaejojgn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.tanke756.top/gtbwstvbql.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hammf.cn/gtcmepaetn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhoulong.xyz/gtifayohqn.html

PHP:  if (empty($x)) {}
来源：http://hz.ybcxt.top/gtsoxodcdo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.gogol.net.cn/gtltvmobfv.html

TS:   if (x == null) {}
来源：http://hz.52xcode.cn/gtbmjndkpk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.chenlongwang.top/gtpkpkatqz.html

Go:   if x == nil {}
来源：http://hz.havefunace.top/gtvkfogdcb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.dashuyun.cn/gtijeoettd.html

C#:   if (x is null) {}
来源：http://hz.shuidangran.top/gtbfyrxvtj.html

[P07] 防抖与节流
来源：http://hz.ivvv.top/gtwqxwbzdf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.iojbl.cn/gtqjfzvwqc.html

PHP:  // 手写时间戳比较
来源：http://hz.xinyue.icu/gtqyzmqchw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sxryk.cn/gtxjiyfstt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuanzx.com/gtqhokgsfs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hammf.cn/gtitnrvivn.html


<!-- 参考信息 -->