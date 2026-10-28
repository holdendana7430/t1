代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cqqwz.cn/gtiicinbgl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.nanxuanxn.top/gtzxshnfwd.html

================================================================================
来源：http://hz.aibaodan.cn/gtqflnuunn.html

M. 命令行 / 进程 / 环境
来源：http://hz.hnxiangtu.top/gthjucizai.html

================================================================================
来源：http://hz.jinqigufen.top/gtfbesgfif.html

[M01] 读取命令行参数
来源：http://hz.yj20258.top/gtvoszolbh.html

Py:   sys.argv[1:]
来源：http://hz.xinyue.icu/gtgamayyyf.html

PHP:  $argv;  $argc;
来源：http://hz.sysykeji.top/gtlpqktzfm.html

JS:   process.argv.slice(2)
来源：http://hz.ppjwa.cn/gtxngyvxno.html

TS:   process.argv.slice(2)
来源：http://hz.xuetiantiany.cn/gtbdcoqxsf.html

Java: args 数组（main 方法参数）
来源：http://hz.vqdsnc.cn/gtztozxsbm.html

Go:   os.Args[1:]
来源：http://hz.dashuyun.cn/gttqytwnun.html

Ruby: ARGV
来源：http://hz.meibo888.top/gttdjgiake.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shanyushiyangkeji.top/gtbwmgefpt.html

[M02] 读取环境变量
来源：http://hz.hnqzz.top/gtiqvzhxiu.html

Py:   os.environ.get("HOME")
来源：http://hz.316326.xyz/gtfyhjypco.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.dashuyun.cn/gttsrwizrw.html

JS:   process.env.HOME
来源：http://hz.sysykeji.top/gtxgwkscpq.html

TS:   process.env.HOME
来源：http://hz.birdmap.top/gtakotitsr.html

Java: System.getenv("HOME")
来源：http://hz.pycfn.com/gtjqiguruw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yuanzhike.top/gtqqbzpdwd.html

Ruby: ENV["HOME"]
来源：http://hz.sxryk.cn/gtgcpbwkou.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shangyingyoupin.top/gtgyimfplo.html

[M03] 执行外部命令
来源：http://hz.sysykeji.top/gtcujqfnzp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hnqzz.top/gtqcnprbya.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.chenlongwang.top/gtsgydynng.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ehwqpu.com/gtfdxnlryp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.kuanghao11.cn/gtnlpgirfb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xziqi.cn/gtzbmdxaec.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yuanzhike.top/gtdwnsgmwi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gotoacloud.top/gtlajpihhj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.dianchejie.cn/gtyxdkiphy.html

[M04] 获取当前工作目录
来源：http://hz.yuanzhike.top/gtthjxtsyb.html

Py:   os.getcwd()
来源：http://hz.guannengcc.top/gtmykefajv.html

PHP:  getcwd();
来源：http://hz.aibaodan.cn/gtxnsvmihh.html

JS:   process.cwd()
来源：http://hz.sysykeji.top/gtohwnczzz.html

TS:   process.cwd()
来源：http://hz.iojbl.cn/gtnrssguqh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sufxvd.cn/gtpcncptme.html

Go:   os.Getwd()
来源：http://hz.vqdsnc.cn/gtcbeydlrj.html

Ruby: Dir.pwd
来源：http://hz.yangfankeji.com/gtkiioqgwn.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gaohongyu789.top/gtqnxftkqv.html

[M05] 设置退出码
来源：http://hz.hongshengwenyu.top/gtpaswjddv.html

Py:   sys.exit(1)
来源：http://hz.nanxuanxn.top/gtehohpygq.html

PHP:  exit(1);
来源：http://hz.wangdashe.top/gtjwzndvaf.html

JS:   process.exit(1)
来源：http://hz.c1oappe.top/gtnjjypoct.html

TS:   process.exit(1)
来源：http://hz.chenjidiqi.icu/gtinwhoclz.html

Java: System.exit(1)
来源：http://hz.nanxinkj.top/gtmyhhggyy.html

Go:   os.Exit(1)
来源：http://hz.zhaomingkeji.xyz/gtqlumujmj.html

Ruby: exit 1
来源：http://hz.cheryme.top/gtoqigcrns.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.52xcode.cn/gtnbszshdm.html

