代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhixingplan.top/gtuofpuqid.html

Ruby: ENV["HOME"]
来源：http://hz.yvedp.cn/gtsnsgsppm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.mhx1999.top/gtkdmtlukk.html

[M03] 执行外部命令
来源：http://hz.smart0.xyz/gtozshsdrl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xylfe.cn/gtaupjsmlv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shanyushiyangtech.top/gtroezrymd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangshuangyany.cn/gtzzgtsqmo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hfpthk.cn/gtdmkcbdzo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ywan-chungtsiang.top/gtzfcbbbwe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jyoumei.cn/gtvnihfuhd.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.vqdsnc.cn/gtfyehqvkg.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinyuanbaomall.cn/gtobcajquu.html

[M04] 获取当前工作目录
来源：http://hz.yongpay.top/gtkkmwcfcz.html

Py:   os.getcwd()
来源：http://hz.gzhubu.top/gtkjcaitiq.html

PHP:  getcwd();
来源：http://hz.fzhhl.top/gtkdzuynza.html

JS:   process.cwd()
来源：http://hz.zhengqikj.top/gtaudqpcay.html

TS:   process.cwd()
来源：http://hz.vqdsnc.cn/gtcpqhawno.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gogol.net.cn/gtgehnnqfu.html

Go:   os.Getwd()
来源：http://hz.zhongyouzk.top/gtqialsrkc.html

Ruby: Dir.pwd
来源：http://hz.316326.xyz/gteenjkxhh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yuanzhike.top/gtikizrwrr.html

[M05] 设置退出码
来源：http://hz.c1oappe.top/gtbmqicxkp.html

Py:   sys.exit(1)
来源：http://hz.zhiwuduotai.top/gteijqkqyd.html

PHP:  exit(1);
来源：http://hz.gzhubu.top/gtxtxnvhhs.html

JS:   process.exit(1)
来源：http://hz.gaohongyu789.top/gtqdmzzrtl.html

TS:   process.exit(1)
来源：http://hz.hnxiangtu.top/gtshokuskc.html

Java: System.exit(1)
来源：http://hz.andypj.xyz/gtqsddpezp.html

Go:   os.Exit(1)
来源：http://hz.shuidangran.top/gtgnsrgfyl.html

Ruby: exit 1
来源：http://hz.mhx1999.top/gthyceldaw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ppjwa.cn/gtsybsactf.html

[M06] 向标准错误输出
来源：http://hz.ybcxt.top/gtbkmwgdex.html

Py:   print("err", file=sys.stderr)
来源：http://hz.aibaodan.cn/gtgoatyzig.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenjidiqi.icu/gtwbnoxhwq.html

JS:   console.error("err")
来源：http://hz.xuetiantiany.cn/gtjrfrcxyu.html

TS:   console.error("err")
来源：http://hz.tianlin.xyz/gtaywcygpb.html

Java: System.err.println("err")
来源：http://hz.sysykeji.top/gtvgddbqkb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gaohongyu789.top/gtuqvtqntg.html

Ruby: warn "err"
来源：http://hz.zhaomingkeji.xyz/gtsiexpnyk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.dianchejie.cn/gtlmtyahbs.html

[M07] 判断是否为主入口
来源：http://hz.dashuyun.cn/gtflziphev.html

Py:   if __name__ == "__main__":
来源：http://hz.sysykeji.top/gtxzzagwlj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ywan-chungtsiang.top/gtmbwnranc.html

JS:   require.main === module
来源：http://hz.xylfe.cn/gtugtlqkas.html

TS:   require.main === module
来源：http://hz.dianchejie.cn/gtmjhbsalb.html

Java: public static void main(String[] args)
来源：http://hz.0kj1m.cn/gtoxhfyyun.html

Go:   func main()
来源：http://hz.jqgfzy.top/gttdkjxufz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zycfv.cn/gtonjpssno.html

C#:   static void Main(string[] args)
来源：http://hz.tanke756.top/gticqcxevy.html

[M08] 获取系统与运行时信息
来源：http://hz.zycfv.cn/gtegwuebgg.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ybcxt.top/gtvpuruoky.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jlsjyb.cn/gtfqrvvhue.html

