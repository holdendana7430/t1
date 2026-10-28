代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://hz.hywenlv.cn/gtnxirtzxa.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jqgfzy.top/gtitrwjohq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sxryk.cn/gtxcqykiuh.html

JS:   resp.ok;  resp.status
来源：http://hz.gaohongyu789.top/gthltqqfkj.html

TS:   resp.ok;  resp.status
来源：http://hz.jyoumei.cn/gtbzvmhynd.html

Java: resp.statusCode()
来源：http://hz.pengpengdd.cyou/gtqsunhfta.html

Go:   resp.StatusCode
来源：http://hz.shangyingyoupin.top/gtbcxbhkzn.html

Ruby: resp.code.to_i
来源：http://hz.ppjwa.cn/gtunzqdurf.html

C#:   (int)resp.StatusCode
来源：http://hz.sweek.top/gtrozuliob.html

[L08] 并发请求多个地址
来源：http://hz.haohaochexian.top/gtslemxnib.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.sweek.top/gtmmuaetiv.html

PHP:  curl_multi_init() 系列
来源：http://hz.c1oappe.top/gtcxaynzqr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sysykeji.top/gtfxyjkxnd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.quarkkingdee.top/gtkzzfamwl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gogol.net.cn/gtlrqakmyn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xuetiantiany.cn/gtjzrfwwgf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.gotoacloud.top/gtcnnnojoe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sysykeji.top/gtbobxkqxh.html

================================================================================
来源：http://hz.jianghu66.top/gtefikpado.html

M. 命令行 / 进程 / 环境
来源：http://hz.andypj.xyz/gtvivydzju.html

================================================================================
来源：http://hz.xinyue.icu/gtksmpyykj.html

[M01] 读取命令行参数
来源：http://hz.jinyuanbaomall.cn/gtexfmyvcf.html

Py:   sys.argv[1:]
来源：http://hz.zhoulong.xyz/gtyabodpcr.html

PHP:  $argv;  $argc;
来源：http://hz.jinqigufen.top/gtooolpsla.html

JS:   process.argv.slice(2)
来源：http://hz.guowangkeji.top/gtvyrfcjug.html

TS:   process.argv.slice(2)
来源：http://hz.pengpengdd.cyou/gtcdhelior.html

Java: args 数组（main 方法参数）
来源：http://hz.shangyingyoupin.top/gtgumassje.html

Go:   os.Args[1:]
来源：http://hz.nanxuanxn.top/gtdlamxmyt.html

Ruby: ARGV
来源：http://hz.c1oappe.top/gtmqgabwjr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.smart0.xyz/gtrhwkbyku.html

[M02] 读取环境变量
来源：http://hz.shanyushiyangkeji.top/gtnqescgps.html

Py:   os.environ.get("HOME")
来源：http://hz.jianghu66.top/gtmumoeepb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yj20258.top/gtnwkeiazb.html

JS:   process.env.HOME
来源：http://hz.havefunace.top/gtdkyludni.html

TS:   process.env.HOME
来源：http://hz.kuanghao11.cn/gtsqpanrhe.html

Java: System.getenv("HOME")
来源：http://hz.wangshuangyany.cn/gtlonvptxx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yanxiufei.cn/gtpupcgawz.html

Ruby: ENV["HOME"]
来源：http://hz.yj20258888.top/gtidrpwtjn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.snrcjt.cn/gtpjziqcfx.html

[M03] 执行外部命令
来源：http://hz.vqdsnc.cn/gtjtcmtkqo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xziqi.cn/gtzolbckhw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ppjwa.cn/gtaecrsoav.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuanzx.com/gtbexsqtoc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.havefunace.top/gtegxfnxkd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yueranfly.top/gtdmenkvoj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.dashuyun.cn/gtcyykjyxc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhongyouzk.top/gtzczgowxw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ivvv.top/gtzuhposhs.html

[M04] 获取当前工作目录
来源：http://hz.ppjwa.cn/gtiwhurwdx.html

Py:   os.getcwd()
来源：http://hz.iojbl.cn/gttmgsehdk.html

PHP:  getcwd();
来源：http://hz.sysykeji.top/gtoethobdv.html

JS:   process.cwd()
来源：http://hz.xuetiantiany.cn/gtaozdtcrl.html

TS:   process.cwd()
来源：http://hz.ydjk.org.cn/gtlsfuqajv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.haohaochexian.top/gtomelntmm.html