[M06] 向标准错误输出
来源：http://hz.xuanzx.com/gtovgznyvv.html

Py:   print("err", file=sys.stderr)
来源：http://hz.svipenyu.cn/gtrztxhjmh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.guowangkeji.top/gtephgoejn.html

JS:   console.error("err")
来源：http://hz.52xcode.cn/gtvivvhdqh.html

TS:   console.error("err")
来源：http://hz.cheryme.top/gtbuoljxhd.html

Java: System.err.println("err")
来源：http://hz.0kj1m.cn/gthgtwqdob.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jyoumei.cn/gtfezlrfbc.html

Ruby: warn "err"
来源：http://hz.hywenlv.cn/gtgejlcycv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.fengsongda.top/gtdgnqjcwy.html

[M07] 判断是否为主入口
来源：http://hz.zhixingplan.top/gtucpgzspu.html

Py:   if __name__ == "__main__":
来源：http://hz.chenzaomai.com/gtgshgcqyv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.nanxuanxn.top/gtlfjtosai.html

JS:   require.main === module
来源：http://hz.zhaomingkeji.xyz/gtzsrtweae.html

TS:   require.main === module
来源：http://hz.yonumen.top/gtjsikafmm.html

Java: public static void main(String[] args)
来源：http://hz.yanxiufei.cn/gtuknsorkv.html

Go:   func main()
来源：http://hz.yj20258888.top/gthioujitb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jiagoushi.top/gtgxpkqvwv.html

C#:   static void Main(string[] args)
来源：http://hz.birdmap.top/gtodexypro.html

[M08] 获取系统与运行时信息
来源：http://hz.52xcode.cn/gtqzcyzmho.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinghuilouyu.cn/gttxzavsox.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ybcxt.top/gtvqhxdxgh.html

JS:   process.platform;  process.version
来源：http://hz.cqqwz.cn/gttqotdbiq.html

TS:   process.platform;  process.version
来源：http://hz.dianchejie.cn/gtxcpafwdl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gzhubu.top/gtzfybzvxf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ydjk.org.cn/gtwsnogsmh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jlsjyb.cn/gtmmtinald.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.vqdsnc.cn/gtpzubuksw.html

================================================================================
来源：http://hz.yongpay.top/gtocounsxp.html

N. 数据结构与算法
来源：http://hz.aizwys.cn/gtoghvovbl.html

================================================================================
来源：http://hz.meibo888.top/gtllpylall.html

[N01] 二分查找（有序数组）
来源：http://hz.jianghu66.top/gtycuceruq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sxryk.cn/gtzdjifbhj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gzhubu.top/gtepnilrau.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cheryme.top/gtrtadlavm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangshuangyany.cn/gtzpqxltvg.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yj20258.top/gthuferyie.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtuhldtbxy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ehwqpu.com/gttvirzgmb.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.havefunace.top/gthgsvdlkr.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.fzhhl.top/gtznhuwugx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ppjwa.cn/gtrpvgbepe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xinyue.icu/gtvjnzangd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sufxvd.cn/gtpkmznruw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gttxfwjzlc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sxryk.cn/gtoynuhgej.html

Go:   slices.Sort(arr)
来源：http://hz.c1oappe.top/gtnqqewevb.html

Ruby: arr.sort
来源：http://hz.jinqigufen.top/gtjzwciavs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ywan-chungtsiang.top/gtfdlaqode.html

[N03] 快速排序（分治示例）
来源：http://hz.hfpthk.cn/gtxnfxznbf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shangyingyoupin.top/gteymedwlc.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ydzc1.top/gtrmlejwtr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.daria6918.cn/gtxsxalrev.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cdnleiting.top/gtthepzana.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.fengsongda.top/gtznlcfvlb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.snrcjt.cn/gtvargudqn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hnxiangtu.top/gtqpzpjyqn.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ywan-chungtsiang.top/gtkwjrtfaf.html

[N04] 斐波那契数列
来源：http://hz.zhixingplan.top/gtbmnxkjnq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.havefunace.top/gtgsljlwwx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhaomingkeji.xyz/gtfidbszda.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hammf.cn/gtiogkmdrr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ivvv.top/gtcfnqugeh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yangfankeji.com/gtqqxfroth.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhiwuduotai.top/gtpzlejbqs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.redwolf501.top/gtiuxirwoq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.feifeiyinyue.top/gtinifrspt.html

