代发 wailian999

TS:   resp.ok;  resp.status
来源：http://hz.zhixingplan.top/gtfrnhtsvf.html

Java: resp.statusCode()
来源：http://hz.nanxinkj.top/gtfunffklt.html

Go:   resp.StatusCode
来源：http://hz.fzhhl.top/gthlarrkbw.html

Ruby: resp.code.to_i
来源：http://hz.cheryme.top/gtarqqrrpz.html

C#:   (int)resp.StatusCode
来源：http://hz.snrcjt.cn/gthtriqznv.html

[L08] 并发请求多个地址
来源：http://hz.gaohongyu789.top/gtwtnhuaux.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yuanzhike.top/gtmrjhpvkh.html

PHP:  curl_multi_init() 系列
来源：http://hz.ehwqpu.com/gtqrisoyjw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhijiandao.cn/gtjkdkrbui.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinyuanbaomall.cn/gtfviujsan.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.aizwys.cn/gtkestmplb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jianghu66.top/gtdbromkqx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ehwqpu.com/gtoubfrsdm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hammf.cn/gtipwlobvt.html

================================================================================
来源：http://hz.hammf.cn/gtqgjejhhv.html

M. 命令行 / 进程 / 环境
来源：http://hz.yj20258.top/gtbiwfqvkw.html

================================================================================
来源：http://hz.jyoumei.cn/gtiocsnwdt.html

[M01] 读取命令行参数
来源：http://hz.feifeiyinyue.top/gtvovpdghs.html

Py:   sys.argv[1:]
来源：http://hz.hammf.cn/gtotkrocii.html

PHP:  $argv;  $argc;
来源：http://hz.ydjk.org.cn/gthqhltgni.html

JS:   process.argv.slice(2)
来源：http://hz.hongshengwenyu.top/gtvcaunbpk.html

TS:   process.argv.slice(2)
来源：http://hz.nanxuanxn.top/gtvnuwintn.html

Java: args 数组（main 方法参数）
来源：http://hz.gzhubu.top/gttegwsgei.html

Go:   os.Args[1:]
来源：http://hz.yonumen.top/gtdpmkyyss.html

Ruby: ARGV
来源：http://hz.aizwys.cn/gthjofsoof.html

C#:   args 数组（Main 方法参数）
来源：http://hz.aibaodan.cn/gtxvgnurjk.html

[M02] 读取环境变量
来源：http://hz.yj20258888.top/gtboaxsmvi.html

Py:   os.environ.get("HOME")
来源：http://hz.zdqjudy.top/gtgjdoikar.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.gotoacloud.top/gtbxokpmdr.html

JS:   process.env.HOME
来源：http://hz.gotoacloud.top/gtykvekouu.html

TS:   process.env.HOME
来源：http://hz.gogol.net.cn/gtmgxmrabe.html

Java: System.getenv("HOME")
来源：http://hz.jinqigufen.top/gtvavjhkeu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.nanxinkj.top/gtjfiuutov.html

Ruby: ENV["HOME"]
来源：http://hz.shzxlz.cn/gtkxwlbtdj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yj20258888.top/gtrpngiisj.html

[M03] 执行外部命令
来源：http://hz.sxryk.cn/gtzetwtciy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cdnleiting.top/gtzlkofkrz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.redwolf501.top/gteveksmny.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhongyouzk.top/gtrpthrkme.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.vqdsnc.cn/gtuouzqfxp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.9152youxi.cn/gtbcekevdu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.vqdsnc.cn/gtnpopjjwn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jlsjyb.cn/gtprpwzeeb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ehwqpu.com/gtejjemrcw.html

[M04] 获取当前工作目录
来源：http://hz.ehwqpu.com/gthwtwujbd.html

Py:   os.getcwd()
来源：http://hz.sxryk.cn/gterdwulfy.html

PHP:  getcwd();
来源：http://hz.jyoumei.cn/gtolrhprou.html

JS:   process.cwd()
来源：http://hz.quarkkingdee.top/gtcqavlnfg.html

TS:   process.cwd()
来源：http://hz.shanyushiyangkeji.top/gtiwrtaovt.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.aibaodan.cn/gtukgfffko.html

Go:   os.Getwd()
来源：http://hz.yj20258.top/gtuedpnoyq.html

Ruby: Dir.pwd
来源：http://hz.daria6918.cn/gtbhazahzr.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.wangdashe.top/gtsoacvwjk.html

