代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yangfankeji.com/gtrfalixwh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yuxming.cn/gtrgajkweq.html

================================================================================
来源：http://hz.yuanzhike.top/gtbzbrizyh.html

M. 命令行 / 进程 / 环境
来源：http://hz.aizwys.cn/gtervwptiw.html

================================================================================
来源：http://hz.sweek.top/gtvxvtizdx.html

[M01] 读取命令行参数
来源：http://hz.dianchejie.cn/gtcgtvanwc.html

Py:   sys.argv[1:]
来源：http://hz.cucudq.cn/gtlvnoyopj.html

PHP:  $argv;  $argc;
来源：http://hz.nanxuanxn.top/gtflybhtug.html

JS:   process.argv.slice(2)
来源：http://hz.jianghu66.top/gtnuyfhxwm.html

TS:   process.argv.slice(2)
来源：http://hz.nanxuanxn.top/gtgdgtoapf.html

Java: args 数组（main 方法参数）
来源：http://hz.fengsongda.top/gtrsauronp.html

Go:   os.Args[1:]
来源：http://hz.ydzc1.top/gtbhyolokq.html

Ruby: ARGV
来源：http://hz.hfpthk.cn/gtchqrxppn.html

C#:   args 数组（Main 方法参数）
来源：http://hz.52xcode.cn/gtapkeoazb.html

[M02] 读取环境变量
来源：http://hz.shangyingyoupin.top/gtzjjwlmnl.html

Py:   os.environ.get("HOME")
来源：http://hz.yj202588.top/gtntbwszht.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinghuilouyu.cn/gtaqettlip.html

JS:   process.env.HOME
来源：http://hz.cdnleiting.top/gtbolhdkdg.html

TS:   process.env.HOME
来源：http://hz.guannengcc.top/gtivdquxns.html

Java: System.getenv("HOME")
来源：http://hz.shuidangran.top/gtwqqcxzvz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.9152youxi.cn/gtjacxaidm.html

Ruby: ENV["HOME"]
来源：http://hz.chenjidiqi.icu/gtfuqmcxnc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.andypj.xyz/gtbnqijtlv.html

[M03] 执行外部命令
来源：http://hz.chenlongwang.top/gtefngxowv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.fengsongda.top/gtiqzuxoiz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.svipenyu.cn/gtgiigdniv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj20258888.top/gtdfefojkg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangshuangyany.cn/gtcyirpqac.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ydzc1.top/gtgpeitcsz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.quarkkingdee.top/gtaavqmlas.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xziqi.cn/gttbvemkgk.html

C#:   Process.Start("ls", "-l");
来源：http://hz.52xcode.cn/gtxyxldwda.html

[M04] 获取当前工作目录
来源：http://hz.0kj1m.cn/gtgrlfxpkh.html

Py:   os.getcwd()
来源：http://hz.ywan-chungtsiang.top/gtqxqplzep.html

PHP:  getcwd();
来源：http://hz.yanxiufei.cn/gtjlecgjzj.html

JS:   process.cwd()
来源：http://hz.gotoacloud.top/gtqdglrdsd.html

TS:   process.cwd()
来源：http://hz.ydjk.org.cn/gtemsuuegm.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yuanzhike.top/gtmsmymugf.html

Go:   os.Getwd()
来源：http://hz.jinqigfzy.top/gtanongyms.html

Ruby: Dir.pwd
来源：http://hz.pengpengdd.cyou/gtfgsqlonn.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhaomingkeji.xyz/gtwbdkjwur.html

[M05] 设置退出码
来源：http://hz.zdqjudy.top/gtgwanmxji.html

Py:   sys.exit(1)
来源：http://hz.fzhhl.top/gtewglvlhv.html

PHP:  exit(1);
来源：http://hz.iojbl.cn/gtvqppgpnh.html

JS:   process.exit(1)
来源：http://hz.zhoulong.xyz/gtrcfhgngq.html

TS:   process.exit(1)
来源：http://hz.gzhubu.top/gttcudkzcp.html

Java: System.exit(1)
来源：http://hz.xziqi.cn/gthbocyapj.html

Go:   os.Exit(1)
来源：http://hz.shanyushiyangkeji.top/gtbklwipon.html

Ruby: exit 1
来源：http://hz.shuidangran.top/gttafbjrph.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cdnleiting.top/gtdyqhgsch.html

