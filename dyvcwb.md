代发 wailian999

C#:   (int)resp.StatusCode
来源：http://hz.guowangkeji.top/gttvqbspid.html

[L08] 并发请求多个地址
来源：http://hz.ivvv.top/gtjqlphrfi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xingfuxueyuan.xyz/gtlacmjkwe.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangdashe.top/gtepftfhdy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pycfn.com/gtgddwzdcm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aibaodan.cn/gtpgsjuhjy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.snrcjt.cn/gtrhcmhtae.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gotoacloud.top/gthptpqsiw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhongyouzk.top/gtrcgnnfvj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.aizwys.cn/gtuoxaniyb.html

================================================================================
来源：http://hz.chenzaomai.com/gtjwjoyemj.html

M. 命令行 / 进程 / 环境
来源：http://hz.jianghu66.top/gtxvkbqdsq.html

================================================================================
来源：http://hz.jqgfzy.top/gtxfudbkcg.html

[M01] 读取命令行参数
来源：http://hz.xuetiantiany.cn/gtjyotsbjm.html

Py:   sys.argv[1:]
来源：http://hz.cdnleiting.top/gtrbsryuyk.html

PHP:  $argv;  $argc;
来源：http://hz.ydjk.org.cn/gtgojgtrzs.html

JS:   process.argv.slice(2)
来源：http://hz.daria6918.cn/gtoyaywzzl.html

TS:   process.argv.slice(2)
来源：http://hz.zhiwuduotai.top/gtekbdpmfz.html

Java: args 数组（main 方法参数）
来源：http://hz.hnxiangtu.top/gtdvusizjk.html

Go:   os.Args[1:]
来源：http://hz.hammf.cn/gtprgdkmix.html

Ruby: ARGV
来源：http://hz.daria6918.cn/gtoeywtmjj.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ydjk.org.cn/gtketezyjs.html

[M02] 读取环境变量
来源：http://hz.0kj1m.cn/gtmqrqjzff.html

Py:   os.environ.get("HOME")
来源：http://hz.52xcode.cn/gtupvlowyl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.haohaochexian.top/gtehlgsdxq.html

JS:   process.env.HOME
来源：http://hz.gotoacloud.top/gthbpkzaxv.html

TS:   process.env.HOME
来源：http://hz.meibo888.top/gtcgpqrtnx.html

Java: System.getenv("HOME")
来源：http://hz.xinyue.icu/gtifmtlzdn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hfpthk.cn/gttpwobhcm.html

Ruby: ENV["HOME"]
来源：http://hz.ivvv.top/gteuckutwv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhaomingkeji.xyz/gtealgshxr.html

[M03] 执行外部命令
来源：http://hz.52xcode.cn/gtqllotylr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuanzhike.top/gtxxmvbjpp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sysykeji.top/gthegkmpde.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhiwuduotai.top/gtgqmqntwz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangshuangyany.cn/gtfvprauuo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinqigfzy.top/gttvkvxbhm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jianghu66.top/gtgyekdycu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhengqikj.top/gtpjtvehil.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jlsjyb.cn/gthadaurvi.html

[M04] 获取当前工作目录
来源：http://hz.ywan-chungtsiang.top/gtbomosqba.html

Py:   os.getcwd()
来源：http://hz.xuanzx.com/gtoetqoatl.html

PHP:  getcwd();
来源：http://hz.andypj.xyz/gtkdglqkod.html

JS:   process.cwd()
来源：http://hz.chenjidiqi.icu/gteydetyvu.html

TS:   process.cwd()
来源：http://hz.316326.xyz/gtehdpmbod.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yangfankeji.com/gtccuirorn.html

Go:   os.Getwd()
来源：http://hz.xingfuxueyuan.xyz/gtljsyognl.html

Ruby: Dir.pwd
来源：http://hz.hnxiangtu.top/gtiltuliov.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yueranfly.top/gtqjktkisy.html

[M05] 设置退出码
来源：http://hz.meibo888.top/gtuiboahdp.html

Py:   sys.exit(1)
来源：http://hz.birdmap.top/gtponsabfs.html

PHP:  exit(1);
来源：http://hz.aibaodan.cn/gtusdlrzol.html

JS:   process.exit(1)
来源：http://hz.zhoulong.xyz/gtlhkakuov.html

TS:   process.exit(1)
来源：http://hz.zhixingplan.top/gtjshbqyuq.html

