代发 wailian999

================================================================================
来源：http://hz.nanxinkj.top/gtdhgsinqd.html

[M01] 读取命令行参数
来源：http://hz.jinqigfzy.top/gtvscvfotz.html

Py:   sys.argv[1:]
来源：http://hz.ywan-chungtsiang.top/gtfemozsfr.html

PHP:  $argv;  $argc;
来源：http://hz.hysaishi.cn/gtajetijfn.html

JS:   process.argv.slice(2)
来源：http://hz.yj202588.top/gtvjsgqaxw.html

TS:   process.argv.slice(2)
来源：http://hz.guowangkeji.top/gtmqxdnrid.html

Java: args 数组（main 方法参数）
来源：http://hz.cqqwz.cn/gtwrmraded.html

Go:   os.Args[1:]
来源：http://hz.andypj.xyz/gtofyrxbzr.html

Ruby: ARGV
来源：http://hz.yanxiufei.cn/gtrqnfroej.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hnxiangtu.top/gtubrcslzd.html

[M02] 读取环境变量
来源：http://hz.ivvv.top/gtezxjthkm.html

Py:   os.environ.get("HOME")
来源：http://hz.cheryme.top/gtsbwatxuf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yonumen.top/gtgrbxkmov.html

JS:   process.env.HOME
来源：http://hz.ivvv.top/gtcyqefata.html

TS:   process.env.HOME
来源：http://hz.dashuyun.cn/gtuxfpibhd.html

Java: System.getenv("HOME")
来源：http://hz.shuidangran.top/gtqnljrzqt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.mhx1999.top/gtfxnicnxx.html

Ruby: ENV["HOME"]
来源：http://hz.yvedp.cn/gtfcxdcbjs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cqqwz.cn/gttantflgg.html

[M03] 执行外部命令
来源：http://hz.jiagoushi.top/gtiuqwwbln.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.pengpengdd.cyou/gtntdlpdqw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.52xcode.cn/gtgafzjlec.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.guannengcc.top/gtdegtbekb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cqqwz.cn/gtdvxqhrkp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zycfv.cn/gtnamtvnae.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cdnleiting.top/gtbotenngp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xylfe.cn/gtqloczqaq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.daxiang520.top/gtggrzwzcy.html

[M04] 获取当前工作目录
来源：http://hz.sufxvd.cn/gtsjsnbrqs.html

Py:   os.getcwd()
来源：http://hz.vqdsnc.cn/gtttvitpav.html

PHP:  getcwd();
来源：http://hz.0kj1m.cn/gtbeoezeue.html

JS:   process.cwd()
来源：http://hz.yj202588.top/gtavsnsmfh.html

TS:   process.cwd()
来源：http://hz.zhixingplan.top/gteumfqksz.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gaohongyu789.top/gtgbabpsxi.html

Go:   os.Getwd()
来源：http://hz.xingfuxueyuan.xyz/gtobxubbfs.html

Ruby: Dir.pwd
来源：http://hz.dashuyun.cn/gtewvjwofk.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jyoumei.cn/gtbzdfzqnh.html

[M05] 设置退出码
来源：http://hz.yanxiufei.cn/gtbyvydzad.html

Py:   sys.exit(1)
来源：http://hz.shuidangran.top/gtbjrhlcwy.html

PHP:  exit(1);
来源：http://hz.cucudq.cn/gtuijiennv.html

JS:   process.exit(1)
来源：http://hz.zycfv.cn/gtjxbvmttu.html

TS:   process.exit(1)
来源：http://hz.52xcode.cn/gtosptlhoh.html

Java: System.exit(1)
来源：http://hz.ivvv.top/gtkvyrgdut.html

Go:   os.Exit(1)
来源：http://hz.guannengcc.top/gtkypskbnb.html

Ruby: exit 1
来源：http://hz.jiagoushi.top/gtezwvasqb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jlsjyb.cn/gtovxhggqe.html

[M06] 向标准错误输出
来源：http://hz.zhiwuduotai.top/gthrzdzldb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.chenzaomai.com/gtbjivpvzs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ybcxt.top/gtzkgwykok.html

JS:   console.error("err")
来源：http://hz.gogol.net.cn/gtaffjbvob.html

TS:   console.error("err")
来源：http://hz.andypj.xyz/gtzpvmlwrl.html

