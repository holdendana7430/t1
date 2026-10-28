代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hnqzz.top/gtfdhnfrvi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.0kj1m.cn/gtvupfucqb.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shzxlz.cn/gtskmhjjmq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shzxlz.cn/gtwkwvczuh.html

[L07] 处理 HTTP 状态码
来源：http://hz.hammf.cn/gtxbtufzmj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.meibo888.top/gtzkxvflme.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.smart0.xyz/gttgssyren.html

JS:   resp.ok;  resp.status
来源：http://hz.vqdsnc.cn/gtspqpcqlb.html

TS:   resp.ok;  resp.status
来源：http://hz.quarkkingdee.top/gtmzbuvtkr.html

Java: resp.statusCode()
来源：http://hz.sweek.top/gtxtffxpgb.html

Go:   resp.StatusCode
来源：http://hz.jinghuilouyu.cn/gtdxnjrjid.html

Ruby: resp.code.to_i
来源：http://hz.feifeiyinyue.top/gthsnoxsjn.html

C#:   (int)resp.StatusCode
来源：http://hz.shzxlz.cn/gtwhpxwfto.html

[L08] 并发请求多个地址
来源：http://hz.jqgfzy.top/gtrxgnupas.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xingfuxueyuan.xyz/gtnjrdngxr.html

PHP:  curl_multi_init() 系列
来源：http://hz.xuetiantiany.cn/gtfkdfkref.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydzc1.top/gtuzvfteio.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tian-w.cn/gtleiildhe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinghuilouyu.cn/gtrjjaqatg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hywenlv.cn/gtjekcrvir.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.vqdsnc.cn/gtzlboikdc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cqqwz.cn/gtknbpwivj.html

================================================================================
来源：http://hz.yanxiufei.cn/gtqrfillgs.html

M. 命令行 / 进程 / 环境
来源：http://hz.aizwys.cn/gtifyabceb.html

================================================================================
来源：http://hz.guowangkeji.top/gttljrvtag.html

[M01] 读取命令行参数
来源：http://hz.jyoumei.cn/gtgcxundlc.html

Py:   sys.argv[1:]
来源：http://hz.cheryme.top/gtoelwcqsl.html

PHP:  $argv;  $argc;
来源：http://hz.yj20258888.top/gtylvhykrw.html

JS:   process.argv.slice(2)
来源：http://hz.yj20258.top/gtxmtbjnre.html

TS:   process.argv.slice(2)
来源：http://hz.iojbl.cn/gtrdgphphd.html

Java: args 数组（main 方法参数）
来源：http://hz.cqqwz.cn/gtfxbfrizu.html

Go:   os.Args[1:]
来源：http://hz.yj202588.top/gtyhllyxad.html

Ruby: ARGV
来源：http://hz.fzhhl.top/gtsmsbumvk.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shzxlz.cn/gtrsrxzgyu.html

[M02] 读取环境变量
来源：http://hz.ywan-chungtsiang.top/gtudaxlzhe.html

Py:   os.environ.get("HOME")
来源：http://hz.jyoumei.cn/gtviwxscjq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.pengpengdd.cyou/gttugqmwwk.html

JS:   process.env.HOME
来源：http://hz.xuanzx.com/gtcpckzveb.html

TS:   process.env.HOME
来源：http://hz.316326.xyz/gtxqedyfvf.html

Java: System.getenv("HOME")
来源：http://hz.svipenyu.cn/gthyletkpq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jianghu66.top/gteafepscw.html

Ruby: ENV["HOME"]
来源：http://hz.cheryme.top/gtpeskjdbs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gotoacloud.top/gtkjrkuqea.html

[M03] 执行外部命令
来源：http://hz.havefunace.top/gtceepxvbd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xuetiantiany.cn/gtlfthkgcx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.fengsongda.top/gtnfolyjuz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.316326.xyz/gtqtbjipew.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.fzhhl.top/gtcfnzexgf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ywan-chungtsiang.top/gtmbgxyxna.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.wangshuangyany.cn/gtqhueapua.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cqqwz.cn/gteikoafmo.html

C#:   Process.Start("ls", "-l");
来源：http://hz.redwolf501.top/gtcmfnhryd.html

[M04] 获取当前工作目录
来源：http://hz.snrcjt.cn/gtodyhjrjd.html

Py:   os.getcwd()
来源：http://hz.cashguo.top/gtassprpvf.html