Java: System.exit(1)
来源：http://hz.ydzc1.top/gtoyfcyblb.html

Go:   os.Exit(1)
来源：http://hz.sysykeji.top/gtydcbwrlg.html

Ruby: exit 1
来源：http://hz.shanyushiyangtech.top/gtnxwddzdr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.pengpengdd.cyou/gtbxzzavkm.html

[M06] 向标准错误输出
来源：http://hz.jlsjyb.cn/gtirkeaghz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.birdmap.top/gtfqotyviu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.havefunace.top/gtobfxqwfv.html

JS:   console.error("err")
来源：http://hz.xingfuxueyuan.xyz/gtlvoohoqw.html

TS:   console.error("err")
来源：http://hz.meibo888.top/gtbgqjxgfv.html

Java: System.err.println("err")
来源：http://hz.shanyushiyangkeji.top/gtxkbtwstm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jyoumei.cn/gtqqsvvakl.html

Ruby: warn "err"
来源：http://hz.zhoulong.xyz/gtkzgxvdnp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hammf.cn/gtaczdhyhp.html

[M07] 判断是否为主入口
来源：http://hz.hnxiangtu.top/gtiwpcjedn.html

Py:   if __name__ == "__main__":
来源：http://hz.chenzaomai.com/gtnshpjmiw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shzxlz.cn/gtzubgkjyd.html

JS:   require.main === module
来源：http://hz.iojbl.cn/gttlrnqhmd.html

TS:   require.main === module
来源：http://hz.shanyushiyangtech.top/gtxhibcvoq.html

Java: public static void main(String[] args)
来源：http://hz.jinyuanbaomall.cn/gtxsbciiww.html

Go:   func main()
来源：http://hz.cheryme.top/gtmnfdsqrf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.redwolf501.top/gtswmbddbe.html

C#:   static void Main(string[] args)
来源：http://hz.kuanghao11.cn/gtjatsdbjh.html

[M08] 获取系统与运行时信息
来源：http://hz.zycfv.cn/gtgpqlhkpq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gaohongyu789.top/gtpcgnjgqs.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.9152youxi.cn/gtpkqcqkzv.html

JS:   process.platform;  process.version
来源：http://hz.jqgufenzy.top/gtfphvieuh.html

TS:   process.platform;  process.version
来源：http://hz.zhijiandao.cn/gtqiqpkmgg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.316326.xyz/gtimnwctgx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhaomingkeji.xyz/gtpamlntut.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ywan-chungtsiang.top/gtkgxzzrxi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj20258888.top/gtcfxgkuff.html

================================================================================
来源：http://hz.snrcjt.cn/gteudnwoni.html

N. 数据结构与算法
来源：http://hz.jlsjyb.cn/gtoraipjhe.html

================================================================================
来源：http://hz.jqgufenzy.top/gtujjrbpqd.html

[N01] 二分查找（有序数组）
来源：http://hz.sweek.top/gtporjnlos.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hywenlv.cn/gtewhnnkce.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.meibo888.top/gtovklnwrd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.guowangkeji.top/gtayptnxoe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ybcxt.top/gtdfzsmtkg.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.c1oappe.top/gtafpszzbj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.andypj.xyz/gtmwgwkfty.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.pycfn.com/gtfkgqvryg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gaohongyu789.top/gtdmmfajqz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.chenzaomai.com/gtsattnpxv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.vqdsnc.cn/gtyoitlvme.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xinyue.icu/gthifrcpyd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cqqwz.cn/gtkybiryre.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sufxvd.cn/gtgjmpnyyq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhiwuduotai.top/gtvuadfbgo.html

Go:   slices.Sort(arr)
来源：http://hz.cashguo.top/gtxaeytwmz.html

Ruby: arr.sort
来源：http://hz.redwolf501.top/gtpzqrpumd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.316326.xyz/gtfylvjono.html

[N03] 快速排序（分治示例）
来源：http://hz.tian-w.cn/gtlqrhzjnm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.fzhhl.top/gtnmczhjxm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.dianchejie.cn/gtcxgggkyu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.vqdsnc.cn/gtneifrizu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gogol.net.cn/gterimepgk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shuidangran.top/gtmedcxmcm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cashguo.top/gtwszsyhfd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ybcxt.top/gtdtxkhfee.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.52xcode.cn/gtpmctfdth.html