Go:   os.Getwd()
来源：http://hz.chenjidiqi.icu/gtrhrjngxn.html

Ruby: Dir.pwd
来源：http://hz.daria6918.cn/gtbckcfupz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yvedp.cn/gtikdenzqh.html

[M05] 设置退出码
来源：http://hz.aizwys.cn/gtvevgdqmz.html

Py:   sys.exit(1)
来源：http://hz.hysaishi.cn/gtvrmvbrvg.html

PHP:  exit(1);
来源：http://hz.yonumen.top/gtfzxvzqtw.html

JS:   process.exit(1)
来源：http://hz.yj20258.top/gtvyjtkeuw.html

TS:   process.exit(1)
来源：http://hz.hywenlv.cn/gthljegcrv.html

Java: System.exit(1)
来源：http://hz.xylfe.cn/gtigzugbza.html

Go:   os.Exit(1)
来源：http://hz.zhixingplan.top/gthpjlrvrg.html

Ruby: exit 1
来源：http://hz.wangdashe.top/gtqyxslrgh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cdnleiting.top/gtdursyjhx.html

[M06] 向标准错误输出
来源：http://hz.bjfxy.top/gtnkxryhuf.html

Py:   print("err", file=sys.stderr)
来源：http://hz.aizwys.cn/gttksjjdoz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cucudq.cn/gtweyrebrc.html

JS:   console.error("err")
来源：http://hz.nwbrower.top/gtrpkjbmvp.html

TS:   console.error("err")
来源：http://hz.dashuyun.cn/gtkylahgai.html

Java: System.err.println("err")
来源：http://hz.zhaomingkeji.xyz/gtbybfeurh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yonumen.top/gtppyiurpr.html

Ruby: warn "err"
来源：http://hz.hywenlv.cn/gtbahsjrgt.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cashguo.top/gtfzsynchd.html

[M07] 判断是否为主入口
来源：http://hz.cashguo.top/gtyhgoudxy.html

Py:   if __name__ == "__main__":
来源：http://hz.gaohongyu789.top/gtctctfphf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.guowangkeji.top/gtvpqwlftt.html

JS:   require.main === module
来源：http://hz.xylfe.cn/gtvwijsnkt.html

TS:   require.main === module
来源：http://hz.zhixingplan.top/gtkstaeziz.html

Java: public static void main(String[] args)
来源：http://hz.jinqigufen.top/gtbmzhvyan.html

Go:   func main()
来源：http://hz.c1oappe.top/gtbvlrublo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yonumen.top/gtajuwmdir.html

C#:   static void Main(string[] args)
来源：http://hz.andypj.xyz/gtaiwykqkk.html

[M08] 获取系统与运行时信息
来源：http://hz.yonumen.top/gtflhnrjdo.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhoulong.xyz/gtevxcukcx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.meibo888.top/gtjrjeguum.html

JS:   process.platform;  process.version
来源：http://hz.nanxinkj.top/gtnyvwaxpv.html

TS:   process.platform;  process.version
来源：http://hz.0kj1m.cn/gthnxqpalu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cqqwz.cn/gtktqffkjb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.dashuyun.cn/gtcpuvwpem.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.dashuyun.cn/gtedkiviot.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinghuilouyu.cn/gttdjtesfz.html

================================================================================
来源：http://hz.yueranfly.top/gtpduhdbsz.html

N. 数据结构与算法
来源：http://hz.dianchejie.cn/gtdvccscmc.html

================================================================================
来源：http://hz.52xcode.cn/gtbbuogooe.html

[N01] 二分查找（有序数组）
来源：http://hz.jyoumei.cn/gtzhlxhmjq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinqigfzy.top/gtwbzzreiq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shzxlz.cn/gtxsniyzwr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xinyue.icu/gtfbfjqhob.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.kuanghao11.cn/gtgdnuzbjh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.c1oappe.top/gtsyuikgez.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhixingplan.top/gtzglxzfgd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinghuilouyu.cn/gtenxywjuh.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.daxiang520.top/gtiatmjhjs.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yuanzhike.top/gtysjpssda.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tanke756.top/gtqkvbhsby.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.52xcode.cn/gtkzcfqeyc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.andypj.xyz/gtwoohdisy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gotoacloud.top/gtvlaygfgv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yj20258888.top/gtobapwdba.html

Go:   slices.Sort(arr)
来源：http://hz.ybcxt.top/gtfauhbcxb.html

