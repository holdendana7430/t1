代发 wailian999

C#:   (int)resp.StatusCode
来源：http://hz.dianchejie.cn/gtcecafitj.html

[L08] 并发请求多个地址
来源：http://hz.hywenlv.cn/gtisatwdof.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yuanzhike.top/gtxqntyzui.html

PHP:  curl_multi_init() 系列
来源：http://hz.jlsjyb.cn/gtnamlglfr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.mhx1999.top/gtvmlsbnye.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tian-w.cn/gttpwkbvvf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xingfuxueyuan.xyz/gtwqrsjrjm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.52xcode.cn/gtoywwoehq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shuidangran.top/gtyucemyzw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.andypj.xyz/gtaqvzwzzv.html

================================================================================
来源：http://hz.dashuyun.cn/gthszgafta.html

M. 命令行 / 进程 / 环境
来源：http://hz.havefunace.top/gtdalkvozc.html

================================================================================
来源：http://hz.birdmap.top/gtwtpsevel.html

[M01] 读取命令行参数
来源：http://hz.tian-w.cn/gttepzwhmg.html

Py:   sys.argv[1:]
来源：http://hz.nanxinkj.top/gtmifpaoia.html

PHP:  $argv;  $argc;
来源：http://hz.vqdsnc.cn/gtavgkhnoe.html

JS:   process.argv.slice(2)
来源：http://hz.daxiang520.top/gtiuzdoxsz.html

TS:   process.argv.slice(2)
来源：http://hz.gzhubu.top/gtjqsottxc.html

Java: args 数组（main 方法参数）
来源：http://hz.xylfe.cn/gthrlzilfh.html

Go:   os.Args[1:]
来源：http://hz.dianchejie.cn/gtzyzexupl.html

Ruby: ARGV
来源：http://hz.xingfuxueyuan.xyz/gtdquakuec.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xuanzx.com/gtqirtmqek.html

[M02] 读取环境变量
来源：http://hz.52xcode.cn/gtenbeychm.html

Py:   os.environ.get("HOME")
来源：http://hz.cheryme.top/gtsbgdgamq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ybcxt.top/gtwoccjxcl.html

JS:   process.env.HOME
来源：http://hz.tianlin.xyz/gtcrwgltud.html

TS:   process.env.HOME
来源：http://hz.dashuyun.cn/gtuofanrzj.html

Java: System.getenv("HOME")
来源：http://hz.jiagoushi.top/gtavsbvhxy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gzhubu.top/gtbkvprmjw.html

Ruby: ENV["HOME"]
来源：http://hz.yonumen.top/gtetdtyjkt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.haohaochexian.top/gttyaslaco.html

[M03] 执行外部命令
来源：http://hz.hnxiangtu.top/gtvjwerbge.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj202588.top/gtwvfuwrep.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ehwqpu.com/gtbktlmnae.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhijiandao.cn/gtzhpojawb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.feifeiyinyue.top/gthsxupyrx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhijiandao.cn/gtxecdavsl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ehwqpu.com/gtudnjglcv.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.svipenyu.cn/gtdidakksg.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinqigfzy.top/gtwjykwajs.html

[M04] 获取当前工作目录
来源：http://hz.gzhubu.top/gtkcdlnclm.html

Py:   os.getcwd()
来源：http://hz.fengsongda.top/gtxmusaxop.html

PHP:  getcwd();
来源：http://hz.jinqigfzy.top/gtuoocgkac.html

JS:   process.cwd()
来源：http://hz.xinyue.icu/gtrbkptktb.html

TS:   process.cwd()
来源：http://hz.xinyue.icu/gtiltuqhvw.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.wangdashe.top/gtmpeylicd.html

Go:   os.Getwd()
来源：http://hz.daxiang520.top/gtkfyqvhix.html

Ruby: Dir.pwd
来源：http://hz.sxryk.cn/gtzvtutybm.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yueranfly.top/gtmslozxjl.html

[M05] 设置退出码
来源：http://hz.hysaishi.cn/gtgrrkhtoj.html

Py:   sys.exit(1)
来源：http://hz.jiagoushi.top/gtyzzjvcac.html

PHP:  exit(1);
来源：http://hz.zhoulong.xyz/gtzvcpyknx.html

JS:   process.exit(1)
来源：http://hz.shuidangran.top/gtclicakyx.html