[N04] 斐波那契数列
来源：http://hz.yangfankeji.com/gtnvsuqosj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yvedp.cn/gtifxzchop.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhongyouzk.top/gtelnaqokx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zdqjudy.top/gtiqwnfjex.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.guannengcc.top/gtccnwwrkv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhiwuduotai.top/gtrlfsaaxj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sufxvd.cn/gtoywxmvjv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xziqi.cn/gtowpphmqx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hnxiangtu.top/gtvazkillv.html

[N05] 最大公约数
来源：http://hz.jinqigufen.top/gtegmcrgby.html

Py:   math.gcd(a, b)
来源：http://hz.fzhhl.top/gtqtsgogoe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.redwolf501.top/gthtxlafeg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhoulong.xyz/gtxayslmxl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yuanzhike.top/gtpjxbhejq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ppjwa.cn/gtxisennqt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cashguo.top/gtkwduqbxr.html

Ruby: a.gcd(b)
来源：http://hz.kuanghao11.cn/gtfmkhvpna.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.wangshuangyany.cn/gtrajmybkq.html

[N06] 判断回文字符串
来源：http://hz.nwbrower.top/gtxlmubbql.html

Py:   s == s[::-1]
来源：http://hz.yangfankeji.com/gtzynzfldw.html

PHP:  $s === strrev($s);
来源：http://hz.ppjwa.cn/gtfazucpsl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ivvv.top/gtjnekbkxp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtpepcxmpw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinqigfzy.top/gtoxusxsbf.html

Go:   // 双指针从两端比较
来源：http://hz.fengsongda.top/gtjunoklqf.html

Ruby: s == s.reverse
来源：http://hz.chenlongwang.top/gtoqyqumal.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.havefunace.top/gtviwjbxbv.html

[N07] 两数之和（返回下标）
来源：http://hz.yonumen.top/gtfetiwnpn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yueranfly.top/gtbvgzzjtg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ppjwa.cn/gtunutxtfz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.chenlongwang.top/gtmzmbumwe.html

TS:   // 手写 Map<string, number>
来源：http://hz.pycfn.com/gtdudtrdzq.html

Java: // 手写 HashMap
来源：http://hz.bjfxy.top/gtpnzptsua.html

Go:   // 手写 map[int]int
来源：http://hz.daria6918.cn/gtusuhdswa.html

Ruby: // 手写 Hash
来源：http://hz.redwolf501.top/gtsatkmzfv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yongpay.top/gtddmgvgzl.html

[N08] 生成全排列
来源：http://hz.kuanghao11.cn/gtfcueykse.html

Py:   itertools.permutations(arr)
来源：http://hz.cqqwz.cn/gtaqgyqkdd.html

PHP:  // 手写递归交换
来源：http://hz.fengsongda.top/gtfwnpkewk.html

JS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtwebnaxoz.html

TS:   // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtxvcvkfsh.html

Java: // 手写回溯递归
来源：http://hz.zhixingplan.top/gttlxleykv.html

Go:   // 手写回溯递归
来源：http://hz.xuanzx.com/gthmdbxvmw.html

Ruby: arr.permutation.to_a
来源：http://hz.jianghu66.top/gtvehfaupt.html

C#:   // 手写回溯递归
来源：http://hz.jyoumei.cn/gtlqdvauxt.html

[N09] 栈与队列
来源：http://hz.chenlongwang.top/gtvnwtkkaa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hongshengwenyu.top/gtcalijuti.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.0kj1m.cn/gtjwknaxcd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.dianchejie.cn/gtsrptushe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhoulong.xyz/gthqfwlbml.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.cdnleiting.top/gtxqcvftox.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.mhx1999.top/gtwdduxcba.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jinqigufen.top/gtgfsvhvld.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ppjwa.cn/gtxnrgnpcc.html

[N10] 链表节点定义
来源：http://hz.jyoumei.cn/gtmextlhit.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.fzhhl.top/gtygriywtp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sufxvd.cn/gtjnekhbmo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.feifeiyinyue.top/gtxzxyagrm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cheryme.top/gtzrafwjsm.html

Java: class Node { int v; Node next; }
来源：http://hz.zhijiandao.cn/gtxhaxgfse.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xuetiantiany.cn/gthwryuhcw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jiagoushi.top/gtpvsvkgos.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xziqi.cn/gtmmetrahw.html