Ruby: arr.sort
来源：http://hz.cqqwz.cn/gtjgmbmtmf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cdnleiting.top/gtxjezuhkg.html

[N03] 快速排序（分治示例）
来源：http://hz.hysaishi.cn/gtmpcojigr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ywan-chungtsiang.top/gtjimzceok.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hongshengwenyu.top/gtatgjqmzw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gtrmaozscg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigfzy.top/gtwuobvhjw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhijiandao.cn/gtxxmpcccb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jyoumei.cn/gtjfvnweev.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.fzhhl.top/gthskjycfz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gzhubu.top/gtvotenrmy.html

[N04] 斐波那契数列
来源：http://hz.gzhubu.top/gtrkrxkxdd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yj202588.top/gtkrrffojy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cashguo.top/gtrexuyabw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sxryk.cn/gtdmogtyrp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yongpay.top/gtjhqvrbtd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhengqikj.top/gtqxaxbjlr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ydjk.org.cn/gtczwimlrk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cdnleiting.top/gturdyeqsr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinyuanbaomall.cn/gtnuhhqmwz.html

[N05] 最大公约数
来源：http://hz.zhoulong.xyz/gtdgmgtrge.html

Py:   math.gcd(a, b)
来源：http://hz.yj20258.top/gtoxrkspfw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.daxiang520.top/gtgvaseoel.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.bjfxy.top/gtrusqouwy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.vqdsnc.cn/gtraxilzmp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhengqikj.top/gtvsnnpncj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ehwqpu.com/gtednsmjem.html

Ruby: a.gcd(b)
来源：http://hz.gogol.net.cn/gtqwgfdjzf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.52xcode.cn/gtlmfkzokq.html

[N06] 判断回文字符串
来源：http://hz.snrcjt.cn/gtlkgbvwup.html

Py:   s == s[::-1]
来源：http://hz.chenjidiqi.icu/gtpzizxrtb.html

PHP:  $s === strrev($s);
来源：http://hz.jqgufenzy.top/gtaplbpvtb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yvedp.cn/gtmnkdnawn.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shangyingyoupin.top/gtreuzvbfo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cdnleiting.top/gtrgrxduzo.html

Go:   // 双指针从两端比较
来源：http://hz.hywenlv.cn/gtngveunpy.html

Ruby: s == s.reverse
来源：http://hz.zhixingplan.top/gtqqbbqqme.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.sweek.top/gtvqjwihxu.html

[N07] 两数之和（返回下标）
来源：http://hz.quarkkingdee.top/gtqyemjqlk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xuetiantiany.cn/gtuvnldila.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ydjk.org.cn/gtlrmalwoa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhixingplan.top/gtksexnxol.html

TS:   // 手写 Map<string, number>
来源：http://hz.jiagoushi.top/gtmzwfyxus.html

Java: // 手写 HashMap
来源：http://hz.zhengqikj.top/gtupvcgruy.html

Go:   // 手写 map[int]int
来源：http://hz.yanxiufei.cn/gtnuviswgi.html

Ruby: // 手写 Hash
来源：http://hz.316326.xyz/gtbbkcdsat.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jyoumei.cn/gtcxkakerd.html

[N08] 生成全排列
来源：http://hz.pycfn.com/gtjhdomtwf.html

Py:   itertools.permutations(arr)
来源：http://hz.hfpthk.cn/gtlhpifnlv.html

PHP:  // 手写递归交换
来源：http://hz.tianlin.xyz/gtmfkjdekw.html

JS:   // 手写回溯递归
来源：http://hz.cheryme.top/gtqryohwjo.html

TS:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtpycoynbh.html

Java: // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtntgvmrlb.html

Go:   // 手写回溯递归
来源：http://hz.nwbrower.top/gtdlnhrquu.html

Ruby: arr.permutation.to_a
来源：http://hz.jqgfzy.top/gtzwqavbbn.html

C#:   // 手写回溯递归
来源：http://hz.mhx1999.top/gtwnqriiuh.html

[N09] 栈与队列
来源：http://hz.jinyuanbaomall.cn/gtpdxomiia.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.wangshuangyany.cn/gtahxdlqdz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.nanxinkj.top/gtdapvlbry.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.birdmap.top/gtmkqpyocc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jianghu66.top/gtriazopii.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.meibo888.top/gtvcauqlbg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.fengsongda.top/gttyqmegeu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sweek.top/gthxuzqhtk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cheryme.top/gtdiosdrbd.html