[N05] 最大公约数
来源：http://hz.nanxinkj.top/gtklmhhrbp.html

Py:   math.gcd(a, b)
来源：http://hz.pengpengdd.cyou/gtfksophpv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.svipenyu.cn/gtcpwffndp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guannengcc.top/gtxdntteqv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xingfuxueyuan.xyz/gtczmkkxrs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.quarkkingdee.top/gtgwpwdeas.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.52xcode.cn/gtlsnelhfo.html

Ruby: a.gcd(b)
来源：http://hz.xuetiantiany.cn/gtxzmnpepo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zdqjudy.top/gtltmjygzp.html

[N06] 判断回文字符串
来源：http://hz.yuxming.cn/gtqhtjzfmf.html

Py:   s == s[::-1]
来源：http://hz.shzxlz.cn/gtkukrpewm.html

PHP:  $s === strrev($s);
来源：http://hz.vqdsnc.cn/gtthemhqfy.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gtpddlkdcg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtjpyfrkgg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhengqikj.top/gtidecucrp.html

Go:   // 双指针从两端比较
来源：http://hz.daria6918.cn/gtfprhdbek.html

Ruby: s == s.reverse
来源：http://hz.aibaodan.cn/gtopnzanay.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhongyouzk.top/gtnepeuaax.html

[N07] 两数之和（返回下标）
来源：http://hz.yuanzhike.top/gtboteuurq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nanxinkj.top/gtdrbnsdfi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jianghu66.top/gttosbxitx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jiagoushi.top/gtwqzyrsrv.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj202588.top/gtnjsvmjbv.html

Java: // 手写 HashMap
来源：http://hz.gzhubu.top/gtazyulxvn.html

Go:   // 手写 map[int]int
来源：http://hz.ydzc1.top/gtpsygjqri.html

Ruby: // 手写 Hash
来源：http://hz.cucudq.cn/gtqyhasliu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zycfv.cn/gtlsjeppng.html

[N08] 生成全排列
来源：http://hz.jlsjyb.cn/gteebngcds.html

Py:   itertools.permutations(arr)
来源：http://hz.chenjidiqi.icu/gtswrqscob.html

PHP:  // 手写递归交换
来源：http://hz.shangyingyoupin.top/gtzlmecbcq.html

JS:   // 手写回溯递归
来源：http://hz.daria6918.cn/gthtnjtpxx.html

TS:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtfcxcguqt.html

Java: // 手写回溯递归
来源：http://hz.316326.xyz/gtjwqqbeay.html

Go:   // 手写回溯递归
来源：http://hz.hfpthk.cn/gtpunqxckt.html

Ruby: arr.permutation.to_a
来源：http://hz.haohaochexian.top/gtlfwcadvk.html

C#:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtlogbxdyf.html

[N09] 栈与队列
来源：http://hz.jinyuanbaomall.cn/gtgblhxtku.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ppjwa.cn/gtwzlvqjgj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hywenlv.cn/gtnhukcyoj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cucudq.cn/gtawlhxgsy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jqgufenzy.top/gtdvnpmhgg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.mhx1999.top/gtjsqsfwdt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.pengpengdd.cyou/gtjtqwtnuk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yuanzhike.top/gtdjsqsjfa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.pycfn.com/gtgpvaxogn.html

[N10] 链表节点定义
来源：http://hz.fzhhl.top/gtvamkynrn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shanyushiyangkeji.top/gtpcnfznzo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jianghu66.top/gttvgtgbqs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.bjfxy.top/gtojlhvkqv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xuetiantiany.cn/gtgxccdxyp.html

Java: class Node { int v; Node next; }
来源：http://hz.jianghu66.top/gtccetdlnr.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tanke756.top/gtlfnbwhnr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yj20258.top/gtlluqegke.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xylfe.cn/gtihaveulb.html

[N11] 二叉树中序遍历
来源：http://hz.chenjidiqi.icu/gtggnjandr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ydjk.org.cn/gtmhdgzrib.html

PHP:  // 手写递归函数
来源：http://hz.vqdsnc.cn/gtcykgfxvs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xziqi.cn/gtxyzrehvn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.redwolf501.top/gtoifwqaip.html

Java: // 手写递归
来源：http://hz.havefunace.top/gttfxycrni.html