PHP:  getcwd();
来源：http://hz.ybcxt.top/gtlthnitdm.html

JS:   process.cwd()
来源：http://hz.chenzaomai.com/gtttczlaba.html

TS:   process.cwd()
来源：http://hz.xinyue.icu/gtovxjyvdo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yangfankeji.com/gtvcvabzms.html

Go:   os.Getwd()
来源：http://hz.zycfv.cn/gtrrqfqfnb.html

Ruby: Dir.pwd
来源：http://hz.yuxming.cn/gtextlvaht.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.52xcode.cn/gthtsrgllo.html

[M05] 设置退出码
来源：http://hz.yuxming.cn/gtovmyhmpw.html

Py:   sys.exit(1)
来源：http://hz.tanke756.top/gtuuhysmmi.html

PHP:  exit(1);
来源：http://hz.sweek.top/gtwgigbiuf.html

JS:   process.exit(1)
来源：http://hz.yueranfly.top/gtfgqzymzp.html

TS:   process.exit(1)
来源：http://hz.sysykeji.top/gtycpclgag.html

Java: System.exit(1)
来源：http://hz.ehwqpu.com/gtylkdmbxk.html

Go:   os.Exit(1)
来源：http://hz.cheryme.top/gtvwjdbhpi.html

Ruby: exit 1
来源：http://hz.cdnleiting.top/gtdlvdejnn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.9152youxi.cn/gtbtokjgvk.html

[M06] 向标准错误输出
来源：http://hz.bjfxy.top/gtlzvtyxrl.html

Py:   print("err", file=sys.stderr)
来源：http://hz.tian-w.cn/gtnaqmfuam.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ydjk.org.cn/gtxgooabmg.html

JS:   console.error("err")
来源：http://hz.gogol.net.cn/gtyvwlbjgr.html

TS:   console.error("err")
来源：http://hz.sufxvd.cn/gtnggrnhes.html

Java: System.err.println("err")
来源：http://hz.wangshuangyany.cn/gtaglwbkrp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhengqikj.top/gtrlplaysk.html

Ruby: warn "err"
来源：http://hz.jiagoushi.top/gtuiijbydh.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.andypj.xyz/gthfyzoxuo.html

[M07] 判断是否为主入口
来源：http://hz.xuetiantiany.cn/gtmbkonzpa.html

Py:   if __name__ == "__main__":
来源：http://hz.mhx1999.top/gtpfcqxkkv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ivvv.top/gtgkdusszx.html

JS:   require.main === module
来源：http://hz.chenjidiqi.icu/gttxvphyom.html

TS:   require.main === module
来源：http://hz.sxryk.cn/gtvewxrbaa.html

Java: public static void main(String[] args)
来源：http://hz.yuxming.cn/gtnshfmzwb.html

Go:   func main()
来源：http://hz.xuetiantiany.cn/gthuetykda.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xylfe.cn/gtbbnurvhj.html

C#:   static void Main(string[] args)
来源：http://hz.zhengqikj.top/gtjslnsdel.html

[M08] 获取系统与运行时信息
来源：http://hz.zhaomingkeji.xyz/gtwizmwrfl.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ydjk.org.cn/gtrdhpzjdu.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shangyingyoupin.top/gtghrfusbk.html

JS:   process.platform;  process.version
来源：http://hz.nanxuanxn.top/gtpzhswgdq.html

TS:   process.platform;  process.version
来源：http://hz.hnqzz.top/gtkgmlproe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gotoacloud.top/gtrabhsiof.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sxryk.cn/gttecyolgq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ywan-chungtsiang.top/gtxazyaozq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jianghu66.top/gtduduknju.html

================================================================================
来源：http://hz.hfpthk.cn/gtuenzdhgk.html

N. 数据结构与算法
来源：http://hz.shangyingyoupin.top/gtxuzlmxyg.html

================================================================================
来源：http://hz.yuxming.cn/gturciqzld.html

[N01] 二分查找（有序数组）
来源：http://hz.shuidangran.top/gtxiizymdg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xuanzx.com/gtdpdfqgdm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.snrcjt.cn/gttqbehhhp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangshuangyany.cn/gtbpssajid.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cashguo.top/gtbbsxshvj.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.9152youxi.cn/gtbjeddvry.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtvqfazhvo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.daxiang520.top/gthjzmrhvm.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.havefunace.top/gtgnllzpup.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.havefunace.top/gtikqgjscu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yuanzhike.top/gtaxsrnziz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj20258.top/gthajfhedw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinqigfzy.top/gtdjugduiu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinqigfzy.top/gtrvesukfc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.snrcjt.cn/gtgrjflbgl.html