[M05] 设置退出码
来源：http://hz.jianghu66.top/gtgylfihlt.html

Py:   sys.exit(1)
来源：http://hz.zhongyouzk.top/gtmrbxjsbr.html

PHP:  exit(1);
来源：http://hz.0kj1m.cn/gtjtuvqczp.html

JS:   process.exit(1)
来源：http://hz.ivvv.top/gtbkgojpfs.html

TS:   process.exit(1)
来源：http://hz.vqdsnc.cn/gtbejddqbg.html

Java: System.exit(1)
来源：http://hz.shanyushiyangtech.top/gtgjfwpvjk.html

Go:   os.Exit(1)
来源：http://hz.meibo888.top/gtsemehlrr.html

Ruby: exit 1
来源：http://hz.shzxlz.cn/gtcsfpoozk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.quarkkingdee.top/gtsfdgpbku.html

[M06] 向标准错误输出
来源：http://hz.zhaomingkeji.xyz/gtflkwbzrv.html

Py:   print("err", file=sys.stderr)
来源：http://hz.tanke756.top/gtlqzonlrm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.aizwys.cn/gtgqijkktb.html

JS:   console.error("err")
来源：http://hz.yuxming.cn/gtmejvkuft.html

TS:   console.error("err")
来源：http://hz.xinyue.icu/gtdszzzzce.html

Java: System.err.println("err")
来源：http://hz.cucudq.cn/gtgpacmkpl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sxryk.cn/gtetbfjkej.html

Ruby: warn "err"
来源：http://hz.meibo888.top/gtougqvnho.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hnxiangtu.top/gtwbyxanvy.html

[M07] 判断是否为主入口
来源：http://hz.yj202588.top/gtygvmqlad.html

Py:   if __name__ == "__main__":
来源：http://hz.jqgfzy.top/gtypxzorff.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xuanzx.com/gtlpbgpcww.html

JS:   require.main === module
来源：http://hz.vqdsnc.cn/gtqwunypci.html

TS:   require.main === module
来源：http://hz.yvedp.cn/gtwsbvqjkg.html

Java: public static void main(String[] args)
来源：http://hz.cucudq.cn/gtwvggdzrx.html

Go:   func main()
来源：http://hz.redwolf501.top/gthqxnnruy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.aibaodan.cn/gttqnqdhfe.html

C#:   static void Main(string[] args)
来源：http://hz.havefunace.top/gtpruyfvxf.html

[M08] 获取系统与运行时信息
来源：http://hz.yuxming.cn/gtiivfisms.html

Py:   platform.system();  platform.python_version()
来源：http://hz.aibaodan.cn/gtbytpdcdx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shangyingyoupin.top/gtdtjhopyu.html

JS:   process.platform;  process.version
来源：http://hz.tianlin.xyz/gtvftjlldr.html

TS:   process.platform;  process.version
来源：http://hz.vqdsnc.cn/gttvvfprhw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.daria6918.cn/gtiobkuvlq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yueranfly.top/gtahkofzdt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.svipenyu.cn/gtaficzmxw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.chenjidiqi.icu/gtfjujdhbg.html

================================================================================
来源：http://hz.yuxming.cn/gtxcltoeeo.html

N. 数据结构与算法
来源：http://hz.guannengcc.top/gtnvswkvce.html

================================================================================
来源：http://hz.haohaochexian.top/gtceqmjksi.html

[N01] 二分查找（有序数组）
来源：http://hz.nanxuanxn.top/gtenpksmab.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hysaishi.cn/gtzzhngage.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.pycfn.com/gtapxtiamh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.vqdsnc.cn/gtpuowqttq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dashuyun.cn/gtwureloqo.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.sxryk.cn/gtjrvruphv.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.316326.xyz/gtezklcpbh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.daxiang520.top/gtcaiiwzvc.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ydjk.org.cn/gtoxqxjgme.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yongpay.top/gtitwvgqjl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.nwbrower.top/gtoeeyacxo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.c1oappe.top/gtykphlyfr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yvedp.cn/gtmypngniu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxinkj.top/gtxtpzbkii.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shangyingyoupin.top/gtrknpomhm.html

Go:   slices.Sort(arr)
来源：http://hz.xinyue.icu/gtldplreoq.html

Ruby: arr.sort
来源：http://hz.52xcode.cn/gtuadkwihj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yueranfly.top/gtwujulpco.html