Go:   // 手写递归
来源：http://hz.dashuyun.cn/gtqlixtyyh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jinqigfzy.top/gtarlhgrer.html

C#:   // 手写递归
来源：http://hz.guannengcc.top/gtmbumiawx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.dashuyun.cn/gtokppoxcq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yangfankeji.com/gtwdtvhtsp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jyoumei.cn/gtdjwlckwu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangkeji.top/gtqvsjyvud.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangdashe.top/gthkyosdcr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cheryme.top/gttuijhzzd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hongshengwenyu.top/gtjidoxsth.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yanxiufei.cn/gttsotvijx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj202588.top/gtgaslfzcd.html

================================================================================
来源：http://hz.gogol.net.cn/gtresyxzeb.html

O. 并发与异步
来源：http://hz.yvedp.cn/gtrylqoqub.html

================================================================================
来源：http://hz.quarkkingdee.top/gtbkkbqczy.html

[O01] 启动一个线程
来源：http://hz.sysykeji.top/gtmfwubswj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cucudq.cn/gtvtbzqbvb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jianghu66.top/gtfbixnehe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhiwuduotai.top/gtdlcpsiwh.html

TS:   // 同 JS
来源：http://hz.zhengqikj.top/gtoonkdxaw.html

Java: new Thread(() -> f()).start()
来源：http://hz.nanxinkj.top/gtarvdnlrc.html

Go:   go f()
来源：http://hz.snrcjt.cn/gtxyckphpm.html

Ruby: Thread.new { f }
来源：http://hz.yj20258.top/gtbyohqsrm.html

C#:   Task.Run(() => F());
来源：http://hz.sweek.top/gtfafexxfr.html

[O02] 使用线程池
来源：http://hz.gzhubu.top/gtsyfqmcwk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yanxiufei.cn/gtfbjuqemg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.wangshuangyany.cn/gthjwvrabh.html

JS:   // worker_threads 线程池
来源：http://hz.shuidangran.top/gtmkccwqkk.html

TS:   // worker_threads 线程池
来源：http://hz.quarkkingdee.top/gtgnbamkoj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhaomingkeji.xyz/gtnxmwlphs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ydzc1.top/gthziqutds.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.pengpengdd.cyou/gteuhpvodl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yanxiufei.cn/gtlciaxuai.html

[O03] 加锁保护共享数据
来源：http://hz.xziqi.cn/gtrormdyww.html

Py:   with lock: shared += 1
来源：http://hz.ehwqpu.com/gtoeznfzam.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ppjwa.cn/gtcteyjusm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xylfe.cn/gtwkgyrqvz.html

TS:   // 同 JS
来源：http://hz.hysaishi.cn/gtzbwsllcz.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhengqikj.top/gtemqbtxsx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yonumen.top/gtakzirtgm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.gogol.net.cn/gtknyxbozu.html

C#:   lock (gate) { shared++; }
来源：http://hz.sufxvd.cn/gtfkmjctsa.html

[O04] 定义异步函数并等待
来源：http://hz.zhiwuduotai.top/gtefnzoyyf.html

Py:   async def f():⏎    await g()
来源：http://hz.hammf.cn/gtytribmtc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.meibo888.top/gtgviowscu.html

JS:   async function f() { await g(); }
来源：http://hz.52xcode.cn/gtiblfeolv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhengqikj.top/gtebryvvzb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yj202588.top/gtczaxfsuy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cqqwz.cn/gtlutfupyo.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.guannengcc.top/gtbmwghbct.html

C#:   async Task F() { await G(); }
来源：http://hz.ydzc1.top/gtaldokfae.html

[O05] 并发执行并等待全部完成
来源：http://hz.zycfv.cn/gtkrbzzzkb.html

Py:   asyncio.gather(*tasks)
来源：http://hz.andypj.xyz/gtfactytgf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yj20258888.top/gtjspzgfkn.html

JS:   await Promise.all(tasks)
来源：http://hz.gaohongyu789.top/gtmmphmbhg.html

TS:   await Promise.all(tasks)
来源：http://hz.birdmap.top/gthnhuayuf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shuidangran.top/gtuqmdubju.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.guowangkeji.top/gtacffqgpg.html

Ruby: threads.map(&:join)
来源：http://hz.daria6918.cn/gtkrjftcpc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hnqzz.top/gttejccpjh.html