Go:   slices.Sort(arr)
来源：http://hz.yonumen.top/gtctgyctou.html

Ruby: arr.sort
来源：http://hz.yvedp.cn/gteidxvtfd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shangyingyoupin.top/gtckhcaqbk.html

[N03] 快速排序（分治示例）
来源：http://hz.fzhhl.top/gtaqzbhxvx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.nanxinkj.top/gtfvhaebqk.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sxryk.cn/gttqepjkuv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cucudq.cn/gtxbnqafaa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dianchejie.cn/gtvryffuzh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yuanzhike.top/gtlvmkfbng.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jlsjyb.cn/gtpzsbwfff.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.haohaochexian.top/gtdnyrtpze.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yuanzhike.top/gtftcsajzh.html

[N04] 斐波那契数列
来源：http://hz.0kj1m.cn/gtcbtvygcu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xylfe.cn/gtplsvvlqc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.quarkkingdee.top/gtdnvkhokf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shuidangran.top/gtjndkzzhf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnqzz.top/gtobtcilhk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gaohongyu789.top/gtktuyylqn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hnxiangtu.top/gtozaznrdf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yuanzhike.top/gtegjiggja.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.tianlin.xyz/gtfbjewypy.html

[N05] 最大公约数
来源：http://hz.gotoacloud.top/gtdhutmtvd.html

Py:   math.gcd(a, b)
来源：http://hz.hfpthk.cn/gtnmclvwmz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.mhx1999.top/gtaryrghfq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.snrcjt.cn/gtfdjtvzbq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zdqjudy.top/gtflhfdvnk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hongshengwenyu.top/gtewuutwop.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.feifeiyinyue.top/gtgrqvxmqz.html

Ruby: a.gcd(b)
来源：http://hz.jinqigfzy.top/gtzrhgoytu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhijiandao.cn/gtytlnbgrb.html

[N06] 判断回文字符串
来源：http://hz.zhiwuduotai.top/gtbbqafhjn.html

Py:   s == s[::-1]
来源：http://hz.jinghuilouyu.cn/gtniaaavea.html

PHP:  $s === strrev($s);
来源：http://hz.jyoumei.cn/gtbapxbiyw.html

JS:   s === [...s].reverse().join("")
来源：http://hz.aizwys.cn/gtpynzkusj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtybmxpdyq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jianghu66.top/gtailgksny.html

Go:   // 双指针从两端比较
来源：http://hz.sufxvd.cn/gtedizimrg.html

Ruby: s == s.reverse
来源：http://hz.dianchejie.cn/gtiylojcjs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yvedp.cn/gttuhvxykk.html

[N07] 两数之和（返回下标）
来源：http://hz.zycfv.cn/gtcnpqyxqi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.fzhhl.top/gthxfjowag.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jqgfzy.top/gtxpkyctja.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.tianlin.xyz/gtimqlnirt.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhijiandao.cn/gtpzefbjgl.html

Java: // 手写 HashMap
来源：http://hz.316326.xyz/gtqoorbvhr.html

Go:   // 手写 map[int]int
来源：http://hz.jqgfzy.top/gtricdtdnc.html

Ruby: // 手写 Hash
来源：http://hz.yvedp.cn/gtilbsoqll.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.chenjidiqi.icu/gtmptxkavv.html

[N08] 生成全排列
来源：http://hz.chenzaomai.com/gtwjtlbiwi.html

Py:   itertools.permutations(arr)
来源：http://hz.bjfxy.top/gtepduiewx.html

PHP:  // 手写递归交换
来源：http://hz.zhoulong.xyz/gtnjeazhnh.html

JS:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gttdgcgryl.html

TS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtfhtqyecm.html

Java: // 手写回溯递归
来源：http://hz.shuidangran.top/gtrjlovgwt.html

Go:   // 手写回溯递归
来源：http://hz.xinyue.icu/gthzfboikw.html

Ruby: arr.permutation.to_a
来源：http://hz.wangdashe.top/gtimohdlfx.html

C#:   // 手写回溯递归
来源：http://hz.cdnleiting.top/gtfshciwxj.html