Java: System.err.println("err")
来源：http://hz.guowangkeji.top/gtqnwahegd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.dianchejie.cn/gttaslvjts.html

Ruby: warn "err"
来源：http://hz.sufxvd.cn/gtniqhbxgg.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yj202588.top/gtaqryrith.html

[M07] 判断是否为主入口
来源：http://hz.shanyushiyangtech.top/gthfsbhjwd.html

Py:   if __name__ == "__main__":
来源：http://hz.quarkkingdee.top/gtqtdfnrps.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yueranfly.top/gtvqoikfja.html

JS:   require.main === module
来源：http://hz.gotoacloud.top/gtlosjkcdk.html

TS:   require.main === module
来源：http://hz.c1oappe.top/gtddmkrgtm.html

Java: public static void main(String[] args)
来源：http://hz.chenlongwang.top/gtsnihijjt.html

Go:   func main()
来源：http://hz.jinqigufen.top/gtqweutilz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ivvv.top/gtyahvenki.html

C#:   static void Main(string[] args)
来源：http://hz.mhx1999.top/gttkbdmhci.html

[M08] 获取系统与运行时信息
来源：http://hz.hfpthk.cn/gtzfthkrdr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cdnleiting.top/gturtsydra.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gogol.net.cn/gtmljrfgzt.html

JS:   process.platform;  process.version
来源：http://hz.ivvv.top/gtauzobqzt.html

TS:   process.platform;  process.version
来源：http://hz.daria6918.cn/gtktubpjty.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sxryk.cn/gtpzumjoxm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.nwbrower.top/gthbpfciln.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yongpay.top/gtecionkfu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.fengsongda.top/gtujskyqhy.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtwakzmxjb.html

N. 数据结构与算法
来源：http://hz.gogol.net.cn/gtlcxnogon.html

================================================================================
来源：http://hz.hnxiangtu.top/gtjcnjzpto.html

[N01] 二分查找（有序数组）
来源：http://hz.zhijiandao.cn/gtwtdbptle.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.pycfn.com/gtdwdkswub.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ppjwa.cn/gtffhthwlm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ehwqpu.com/gtdpxglfzv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aibaodan.cn/gtoxblqsec.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ydjk.org.cn/gtlyaipsna.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.meibo888.top/gthbcavdcv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yuanzhike.top/gtavbzmpou.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shanyushiyangtech.top/gttyxcoqti.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhaomingkeji.xyz/gtnzixtjqe.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj202588.top/gtjdvflysc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yangfankeji.com/gtefkejgvy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuetiantiany.cn/gttjlepyxh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aibaodan.cn/gtvoinpimt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.chenlongwang.top/gtdchajhmi.html

Go:   slices.Sort(arr)
来源：http://hz.cqqwz.cn/gtfeahkfkv.html

Ruby: arr.sort
来源：http://hz.redwolf501.top/gtorxrddiq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.aizwys.cn/gtzcyezkmt.html

[N03] 快速排序（分治示例）
来源：http://hz.yanxiufei.cn/gtboxqcvob.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.iojbl.cn/gtodbehljp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.havefunace.top/gtuzdhkvol.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guannengcc.top/gtlqaqcecd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dianchejie.cn/gtlrnzjgnz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.haohaochexian.top/gthkrazqcp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shuidangran.top/gtajpkbfva.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xylfe.cn/gttailhbbs.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhijiandao.cn/gtsyzppulm.html

[N04] 斐波那契数列
来源：http://hz.iojbl.cn/gtshqpckea.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hammf.cn/gtyotxmech.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.wangshuangyany.cn/gtokmcjwtl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.c1oappe.top/gtgjcfjdtw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.9152youxi.cn/gtrkrpylcl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jiagoushi.top/gtiivaphti.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhiwuduotai.top/gtnhqdbplx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigufen.top/gtjxvlnssr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hysaishi.cn/gtuuqogerx.html

[N05] 最大公约数
来源：http://hz.gogol.net.cn/gtdtpxiphz.html

Py:   math.gcd(a, b)
来源：http://hz.iojbl.cn/gtktqmhrfn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shanyushiyangkeji.top/gtpqjckdiy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhoulong.xyz/gtwlrwdvwm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhijiandao.cn/gtsdpkbrot.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.andypj.xyz/gtgolfbddh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.svipenyu.cn/gtxmmdqmnc.html