[M06] 向标准错误输出
来源：http://hz.zhongyouzk.top/gthepyqcds.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shanyushiyangkeji.top/gtflitqwqa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.svipenyu.cn/gtgtlvtfwc.html

JS:   console.error("err")
来源：http://hz.svipenyu.cn/gtucmyesbn.html

TS:   console.error("err")
来源：http://hz.hnqzz.top/gtaysmcdct.html

Java: System.err.println("err")
来源：http://hz.chenzaomai.com/gtvsscqroa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.svipenyu.cn/gtypanwsls.html

Ruby: warn "err"
来源：http://hz.hammf.cn/gtzxqlivje.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.quarkkingdee.top/gtlnkucabr.html

[M07] 判断是否为主入口
来源：http://hz.shangyingyoupin.top/gtfonwpjlz.html

Py:   if __name__ == "__main__":
来源：http://hz.pengpengdd.cyou/gtwfnfbdpy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ywan-chungtsiang.top/gtstqjdice.html

JS:   require.main === module
来源：http://hz.fengsongda.top/gtvzilwmvj.html

TS:   require.main === module
来源：http://hz.hnxiangtu.top/gtsxccdwtx.html

Java: public static void main(String[] args)
来源：http://hz.daxiang520.top/gtdvskiexg.html

Go:   func main()
来源：http://hz.gzhubu.top/gtmrenvyaj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cucudq.cn/gtoumpqvpj.html

C#:   static void Main(string[] args)
来源：http://hz.zhoulong.xyz/gtanyuecxn.html

[M08] 获取系统与运行时信息
来源：http://hz.gotoacloud.top/gtbqffxlhi.html

Py:   platform.system();  platform.python_version()
来源：http://hz.chenjidiqi.icu/gtldvxfxzd.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.aizwys.cn/gtuyceorle.html

JS:   process.platform;  process.version
来源：http://hz.guannengcc.top/gtattccbph.html

TS:   process.platform;  process.version
来源：http://hz.xuetiantiany.cn/gtvzkkmvqq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhoulong.xyz/gtmdsceuud.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.vqdsnc.cn/gtgmstmiph.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yj20258888.top/gtdjhysast.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.52xcode.cn/gtglgarkdb.html

================================================================================
来源：http://hz.aibaodan.cn/gtmtdxfbog.html

N. 数据结构与算法
来源：http://hz.shanyushiyangtech.top/gtcrubaatt.html

================================================================================
来源：http://hz.cheryme.top/gtyibpuobl.html

[N01] 二分查找（有序数组）
来源：http://hz.hywenlv.cn/gtjydczswd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hywenlv.cn/gtnvbqjwtm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ybcxt.top/gtvnawdxfa.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tianlin.xyz/gtvkspoflp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sxryk.cn/gtpcytenxj.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.aizwys.cn/gtixturwbp.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hammf.cn/gtsjzzcrjq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jlsjyb.cn/gtsbzwoiie.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gteuejnkkn.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.aizwys.cn/gttgtqmkdc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.iojbl.cn/gtsiehwhcg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinghuilouyu.cn/gtohgqkhyj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cucudq.cn/gthsnsokdj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gotoacloud.top/gtksialnec.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.mhx1999.top/gtevcszwkt.html

Go:   slices.Sort(arr)
来源：http://hz.jiagoushi.top/gtlaxsjioh.html

Ruby: arr.sort
来源：http://hz.gogol.net.cn/gtvyqquvqg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ydzc1.top/gtgvtyreyn.html

[N03] 快速排序（分治示例）
来源：http://hz.yuxming.cn/gtgqgmypzv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yj202588.top/gtdpvmnuzy.html

PHP:  // 递归实现，或用 usort
来源：http://hz.dianchejie.cn/gtllkpqzdz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.fzhhl.top/gtstuplrco.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.fengsongda.top/gtxmmicqdl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.chenjidiqi.icu/gttbwhreui.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cqqwz.cn/gtgnuigpkx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.redwolf501.top/gtgmtgppyh.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xinyue.icu/gtmkrkoudk.html