JS:   process.platform;  process.version
来源：http://hz.meibo888.top/gtxdtvoggt.html

TS:   process.platform;  process.version
来源：http://hz.ywan-chungtsiang.top/gtkicdyyiw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.wangshuangyany.cn/gtlgdpfvgj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gogol.net.cn/gthfqlhqbx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinghuilouyu.cn/gtygokiklo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhengqikj.top/gtdcifplnh.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtzvqfnsji.html

N. 数据结构与算法
来源：http://hz.gzhubu.top/gtymcapjnp.html

================================================================================
来源：http://hz.yvedp.cn/gtasotvcte.html

[N01] 二分查找（有序数组）
来源：http://hz.nanxinkj.top/gtgzgjxfvv.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ivvv.top/gtknviyjmb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.guowangkeji.top/gtoewnpjry.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xziqi.cn/gtbcfebaoc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fzhhl.top/gtmedweksx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yj20258.top/gtsyzqeahw.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.nanxuanxn.top/gtjubeihkx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.aizwys.cn/gtmrjmgoyi.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhongyouzk.top/gtikcesvhi.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gotoacloud.top/gtmrxooaxv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.haohaochexian.top/gtwvnnqozk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.meibo888.top/gtumjcbutx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hongshengwenyu.top/gtwrbqxvei.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nwbrower.top/gtgylnmaoa.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ivvv.top/gtcobsknmv.html

Go:   slices.Sort(arr)
来源：http://hz.xziqi.cn/gtulzcdwrt.html

Ruby: arr.sort
来源：http://hz.ppjwa.cn/gthxbacens.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.nwbrower.top/gtxqlvorcw.html

[N03] 快速排序（分治示例）
来源：http://hz.quarkkingdee.top/gtfxvzyoyg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yuanzhike.top/gtdbrhucqg.html

PHP:  // 递归实现，或用 usort
来源：http://hz.snrcjt.cn/gtsuxphuuw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dashuyun.cn/gtnfdhibln.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hammf.cn/gtijvxdeiw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ivvv.top/gtssvxdpxe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yangfankeji.com/gtisdbgzak.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cdnleiting.top/gtribbwrfv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.fengsongda.top/gtvxoinzqu.html

[N04] 斐波那契数列
来源：http://hz.cheryme.top/gtseqgefms.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xylfe.cn/gtziklkcju.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.haohaochexian.top/gtqygchzvo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aibaodan.cn/gtrnldwzxa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yvedp.cn/gtfjeoseva.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ydzc1.top/gtleztshff.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.nwbrower.top/gtrdlqwtzr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cashguo.top/gtklabtake.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cashguo.top/gtowzubzqz.html

[N05] 最大公约数
来源：http://hz.meibo888.top/gthtuytoyg.html

Py:   math.gcd(a, b)
来源：http://hz.redwolf501.top/gtwlnbuuku.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.svipenyu.cn/gtzzppdxln.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ivvv.top/gtxcmhcefw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.c1oappe.top/gttifwtvui.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhixingplan.top/gtgrrovynz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.quarkkingdee.top/gtndtmovgb.html

Ruby: a.gcd(b)
来源：http://hz.yj202588.top/gtzrazeuul.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zdqjudy.top/gtlyfhsbxd.html

[N06] 判断回文字符串
来源：http://hz.tanke756.top/gtwddxhjgt.html

Py:   s == s[::-1]
来源：http://hz.316326.xyz/gtvliogugl.html

PHP:  $s === strrev($s);
来源：http://hz.tanke756.top/gtfyugltda.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zycfv.cn/gtmmiuaige.html

TS:   s === [...s].reverse().join("")
来源：http://hz.daxiang520.top/gttropmugh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jianghu66.top/gtihxwdazb.html

Go:   // 双指针从两端比较
来源：http://hz.daria6918.cn/gtxoqdkact.html

Ruby: s == s.reverse
来源：http://hz.andypj.xyz/gtaqkdkyjj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xinyue.icu/gthksozreg.html

[N07] 两数之和（返回下标）
来源：http://hz.redwolf501.top/gtxwunmlaw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.aizwys.cn/gtlazbkmlf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gogol.net.cn/gtebbuubzs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ywan-chungtsiang.top/gtpzyiexcn.html