Ruby: a.gcd(b)
来源：http://hz.cqqwz.cn/gtjgrnigdl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jiagoushi.top/gtsknhcnqk.html

[N06] 判断回文字符串
来源：http://hz.wangdashe.top/gtgthjnodl.html

Py:   s == s[::-1]
来源：http://hz.jinghuilouyu.cn/gtkcodxbsv.html

PHP:  $s === strrev($s);
来源：http://hz.daxiang520.top/gthygznyti.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gtuwyibgwo.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtnrhvxvqw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cqqwz.cn/gtfyctplfi.html

Go:   // 双指针从两端比较
来源：http://hz.zdqjudy.top/gtamthzqjy.html

Ruby: s == s.reverse
来源：http://hz.havefunace.top/gthdhveadv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.vqdsnc.cn/gtstxavemw.html

[N07] 两数之和（返回下标）
来源：http://hz.yuanzhike.top/gttqhespwn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.dianchejie.cn/gtdiqunrel.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sysykeji.top/gtjyhyzzzc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinqigfzy.top/gtubmciane.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj20258.top/gtkcotlfar.html

Java: // 手写 HashMap
来源：http://hz.cqqwz.cn/gtjfzdqeha.html

Go:   // 手写 map[int]int
来源：http://hz.yuanzhike.top/gtsrkhamtz.html

Ruby: // 手写 Hash
来源：http://hz.hysaishi.cn/gtbddsskxi.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhaomingkeji.xyz/gtpoqitsik.html

[N08] 生成全排列
来源：http://hz.gaohongyu789.top/gtxhwnucwl.html

Py:   itertools.permutations(arr)
来源：http://hz.iojbl.cn/gtzmczhrkj.html

PHP:  // 手写递归交换
来源：http://hz.svipenyu.cn/gtkrxweimk.html

JS:   // 手写回溯递归
来源：http://hz.ivvv.top/gtsydzncdt.html

TS:   // 手写回溯递归
来源：http://hz.vqdsnc.cn/gthldsjldf.html

Java: // 手写回溯递归
来源：http://hz.meibo888.top/gtevrfepeo.html

Go:   // 手写回溯递归
来源：http://hz.jianghu66.top/gthntezhjk.html

Ruby: arr.permutation.to_a
来源：http://hz.tian-w.cn/gtjkufhlkn.html

C#:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtldveqjnd.html

[N09] 栈与队列
来源：http://hz.havefunace.top/gtqmpmakuw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xylfe.cn/gtlsrpnyxx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.dianchejie.cn/gtzcqdzvmc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.mhx1999.top/gtzqzrnyff.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.wangshuangyany.cn/gtpjznzqho.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hnqzz.top/gtcbtowwcb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hnxiangtu.top/gtjtzkjvfz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.gaohongyu789.top/gteycyqrnm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.quarkkingdee.top/gtnshwniad.html

[N10] 链表节点定义
来源：http://hz.jinyuanbaomall.cn/gtfjgtcitk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhoulong.xyz/gtemuxssdq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xinyue.icu/gtbrfnvpnz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.tian-w.cn/gtqqcprjgs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cashguo.top/gtghgfufaa.html

Java: class Node { int v; Node next; }
来源：http://hz.fengsongda.top/gtcrqutpvj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.c1oappe.top/gtsbpotfuj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xylfe.cn/gtzozxqcnw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shuidangran.top/gtucbpveok.html

[N11] 二叉树中序遍历
来源：http://hz.zhoulong.xyz/gtfkbcbidq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhaomingkeji.xyz/gtapajfpad.html

PHP:  // 手写递归函数
来源：http://hz.redwolf501.top/gtqkqxqmtk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guannengcc.top/gtpvuwrikd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jyoumei.cn/gttehkutab.html

Java: // 手写递归
来源：http://hz.jianghu66.top/gtwgdibeab.html

Go:   // 手写递归
来源：http://hz.zhongyouzk.top/gtzgfyejca.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhoulong.xyz/gtgxaktygq.html

C#:   // 手写递归
来源：http://hz.zycfv.cn/gtxxcnsgul.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hnxiangtu.top/gtvrebsvnb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinghuilouyu.cn/gtqdllrlic.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cdnleiting.top/gtntkrskfg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258888.top/gtttbrjlsx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cqqwz.cn/gtdbwhqfmn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guannengcc.top/gtjnzfdtkh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.dashuyun.cn/gtgbhzqpys.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ehwqpu.com/gtwfqzatuq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hywenlv.cn/gtrvukqtwb.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtrxgawbzn.html