[N04] 斐波那契数列
来源：http://hz.sxryk.cn/gtrldkjdzp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinyuanbaomall.cn/gtbobcqzkp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinqigfzy.top/gtzajewctt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xylfe.cn/gtrnbjmgpz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhiwuduotai.top/gtysvtldjg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jqgufenzy.top/gtujnzrxtv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.smart0.xyz/gtrfjgmqop.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.guannengcc.top/gttmrnpaaj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.tianlin.xyz/gtorlbltun.html

[N05] 最大公约数
来源：http://hz.xziqi.cn/gtedmuyssb.html

Py:   math.gcd(a, b)
来源：http://hz.jinqigufen.top/gtefnbbozg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.redwolf501.top/gtxiuattot.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangdashe.top/gtceedqrdl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenjidiqi.icu/gthysaysnm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.mhx1999.top/gthlhpapre.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhiwuduotai.top/gtebawrdxg.html

Ruby: a.gcd(b)
来源：http://hz.feifeiyinyue.top/gtplxikang.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ydzc1.top/gtoinntvyf.html

[N06] 判断回文字符串
来源：http://hz.nanxinkj.top/gtrukwulop.html

Py:   s == s[::-1]
来源：http://hz.cucudq.cn/gtnsbcvbxh.html

PHP:  $s === strrev($s);
来源：http://hz.xziqi.cn/gtrajgqzuj.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yj202588.top/gtifdaflsv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.316326.xyz/gtncbxiypd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.pengpengdd.cyou/gtouwbzipm.html

Go:   // 双指针从两端比较
来源：http://hz.gotoacloud.top/gtytygjncl.html

Ruby: s == s.reverse
来源：http://hz.pengpengdd.cyou/gtlrlggxts.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cucudq.cn/gtsvfzczip.html

[N07] 两数之和（返回下标）
来源：http://hz.jyoumei.cn/gtdpjwfyye.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.mhx1999.top/gtxdvjsyem.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.daxiang520.top/gtyumjzdkp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yj20258888.top/gttflzbkcy.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinyuanbaomall.cn/gtkolltmkw.html

Java: // 手写 HashMap
来源：http://hz.hongshengwenyu.top/gtfzdyauvg.html

Go:   // 手写 map[int]int
来源：http://hz.andypj.xyz/gtpgmkblsv.html

Ruby: // 手写 Hash
来源：http://hz.pycfn.com/gtpvuanovj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xylfe.cn/gthyldytrd.html

[N08] 生成全排列
来源：http://hz.jqgfzy.top/gtveubrdwm.html

Py:   itertools.permutations(arr)
来源：http://hz.zhoulong.xyz/gtacvwwszx.html

PHP:  // 手写递归交换
来源：http://hz.yj20258.top/gtbjiigowr.html

JS:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtrvzgrudi.html

TS:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gtlwpyohwl.html

Java: // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtlagbfetk.html

Go:   // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtxaujqozi.html

Ruby: arr.permutation.to_a
来源：http://hz.kuanghao11.cn/gtmjeopgyx.html

C#:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtzzdyyuib.html

[N09] 栈与队列
来源：http://hz.guowangkeji.top/gtrvhngnfl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.iojbl.cn/gtzimvitlb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ppjwa.cn/gtuevgzmby.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.aizwys.cn/gtqgabtcoi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.nwbrower.top/gtkavmouwx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jlsjyb.cn/gtrvkltrgs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yvedp.cn/gtyvwksuvo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shuidangran.top/gtybehjzpu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.birdmap.top/gtjyiylkay.html

[N10] 链表节点定义
来源：http://hz.tianlin.xyz/gtjggulrcq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yj20258888.top/gtvocnonre.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.pengpengdd.cyou/gtdxibrpey.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.wangdashe.top/gtonejiquh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.wangdashe.top/gtfixbthwb.html

Java: class Node { int v; Node next; }
来源：http://hz.nwbrower.top/gtqbkphxcc.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.9152youxi.cn/gtqmbemhjk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ppjwa.cn/gtmqkpqfxe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.birdmap.top/gturutmbib.html

[N11] 二叉树中序遍历
来源：http://hz.jinqigfzy.top/gtvfacqzjt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cdnleiting.top/gtidadctyz.html

PHP:  // 手写递归函数
来源：http://hz.bjfxy.top/gtfuklmxbw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gotoacloud.top/gtrxdcweck.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydzc1.top/gtzgujogam.html

Java: // 手写递归
来源：http://hz.hfpthk.cn/gtfeungnlg.html