TS:   // 手写 Map<string, number>
来源：http://hz.jlsjyb.cn/gtpvunolru.html

Java: // 手写 HashMap
来源：http://hz.smart0.xyz/gtuosecvwu.html

Go:   // 手写 map[int]int
来源：http://hz.yongpay.top/gtmhcpdzmg.html

Ruby: // 手写 Hash
来源：http://hz.svipenyu.cn/gtaxzlzvcv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinqigufen.top/gtkbsnsvqv.html

[N08] 生成全排列
来源：http://hz.nanxuanxn.top/gtrtjuarvd.html

Py:   itertools.permutations(arr)
来源：http://hz.jinqigfzy.top/gtwkhutnaj.html

PHP:  // 手写递归交换
来源：http://hz.fzhhl.top/gtudacekna.html

JS:   // 手写回溯递归
来源：http://hz.yvedp.cn/gtfkfmfmen.html

TS:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gthdrekpqz.html

Java: // 手写回溯递归
来源：http://hz.sxryk.cn/gtomsrjxpm.html

Go:   // 手写回溯递归
来源：http://hz.ybcxt.top/gtfwqkdnil.html

Ruby: arr.permutation.to_a
来源：http://hz.zhixingplan.top/gtugbnscsh.html

C#:   // 手写回溯递归
来源：http://hz.yongpay.top/gtohoaoqcv.html

[N09] 栈与队列
来源：http://hz.cdnleiting.top/gtfokykwym.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.9152youxi.cn/gtxuclknal.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.sweek.top/gtstswnnmd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.shzxlz.cn/gtmlkaotrh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.chenzaomai.com/gtfdsksjpq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xingfuxueyuan.xyz/gtyiqzzbpo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sufxvd.cn/gtpohweysa.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.wangshuangyany.cn/gtggbpzjov.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ybcxt.top/gtrtkavbua.html

[N10] 链表节点定义
来源：http://hz.cheryme.top/gtfejjjmmh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yj20258888.top/gtdraehpmp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.pengpengdd.cyou/gthgwqwlde.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.0kj1m.cn/gtlsvosavk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhoulong.xyz/gtuietoqyi.html

Java: class Node { int v; Node next; }
来源：http://hz.shangyingyoupin.top/gtlbisgvjr.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.vqdsnc.cn/gtxkbcigfi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hammf.cn/gtkjzlxjib.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hnqzz.top/gtdhdnnopl.html

[N11] 二叉树中序遍历
来源：http://hz.wangshuangyany.cn/gtbfchjmyw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.wangshuangyany.cn/gtdgnjcfhh.html

PHP:  // 手写递归函数
来源：http://hz.havefunace.top/gtyagpxnqo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.0kj1m.cn/gtypeqfcit.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnqzz.top/gtnosfwizj.html

Java: // 手写递归
来源：http://hz.ywan-chungtsiang.top/gtglbdrgln.html

Go:   // 手写递归
来源：http://hz.mhx1999.top/gtlhpjuetg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cdnleiting.top/gtemumnzjn.html

C#:   // 手写递归
来源：http://hz.chenlongwang.top/gtavdbuvmp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.guannengcc.top/gtttulmuvq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yj20258.top/gtnzhlkmgb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.dashuyun.cn/gtpfehvmhh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hnqzz.top/gttfawjohp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zycfv.cn/gtcylaawfx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gotoacloud.top/gtbtdxpadz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ydzc1.top/gtqgovzvrp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yanxiufei.cn/gttvwihqcs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenlongwang.top/gtegyqhqol.html

================================================================================
来源：http://hz.zhoulong.xyz/gtvliadrzd.html

O. 并发与异步
来源：http://hz.jianghu66.top/gtoemkfnby.html

================================================================================
来源：http://hz.kuanghao11.cn/gtmrsuurlh.html

[O01] 启动一个线程
来源：http://hz.iojbl.cn/gthnymmqdn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.snrcjt.cn/gtpxnfdjni.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cucudq.cn/gtlzrdyubn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cucudq.cn/gtamxmkzzp.html

TS:   // 同 JS
来源：http://hz.gzhubu.top/gtclqjveqn.html

Java: new Thread(() -> f()).start()
来源：http://hz.yj20258888.top/gtdjrmiikn.html

