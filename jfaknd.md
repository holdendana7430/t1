代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://hz.cucudq.cn/gtawnysrtb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hnxiangtu.top/gtxgyhkcac.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.wangdashe.top/gtewkeoenx.html

JS:   resp.ok;  resp.status
来源：http://hz.ydjk.org.cn/gttoqqklfa.html

TS:   resp.ok;  resp.status
来源：http://hz.hnxiangtu.top/gtwciexkbx.html

Java: resp.statusCode()
来源：http://hz.xuetiantiany.cn/gtcsrcsxsy.html

Go:   resp.StatusCode
来源：http://hz.yangfankeji.com/gtuhpkpqxv.html

Ruby: resp.code.to_i
来源：http://hz.ivvv.top/gtgkxpjyqd.html

C#:   (int)resp.StatusCode
来源：http://hz.sufxvd.cn/gtvmqtragi.html

[L08] 并发请求多个地址
来源：http://hz.ydjk.org.cn/gtmclrnbej.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.redwolf501.top/gtnkfogaen.html

PHP:  curl_multi_init() 系列
来源：http://hz.xinyue.icu/gthyqlytfx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.bjfxy.top/gtbiknrvdv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shzxlz.cn/gtdvfbgypd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.chenjidiqi.icu/gtsmxprjal.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shzxlz.cn/gtgqjyehrk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ydjk.org.cn/gtayonfish.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.guowangkeji.top/gtbgjjgfxv.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtbhlxxzxc.html

M. 命令行 / 进程 / 环境
来源：http://hz.birdmap.top/gtntfdxgns.html

================================================================================
来源：http://hz.sufxvd.cn/gtxcnijmpv.html

[M01] 读取命令行参数
来源：http://hz.zhaomingkeji.xyz/gtpofuiddm.html

Py:   sys.argv[1:]
来源：http://hz.hnqzz.top/gtwdlezqjh.html

PHP:  $argv;  $argc;
来源：http://hz.yuanzhike.top/gtkzioaxom.html

JS:   process.argv.slice(2)
来源：http://hz.svipenyu.cn/gtjbrrddyh.html

TS:   process.argv.slice(2)
来源：http://hz.guannengcc.top/gtoylyetvm.html

Java: args 数组（main 方法参数）
来源：http://hz.52xcode.cn/gtqefvtbgu.html

Go:   os.Args[1:]
来源：http://hz.ivvv.top/gtoekhouvm.html

Ruby: ARGV
来源：http://hz.birdmap.top/gtobhrlddm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.snrcjt.cn/gtlhvcbqns.html

[M02] 读取环境变量
来源：http://hz.jianghu66.top/gtdiqdeqyt.html

Py:   os.environ.get("HOME")
来源：http://hz.nanxuanxn.top/gtphlirrwr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ydjk.org.cn/gtzyqepsre.html

JS:   process.env.HOME
来源：http://hz.smart0.xyz/gtgnbzabrg.html

TS:   process.env.HOME
来源：http://hz.ppjwa.cn/gtkvzgoarh.html

Java: System.getenv("HOME")
来源：http://hz.zhaomingkeji.xyz/gtpumdntsv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yonumen.top/gtzyauslds.html

Ruby: ENV["HOME"]
来源：http://hz.chenlongwang.top/gtwhxoeotv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhongyouzk.top/gtdqmjzmug.html

[M03] 执行外部命令
来源：http://hz.shzxlz.cn/gtnacgolag.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yvedp.cn/gttwvigbav.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cheryme.top/gtvcmipyaw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.haohaochexian.top/gtldrtmbii.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.fengsongda.top/gtmvkmgfnh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sufxvd.cn/gtyhzfuplg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.gaohongyu789.top/gtzbekdrsp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.daxiang520.top/gtpwouvobe.html

C#:   Process.Start("ls", "-l");
来源：http://hz.feifeiyinyue.top/gtmnfmiajf.html

[M04] 获取当前工作目录
来源：http://hz.0kj1m.cn/gtwagkbobt.html

Py:   os.getcwd()
来源：http://hz.jiagoushi.top/gtnlzvshkr.html

PHP:  getcwd();
来源：http://hz.mhx1999.top/gtcdayiodl.html

JS:   process.cwd()
来源：http://hz.zhaomingkeji.xyz/gtowbratuj.html

TS:   process.cwd()
来源：http://hz.zhaomingkeji.xyz/gtbmloydbr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jianghu66.top/gtimiqspxl.html