TS:   process.exit(1)
来源：http://hz.chenlongwang.top/gtiqupypow.html

Java: System.exit(1)
来源：http://hz.yongpay.top/gtxazdyfof.html

Go:   os.Exit(1)
来源：http://hz.chenlongwang.top/gtafkuxorc.html

Ruby: exit 1
来源：http://hz.gzhubu.top/gtvnenmbpu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cucudq.cn/gtwwtjcsfd.html

[M06] 向标准错误输出
来源：http://hz.xylfe.cn/gtomtdvrin.html

Py:   print("err", file=sys.stderr)
来源：http://hz.aizwys.cn/gtelnrzvod.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.haohaochexian.top/gtangehotm.html

JS:   console.error("err")
来源：http://hz.shangyingyoupin.top/gtwsqenxcq.html

TS:   console.error("err")
来源：http://hz.tianlin.xyz/gtnfgcoxtj.html

Java: System.err.println("err")
来源：http://hz.shanyushiyangtech.top/gtavgfaiek.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhaomingkeji.xyz/gtnpiostvw.html

Ruby: warn "err"
来源：http://hz.guowangkeji.top/gtvbhbfshs.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ppjwa.cn/gtciuqkscv.html

[M07] 判断是否为主入口
来源：http://hz.sysykeji.top/gtngurumtv.html

Py:   if __name__ == "__main__":
来源：http://hz.ehwqpu.com/gtxftgfaxq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.redwolf501.top/gtpexpndkl.html

JS:   require.main === module
来源：http://hz.tian-w.cn/gtscydpizr.html

TS:   require.main === module
来源：http://hz.ivvv.top/gtqfwrwpzt.html

Java: public static void main(String[] args)
来源：http://hz.quarkkingdee.top/gtswepbgaf.html

Go:   func main()
来源：http://hz.shzxlz.cn/gtbbisvaqd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.redwolf501.top/gtbpvvpzgu.html

C#:   static void Main(string[] args)
来源：http://hz.jqgufenzy.top/gtigzgvtqf.html

[M08] 获取系统与运行时信息
来源：http://hz.hnxiangtu.top/gtsgkguoct.html

Py:   platform.system();  platform.python_version()
来源：http://hz.chenjidiqi.icu/gtitqqphjl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.52xcode.cn/gtiibqqwjn.html

JS:   process.platform;  process.version
来源：http://hz.dianchejie.cn/gtmuymakjs.html

TS:   process.platform;  process.version
来源：http://hz.daria6918.cn/gtjbowltmb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.haohaochexian.top/gttpmuvdnh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.iojbl.cn/gtckxpkjfp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.c1oappe.top/gtyeqxjnzv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xuanzx.com/gtctfidips.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtwpenbaan.html

N. 数据结构与算法
来源：http://hz.ydjk.org.cn/gtoyzajdjr.html

================================================================================
来源：http://hz.zhongyouzk.top/gtfnjrpzgx.html

[N01] 二分查找（有序数组）
来源：http://hz.shangyingyoupin.top/gtjelajltl.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.cqqwz.cn/gtmcppkeqr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.smart0.xyz/gtqyakiqni.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhongyouzk.top/gtcqiyejyc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.kuanghao11.cn/gtbsqfokan.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.9152youxi.cn/gtxottwvxi.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.aibaodan.cn/gtwmqhgskt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.cheryme.top/gtavzribvf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.meibo888.top/gtmwevcyny.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cdnleiting.top/gtwycvpjhw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shuidangran.top/gtmqfpgiwb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.snrcjt.cn/gtaxjqzxhd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.andypj.xyz/gtitcgeyfd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangtech.top/gtyuxuyctm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhengqikj.top/gtbqqqvfjn.html

Go:   slices.Sort(arr)
来源：http://hz.yangfankeji.com/gtnoyxehqo.html

Ruby: arr.sort
来源：http://hz.yonumen.top/gtxhlzuhlp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zdqjudy.top/gtcuudhtwu.html

[N03] 快速排序（分治示例）
来源：http://hz.shuidangran.top/gtmmwjboew.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shanyushiyangtech.top/gtobnpogrr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhiwuduotai.top/gtuukgzcog.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jyoumei.cn/gtzujsubhf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gotoacloud.top/gtlccxjbks.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj202588.top/gthnzujsjt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhoulong.xyz/gtxbstnusg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.iojbl.cn/gtdjvbwhjk.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yonumen.top/gtrmhdtdoq.html