O. 并发与异步
来源：http://hz.guowangkeji.top/gtpkldfqwd.html

================================================================================
来源：http://hz.c1oappe.top/gtzomcxlzk.html

[O01] 启动一个线程
来源：http://hz.zdqjudy.top/gtkhdaowwd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.pycfn.com/gtgistvpqb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gzhubu.top/gtkxtaaxdm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.9152youxi.cn/gtapfoouco.html

TS:   // 同 JS
来源：http://hz.bjfxy.top/gtbxomiuin.html

Java: new Thread(() -> f()).start()
来源：http://hz.aibaodan.cn/gtiuwodcep.html

Go:   go f()
来源：http://hz.hammf.cn/gtgijbpfoz.html

Ruby: Thread.new { f }
来源：http://hz.shangyingyoupin.top/gtnwhstxnn.html

C#:   Task.Run(() => F());
来源：http://hz.shanyushiyangtech.top/gtrdsvivmw.html

[O02] 使用线程池
来源：http://hz.svipenyu.cn/gtzuwghmlw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.snrcjt.cn/gtkswmdjcy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cqqwz.cn/gtodyqcoux.html

JS:   // worker_threads 线程池
来源：http://hz.bjfxy.top/gthotvbskl.html

TS:   // worker_threads 线程池
来源：http://hz.pengpengdd.cyou/gtkyfybseo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xylfe.cn/gtuvayvwop.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhengqikj.top/gtkkrjgjkv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhongyouzk.top/gtqgafskik.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.0kj1m.cn/gtzltqtqzg.html

[O03] 加锁保护共享数据
来源：http://hz.zdqjudy.top/gtnflzvnda.html

Py:   with lock: shared += 1
来源：http://hz.yj20258.top/gtlxbaoldr.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yvedp.cn/gtopcsxjum.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yueranfly.top/gtusaztvij.html

TS:   // 同 JS
来源：http://hz.zhoulong.xyz/gtmanwwwzf.html

Java: synchronized (this) { shared++; }
来源：http://hz.ydzc1.top/gthvgnlbdb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yj20258.top/gtdcwcpoom.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.aibaodan.cn/gtonlmlcnv.html

C#:   lock (gate) { shared++; }
来源：http://hz.hysaishi.cn/gtyyduxntz.html

[O04] 定义异步函数并等待
来源：http://hz.yj202588.top/gtaqnvoeki.html

Py:   async def f():⏎    await g()
来源：http://hz.jianghu66.top/gtdamuqtwh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hywenlv.cn/gtzwhnbcnv.html

JS:   async function f() { await g(); }
来源：http://hz.yuxming.cn/gtpeymcalm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.mhx1999.top/gtdbwxnfzk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.52xcode.cn/gtiypusbku.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhiwuduotai.top/gtfzzmwozv.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shzxlz.cn/gtarkthxhr.html

C#:   async Task F() { await G(); }
来源：http://hz.guowangkeji.top/gtbmmeewmg.html

[O05] 并发执行并等待全部完成
来源：http://hz.wangdashe.top/gtgfqwiijr.html

Py:   asyncio.gather(*tasks)
来源：http://hz.9152youxi.cn/gtbzzckqne.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xuetiantiany.cn/gtfpxxfidi.html

JS:   await Promise.all(tasks)
来源：http://hz.jlsjyb.cn/gtyebsdvom.html

TS:   await Promise.all(tasks)
来源：http://hz.jinyuanbaomall.cn/gtbddgccii.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xinyue.icu/gtnnwnboqg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.wangshuangyany.cn/gtazexeere.html

Ruby: threads.map(&:join)
来源：http://hz.snrcjt.cn/gtuylgqdbw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ybcxt.top/gtzjewvrrv.html

[O06] 使用进程池
来源：http://hz.nanxinkj.top/gtwucdmvjo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhiwuduotai.top/gtkwslnwxi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hongshengwenyu.top/gtjdvhdsgd.html

JS:   // child_process / cluster 模块
来源：http://hz.hywenlv.cn/gtpcrfbxzu.html

TS:   // child_process / cluster 模块
来源：http://hz.sxryk.cn/gtubdhpcsp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.52xcode.cn/gtkjdpawbu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.svipenyu.cn/gthkqsbzor.html