Go:   os.Getwd()
来源：http://hz.ppjwa.cn/gtwjxjband.html

Ruby: Dir.pwd
来源：http://hz.nwbrower.top/gtmvdcjqcp.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.guannengcc.top/gtedhhceve.html

[M05] 设置退出码
来源：http://hz.chenzaomai.com/gthwqwdfna.html

Py:   sys.exit(1)
来源：http://hz.kuanghao11.cn/gtxuxzqrha.html

PHP:  exit(1);
来源：http://hz.xinyue.icu/gtwibbmomp.html

JS:   process.exit(1)
来源：http://hz.zhoulong.xyz/gtnglysghd.html

TS:   process.exit(1)
来源：http://hz.nanxinkj.top/gtfkenbhdg.html

Java: System.exit(1)
来源：http://hz.52xcode.cn/gtexuqiokz.html

Go:   os.Exit(1)
来源：http://hz.cqqwz.cn/gtpfvtvfnq.html

Ruby: exit 1
来源：http://hz.52xcode.cn/gtzbvsnhtd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.feifeiyinyue.top/gtrumlzsnp.html

[M06] 向标准错误输出
来源：http://hz.vqdsnc.cn/gtdprztzol.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sweek.top/gtrcmaaggk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zdqjudy.top/gttomomlam.html

JS:   console.error("err")
来源：http://hz.xingfuxueyuan.xyz/gtvqbztjwz.html

TS:   console.error("err")
来源：http://hz.sufxvd.cn/gtsgssxodp.html

Java: System.err.println("err")
来源：http://hz.aibaodan.cn/gtzmyeuxrw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jinqigufen.top/gtfwanlstg.html

Ruby: warn "err"
来源：http://hz.guowangkeji.top/gtnmuzpjpx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.chenlongwang.top/gtegggzauo.html

[M07] 判断是否为主入口
来源：http://hz.jqgufenzy.top/gtjeuekbjz.html

Py:   if __name__ == "__main__":
来源：http://hz.xziqi.cn/gtkhlurwjq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jyoumei.cn/gtbfjkoust.html

JS:   require.main === module
来源：http://hz.daria6918.cn/gtiokgtyfz.html

TS:   require.main === module
来源：http://hz.havefunace.top/gtvcteskci.html

Java: public static void main(String[] args)
来源：http://hz.chenzaomai.com/gtpmxdnhqn.html

Go:   func main()
来源：http://hz.hfpthk.cn/gtlglhbosh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.meibo888.top/gtnnjdkvpf.html

C#:   static void Main(string[] args)
来源：http://hz.cdnleiting.top/gtjzmsjsbi.html

[M08] 获取系统与运行时信息
来源：http://hz.cdnleiting.top/gtwjkypozy.html

Py:   platform.system();  platform.python_version()
来源：http://hz.snrcjt.cn/gtkzadxrtb.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.snrcjt.cn/gtqtvcwvkq.html

JS:   process.platform;  process.version
来源：http://hz.cqqwz.cn/gteesphxvy.html

TS:   process.platform;  process.version
来源：http://hz.yueranfly.top/gtymocbjpa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gotoacloud.top/gtxfdhawwm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yonumen.top/gtozuluahl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.havefunace.top/gtkecpdrhf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yongpay.top/gtjuzvikct.html

================================================================================
来源：http://hz.shzxlz.cn/gtvjakrhpr.html

N. 数据结构与算法
来源：http://hz.smart0.xyz/gtmrxqfkcy.html

================================================================================
来源：http://hz.ybcxt.top/gtffctutkw.html

[N01] 二分查找（有序数组）
来源：http://hz.jinyuanbaomall.cn/gtbzkoyxqd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj20258.top/gtugnzywbi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gotoacloud.top/gtmldathcg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yuxming.cn/gtvpnpjsqh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhengqikj.top/gttozductk.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhixingplan.top/gtklqbhmiu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yonumen.top/gtlrbckmcv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.daxiang520.top/gtxdcrhaeq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hnqzz.top/gtnaxrxtyf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhongyouzk.top/gtzpjmckqg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhiwuduotai.top/gtjridmfai.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cashguo.top/gthtukkefa.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.redwolf501.top/gtpyzmhnce.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtokrrtzme.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.tanke756.top/gtshngrcmu.html

Go:   slices.Sort(arr)
来源：http://hz.yj20258888.top/gtujgkbdax.html