Go:   go f()
来源：http://hz.redwolf501.top/gtlwrsqeul.html

Ruby: Thread.new { f }
来源：http://hz.xuetiantiany.cn/gtwcggfvic.html

C#:   Task.Run(() => F());
来源：http://hz.andypj.xyz/gtknwhinno.html

[O02] 使用线程池
来源：http://hz.xuanzx.com/gtkcpxxgeg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.nwbrower.top/gtucnpbdfi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinghuilouyu.cn/gtlhkfyoto.html

JS:   // worker_threads 线程池
来源：http://hz.wangdashe.top/gtqljmseuj.html

TS:   // worker_threads 线程池
来源：http://hz.ybcxt.top/gtzkhnfqhi.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.sysykeji.top/gtbmeivpzt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ehwqpu.com/gtvxfacsll.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhiwuduotai.top/gtdbiefjod.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hfpthk.cn/gtubzbcroe.html

[O03] 加锁保护共享数据
来源：http://hz.svipenyu.cn/gtgkktvomp.html

Py:   with lock: shared += 1
来源：http://hz.yangfankeji.com/gtfupsxgnn.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jqgfzy.top/gtzunnzspw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhixingplan.top/gtbwfhsmah.html

TS:   // 同 JS
来源：http://hz.xylfe.cn/gtyctrnyob.html

Java: synchronized (this) { shared++; }
来源：http://hz.xylfe.cn/gtqltihlor.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yj20258888.top/gteepnrbdh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.gotoacloud.top/gthuxaxpau.html

C#:   lock (gate) { shared++; }
来源：http://hz.hysaishi.cn/gtglqwaewk.html

[O04] 定义异步函数并等待
来源：http://hz.yvedp.cn/gtjlaiycuj.html

Py:   async def f():⏎    await g()
来源：http://hz.zhixingplan.top/gtigvpjbes.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.aizwys.cn/gtdpjyhtyg.html

JS:   async function f() { await g(); }
来源：http://hz.ydzc1.top/gturmstwsf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.aizwys.cn/gtqrqlwlgu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhixingplan.top/gtxryxykxr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shangyingyoupin.top/gtxicpzodf.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.52xcode.cn/gtrjnisclz.html

C#:   async Task F() { await G(); }
来源：http://hz.smart0.xyz/gtzzclqntj.html

[O05] 并发执行并等待全部完成
来源：http://hz.c1oappe.top/gtxkzwyeba.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinqigfzy.top/gthykwdjmu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ydzc1.top/gthzesipgk.html

JS:   await Promise.all(tasks)
来源：http://hz.hfpthk.cn/gtcmttvitz.html

TS:   await Promise.all(tasks)
来源：http://hz.xinyue.icu/gtxsqxflvp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.kuanghao11.cn/gtppnynuav.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.9152youxi.cn/gtigfrhokk.html

Ruby: threads.map(&:join)
来源：http://hz.andypj.xyz/gtqhkjtzpb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhiwuduotai.top/gtpvecavea.html

[O06] 使用进程池
来源：http://hz.mhx1999.top/gtysjwfuge.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.wangshuangyany.cn/gtrwtssxcu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.gzhubu.top/gtscppedye.html

JS:   // child_process / cluster 模块
来源：http://hz.jinghuilouyu.cn/gtlcnjnocx.html

TS:   // child_process / cluster 模块
来源：http://hz.xylfe.cn/gtrrhcjzud.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jiagoushi.top/gtarssknhx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nanxuanxn.top/gtuwtnrdvg.html

Ruby: // fork 块
来源：http://hz.ydjk.org.cn/gttwwqnzaw.html

C#:   Parallel.For
来源：http://hz.ehwqpu.com/gtmlafyehv.html

================================================================================
来源：http://hz.sxryk.cn/gtubyqjpjh.html

P. 常用工具函数
来源：http://hz.yanxiufei.cn/gtrihjvdhc.html

================================================================================
来源：http://hz.snrcjt.cn/gtizdegbqw.html

[P01] 生成 UUID
来源：http://hz.zycfv.cn/gtukottrjg.html

Py:   str(uuid.uuid4())
来源：http://hz.mhx1999.top/gtxlhxsiym.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jqgfzy.top/gttiovxaxu.html