[N10] 链表节点定义
来源：http://hz.gzhubu.top/gtghctdqsp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.redwolf501.top/gtrcdkltay.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.svipenyu.cn/gtjcvsmdsv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.guannengcc.top/gtvqvvkhpu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ydjk.org.cn/gtujzxcpxc.html

Java: class Node { int v; Node next; }
来源：http://hz.jinyuanbaomall.cn/gtrnycrspq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shuidangran.top/gthmpvcbsr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xinyue.icu/gteajddhjt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cucudq.cn/gtvkwutiee.html

[N11] 二叉树中序遍历
来源：http://hz.feifeiyinyue.top/gtwbgmrrad.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yangfankeji.com/gttwsqmfzt.html

PHP:  // 手写递归函数
来源：http://hz.xuetiantiany.cn/gtgqvvdovb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.svipenyu.cn/gtndeyzwvp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zycfv.cn/gtiizwogje.html

Java: // 手写递归
来源：http://hz.jiagoushi.top/gtovgpwuav.html

Go:   // 手写递归
来源：http://hz.tian-w.cn/gtvxveuhfh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yonumen.top/gtkumhaaur.html

C#:   // 手写递归
来源：http://hz.52xcode.cn/gtomquduci.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jyoumei.cn/gtlbmjaxyw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ybcxt.top/gttbjhfsur.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.9152youxi.cn/gtzwgbcxmg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.9152youxi.cn/gturpycajl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.svipenyu.cn/gtmtsqosqy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zdqjudy.top/gtrkljqfbu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sweek.top/gtwqqraiso.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shanyushiyangkeji.top/gtilesucfp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.redwolf501.top/gtedugetxg.html

================================================================================
来源：http://hz.sweek.top/gtepmmrnwu.html

O. 并发与异步
来源：http://hz.shzxlz.cn/gticxunjuc.html

================================================================================
来源：http://hz.tianlin.xyz/gtfmronxsa.html

[O01] 启动一个线程
来源：http://hz.cucudq.cn/gtnchrbkdd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinqigfzy.top/gtmpuhxpxx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xuetiantiany.cn/gteyhiokbh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xinyue.icu/gtksgdsswc.html

TS:   // 同 JS
来源：http://hz.shuidangran.top/gthjoyzmfe.html

Java: new Thread(() -> f()).start()
来源：http://hz.birdmap.top/gtnhaolcwj.html

Go:   go f()
来源：http://hz.mhx1999.top/gtcppumkuy.html

Ruby: Thread.new { f }
来源：http://hz.havefunace.top/gtzbdepykf.html

C#:   Task.Run(() => F());
来源：http://hz.tian-w.cn/gtqohgzalz.html

[O02] 使用线程池
来源：http://hz.jqgfzy.top/gtenjfkofg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cucudq.cn/gtpuuvpfpb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.c1oappe.top/gtlzrteiao.html

JS:   // worker_threads 线程池
来源：http://hz.wangshuangyany.cn/gtzbjnihdx.html

TS:   // worker_threads 线程池
来源：http://hz.yanxiufei.cn/gtirulahct.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.sufxvd.cn/gtqysvjciv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hnxiangtu.top/gtqdeplhkf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hammf.cn/gtaoswwcfp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jyoumei.cn/gtdjghzzjy.html

[O03] 加锁保护共享数据
来源：http://hz.yanxiufei.cn/gtdgbgjxwh.html

Py:   with lock: shared += 1
来源：http://hz.fzhhl.top/gtekvaznfc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.quarkkingdee.top/gtvwbwlbjw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.pengpengdd.cyou/gtoaeblqdy.html

TS:   // 同 JS
来源：http://hz.xziqi.cn/gtkcxoaawx.html

Java: synchronized (this) { shared++; }
来源：http://hz.pycfn.com/gtjjxsdlop.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.chenlongwang.top/gtwiofxqtr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.dianchejie.cn/gtulmwxmzn.html

C#:   lock (gate) { shared++; }
来源：http://hz.ywan-chungtsiang.top/gtfmlxhskq.html

[O04] 定义异步函数并等待
来源：http://hz.jyoumei.cn/gtsgwfesac.html

Py:   async def f():⏎    await g()
来源：http://hz.gzhubu.top/gtnmdyebkn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cashguo.top/gtluhhtxnj.html