Ruby: // fork 块
来源：http://hz.zhiwuduotai.top/gtnyyafiya.html

C#:   Parallel.For
来源：http://hz.hnxiangtu.top/gtemqajdnh.html

================================================================================
来源：http://hz.svipenyu.cn/gtgcmjrmud.html

P. 常用工具函数
来源：http://hz.yuanzhike.top/gtdmctwzac.html

================================================================================
来源：http://hz.shzxlz.cn/gtcuhdigsh.html

[P01] 生成 UUID
来源：http://hz.hfpthk.cn/gtshbpzgwg.html

Py:   str(uuid.uuid4())
来源：http://hz.meibo888.top/gtswwduala.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xuetiantiany.cn/gtfskcmxek.html

JS:   crypto.randomUUID()
来源：http://hz.jianghu66.top/gtysqgaktw.html

TS:   crypto.randomUUID()
来源：http://hz.cheryme.top/gtndbntojb.html

Java: UUID.randomUUID().toString()
来源：http://hz.jinyuanbaomall.cn/gtuprzkwlt.html

Go:   // 用 github.com/google/uuid
来源：http://hz.c1oappe.top/gtgtpbpwss.html

Ruby: SecureRandom.uuid
来源：http://hz.cqqwz.cn/gtumegklzh.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yvedp.cn/gtonapiiud.html

[P02] MD5 / SHA256 摘要
来源：http://hz.gogol.net.cn/gtdsxiesty.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenjidiqi.icu/gtqgnlpvyx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhixingplan.top/gtdofrnhiw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xuanzx.com/gtaqbhmxvt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.guannengcc.top/gtvxrdtpno.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xinyue.icu/gtmnjghxwg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.tian-w.cn/gtlsqsoknk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhiwuduotai.top/gtwniayqjj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.dianchejie.cn/gtogoilagk.html

[P03] 生成短随机字符串
来源：http://hz.chenzaomai.com/gtwggushwv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.tanke756.top/gtrgtyharv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhengqikj.top/gtqpyztrnh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hongshengwenyu.top/gtvgioaqaa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenjidiqi.icu/gtjmtxusbq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xinyue.icu/gtdjyutzyn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.tian-w.cn/gtttkiixhl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinqigfzy.top/gtzevmwxhj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cheryme.top/gtxpmswlrh.html

[P04] 求长度
来源：http://hz.aibaodan.cn/gtvjyodfnr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yvedp.cn/gtpcafbkoi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yanxiufei.cn/gtfcdmcujf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhaomingkeji.xyz/gtocwdvnfk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fengsongda.top/gtitaztxhq.html

Java: list.size();  map.size();  s.length()
来源：http://hz.andypj.xyz/gtrpbfcxtu.html

Go:   len(arr);  len(m)
来源：http://hz.yuanzhike.top/gttnpzgdnb.html

Ruby: x.length;  x.size
来源：http://hz.svipenyu.cn/gtkcrinhgk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.redwolf501.top/gtozopkpgv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhengqikj.top/gtpghblrga.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xuetiantiany.cn/gtvocemxnk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hammf.cn/gtkoodimlv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nanxuanxn.top/gtfqfntjuo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hammf.cn/gtiwygzmhe.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yuanzhike.top/gtspfsjltb.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.nanxinkj.top/gtpdiirpta.html

Ruby: a == b
来源：http://hz.havefunace.top/gtmzvnsmbc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shangyingyoupin.top/gthzwivcgz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.fzhhl.top/gtootqzgty.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.sysykeji.top/gtjguafwqf.html

PHP:  if (empty($x)) {}
来源：http://hz.shanyushiyangkeji.top/gtdozaqjqk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hnqzz.top/gtihlyvcip.html

TS:   if (x == null) {}
来源：http://hz.yuanzhike.top/gtcygzpcrn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.tianlin.xyz/gtodkfqgou.html

Go:   if x == nil {}
来源：http://hz.tianlin.xyz/gtzyczcxfs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xziqi.cn/gtcburchrz.html

C#:   if (x is null) {}
来源：http://hz.xuanzx.com/gtdjklybuc.html

[P07] 防抖与节流
来源：http://hz.zhengqikj.top/gtchtstmpn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cashguo.top/gtexpyyyqm.html


<!-- 参考信息 -->