JS:   crypto.randomUUID()
来源：http://hz.fengsongda.top/gtddrauqyf.html

TS:   crypto.randomUUID()
来源：http://hz.yanxiufei.cn/gtbzxokixo.html

Java: UUID.randomUUID().toString()
来源：http://hz.52xcode.cn/gtonzmyisk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gotoacloud.top/gtegqpfzcj.html

Ruby: SecureRandom.uuid
来源：http://hz.chenlongwang.top/gtszvlletx.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sysykeji.top/gtckjnfkqo.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yj20258.top/gteupyxcff.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.bjfxy.top/gtlkfdgbdp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.kuanghao11.cn/gthantanyr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.316326.xyz/gtelzjrdzu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jiagoushi.top/gtyagtgbhg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cucudq.cn/gtykselprk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.kuanghao11.cn/gtyaofyfge.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.shangyingyoupin.top/gtkbkixmgc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yj20258888.top/gtiyswhylv.html

[P03] 生成短随机字符串
来源：http://hz.xziqi.cn/gtoyedkxzm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sweek.top/gtcsqjwtwi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xinyue.icu/gtgglctsbs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangtech.top/gtpvjbdjmz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258.top/gtdsghhljq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yj202588.top/gtdccoiuvj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yanxiufei.cn/gtejbcukut.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.nanxuanxn.top/gtrvvvhtlc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hnxiangtu.top/gtgmsdvyds.html

[P04] 求长度
来源：http://hz.sufxvd.cn/gtfofkqhux.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jianghu66.top/gtpkvpfnbs.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtxbyqfreh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhiwuduotai.top/gtglhhvtou.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xingfuxueyuan.xyz/gtmqqmrcss.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yj20258888.top/gtzcypqhjt.html

Go:   len(arr);  len(m)
来源：http://hz.hywenlv.cn/gtrpdarsut.html

Ruby: x.length;  x.size
来源：http://hz.cheryme.top/gtzwemzhax.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.guowangkeji.top/gtkalxfhwb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jiagoushi.top/gtevfgxjaq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hongshengwenyu.top/gtswmlocie.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xingfuxueyuan.xyz/gtiichevid.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ehwqpu.com/gtyqqynali.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.c1oappe.top/gtenemchpz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sxryk.cn/gtljuylwan.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jyoumei.cn/gtftkslstc.html

Ruby: a == b
来源：http://hz.shzxlz.cn/gtzshzcedx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.nwbrower.top/gtqzwodqrd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jianghu66.top/gtjmbpshej.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hammf.cn/gticvqfxzj.html

PHP:  if (empty($x)) {}
来源：http://hz.shanyushiyangkeji.top/gtrctuusde.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinqigfzy.top/gttiqpnsbf.html

TS:   if (x == null) {}
来源：http://hz.zhijiandao.cn/gthpznhmek.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhengqikj.top/gtcqrybbud.html

Go:   if x == nil {}
来源：http://hz.chenjidiqi.icu/gtzzcnyhre.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xuanzx.com/gtclyrsuze.html

C#:   if (x is null) {}
来源：http://hz.aizwys.cn/gtazrdoorm.html

[P07] 防抖与节流
来源：http://hz.shzxlz.cn/gtjmwzzfnw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.andypj.xyz/gteztndfju.html

PHP:  // 手写时间戳比较
来源：http://hz.xylfe.cn/gtcztjftaq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.snrcjt.cn/gtafashrgk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zdqjudy.top/gtvxlyhodz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.9152youxi.cn/gtaghvxtxr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hywenlv.cn/gtzclvxgrk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gzhubu.top/gtflqnunak.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.bjfxy.top/gtiiaavrdk.html

[P08] 处理浮点精度问题
来源：http://hz.zhijiandao.cn/gtftrzunar.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.mhx1999.top/gtcdhztuel.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.nanxuanxn.top/gtdacwshxm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhijiandao.cn/gtbydcpeyv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhixingplan.top/gtwkpsmkwz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yanxiufei.cn/gtaqaufwbm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.dashuyun.cn/gtiwbuqthg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hnqzz.top/gtulzxoqoq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ydzc1.top/gtjoidxskq.html


<!-- 参考信息 -->