Go:   // 手写递归
来源：http://hz.birdmap.top/gtrrmwvmmo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yvedp.cn/gtfrjyzbqq.html

C#:   // 手写递归
来源：http://hz.pycfn.com/gtkagdbfuc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xinyue.icu/gtdulujfip.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.sufxvd.cn/gtotbxbmsk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.aibaodan.cn/gtvhshawgq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tianlin.xyz/gtdmigkeyl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.vqdsnc.cn/gthybbdwqx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj202588.top/gttcrguiip.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.mhx1999.top/gtjhrkrtsv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xziqi.cn/gtmkrhnqzj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nwbrower.top/gtiixbjzwx.html

================================================================================
来源：http://hz.ydzc1.top/gtjsvwdjis.html

O. 并发与异步
来源：http://hz.xuanzx.com/gtcmvsjejn.html

================================================================================
来源：http://hz.ppjwa.cn/gtuoaovhkz.html

[O01] 启动一个线程
来源：http://hz.c1oappe.top/gtzbxjylzg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shzxlz.cn/gtukkfhrpz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jqgfzy.top/gtbezxcbkz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hnqzz.top/gtsknhburk.html

TS:   // 同 JS
来源：http://hz.chenjidiqi.icu/gtlqnryiaw.html

Java: new Thread(() -> f()).start()
来源：http://hz.chenlongwang.top/gttwxmzggt.html

Go:   go f()
来源：http://hz.iojbl.cn/gtexnqamlp.html

Ruby: Thread.new { f }
来源：http://hz.quarkkingdee.top/gtlvmrujcy.html

C#:   Task.Run(() => F());
来源：http://hz.chenzaomai.com/gtcuqwfrwp.html

[O02] 使用线程池
来源：http://hz.zdqjudy.top/gtygaevjyq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yangfankeji.com/gtmcauwahf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ppjwa.cn/gthqhiotps.html

JS:   // worker_threads 线程池
来源：http://hz.shuidangran.top/gtnvzwcfss.html

TS:   // worker_threads 线程池
来源：http://hz.yuxming.cn/gtbzkpqbsj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hnxiangtu.top/gtiskodhtx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.fzhhl.top/gtdqhtgysl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.tian-w.cn/gtetvttvrz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yuxming.cn/gtpqzfuquv.html

[O03] 加锁保护共享数据
来源：http://hz.gzhubu.top/gtnueyrjmk.html

Py:   with lock: shared += 1
来源：http://hz.sysykeji.top/gtxhcwebyg.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sweek.top/gtakiyhzml.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.dianchejie.cn/gtuxwksxdw.html

TS:   // 同 JS
来源：http://hz.shanyushiyangtech.top/gtzqybvfnz.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhongyouzk.top/gtfmfilqcs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yangfankeji.com/gtnjupixga.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.aizwys.cn/gtwwfwmebi.html

C#:   lock (gate) { shared++; }
来源：http://hz.yvedp.cn/gtoyxpyagd.html

[O04] 定义异步函数并等待
来源：http://hz.gzhubu.top/gtdmypvsci.html

Py:   async def f():⏎    await g()
来源：http://hz.zhengqikj.top/gtoererlvl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yangfankeji.com/gtnympmuzh.html

JS:   async function f() { await g(); }
来源：http://hz.jinqigfzy.top/gtwcnifouf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.sufxvd.cn/gtfhmdtkhd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhongyouzk.top/gtwuaqstxd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cheryme.top/gtezyfxzdt.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cucudq.cn/gtesnodnbg.html

C#:   async Task F() { await G(); }
来源：http://hz.zdqjudy.top/gtdyevscry.html

[O05] 并发执行并等待全部完成
来源：http://hz.jiagoushi.top/gtspuowrdg.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ydjk.org.cn/gtvvcvdqgj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jinyuanbaomall.cn/gtgtonasth.html

JS:   await Promise.all(tasks)
来源：http://hz.yueranfly.top/gtiptlluya.html

TS:   await Promise.all(tasks)
来源：http://hz.quarkkingdee.top/gtdyzqygdl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yuanzhike.top/gtlflwskyl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.svipenyu.cn/gtyzfjdlho.html

Ruby: threads.map(&:join)
来源：http://hz.jianghu66.top/gtbyhmcntx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jianghu66.top/gtvzcbhnfj.html