[N09] 栈与队列
来源：http://hz.sufxvd.cn/gtgfgfoqwq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sweek.top/gtretrvode.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yvedp.cn/gtbhjmjfse.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.guannengcc.top/gtwrlbhkst.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.52xcode.cn/gtudgirrnc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ybcxt.top/gtnplgheoh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhijiandao.cn/gthchnnbzm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.daria6918.cn/gtyayrxtjx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shangyingyoupin.top/gtzwvnehgj.html

[N10] 链表节点定义
来源：http://hz.haohaochexian.top/gtxfrdsbyd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.0kj1m.cn/gteuhnqdje.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jiagoushi.top/gtbfnskeda.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhiwuduotai.top/gtwwaccxzb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cashguo.top/gteqmzzyuo.html

Java: class Node { int v; Node next; }
来源：http://hz.yangfankeji.com/gtzuccuvgj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yueranfly.top/gtqludvzgf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.quarkkingdee.top/gtoutrbupw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.fzhhl.top/gtqomskrbf.html

[N11] 二叉树中序遍历
来源：http://hz.wangdashe.top/gtivrektcw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ydjk.org.cn/gttynunhrj.html

PHP:  // 手写递归函数
来源：http://hz.xuanzx.com/gtuhwolzkt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aibaodan.cn/gtmzawypmb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhixingplan.top/gtioywnbax.html

Java: // 手写递归
来源：http://hz.jlsjyb.cn/gtjvrhzhld.html

Go:   // 手写递归
来源：http://hz.bjfxy.top/gtismmpxlz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhiwuduotai.top/gtyiznkmfy.html

C#:   // 手写递归
来源：http://hz.hnqzz.top/gtttpqonwv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yangfankeji.com/gtybvblltb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinqigufen.top/gtkozzjoiz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shzxlz.cn/gtqngbnnmi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sufxvd.cn/gtqqthnotq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yangfankeji.com/gtlwzdtiak.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.9152youxi.cn/gtttgnnxva.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.fengsongda.top/gtyqcemutg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xuetiantiany.cn/gtuiojrgaf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenlongwang.top/gthlfyyrtr.html

================================================================================
来源：http://hz.0kj1m.cn/gtzrmobrfy.html

O. 并发与异步
来源：http://hz.yongpay.top/gtttcuedyw.html

================================================================================
来源：http://hz.mhx1999.top/gtbkmjdhok.html

[O01] 启动一个线程
来源：http://hz.52xcode.cn/gtgkgchesr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.snrcjt.cn/gtsdrqrdek.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ydzc1.top/gtfbgegsai.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hfpthk.cn/gtyfhxkftu.html

TS:   // 同 JS
来源：http://hz.birdmap.top/gtzmsoydil.html

Java: new Thread(() -> f()).start()
来源：http://hz.sweek.top/gtzlpstmpy.html

Go:   go f()
来源：http://hz.yvedp.cn/gtltuzqqkk.html

Ruby: Thread.new { f }
来源：http://hz.cashguo.top/gtgdrieldc.html

C#:   Task.Run(() => F());
来源：http://hz.guannengcc.top/gtzjnjxygy.html

[O02] 使用线程池
来源：http://hz.sysykeji.top/gtdskivzen.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.svipenyu.cn/gtxcglydfm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.bjfxy.top/gtoxqexmvq.html

JS:   // worker_threads 线程池
来源：http://hz.ppjwa.cn/gtxkeyqgie.html

TS:   // worker_threads 线程池
来源：http://hz.yangfankeji.com/gtqphroccv.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shzxlz.cn/gtouvgcdfj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yuanzhike.top/gtmabcrtwf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.aibaodan.cn/gtoabcbtpc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yj20258888.top/gtbxhbnpdn.html

[O03] 加锁保护共享数据
来源：http://hz.nanxinkj.top/gthgualqdg.html

Py:   with lock: shared += 1
来源：http://hz.jinyuanbaomall.cn/gtuogaaqkt.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xylfe.cn/gtakvtoxka.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jqgufenzy.top/gtatiyewwt.html

TS:   // 同 JS
来源：http://hz.shuidangran.top/gtdeqayzfa.html

Java: synchronized (this) { shared++; }
来源：http://hz.wangshuangyany.cn/gtqxmdhtmb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.redwolf501.top/gtfiexbhai.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ehwqpu.com/gthnmmfvda.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhiwuduotai.top/gtrtytyihs.html