Ruby: arr.sort
来源：http://hz.ydjk.org.cn/gtdntkkvfa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yj202588.top/gtitiuqnfw.html

[N03] 快速排序（分治示例）
来源：http://hz.dianchejie.cn/gtwfkvopux.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhongyouzk.top/gtrilkzbom.html

PHP:  // 递归实现，或用 usort
来源：http://hz.pengpengdd.cyou/gtdzbiahli.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhengqikj.top/gtfefjbvka.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xylfe.cn/gthdutiyhl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yongpay.top/gtwiojuzru.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shanyushiyangtech.top/gtyjcbocbr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gotoacloud.top/gtfszfotgi.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hysaishi.cn/gtdyclxrjo.html

[N04] 斐波那契数列
来源：http://hz.aizwys.cn/gtnfhbhqwi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ppjwa.cn/gtdwtrsiug.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.snrcjt.cn/gtoayufexm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tanke756.top/gtnuydzchi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.feifeiyinyue.top/gtvximaoqx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yueranfly.top/gtyqbrpphb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.birdmap.top/gtwzundxbq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.nwbrower.top/gtnjflioqs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yangfankeji.com/gttonbijtq.html

[N05] 最大公约数
来源：http://hz.dianchejie.cn/gtkhghkjyp.html

Py:   math.gcd(a, b)
来源：http://hz.daxiang520.top/gtqbazaxpl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhoulong.xyz/gttleccbqn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydzc1.top/gtbjufxoix.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gtryvcntzx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shanyushiyangkeji.top/gtopysbipt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.wangshuangyany.cn/gtfgpsxggs.html

Ruby: a.gcd(b)
来源：http://hz.shzxlz.cn/gtbgfjzies.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.dianchejie.cn/gtirlgvims.html

[N06] 判断回文字符串
来源：http://hz.chenlongwang.top/gtjewvqaeo.html

Py:   s == s[::-1]
来源：http://hz.chenzaomai.com/gtbucmmbcj.html

PHP:  $s === strrev($s);
来源：http://hz.shuidangran.top/gtplrrukvb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangtech.top/gtyqwlqgyw.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtdiyoqomh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shanyushiyangtech.top/gtvmhqpfuu.html

Go:   // 双指针从两端比较
来源：http://hz.ywan-chungtsiang.top/gtfzwkqfdt.html

Ruby: s == s.reverse
来源：http://hz.ppjwa.cn/gtorimldka.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinyuanbaomall.cn/gtaeydivhm.html

[N07] 两数之和（返回下标）
来源：http://hz.ivvv.top/gtfahanrpf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.vqdsnc.cn/gtidgmcdfu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.vqdsnc.cn/gtvsydudqw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.chenzaomai.com/gtjncixzqy.html

TS:   // 手写 Map<string, number>
来源：http://hz.52xcode.cn/gtnhjnxbjr.html

Java: // 手写 HashMap
来源：http://hz.yonumen.top/gtdyzqzdtf.html

Go:   // 手写 map[int]int
来源：http://hz.aizwys.cn/gtcxirriit.html

Ruby: // 手写 Hash
来源：http://hz.gogol.net.cn/gtncirzzsq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cashguo.top/gtpbdorsuh.html

[N08] 生成全排列
来源：http://hz.daria6918.cn/gtxlagkvsw.html

Py:   itertools.permutations(arr)
来源：http://hz.xziqi.cn/gtdrdrylld.html

PHP:  // 手写递归交换
来源：http://hz.52xcode.cn/gtxxzzllld.html

JS:   // 手写回溯递归
来源：http://hz.jianghu66.top/gtzhqlvzgu.html

TS:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtvnmkijwf.html

Java: // 手写回溯递归
来源：http://hz.smart0.xyz/gtowbxihbn.html

Go:   // 手写回溯递归
来源：http://hz.52xcode.cn/gtpxjfrvsn.html

Ruby: arr.permutation.to_a
来源：http://hz.hongshengwenyu.top/gtrhailjjc.html

C#:   // 手写回溯递归
来源：http://hz.yonumen.top/gtdaputzfr.html

[N09] 栈与队列
来源：http://hz.ydjk.org.cn/gtzadzfryj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.birdmap.top/gtngkmodur.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ybcxt.top/gtijxitejl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hongshengwenyu.top/gtcblsnbwo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.aibaodan.cn/gtlatrrfpv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.52xcode.cn/gtofxxlbwp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.pengpengdd.cyou/gtwasjwtzm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.tanke756.top/gtajdgrwyq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.kuanghao11.cn/gtkhnornvz.html