[N03] 快速排序（分治示例）
来源：http://hz.xuanzx.com/gttbzamzkr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cheryme.top/gtabtggtzq.html

PHP:  // 递归实现，或用 usort
来源：http://hz.chenzaomai.com/gtnqbuvkpm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gthovvutyy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guannengcc.top/gthueqqlyc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yangfankeji.com/gtayexlqax.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xziqi.cn/gtweqqzidk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jianghu66.top/gtsottqhnr.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gaohongyu789.top/gtqidnxrvv.html

[N04] 斐波那契数列
来源：http://hz.aibaodan.cn/gtboxeacno.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hnqzz.top/gtezyjojof.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hongshengwenyu.top/gtybeafamm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangtech.top/gteqbmsekr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hywenlv.cn/gthsqkzxwf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.meibo888.top/gtdcvsnxag.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shanyushiyangtech.top/gtwkhtxgug.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xuanzx.com/gtjnasvdxh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.nanxuanxn.top/gtvxhuzlzk.html

[N05] 最大公约数
来源：http://hz.ehwqpu.com/gtxctqgcer.html

Py:   math.gcd(a, b)
来源：http://hz.yj20258.top/gtwtzkngxc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.haohaochexian.top/gtkxvtigqs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.0kj1m.cn/gtysehyzkp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aizwys.cn/gtroyavcsn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.daxiang520.top/gteabsddmh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.daxiang520.top/gthddckwso.html

Ruby: a.gcd(b)
来源：http://hz.nanxinkj.top/gtvpeqbidn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shanyushiyangtech.top/gtauycxaus.html

[N06] 判断回文字符串
来源：http://hz.daxiang520.top/gthacaokla.html

Py:   s == s[::-1]
来源：http://hz.cashguo.top/gtooatngnz.html

PHP:  $s === strrev($s);
来源：http://hz.hnqzz.top/gtodnsoavh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.gaohongyu789.top/gtbzbtymvq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gtfvucreyd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ybcxt.top/gttundjvde.html

Go:   // 双指针从两端比较
来源：http://hz.zhiwuduotai.top/gtuqgpzyhf.html

Ruby: s == s.reverse
来源：http://hz.zhongyouzk.top/gtjfpebjyt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhengqikj.top/gtausfczyn.html

[N07] 两数之和（返回下标）
来源：http://hz.zhaomingkeji.xyz/gthsohmczt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hnqzz.top/gtimtmmmkf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.mhx1999.top/gtkqhfoiqx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.tianlin.xyz/gtqkiozgor.html

TS:   // 手写 Map<string, number>
来源：http://hz.gzhubu.top/gtozkeyfnp.html

Java: // 手写 HashMap
来源：http://hz.316326.xyz/gtgfigkfbw.html

Go:   // 手写 map[int]int
来源：http://hz.dianchejie.cn/gtmdvnvgnt.html

Ruby: // 手写 Hash
来源：http://hz.hnxiangtu.top/gtwabtrumm.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hfpthk.cn/gtcigaremg.html

[N08] 生成全排列
来源：http://hz.redwolf501.top/gtgqqcunou.html

Py:   itertools.permutations(arr)
来源：http://hz.hammf.cn/gtkxtjoish.html

PHP:  // 手写递归交换
来源：http://hz.ehwqpu.com/gthexnbgio.html

JS:   // 手写回溯递归
来源：http://hz.zycfv.cn/gtewcfcjgi.html

TS:   // 手写回溯递归
来源：http://hz.jiagoushi.top/gtbpueiftg.html

Java: // 手写回溯递归
来源：http://hz.dashuyun.cn/gtprrmlmrg.html

Go:   // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtyhlsevws.html

Ruby: arr.permutation.to_a
来源：http://hz.zhoulong.xyz/gtmmxpyxjx.html

C#:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtokwzrgkq.html

[N09] 栈与队列
来源：http://hz.dashuyun.cn/gtdmbriiwk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shzxlz.cn/gtdvdfurej.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.shanyushiyangtech.top/gthkzngmjw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jqgfzy.top/gtnbdcgpyq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.0kj1m.cn/gtpnurnhnu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shuidangran.top/gtulkwobpu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.0kj1m.cn/gtvbiplkkc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hfpthk.cn/gtdfujgomd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.chenlongwang.top/gtbsalpdig.html