[N04] 斐波那契数列
来源：http://hz.snrcjt.cn/gtkafuiebb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ywan-chungtsiang.top/gtixkpxxmt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.gogol.net.cn/gtvvpubqnn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenjidiqi.icu/gtwensgwco.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gotoacloud.top/gthugqxtfw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ehwqpu.com/gtletqwncq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yangfankeji.com/gtlcdbfczm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.chenzaomai.com/gtzzkcmogg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenzaomai.com/gtcylecufu.html

[N05] 最大公约数
来源：http://hz.daria6918.cn/gtulotxnel.html

Py:   math.gcd(a, b)
来源：http://hz.yj20258.top/gtkxcdbhej.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yueranfly.top/gtnwecwunb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hammf.cn/gtjghwlivu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.kuanghao11.cn/gtrurjkuvk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.nanxinkj.top/gtikszspag.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhaomingkeji.xyz/gtltcqbcdv.html

Ruby: a.gcd(b)
来源：http://hz.0kj1m.cn/gtbkalgudz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.dianchejie.cn/gtafbdvtll.html

[N06] 判断回文字符串
来源：http://hz.shzxlz.cn/gtjmseedgs.html

Py:   s == s[::-1]
来源：http://hz.xingfuxueyuan.xyz/gterwbcbfa.html

PHP:  $s === strrev($s);
来源：http://hz.svipenyu.cn/gtnzrureqi.html

JS:   s === [...s].reverse().join("")
来源：http://hz.c1oappe.top/gtubuqepho.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ivvv.top/gtoeigslwz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinyuanbaomall.cn/gtzyrhrzvs.html

Go:   // 双指针从两端比较
来源：http://hz.nwbrower.top/gtktduiypm.html

Ruby: s == s.reverse
来源：http://hz.cucudq.cn/gtdrhiwoda.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.fengsongda.top/gtglnxtkbd.html

[N07] 两数之和（返回下标）
来源：http://hz.316326.xyz/gtoibaimwe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hnqzz.top/gtnaogcsxt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jiagoushi.top/gtfyjkzmgr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gzhubu.top/gtivshtfgp.html

TS:   // 手写 Map<string, number>
来源：http://hz.zycfv.cn/gtclwscixg.html

Java: // 手写 HashMap
来源：http://hz.chenlongwang.top/gtcqralrkf.html

Go:   // 手写 map[int]int
来源：http://hz.jyoumei.cn/gtuqzoyzxo.html

Ruby: // 手写 Hash
来源：http://hz.guannengcc.top/gtslyqopkd.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.316326.xyz/gtkdwlekxx.html

[N08] 生成全排列
来源：http://hz.iojbl.cn/gtdxvheaow.html

Py:   itertools.permutations(arr)
来源：http://hz.redwolf501.top/gtyeyajpkm.html

PHP:  // 手写递归交换
来源：http://hz.yj202588.top/gtyigaeidu.html

JS:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtqjertgpg.html

TS:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtkidlcevo.html

Java: // 手写回溯递归
来源：http://hz.yj20258888.top/gtmzmisvvg.html

Go:   // 手写回溯递归
来源：http://hz.jqgufenzy.top/gtzkpdqgas.html

Ruby: arr.permutation.to_a
来源：http://hz.316326.xyz/gtuuvhrgfx.html

C#:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gtdlvbklxc.html

[N09] 栈与队列
来源：http://hz.gzhubu.top/gtpvbyrcwf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xziqi.cn/gtdnuwowsq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhaomingkeji.xyz/gtczvjgtzb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.haohaochexian.top/gtctjoxbyi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jyoumei.cn/gthwgebpam.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.chenzaomai.com/gtngdftvrz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.mhx1999.top/gtjctpzhoc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.redwolf501.top/gtnafgngak.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shangyingyoupin.top/gtohvaipfv.html

[N10] 链表节点定义
来源：http://hz.jianghu66.top/gtuyigpmkv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yanxiufei.cn/gtxkbkmrbc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhaomingkeji.xyz/gtisjzofnk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.shuidangran.top/gtyprmdwzx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tianlin.xyz/gtgkhzqjoo.html

Java: class Node { int v; Node next; }
来源：http://hz.yvedp.cn/gtdwnomeyb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.9152youxi.cn/gtgszyocou.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.tanke756.top/gtnlruretb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zdqjudy.top/gtnmzftibu.html