[N10] 链表节点定义
来源：http://hz.jyoumei.cn/gtyhrwbdrl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ybcxt.top/gtkngibwzu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hammf.cn/gtvdkjblaq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ydjk.org.cn/gtjjresrwb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.wangshuangyany.cn/gtcoxoseaf.html

Java: class Node { int v; Node next; }
来源：http://hz.zycfv.cn/gtowpryqwo.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.316326.xyz/gtnpegljul.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinghuilouyu.cn/gtnwtnxaww.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhijiandao.cn/gtmzylzujs.html

[N11] 二叉树中序遍历
来源：http://hz.yueranfly.top/gtrkjhckde.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.dashuyun.cn/gtavytyyof.html

PHP:  // 手写递归函数
来源：http://hz.ydzc1.top/gtnhycclrp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yanxiufei.cn/gtfdbhdvmb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenlongwang.top/gthxshetrz.html

Java: // 手写递归
来源：http://hz.xingfuxueyuan.xyz/gtyedvwyoz.html

Go:   // 手写递归
来源：http://hz.hammf.cn/gtzbwrmaah.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tanke756.top/gtbaxbydpv.html

C#:   // 手写递归
来源：http://hz.shanyushiyangtech.top/gtlxrhegzp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ydzc1.top/gtahfebiiv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.gaohongyu789.top/gtlfuzofrv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinqigfzy.top/gtyvnxovjl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sufxvd.cn/gtylfzvokj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangdashe.top/gtsrtmbotk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.kuanghao11.cn/gtutmnnmel.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.bjfxy.top/gtfetnysmp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinqigufen.top/gtqvrjdfdf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guannengcc.top/gtdsturuqj.html

================================================================================
来源：http://hz.ehwqpu.com/gtzzhsaetc.html

O. 并发与异步
来源：http://hz.ivvv.top/gtvnfrkgei.html

================================================================================
来源：http://hz.zhoulong.xyz/gtmzjhlvbi.html

[O01] 启动一个线程
来源：http://hz.zycfv.cn/gtirmekpir.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.meibo888.top/gtanmuspsa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.wangdashe.top/gtfutclwun.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ywan-chungtsiang.top/gtgkihhqpl.html

TS:   // 同 JS
来源：http://hz.guowangkeji.top/gtdlftzgxm.html

Java: new Thread(() -> f()).start()
来源：http://hz.aizwys.cn/gtpghwrwxk.html

Go:   go f()
来源：http://hz.jqgfzy.top/gtzexifglx.html

Ruby: Thread.new { f }
来源：http://hz.zhongyouzk.top/gtmvlufmmq.html

C#:   Task.Run(() => F());
来源：http://hz.hongshengwenyu.top/gtegnzphoe.html

[O02] 使用线程池
来源：http://hz.hammf.cn/gtydeblmze.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yvedp.cn/gtkkgnnjbw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ywan-chungtsiang.top/gthvtwrcuk.html

JS:   // worker_threads 线程池
来源：http://hz.zhaomingkeji.xyz/gtevrzfzdx.html

TS:   // worker_threads 线程池
来源：http://hz.ivvv.top/gtelxnqhyd.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.nwbrower.top/gtekatauvt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhengqikj.top/gtvqpxvqix.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hammf.cn/gtbutccshb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.snrcjt.cn/gtpimzgbpf.html

[O03] 加锁保护共享数据
来源：http://hz.tanke756.top/gthrkprzqv.html

Py:   with lock: shared += 1
来源：http://hz.kuanghao11.cn/gttwhmuotc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.daxiang520.top/gthfoeptpu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhaomingkeji.xyz/gthavclxwd.html

TS:   // 同 JS
来源：http://hz.zdqjudy.top/gthfdigzxt.html

Java: synchronized (this) { shared++; }
来源：http://hz.jlsjyb.cn/gtkixotsog.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cheryme.top/gtsmtlhsqy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shanyushiyangkeji.top/gtmfjjezrk.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhoulong.xyz/gtjruskglr.html

[O04] 定义异步函数并等待
来源：http://hz.dianchejie.cn/gtfalhtufe.html

Py:   async def f():⏎    await g()
来源：http://hz.ivvv.top/gttcccoylh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.andypj.xyz/gtgrvyjfoq.html