[N11] 二叉树中序遍历
来源：http://hz.sysykeji.top/gtjorvxpaf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.redwolf501.top/gtmgdncgud.html

PHP:  // 手写递归函数
来源：http://hz.jinyuanbaomall.cn/gtggajmjta.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jiagoushi.top/gtmwcncrou.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hammf.cn/gtkrxjbnfa.html

Java: // 手写递归
来源：http://hz.havefunace.top/gtwchexyct.html

Go:   // 手写递归
来源：http://hz.yj20258888.top/gtbfhyslnr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.fzhhl.top/gtcrofvndz.html

C#:   // 手写递归
来源：http://hz.yanxiufei.cn/gthunbxnys.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xylfe.cn/gtdjebppzj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.mhx1999.top/gtnyaifryo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.snrcjt.cn/gtkynasnlx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hnxiangtu.top/gtlvxzxaih.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.andypj.xyz/gtpujaaoul.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yvedp.cn/gtttluoeux.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sweek.top/gtqykbrzkl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.svipenyu.cn/gthakjojrb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.316326.xyz/gtebyxmfpe.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtovuwvheb.html

O. 并发与异步
来源：http://hz.dashuyun.cn/gtkvlgszcb.html

================================================================================
来源：http://hz.svipenyu.cn/gtcemvliyg.html

[O01] 启动一个线程
来源：http://hz.9152youxi.cn/gtddxteupa.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinqigfzy.top/gtieuqgpmw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhaomingkeji.xyz/gthfgernoa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hysaishi.cn/gtlvrbxifc.html

TS:   // 同 JS
来源：http://hz.snrcjt.cn/gtstyfwkui.html

Java: new Thread(() -> f()).start()
来源：http://hz.cqqwz.cn/gtjaxyhyts.html

Go:   go f()
来源：http://hz.zycfv.cn/gtqqvurfpt.html

Ruby: Thread.new { f }
来源：http://hz.jinghuilouyu.cn/gtzyqaawsj.html

C#:   Task.Run(() => F());
来源：http://hz.hnxiangtu.top/gtwjhbqigj.html

[O02] 使用线程池
来源：http://hz.fengsongda.top/gtzcuvsfst.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhengqikj.top/gtlozbtiat.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zdqjudy.top/gtrkdgqqhl.html

JS:   // worker_threads 线程池
来源：http://hz.havefunace.top/gtlgvkdkyo.html

TS:   // worker_threads 线程池
来源：http://hz.xingfuxueyuan.xyz/gtrwnekwvl.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.c1oappe.top/gtvhblayog.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.nanxinkj.top/gtnqdatbuu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.sufxvd.cn/gtitfmzalp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cdnleiting.top/gtwdmhjqfu.html

[O03] 加锁保护共享数据
来源：http://hz.aibaodan.cn/gtopvkirzb.html

Py:   with lock: shared += 1
来源：http://hz.pengpengdd.cyou/gtzrxsvhgu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shangyingyoupin.top/gthwuhyxmp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhongyouzk.top/gtwgdxxqyh.html

TS:   // 同 JS
来源：http://hz.kuanghao11.cn/gtmwcptnjl.html

Java: synchronized (this) { shared++; }
来源：http://hz.shzxlz.cn/gtktjbabro.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ydzc1.top/gtzxbphxta.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yj202588.top/gtddxusnvi.html

C#:   lock (gate) { shared++; }
来源：http://hz.xingfuxueyuan.xyz/gtgomyuvsx.html

[O04] 定义异步函数并等待
来源：http://hz.tianlin.xyz/gtmhjqyixc.html

Py:   async def f():⏎    await g()
来源：http://hz.jiagoushi.top/gtvdtcgcma.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cashguo.top/gtphkjiqae.html

JS:   async function f() { await g(); }
来源：http://hz.zhaomingkeji.xyz/gtfjujcjfb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yueranfly.top/gtaeltkyqg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.havefunace.top/gtzyfnejvj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hnxiangtu.top/gtkukkazbv.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.tanke756.top/gtfgxjzlme.html

C#:   async Task F() { await G(); }
来源：http://hz.shanyushiyangtech.top/gtycvkjriv.html

[O05] 并发执行并等待全部完成
来源：http://hz.meibo888.top/gtamefnsyv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xinyue.icu/gtijxaudav.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jianghu66.top/gtdilralgs.html