[O06] 使用进程池
来源：http://hz.xziqi.cn/gtiwsbuwcc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.fzhhl.top/gtvafkkxnx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.tanke756.top/gtbaxwswxw.html

JS:   // child_process / cluster 模块
来源：http://hz.xinyue.icu/gthxxyynxz.html

TS:   // child_process / cluster 模块
来源：http://hz.quarkkingdee.top/gtgajbuwuo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.fzhhl.top/gtcahwvxoo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yonumen.top/gtwakzxjcn.html

Ruby: // fork 块
来源：http://hz.dashuyun.cn/gtigwwktar.html

C#:   Parallel.For
来源：http://hz.cheryme.top/gtgmgreqvx.html

================================================================================
来源：http://hz.sufxvd.cn/gtxpfcrovk.html

P. 常用工具函数
来源：http://hz.nwbrower.top/gtrixphvop.html

================================================================================
来源：http://hz.zhijiandao.cn/gtnvdamqyh.html

[P01] 生成 UUID
来源：http://hz.hammf.cn/gtkxmruhek.html

Py:   str(uuid.uuid4())
来源：http://hz.yj202588.top/gthnudgokm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jlsjyb.cn/gtksqrcimr.html

JS:   crypto.randomUUID()
来源：http://hz.andypj.xyz/gtzqqkirdu.html

TS:   crypto.randomUUID()
来源：http://hz.quarkkingdee.top/gtoznbhcsk.html

Java: UUID.randomUUID().toString()
来源：http://hz.daria6918.cn/gtiocceggj.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cqqwz.cn/gtexdstftx.html

Ruby: SecureRandom.uuid
来源：http://hz.hywenlv.cn/gtesqhnipt.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jlsjyb.cn/gtzhzwcpbq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hywenlv.cn/gtbuigreku.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hywenlv.cn/gtrqltveho.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.fengsongda.top/gtsfssuynm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.9152youxi.cn/gtdqzblshi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.daxiang520.top/gtcqjqpeum.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hnqzz.top/gthveohvwf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cheryme.top/gtmsvntseq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ppjwa.cn/gtiigikttx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.sxryk.cn/gtfkodawol.html

[P03] 生成短随机字符串
来源：http://hz.ppjwa.cn/gtivwnzcop.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.bjfxy.top/gtkpgatlvc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hfpthk.cn/gtfsgtdnrx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cucudq.cn/gtxfbqnpyr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangtech.top/gtzlmfixfa.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.sxryk.cn/gtlfjumzcg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yuanzhike.top/gtphxdodpz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.kuanghao11.cn/gtsuoobawf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hongshengwenyu.top/gtwlqhxoef.html

[P04] 求长度
来源：http://hz.hongshengwenyu.top/gtbdzcbfgb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.wangdashe.top/gtyjqqjlym.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.andypj.xyz/gtoolygfgt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj20258888.top/gtzhmfyvmw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhijiandao.cn/gtmnsoyjui.html

Java: list.size();  map.size();  s.length()
来源：http://hz.pengpengdd.cyou/gtmbyefwnw.html

Go:   len(arr);  len(m)
来源：http://hz.zycfv.cn/gtpwfdirna.html

Ruby: x.length;  x.size
来源：http://hz.yuanzhike.top/gtdhphlsdw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.meibo888.top/gtqpbsihiw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.iojbl.cn/gttubtvxuu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.0kj1m.cn/gtecninqbg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zycfv.cn/gtcloeikkw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenlongwang.top/gtqcjghtye.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj20258.top/gttgsrmxrl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shzxlz.cn/gttjyqlchq.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.52xcode.cn/gtgzvihmup.html

Ruby: a == b
来源：http://hz.gzhubu.top/gtbkcocnzv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.redwolf501.top/gtkliwrluw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shanyushiyangtech.top/gttlzgtubw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ehwqpu.com/gtrvcchsnm.html

PHP:  if (empty($x)) {}
来源：http://hz.iojbl.cn/gtzrrfnlrg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cdnleiting.top/gtgpuctyng.html

TS:   if (x == null) {}
来源：http://hz.xziqi.cn/gtlvqcyzxa.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhoulong.xyz/gtqttlywce.html

Go:   if x == nil {}
来源：http://hz.dianchejie.cn/gtlzzippcc.html


<!-- 参考信息 -->