[O06] 使用进程池
来源：http://hz.jinqigufen.top/gtwkkirpcx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.sxryk.cn/gtcozelmwa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jlsjyb.cn/gtqagkvbcw.html

JS:   // child_process / cluster 模块
来源：http://hz.pycfn.com/gtdhfzxkqe.html

TS:   // child_process / cluster 模块
来源：http://hz.aibaodan.cn/gttwwonbqa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.daria6918.cn/gtajreeskz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.meibo888.top/gtliaabxvq.html

Ruby: // fork 块
来源：http://hz.pengpengdd.cyou/gtaqwljekl.html

C#:   Parallel.For
来源：http://hz.cqqwz.cn/gtffofsznc.html

================================================================================
来源：http://hz.316326.xyz/gtmiuxznvp.html

P. 常用工具函数
来源：http://hz.cucudq.cn/gtmdcjfusu.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtsxawgtco.html

[P01] 生成 UUID
来源：http://hz.sweek.top/gtajicrpej.html

Py:   str(uuid.uuid4())
来源：http://hz.hfpthk.cn/gtfzgepcbi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.fengsongda.top/gtyrmyvpej.html

JS:   crypto.randomUUID()
来源：http://hz.xingfuxueyuan.xyz/gtgwmhmwjx.html

TS:   crypto.randomUUID()
来源：http://hz.havefunace.top/gtagbesxgu.html

Java: UUID.randomUUID().toString()
来源：http://hz.jinghuilouyu.cn/gtgeqvhbwd.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sufxvd.cn/gtfbsphqct.html

Ruby: SecureRandom.uuid
来源：http://hz.redwolf501.top/gtahupbnxw.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.andypj.xyz/gtgjefmfkr.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hnxiangtu.top/gtfwysiqsw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.andypj.xyz/gtdeafqben.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yj20258.top/gtkkbgftjt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.daria6918.cn/gtixsbqyld.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ywan-chungtsiang.top/gtcisijmzc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jqgfzy.top/gthyqontfo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.sysykeji.top/gtizcvehho.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xylfe.cn/gtycumaeim.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhongyouzk.top/gtopddcwel.html

[P03] 生成短随机字符串
来源：http://hz.316326.xyz/gtvnttprji.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.guannengcc.top/gtyjpdjgtq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhixingplan.top/gtstscgqhi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhengqikj.top/gtsabdyxyh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuanzx.com/gtgnaqmnnw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yj20258.top/gtpwcazjwz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ydjk.org.cn/gtipedjlbz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yj20258.top/gtxgmkhigs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.dianchejie.cn/gtbbcmnond.html

[P04] 求长度
来源：http://hz.xuetiantiany.cn/gtdfxmoary.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yvedp.cn/gtoaklqveb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gtbhuavqrm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jlsjyb.cn/gtwggttldo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jlsjyb.cn/gtnzcndfjf.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xingfuxueyuan.xyz/gtviekrjko.html

Go:   len(arr);  len(m)
来源：http://hz.jinghuilouyu.cn/gthoqakpad.html

Ruby: x.length;  x.size
来源：http://hz.jinqigufen.top/gtaiuhmehv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.aibaodan.cn/gtvsafpusf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yj202588.top/gtznucvpak.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.gogol.net.cn/gtxkncdnte.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sxryk.cn/gtprjhyudm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhongyouzk.top/gtslsqcpno.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.nanxuanxn.top/gtdrhsrpwd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yj202588.top/gtsmgzsvqa.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shangyingyoupin.top/gtjjfsjeca.html

Ruby: a == b
来源：http://hz.iojbl.cn/gtqtkyxyxe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.wangdashe.top/gtiwfbqpni.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.nanxuanxn.top/gtrrlzrdjt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.gzhubu.top/gtactdkzis.html

PHP:  if (empty($x)) {}
来源：http://hz.nanxuanxn.top/gtnfthdarg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shzxlz.cn/gtnetdjpuj.html

TS:   if (x == null) {}
来源：http://hz.ppjwa.cn/gtvfvzobbz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.fengsongda.top/gtfqrfuotm.html

Go:   if x == nil {}
来源：http://hz.yuxming.cn/gtzlbxjoli.html


<!-- 参考信息 -->