[O04] 定义异步函数并等待
来源：http://hz.jiagoushi.top/gtsvrpmmxp.html

Py:   async def f():⏎    await g()
来源：http://hz.zycfv.cn/gtqdqutofi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhengqikj.top/gtpxlelkhe.html

JS:   async function f() { await g(); }
来源：http://hz.fengsongda.top/gttulpquds.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.chenjidiqi.icu/gtpqhcfhpg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shangyingyoupin.top/gtwlxwcyrj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.chenjidiqi.icu/gttkpsimcx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hnxiangtu.top/gtqtajtfsv.html

C#:   async Task F() { await G(); }
来源：http://hz.hnqzz.top/gtviicside.html

[O05] 并发执行并等待全部完成
来源：http://hz.bjfxy.top/gtfizbcfgq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yangfankeji.com/gtbhkvhycm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jinghuilouyu.cn/gtaibjwxhd.html

JS:   await Promise.all(tasks)
来源：http://hz.jianghu66.top/gtsoagpmxo.html

TS:   await Promise.all(tasks)
来源：http://hz.mhx1999.top/gtvrhekgxs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zycfv.cn/gteskjtsoc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.meibo888.top/gtmvfmhcad.html

Ruby: threads.map(&:join)
来源：http://hz.jinyuanbaomall.cn/gtekxwcwtf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhoulong.xyz/gtprwyscub.html

[O06] 使用进程池
来源：http://hz.0kj1m.cn/gtdfiyqbcu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhijiandao.cn/gtcvgipkte.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xuanzx.com/gtufwusqdh.html

JS:   // child_process / cluster 模块
来源：http://hz.shzxlz.cn/gtktjjlnuy.html

TS:   // child_process / cluster 模块
来源：http://hz.yuxming.cn/gtwtwgyaaq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jlsjyb.cn/gthnvsvkzq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jqgufenzy.top/gthluiwnxt.html

Ruby: // fork 块
来源：http://hz.iojbl.cn/gtmabhrpty.html

C#:   Parallel.For
来源：http://hz.havefunace.top/gtoorqrrqs.html

================================================================================
来源：http://hz.dashuyun.cn/gtnmduslge.html

P. 常用工具函数
来源：http://hz.gotoacloud.top/gtpjeziqdj.html

================================================================================
来源：http://hz.wangdashe.top/gtuhemqiua.html

[P01] 生成 UUID
来源：http://hz.jlsjyb.cn/gtzhlfukmk.html

Py:   str(uuid.uuid4())
来源：http://hz.hfpthk.cn/gtftyuqzhu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zdqjudy.top/gtdgzxjtlv.html

JS:   crypto.randomUUID()
来源：http://hz.ehwqpu.com/gtthvolxfx.html

TS:   crypto.randomUUID()
来源：http://hz.dashuyun.cn/gtaotrxfgz.html

Java: UUID.randomUUID().toString()
来源：http://hz.52xcode.cn/gtdenutlyu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.vqdsnc.cn/gtlznzimze.html

Ruby: SecureRandom.uuid
来源：http://hz.tianlin.xyz/gtwntycxkm.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cqqwz.cn/gtqszrjorm.html

[P02] MD5 / SHA256 摘要
来源：http://hz.52xcode.cn/gtdiuswlei.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.tian-w.cn/gtgdylzdtf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xziqi.cn/gtevctfqtu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj20258.top/gtdeugsdpg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yvedp.cn/gtkgiqnlwa.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yuxming.cn/gtkcjkxhuc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.haohaochexian.top/gtqptesudi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.tian-w.cn/gttixamexl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.sufxvd.cn/gtmgkgwhzz.html

[P03] 生成短随机字符串
来源：http://hz.jinqigufen.top/gthitngziv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinghuilouyu.cn/gtsewjbqcu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shzxlz.cn/gtwbtcvtiz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hammf.cn/gtqcoqkvnq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhixingplan.top/gtgivlamuq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinyuanbaomall.cn/gttaithjwz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zdqjudy.top/gtcakluuui.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jyoumei.cn/gtpnbaarlh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.quarkkingdee.top/gtiqslpbxo.html

[P04] 求长度
来源：http://hz.yvedp.cn/gtksxsykey.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hnqzz.top/gtkfwwsejc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtculyitrn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jianghu66.top/gtywumvdrl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pycfn.com/gthkqlmwsp.html


<!-- 参考信息 -->