[N11] 二叉树中序遍历
来源：http://hz.yvedp.cn/gtiyoefsfb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hammf.cn/gtocridzhb.html

PHP:  // 手写递归函数
来源：http://hz.hfpthk.cn/gtyqlmoyus.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yangfankeji.com/gtouosxcfz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhengqikj.top/gtszysveki.html

Java: // 手写递归
来源：http://hz.zdqjudy.top/gtkrlotsja.html

Go:   // 手写递归
来源：http://hz.wangshuangyany.cn/gtjvgohgcu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jyoumei.cn/gtyqddbpmc.html

C#:   // 手写递归
来源：http://hz.gogol.net.cn/gtivkbwpqy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xylfe.cn/gtutpqutsy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.0kj1m.cn/gtqvufqdhw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sufxvd.cn/gthenbrtxj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.birdmap.top/gtljewdgys.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jiagoushi.top/gtjvsrekwt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jiagoushi.top/gtfzxvnbok.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.andypj.xyz/gtzmvcmuye.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.vqdsnc.cn/gtlkueruew.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.iojbl.cn/gtpdadbjlo.html

================================================================================
来源：http://hz.xinyue.icu/gtdiogvqhk.html

O. 并发与异步
来源：http://hz.52xcode.cn/gtdwbtikqk.html

================================================================================
来源：http://hz.zhoulong.xyz/gtscgfuebm.html

[O01] 启动一个线程
来源：http://hz.jqgfzy.top/gtqjhftzky.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.vqdsnc.cn/gtnyhegych.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ybcxt.top/gtuzgpmqaa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cqqwz.cn/gttgimmpfk.html

TS:   // 同 JS
来源：http://hz.cqqwz.cn/gtnfydyfie.html

Java: new Thread(() -> f()).start()
来源：http://hz.smart0.xyz/gtjqebejxj.html

Go:   go f()
来源：http://hz.haohaochexian.top/gtjlpcqjtv.html

Ruby: Thread.new { f }
来源：http://hz.hywenlv.cn/gtlfbmcukr.html

C#:   Task.Run(() => F());
来源：http://hz.xuetiantiany.cn/gtczdmmpwg.html

[O02] 使用线程池
来源：http://hz.aizwys.cn/gtakspoigv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sysykeji.top/gtsfzuzqku.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.birdmap.top/gtvvjosboh.html

JS:   // worker_threads 线程池
来源：http://hz.daxiang520.top/gtkkebprxc.html

TS:   // worker_threads 线程池
来源：http://hz.jiagoushi.top/gtvlmnhuyu.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhijiandao.cn/gtginrhynu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.haohaochexian.top/gtcquatdrm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xuanzx.com/gtmakxjoql.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xziqi.cn/gtuaekrdpt.html

[O03] 加锁保护共享数据
来源：http://hz.zhongyouzk.top/gttgbwwffs.html

Py:   with lock: shared += 1
来源：http://hz.zhixingplan.top/gtkgdnqgxr.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xylfe.cn/gteloljssn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cashguo.top/gtzrciemjw.html

TS:   // 同 JS
来源：http://hz.xuetiantiany.cn/gtgabrqztq.html

Java: synchronized (this) { shared++; }
来源：http://hz.ehwqpu.com/gtfrfstlud.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ywan-chungtsiang.top/gtteifbyly.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.sweek.top/gtavlyhetx.html

C#:   lock (gate) { shared++; }
来源：http://hz.wangdashe.top/gtrjkisptf.html

[O04] 定义异步函数并等待
来源：http://hz.9152youxi.cn/gttrntsxbj.html

Py:   async def f():⏎    await g()
来源：http://hz.havefunace.top/gthghreixw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.dianchejie.cn/gtmfnqwnpr.html

JS:   async function f() { await g(); }
来源：http://hz.ywan-chungtsiang.top/gtplpghehp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.tianlin.xyz/gtbhimcqco.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.chenjidiqi.icu/gtjeddqdwi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.316326.xyz/gtoinyedir.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.guowangkeji.top/gtwhqmbvqq.html

C#:   async Task F() { await G(); }
来源：http://hz.nanxinkj.top/gtzcuetaoq.html

[O05] 并发执行并等待全部完成
来源：http://hz.yuxming.cn/gthtecrjsa.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xuanzx.com/gtbjxfxcsv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.wangshuangyany.cn/gtzdcnzotc.html