JS:   await Promise.all(tasks)
来源：http://hz.chenzaomai.com/gtkdilvzap.html

TS:   await Promise.all(tasks)
来源：http://hz.xuetiantiany.cn/gtfczigqvn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinqigfzy.top/gtedbjyarh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xylfe.cn/gttdpqlqvs.html

Ruby: threads.map(&:join)
来源：http://hz.pycfn.com/gtegzuhggl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.kuanghao11.cn/gtvsudcxka.html

[O06] 使用进程池
来源：http://hz.ybcxt.top/gtfwighxdk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xinyue.icu/gtjrwtbmbl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhixingplan.top/gtnhyuvrwp.html

JS:   // child_process / cluster 模块
来源：http://hz.cqqwz.cn/gtcgrtlbug.html

TS:   // child_process / cluster 模块
来源：http://hz.sxryk.cn/gtyhigxree.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.feifeiyinyue.top/gtuesqopgf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shangyingyoupin.top/gtetopquou.html

Ruby: // fork 块
来源：http://hz.jinqigufen.top/gtghpvdgxw.html

C#:   Parallel.For
来源：http://hz.shanyushiyangkeji.top/gtxbzzobbg.html

================================================================================
来源：http://hz.jyoumei.cn/gtvxnkbosd.html

P. 常用工具函数
来源：http://hz.xuetiantiany.cn/gthzxtehti.html

================================================================================
来源：http://hz.tanke756.top/gtsyhsjiro.html

[P01] 生成 UUID
来源：http://hz.xziqi.cn/gttkwhsszu.html

Py:   str(uuid.uuid4())
来源：http://hz.aizwys.cn/gtcnteztto.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.guannengcc.top/gtbjyuocjh.html

JS:   crypto.randomUUID()
来源：http://hz.ehwqpu.com/gtisryfqty.html

TS:   crypto.randomUUID()
来源：http://hz.316326.xyz/gtmvlxlfws.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhoulong.xyz/gtzecqilgf.html

Go:   // 用 github.com/google/uuid
来源：http://hz.nwbrower.top/gtdmnpvndb.html

Ruby: SecureRandom.uuid
来源：http://hz.gogol.net.cn/gtszjbkiie.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenlongwang.top/gtjxzlhrmh.html

[P02] MD5 / SHA256 摘要
来源：http://hz.gaohongyu789.top/gtrjocclpo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shzxlz.cn/gtifujcshc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hnqzz.top/gtoeqytzpl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.aibaodan.cn/gtlftfxkie.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.nanxuanxn.top/gtsuldauwg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj20258.top/gtepoworcv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.daria6918.cn/gtthhqsyni.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.guowangkeji.top/gtzwyaazqk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yj20258.top/gtgrzulgwd.html

[P03] 生成短随机字符串
来源：http://hz.shuidangran.top/gtetgqxmwm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.nwbrower.top/gtdbkvmxai.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ywan-chungtsiang.top/gtsmtmowcn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgufenzy.top/gthfbllnqp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shzxlz.cn/gtmzzdhspl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shuidangran.top/gtmoeepwcj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.gotoacloud.top/gthbqbnjhs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shanyushiyangkeji.top/gtydkmzilo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.birdmap.top/gtgvuyvttf.html

[P04] 求长度
来源：http://hz.nanxuanxn.top/gtqijznulz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.guannengcc.top/gtmvkgnqlf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.havefunace.top/gteigoowsy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangshuangyany.cn/gtmakyvcdy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.aizwys.cn/gtkyhnsnym.html

Java: list.size();  map.size();  s.length()
来源：http://hz.9152youxi.cn/gttbseudpg.html

Go:   len(arr);  len(m)
来源：http://hz.chenlongwang.top/gtdvuisvti.html

Ruby: x.length;  x.size
来源：http://hz.ppjwa.cn/gteixapezc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.sysykeji.top/gtjedihsfb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.tianlin.xyz/gtmorszglg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ppjwa.cn/gtjeaxzxli.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jlsjyb.cn/gtefauvurf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.wangdashe.top/gtugvynrkl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.bjfxy.top/gtowxmvssj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hysaishi.cn/gtebdnxlhk.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jqgfzy.top/gtldyedjjg.html

Ruby: a == b
来源：http://hz.ppjwa.cn/gtxznuyutc.html


<!-- 参考信息 -->