[N10] 链表节点定义
来源：http://hz.wangdashe.top/gtgrltmqxi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jyoumei.cn/gtzrcpahel.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shzxlz.cn/gtzwoinczf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jianghu66.top/gtyvpvxsdf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.fzhhl.top/gtcktglkcm.html

Java: class Node { int v; Node next; }
来源：http://hz.jinghuilouyu.cn/gtlmwgvtli.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yj20258888.top/gtoxghxzju.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhoulong.xyz/gtluezkcwe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.pengpengdd.cyou/gtbefdlmfb.html

[N11] 二叉树中序遍历
来源：http://hz.shzxlz.cn/gthlbdessz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jqgufenzy.top/gtygxnucxo.html

PHP:  // 手写递归函数
来源：http://hz.sweek.top/gtjjscsfqd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.0kj1m.cn/gtfqkkntwn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cucudq.cn/gtrtbfuirn.html

Java: // 手写递归
来源：http://hz.c1oappe.top/gtovgmmgzx.html

Go:   // 手写递归
来源：http://hz.316326.xyz/gtepewxbrt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yj20258.top/gtylwamyjg.html

C#:   // 手写递归
来源：http://hz.ydjk.org.cn/gteykdifor.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.smart0.xyz/gtfwpoijdy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.birdmap.top/gtnfxqwiyp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jlsjyb.cn/gtgwheyrqb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hysaishi.cn/gtkuyhzlzs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangdashe.top/gtqkkzfrbd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangkeji.top/gteevjzzvo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yongpay.top/gtgoyuxzyk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jiagoushi.top/gtafigbdny.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.vqdsnc.cn/gtssihuddb.html

================================================================================
来源：http://hz.zhongyouzk.top/gtamilndrv.html

O. 并发与异步
来源：http://hz.jinqigufen.top/gtpcpdvytp.html

================================================================================
来源：http://hz.zdqjudy.top/gtlcuelfat.html

[O01] 启动一个线程
来源：http://hz.mhx1999.top/gtawxiqsqv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cdnleiting.top/gtfnwhjzfo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xuanzx.com/gtefswfbwf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.svipenyu.cn/gtmezqgcor.html

TS:   // 同 JS
来源：http://hz.shanyushiyangkeji.top/gtpvsucqrm.html

Java: new Thread(() -> f()).start()
来源：http://hz.pengpengdd.cyou/gtpzpxhofk.html

Go:   go f()
来源：http://hz.xuetiantiany.cn/gtlnuguvvq.html

Ruby: Thread.new { f }
来源：http://hz.zhiwuduotai.top/gtbaztcxzf.html

C#:   Task.Run(() => F());
来源：http://hz.haohaochexian.top/gtyarltksj.html

[O02] 使用线程池
来源：http://hz.dashuyun.cn/gtekpwvdag.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hnxiangtu.top/gtahbnbabc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yuxming.cn/gtskcysthi.html

JS:   // worker_threads 线程池
来源：http://hz.kuanghao11.cn/gtlnqzygkk.html

TS:   // worker_threads 线程池
来源：http://hz.guannengcc.top/gtxqeudpvl.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zycfv.cn/gtnhihkfss.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hnxiangtu.top/gtcxlfvuqu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jianghu66.top/gtviuezarh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xuetiantiany.cn/gtjwqmvwtb.html

[O03] 加锁保护共享数据
来源：http://hz.yangfankeji.com/gtoazyupme.html

Py:   with lock: shared += 1
来源：http://hz.zhongyouzk.top/gtjcpcexdm.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.redwolf501.top/gtixyzosed.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.fengsongda.top/gtvmlgzfjw.html

TS:   // 同 JS
来源：http://hz.sxryk.cn/gtnqmyxmpv.html

Java: synchronized (this) { shared++; }
来源：http://hz.aibaodan.cn/gteolniqbe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.pycfn.com/gtwvniqnfp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xinyue.icu/gtjxpyjivz.html

C#:   lock (gate) { shared++; }
来源：http://hz.aibaodan.cn/gtcqemrvoa.html

[O04] 定义异步函数并等待
来源：http://hz.ydjk.org.cn/gtxizajuzt.html

Py:   async def f():⏎    await g()
来源：http://hz.gzhubu.top/gtykvqrrdw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.havefunace.top/gtlwwtqice.html

JS:   async function f() { await g(); }
来源：http://hz.andypj.xyz/gtsldnpmhs.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hywenlv.cn/gtuvkeewbb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.0kj1m.cn/gtouxojbuu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhaomingkeji.xyz/gtuspyilan.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.guannengcc.top/gticvxshjx.html