JS:   await Promise.all(tasks)
来源：http://hz.sxryk.cn/gttuwvrlnt.html

TS:   await Promise.all(tasks)
来源：http://hz.sysykeji.top/gtdigotynv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yonumen.top/gtndtfvjfc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xinyue.icu/gtpvarxfxe.html

Ruby: threads.map(&:join)
来源：http://hz.gzhubu.top/gtciqhrcom.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhiwuduotai.top/gtbbscwbrh.html

[O06] 使用进程池
来源：http://hz.0kj1m.cn/gtaypbzmig.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yongpay.top/gtxbttqgyb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.daxiang520.top/gtgfihmdbh.html

JS:   // child_process / cluster 模块
来源：http://hz.fzhhl.top/gtkclkhxkz.html

TS:   // child_process / cluster 模块
来源：http://hz.jianghu66.top/gtbjkozaim.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.316326.xyz/gtntmzways.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jqgufenzy.top/gtjtoobpny.html

Ruby: // fork 块
来源：http://hz.andypj.xyz/gtneeuxbiv.html

C#:   Parallel.For
来源：http://hz.yuxming.cn/gtosokmnro.html

================================================================================
来源：http://hz.nanxuanxn.top/gtggripbyx.html

P. 常用工具函数
来源：http://hz.meibo888.top/gtfwjkijkk.html

================================================================================
来源：http://hz.pengpengdd.cyou/gthyffaxzm.html

[P01] 生成 UUID
来源：http://hz.chenjidiqi.icu/gtwtyobwiu.html

Py:   str(uuid.uuid4())
来源：http://hz.shuidangran.top/gtpnmsfdsk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.guowangkeji.top/gtdspzjelv.html

JS:   crypto.randomUUID()
来源：http://hz.fzhhl.top/gtnzucsvcw.html

TS:   crypto.randomUUID()
来源：http://hz.ivvv.top/gtnwtbiuuc.html

Java: UUID.randomUUID().toString()
来源：http://hz.ivvv.top/gteuuhxsvv.html

Go:   // 用 github.com/google/uuid
来源：http://hz.pengpengdd.cyou/gttpthimpn.html

Ruby: SecureRandom.uuid
来源：http://hz.gaohongyu789.top/gthzjfycgx.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cheryme.top/gttmwwajfz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yuanzhike.top/gttidsbfnk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.quarkkingdee.top/gtzodrlqxm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.cdnleiting.top/gtdbfpkdsp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yuanzhike.top/gtnydtepfx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ydzc1.top/gtbpsilcuf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ehwqpu.com/gtewvwpyzt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xuetiantiany.cn/gteuqkkzlr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.tanke756.top/gtxcyzfaqn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xinyue.icu/gtwrtmoshf.html

[P03] 生成短随机字符串
来源：http://hz.ydjk.org.cn/gtzuanuivn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.birdmap.top/gtrdehvxxe.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.quarkkingdee.top/gtvrhowjkc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuanzhike.top/gtczdfgpsz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cheryme.top/gtjtlexklz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xingfuxueyuan.xyz/gtmldgdeln.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhengqikj.top/gtzrmyrjrk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yj202588.top/gtlbcdvzpt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.tianlin.xyz/gtnnocikrg.html

[P04] 求长度
来源：http://hz.cheryme.top/gtuojcgkiq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.bjfxy.top/gtingevvut.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sweek.top/gtgykepxvx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.316326.xyz/gtmrydbsye.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.tianlin.xyz/gthznboimj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.9152youxi.cn/gtipecpvdr.html

Go:   len(arr);  len(m)
来源：http://hz.nwbrower.top/gtaxhppeue.html

Ruby: x.length;  x.size
来源：http://hz.ywan-chungtsiang.top/gtovlbnmeg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jlsjyb.cn/gtdiexuldw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.bjfxy.top/gtmajpukrb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ydjk.org.cn/gtwpwguhih.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinqigfzy.top/gtzaitjcdz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xuetiantiany.cn/gtuyimxkcp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.0kj1m.cn/gtvjfloxyh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sufxvd.cn/gtbdhngguv.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xuetiantiany.cn/gtssodavax.html

Ruby: a == b
来源：http://hz.shuidangran.top/gttmoxspcw.html


<!-- 参考信息 -->