JS:   async function f() { await g(); }
来源：http://hz.sufxvd.cn/gtvffzzbyj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yuanzhike.top/gtesczyoch.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yonumen.top/gtujpezdsk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ydzc1.top/gtieunbfre.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.aizwys.cn/gtcciulowp.html

C#:   async Task F() { await G(); }
来源：http://hz.zdqjudy.top/gtrcsbsbpk.html

[O05] 并发执行并等待全部完成
来源：http://hz.zdqjudy.top/gtpuuwdybc.html

Py:   asyncio.gather(*tasks)
来源：http://hz.pycfn.com/gtuufihbit.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gogol.net.cn/gtwhttgglj.html

JS:   await Promise.all(tasks)
来源：http://hz.jinyuanbaomall.cn/gtpaohddvo.html

TS:   await Promise.all(tasks)
来源：http://hz.pycfn.com/gtjadvpxvc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.chenjidiqi.icu/gtnwequpzh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hywenlv.cn/gtfcadqvns.html

Ruby: threads.map(&:join)
来源：http://hz.jinyuanbaomall.cn/gtxiputliv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.0kj1m.cn/gthlhtbmyz.html

[O06] 使用进程池
来源：http://hz.shanyushiyangtech.top/gtyibysxdg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.aizwys.cn/gtnxblwloe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhoulong.xyz/gtizjdlopc.html

JS:   // child_process / cluster 模块
来源：http://hz.svipenyu.cn/gtlpjkfvhu.html

TS:   // child_process / cluster 模块
来源：http://hz.kuanghao11.cn/gtspvzghpz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.tian-w.cn/gtgjxlwiff.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hfpthk.cn/gtpxxbkuwe.html

Ruby: // fork 块
来源：http://hz.chenjidiqi.icu/gtezmyhomm.html

C#:   Parallel.For
来源：http://hz.jlsjyb.cn/gtkudtnjhi.html

================================================================================
来源：http://hz.cheryme.top/gtsnujiewx.html

P. 常用工具函数
来源：http://hz.nwbrower.top/gtqmtulvgc.html

================================================================================
来源：http://hz.nanxuanxn.top/gtvelnusxl.html

[P01] 生成 UUID
来源：http://hz.tanke756.top/gtnmczduah.html

Py:   str(uuid.uuid4())
来源：http://hz.pycfn.com/gtwgvsgnxy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinyuanbaomall.cn/gtdbgfweas.html

JS:   crypto.randomUUID()
来源：http://hz.bjfxy.top/gtiyoiexxc.html

TS:   crypto.randomUUID()
来源：http://hz.jqgfzy.top/gtzsgbkrbu.html

Java: UUID.randomUUID().toString()
来源：http://hz.daxiang520.top/gtrtomitpt.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ppjwa.cn/gtqdycgzzg.html

Ruby: SecureRandom.uuid
来源：http://hz.cheryme.top/gtztjbhijc.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.tianlin.xyz/gtxovlqipe.html

[P02] MD5 / SHA256 摘要
来源：http://hz.nanxinkj.top/gtztqcnnju.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yj20258.top/gtbwrhcymm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ybcxt.top/gtzrikiodu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.havefunace.top/gtvcyveedb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhiwuduotai.top/gtcwfwyhis.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.smart0.xyz/gtbjmeusty.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xuanzx.com/gtzutjpguu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jianghu66.top/gtqvjwrneu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cucudq.cn/gtzpncmjlv.html

[P03] 生成短随机字符串
来源：http://hz.zhoulong.xyz/gtudnbqash.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ybcxt.top/gtrvaodkkg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.dashuyun.cn/gtmloosgze.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.haohaochexian.top/gtqyvdbcgi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigufen.top/gtyauprmbw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.fzhhl.top/gtolqgtubg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.havefunace.top/gtzpuivnyz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.nanxinkj.top/gtbferwcti.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.birdmap.top/gtocijkhnh.html

[P04] 求长度
来源：http://hz.guannengcc.top/gtvwbydhgc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gogol.net.cn/gtsbzfrepp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hnqzz.top/gtlfxxvmvj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj202588.top/gtzujkaprc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.bjfxy.top/gtlomfowlk.html

Java: list.size();  map.size();  s.length()
来源：http://hz.guannengcc.top/gtzzqccjcw.html

Go:   len(arr);  len(m)
来源：http://hz.zhiwuduotai.top/gtwwbzsurt.html

Ruby: x.length;  x.size
来源：http://hz.sufxvd.cn/gtaviyvikz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.iojbl.cn/gthgpqswhl.html


<!-- 参考信息 -->