C#:   async Task F() { await G(); }
来源：http://hz.yangfankeji.com/gtjcuttlci.html

[O05] 并发执行并等待全部完成
来源：http://hz.jiagoushi.top/gtkpzgubhf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenzaomai.com/gtfrrtfbwi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jinqigfzy.top/gtjjonqnei.html

JS:   await Promise.all(tasks)
来源：http://hz.316326.xyz/gtnsidxcay.html

TS:   await Promise.all(tasks)
来源：http://hz.meibo888.top/gtvxfrolzu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.birdmap.top/gtwdyfcqlx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xylfe.cn/gtcusgpupb.html

Ruby: threads.map(&:join)
来源：http://hz.iojbl.cn/gtzqnbmjcu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yanxiufei.cn/gttkpgkytq.html

[O06] 使用进程池
来源：http://hz.quarkkingdee.top/gtownuwhrl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.daria6918.cn/gtstwwgnbx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.chenlongwang.top/gtowgnsczq.html

JS:   // child_process / cluster 模块
来源：http://hz.jqgufenzy.top/gtcflpysde.html

TS:   // child_process / cluster 模块
来源：http://hz.zycfv.cn/gttfoivomp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xuetiantiany.cn/gtzqyymnht.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhengqikj.top/gtueboecba.html

Ruby: // fork 块
来源：http://hz.shanyushiyangtech.top/gtquifhtzf.html

C#:   Parallel.For
来源：http://hz.yj20258888.top/gtxulgotzx.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gthjjqzprw.html

P. 常用工具函数
来源：http://hz.bjfxy.top/gtddhrbeee.html

================================================================================
来源：http://hz.yj202588.top/gtmqdfyfaz.html

[P01] 生成 UUID
来源：http://hz.jianghu66.top/gtovqsxuik.html

Py:   str(uuid.uuid4())
来源：http://hz.zycfv.cn/gtkucrwwwy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jianghu66.top/gtgqijpmmd.html

JS:   crypto.randomUUID()
来源：http://hz.zhijiandao.cn/gtxrvyviyc.html

TS:   crypto.randomUUID()
来源：http://hz.sufxvd.cn/gtutaeyzgz.html

Java: UUID.randomUUID().toString()
来源：http://hz.fzhhl.top/gtiqeoqnar.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sxryk.cn/gtlrvkrytq.html

Ruby: SecureRandom.uuid
来源：http://hz.cheryme.top/gtmxnepprl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ydzc1.top/gtarluhmwe.html

[P02] MD5 / SHA256 摘要
来源：http://hz.daria6918.cn/gtzvjusyga.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.tanke756.top/gtkynzikmo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xuanzx.com/gtludgumyz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.andypj.xyz/gtpiapozbl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.andypj.xyz/gtpclnqtoy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.svipenyu.cn/gtxsifgdwl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jyoumei.cn/gtgfcbitek.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.tian-w.cn/gtfgscbbbc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jinqigufen.top/gtytnidwhg.html

[P03] 生成短随机字符串
来源：http://hz.chenjidiqi.icu/gtcgbxwzen.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ydjk.org.cn/gttufuudrs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zycfv.cn/gtkcavyeiq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.quarkkingdee.top/gtmjzwphzz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dashuyun.cn/gtkamjhwbe.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xinyue.icu/gtofzybodb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ehwqpu.com/gtmdchlwdj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhengqikj.top/gtgmrbatpf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.9152youxi.cn/gtpnszsmao.html

[P04] 求长度
来源：http://hz.yj20258.top/gtgniusdml.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.redwolf501.top/gtwhdydwfa.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhoulong.xyz/gttosplpmw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.0kj1m.cn/gthesbrilq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.tanke756.top/gtaqgnjfxu.html

Java: list.size();  map.size();  s.length()
来源：http://hz.tianlin.xyz/gtvwmdudzk.html

Go:   len(arr);  len(m)
来源：http://hz.daria6918.cn/gtvlgdbcpk.html

Ruby: x.length;  x.size
来源：http://hz.ppjwa.cn/gtgnhyvwwx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.guowangkeji.top/gtqmcrgteb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.cucudq.cn/gtocipckse.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jyoumei.cn/gtbooscwbg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jianghu66.top/gtvfzhhple.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.gogol.net.cn/gtcuwzfdvu.html


<!-- 参考信息 -->