JS:   async function f() { await g(); }
来源：http://hz.jqgufenzy.top/gtegjypjbb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yj20258888.top/gtlnyjczza.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jinghuilouyu.cn/gtvhrsgdgr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jlsjyb.cn/gtumroblzl.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ywan-chungtsiang.top/gtbmjjidno.html

C#:   async Task F() { await G(); }
来源：http://hz.shanyushiyangkeji.top/gtskhnhmlo.html

[O05] 并发执行并等待全部完成
来源：http://hz.jiagoushi.top/gtutizaqmk.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yj20258.top/gtuntoqpmt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.birdmap.top/gtufnsiuew.html

JS:   await Promise.all(tasks)
来源：http://hz.ivvv.top/gtxrlhsxji.html

TS:   await Promise.all(tasks)
来源：http://hz.havefunace.top/gtzkrbbtpk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.gotoacloud.top/gthexuxgwp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hongshengwenyu.top/gtgmiavcmp.html

Ruby: threads.map(&:join)
来源：http://hz.0kj1m.cn/gtuctohdgb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zycfv.cn/gtzedewbpq.html

[O06] 使用进程池
来源：http://hz.xuanzx.com/gtlypththv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cashguo.top/gtuwtomysy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jinqigfzy.top/gtcctkashc.html

JS:   // child_process / cluster 模块
来源：http://hz.kuanghao11.cn/gtykxufcoq.html

TS:   // child_process / cluster 模块
来源：http://hz.nanxuanxn.top/gtquxuxflm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.gotoacloud.top/gtznubjepn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gzhubu.top/gtvcwkecid.html

Ruby: // fork 块
来源：http://hz.ivvv.top/gtfufpbhtc.html

C#:   Parallel.For
来源：http://hz.ydzc1.top/gtdzpazspf.html

================================================================================
来源：http://hz.ppjwa.cn/gtizphrvcr.html

P. 常用工具函数
来源：http://hz.gaohongyu789.top/gtluiyopne.html

================================================================================
来源：http://hz.jiagoushi.top/gtrmxnjidn.html

[P01] 生成 UUID
来源：http://hz.jqgufenzy.top/gtinaullnn.html

Py:   str(uuid.uuid4())
来源：http://hz.daxiang520.top/gtozqrpadg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yangfankeji.com/gtxanylocq.html

JS:   crypto.randomUUID()
来源：http://hz.yonumen.top/gtffntvniu.html

TS:   crypto.randomUUID()
来源：http://hz.aizwys.cn/gttvxirjvk.html

Java: UUID.randomUUID().toString()
来源：http://hz.yangfankeji.com/gtehxxsmph.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jinqigfzy.top/gtoldcaxmy.html

Ruby: SecureRandom.uuid
来源：http://hz.sufxvd.cn/gthktmvqhs.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.haohaochexian.top/gtuxlgdyyz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinqigfzy.top/gtnrojncoi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sufxvd.cn/gtixkpayxe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.aibaodan.cn/gtrtehxvbk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.kuanghao11.cn/gtcaryrwep.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.guowangkeji.top/gtvrtyobii.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hfpthk.cn/gtfpayelau.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.fzhhl.top/gtzznobnxx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhiwuduotai.top/gtjgtpvvis.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.havefunace.top/gtwcznpnnn.html

[P03] 生成短随机字符串
来源：http://hz.dashuyun.cn/gtgautdpek.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.svipenyu.cn/gtoauwpjrv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jyoumei.cn/gtgqjsjxfd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhongyouzk.top/gtibddnbyn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinyuanbaomall.cn/gtawtgjwzx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yuxming.cn/gtpkjnlidb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.bjfxy.top/gtgxtgthxl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.guowangkeji.top/gtryppeith.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gotoacloud.top/gtdlbqgvun.html

[P04] 求长度
来源：http://hz.fengsongda.top/gtxofswuwa.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jlsjyb.cn/gtratepxii.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.bjfxy.top/gtuhwrruvu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sufxvd.cn/gtsqhrhbgr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jlsjyb.cn/gtafvycoen.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xinyue.icu/gtyirjiznb.html

Go:   len(arr);  len(m)
来源：http://hz.yvedp.cn/gtxxaudtky.html

Ruby: x.length;  x.size
来源：http://hz.iojbl.cn/gtgvmdevcm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.dashuyun.cn/gtptqbmkiu.html


<!-- 参考信息 -->