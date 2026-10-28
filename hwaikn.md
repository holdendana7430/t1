代发 wailian999

Py:   resp.json()
来源：http://hz.aizwys.cn/gtjmtyftwo.html

PHP:  json_decode($body, true);
来源：http://hz.c1oappe.top/gteduqmqdt.html

JS:   await resp.json()
来源：http://hz.zhoulong.xyz/gtuhfhntty.html

TS:   await resp.json()
来源：http://hz.vqdsnc.cn/gtaclwfrbv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.tian-w.cn/gtsoahocqr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cashguo.top/gtqnsmrcgj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.birdmap.top/gtljzxqxmh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yonumen.top/gthnzrtoyh.html

[L07] 处理 HTTP 状态码
来源：http://hz.52xcode.cn/gtoxtuulwi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.wangshuangyany.cn/gtkwepvlbd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zdqjudy.top/gtwfglgkto.html

JS:   resp.ok;  resp.status
来源：http://hz.zycfv.cn/gtsjpcqqgg.html

TS:   resp.ok;  resp.status
来源：http://hz.feifeiyinyue.top/gtubmmlpdv.html

Java: resp.statusCode()
来源：http://hz.dianchejie.cn/gttkewijjq.html

Go:   resp.StatusCode
来源：http://hz.jlsjyb.cn/gtkylkkqxy.html

Ruby: resp.code.to_i
来源：http://hz.gzhubu.top/gtpnglkeht.html

C#:   (int)resp.StatusCode
来源：http://hz.xylfe.cn/gtrbzcpusb.html

[L08] 并发请求多个地址
来源：http://hz.jinghuilouyu.cn/gtzpqhdutc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ehwqpu.com/gtksmsmxgq.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhixingplan.top/gtewbrxolo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxinkj.top/gttrbnuwyj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guowangkeji.top/gtligkgyyk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ehwqpu.com/gtjjjjmqje.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gogol.net.cn/gtzvzyrgrv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.pycfn.com/gttighgdit.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cdnleiting.top/gttgamojzj.html

================================================================================
来源：http://hz.smart0.xyz/gtxobmoiya.html

M. 命令行 / 进程 / 环境
来源：http://hz.wangshuangyany.cn/gtzxkjzrki.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtliatlarj.html

[M01] 读取命令行参数
来源：http://hz.jiagoushi.top/gthmultizg.html

Py:   sys.argv[1:]
来源：http://hz.hnqzz.top/gthifgskqe.html

PHP:  $argv;  $argc;
来源：http://hz.ybcxt.top/gtdfpodvvu.html

JS:   process.argv.slice(2)
来源：http://hz.gotoacloud.top/gthoaggzue.html

TS:   process.argv.slice(2)
来源：http://hz.ehwqpu.com/gtliojkpob.html

Java: args 数组（main 方法参数）
来源：http://hz.cucudq.cn/gtozthxzth.html

Go:   os.Args[1:]
来源：http://hz.hammf.cn/gtjxaxjyvf.html

Ruby: ARGV
来源：http://hz.jiagoushi.top/gtdxpklgxx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hysaishi.cn/gtdyidfdnm.html

[M02] 读取环境变量
来源：http://hz.dashuyun.cn/gterngrjri.html

Py:   os.environ.get("HOME")
来源：http://hz.jqgfzy.top/gthhjzklex.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.bjfxy.top/gtkkpcdmmx.html

JS:   process.env.HOME
来源：http://hz.aizwys.cn/gtkaxwcolp.html

TS:   process.env.HOME
来源：http://hz.havefunace.top/gthgblhemk.html

Java: System.getenv("HOME")
来源：http://hz.316326.xyz/gtvhkvaasb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yj20258888.top/gtjyfudoxs.html

Ruby: ENV["HOME"]
来源：http://hz.yongpay.top/gtjgyvffro.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gotoacloud.top/gtczoghoch.html

[M03] 执行外部命令
来源：http://hz.gotoacloud.top/gtnratqagp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xingfuxueyuan.xyz/gttmcahghk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhoulong.xyz/gtmoywmpyj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.pengpengdd.cyou/gtyfwbodty.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.fzhhl.top/gtjtxrfomf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cheryme.top/gtvduweudu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cucudq.cn/gtpymgptvd.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gotoacloud.top/gtgbsonvbt.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hfpthk.cn/gtwnndotzp.html

[M04] 获取当前工作目录
来源：http://hz.shzxlz.cn/gtwadpuaqc.html

Py:   os.getcwd()
来源：http://hz.aizwys.cn/gtkuralqjw.html

PHP:  getcwd();
来源：http://hz.yvedp.cn/gtwpwmpdui.html

JS:   process.cwd()
来源：http://hz.ydjk.org.cn/gtsdcadokd.html

TS:   process.cwd()
来源：http://hz.wangdashe.top/gthscvqxmg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinqigfzy.top/gtblqffdns.html

Go:   os.Getwd()
来源：http://hz.tian-w.cn/gtipiiydnp.html

Ruby: Dir.pwd
来源：http://hz.chenlongwang.top/gtcutlgcze.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gotoacloud.top/gtmnuwjnto.html

[M05] 设置退出码
来源：http://hz.xuetiantiany.cn/gttiwdlypq.html

Py:   sys.exit(1)
来源：http://hz.dashuyun.cn/gtmashiket.html

PHP:  exit(1);
来源：http://hz.9152youxi.cn/gtomcvjjhl.html

JS:   process.exit(1)
来源：http://hz.guannengcc.top/gtmnjscysk.html

TS:   process.exit(1)
来源：http://hz.ehwqpu.com/gtmftjdujd.html

Java: System.exit(1)
来源：http://hz.iojbl.cn/gtivtsaevm.html

Go:   os.Exit(1)
来源：http://hz.yj202588.top/gtbdmnyjhz.html

Ruby: exit 1
来源：http://hz.dashuyun.cn/gttljurnhc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.pengpengdd.cyou/gtsdhqytzg.html

[M06] 向标准错误输出
来源：http://hz.sxryk.cn/gtebuxybcn.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shanyushiyangkeji.top/gtpfrpjpks.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xuetiantiany.cn/gtaoaeyipy.html

JS:   console.error("err")
来源：http://hz.xinyue.icu/gtqwyrbfzj.html

TS:   console.error("err")
来源：http://hz.gaohongyu789.top/gtiuzqqmso.html

Java: System.err.println("err")
来源：http://hz.wangshuangyany.cn/gtwkvzydyk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cheryme.top/gttabeqiaw.html

Ruby: warn "err"
来源：http://hz.zhixingplan.top/gthhluwfwz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hywenlv.cn/gtmznatsgf.html

[M07] 判断是否为主入口
来源：http://hz.chenjidiqi.icu/gtfwwwkqir.html

Py:   if __name__ == "__main__":
来源：http://hz.xuetiantiany.cn/gtxlxvnlso.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.sysykeji.top/gtcyhqjppb.html

JS:   require.main === module
来源：http://hz.kuanghao11.cn/gtqvznxdfc.html

TS:   require.main === module
来源：http://hz.xinyue.icu/gtisbcaznw.html

Java: public static void main(String[] args)
来源：http://hz.quarkkingdee.top/gtrjglkuom.html

Go:   func main()
来源：http://hz.shuidangran.top/gtwqquaukr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cdnleiting.top/gthuqbcvah.html

C#:   static void Main(string[] args)
来源：http://hz.daxiang520.top/gtkpmlnhdn.html

[M08] 获取系统与运行时信息
来源：http://hz.dashuyun.cn/gtvkrmjwbe.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yanxiufei.cn/gtepqoyvyv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.iojbl.cn/gtpeniqxha.html

JS:   process.platform;  process.version
来源：http://hz.shuidangran.top/gtmspevbxs.html

TS:   process.platform;  process.version
来源：http://hz.quarkkingdee.top/gtjkyzumcv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.guannengcc.top/gtljbecawu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.quarkkingdee.top/gtrephqdfc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.chenlongwang.top/gtzjlijfrz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hywenlv.cn/gtdgtcgoxo.html

================================================================================
来源：http://hz.c1oappe.top/gtjmpvcpmj.html

N. 数据结构与算法
来源：http://hz.xuetiantiany.cn/gtymwgshml.html

================================================================================
来源：http://hz.aibaodan.cn/gtwprvqurb.html

[N01] 二分查找（有序数组）
来源：http://hz.zhongyouzk.top/gtagqsduec.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sxryk.cn/gtsnwbirxm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jianghu66.top/gtlpiylypz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zdqjudy.top/gtuppqosgl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cucudq.cn/gttqitsztt.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jiagoushi.top/gtrpjzbdae.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hysaishi.cn/gtgkluzuek.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ybcxt.top/gtgrqsoxmk.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.tanke756.top/gtjohthwcn.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yj20258.top/gtzhyekptl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.guannengcc.top/gtftgymhbp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.bjfxy.top/gtjcfmgruh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hysaishi.cn/gtcopqofcf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hysaishi.cn/gtohvlswqh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.vqdsnc.cn/gtaaqdveiu.html

Go:   slices.Sort(arr)
来源：http://hz.dianchejie.cn/gtdfupmzib.html

Ruby: arr.sort
来源：http://hz.zhiwuduotai.top/gtqmfunbxp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.pengpengdd.cyou/gttsiiakgn.html

[N03] 快速排序（分治示例）
来源：http://hz.yueranfly.top/gtssmcvhqs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xylfe.cn/gtzyounmzo.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nanxinkj.top/gtyiuhncoe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sxryk.cn/gtypjitojw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hnxiangtu.top/gtwkdxwrsb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.bjfxy.top/gtqyynclwo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hongshengwenyu.top/gtkrrdjyks.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yangfankeji.com/gtgtoxrrvc.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gaohongyu789.top/gtmhumxwpu.html

[N04] 斐波那契数列
来源：http://hz.52xcode.cn/gtpzuhjajs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.svipenyu.cn/gtmzbdvvib.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinghuilouyu.cn/gtkwoyukpe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigufen.top/gtutmksbux.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenlongwang.top/gthxqllqrh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.c1oappe.top/gtwmgthxuf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jqgufenzy.top/gtgqfroyxc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.birdmap.top/gtquuphrip.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cucudq.cn/gtmxaqmlja.html

[N05] 最大公约数
来源：http://hz.xingfuxueyuan.xyz/gtflqpydjl.html

Py:   math.gcd(a, b)
来源：http://hz.haohaochexian.top/gtidfmrswz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinqigfzy.top/gttjomhtbp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.0kj1m.cn/gtpnizjrze.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.kuanghao11.cn/gthqizbyvt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yuanzhike.top/gtngqfygrm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.daria6918.cn/gtixhtjijc.html

Ruby: a.gcd(b)
来源：http://hz.ppjwa.cn/gtwygtpwrv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.aibaodan.cn/gtqqpabyxz.html

[N06] 判断回文字符串
来源：http://hz.jqgfzy.top/gtnwqutlpx.html

Py:   s == s[::-1]
来源：http://hz.zhaomingkeji.xyz/gtxqpruiky.html

PHP:  $s === strrev($s);
来源：http://hz.0kj1m.cn/gtookznpfp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.feifeiyinyue.top/gtkhiiaihn.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtbjrkycnt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xingfuxueyuan.xyz/gtacndgfms.html

Go:   // 双指针从两端比较
来源：http://hz.jqgufenzy.top/gtjnmkylsq.html

Ruby: s == s.reverse
来源：http://hz.zhoulong.xyz/gtjmdpbotp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ivvv.top/gtnlnjfxqn.html

[N07] 两数之和（返回下标）
来源：http://hz.fengsongda.top/gtsczbnfuo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.quarkkingdee.top/gtvaasywcn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.fengsongda.top/gtcgkvzymt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hysaishi.cn/gtpzgreszg.html

TS:   // 手写 Map<string, number>
来源：http://hz.c1oappe.top/gtrakpwtkq.html

Java: // 手写 HashMap
来源：http://hz.ehwqpu.com/gtcbamkscf.html

Go:   // 手写 map[int]int
来源：http://hz.hysaishi.cn/gtvvplgebh.html

Ruby: // 手写 Hash
来源：http://hz.shangyingyoupin.top/gtoxlnsqaw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cdnleiting.top/gtxbhtfxee.html

[N08] 生成全排列
来源：http://hz.yonumen.top/gtndpjufok.html

Py:   itertools.permutations(arr)
来源：http://hz.0kj1m.cn/gtpugxqdbo.html

PHP:  // 手写递归交换
来源：http://hz.nanxuanxn.top/gttreembkd.html

JS:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtebdvnumz.html

TS:   // 手写回溯递归
来源：http://hz.ybcxt.top/gtowructse.html

Java: // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtditjttqv.html

Go:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtxblkyufx.html

Ruby: arr.permutation.to_a
来源：http://hz.jinqigfzy.top/gtxoefpefa.html

C#:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtrfxyzvzw.html

[N09] 栈与队列
来源：http://hz.hfpthk.cn/gthimudsqu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shangyingyoupin.top/gtcgrophuw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jyoumei.cn/gterbztnxo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jyoumei.cn/gtnlgzlwis.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ydzc1.top/gtyovmvqxq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.chenlongwang.top/gtlozluhxf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hammf.cn/gtjzydiymu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.tanke756.top/gtsfwxjoho.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.dashuyun.cn/gtszxbxlkc.html

[N10] 链表节点定义
来源：http://hz.tianlin.xyz/gtzawjweaj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jiagoushi.top/gtsncorlqo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xuetiantiany.cn/gtkihkotah.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ydzc1.top/gtfallgbwy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hammf.cn/gtrquuciyz.html

Java: class Node { int v; Node next; }
来源：http://hz.52xcode.cn/gtkreajtcc.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinqigufen.top/gtkxgxirzy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.iojbl.cn/gtwggxcydv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.tian-w.cn/gtpuvgvfho.html

[N11] 二叉树中序遍历
来源：http://hz.andypj.xyz/gteavadckt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ybcxt.top/gtxcfyubhw.html

PHP:  // 手写递归函数
来源：http://hz.zycfv.cn/gtzukqmgrf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jyoumei.cn/gtswqvaicm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gaohongyu789.top/gtvfydkihw.html

Java: // 手写递归
来源：http://hz.hnqzz.top/gtpisyyaow.html

Go:   // 手写递归
来源：http://hz.0kj1m.cn/gtusdwotlx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yj202588.top/gtiwhvpvko.html

C#:   // 手写递归
来源：http://hz.jqgfzy.top/gtcosmhjuv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ywan-chungtsiang.top/gtbarefuny.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shangyingyoupin.top/gtbdnbptsd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.nwbrower.top/gtmaqzfdrt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.bjfxy.top/gtniefxuhg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jyoumei.cn/gtcwbcqzxq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuanzx.com/gtyfpjxjyr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.bjfxy.top/gtuftqlobz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhongyouzk.top/gtyifhtbkx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fengsongda.top/gtchhwjggq.html

================================================================================
来源：http://hz.andypj.xyz/gtyszyofez.html

O. 并发与异步
来源：http://hz.yj20258888.top/gtvpdwonxv.html

================================================================================
来源：http://hz.chenlongwang.top/gtwwweteaj.html

[O01] 启动一个线程
来源：http://hz.nwbrower.top/gtghaashzi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.guowangkeji.top/gtygmagwdh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.svipenyu.cn/gthlnmumyx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ppjwa.cn/gtamrodptq.html

TS:   // 同 JS
来源：http://hz.wangdashe.top/gtkonveefl.html

Java: new Thread(() -> f()).start()
来源：http://hz.xylfe.cn/gtrtdurjkj.html

Go:   go f()
来源：http://hz.yj20258888.top/gtauduaypn.html

Ruby: Thread.new { f }
来源：http://hz.daria6918.cn/gtbwcvugif.html

C#:   Task.Run(() => F());
来源：http://hz.hongshengwenyu.top/gtwlemhzos.html

[O02] 使用线程池
来源：http://hz.jianghu66.top/gtnqdcfglx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.snrcjt.cn/gtomhlchtn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.chenjidiqi.icu/gtypzowlcg.html

JS:   // worker_threads 线程池
来源：http://hz.guowangkeji.top/gtyoxyojrj.html

TS:   // worker_threads 线程池
来源：http://hz.nanxinkj.top/gtguqbbvio.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shangyingyoupin.top/gtfpsvetns.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhaomingkeji.xyz/gtincnizjw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.wangshuangyany.cn/gtivcfwkti.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hammf.cn/gtwldgyfef.html

[O03] 加锁保护共享数据
来源：http://hz.sweek.top/gtourtwfaq.html

Py:   with lock: shared += 1
来源：http://hz.pycfn.com/gtnpveorwo.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zdqjudy.top/gtkyaybovi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.mhx1999.top/gtrhawzuem.html

TS:   // 同 JS
来源：http://hz.aibaodan.cn/gtygtgjigy.html

Java: synchronized (this) { shared++; }
来源：http://hz.0kj1m.cn/gtejahbxny.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shanyushiyangkeji.top/gtjcfwqpdt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cucudq.cn/gtspjhlyll.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj20258.top/gtmihsjdul.html

[O04] 定义异步函数并等待
来源：http://hz.chenjidiqi.icu/gtdpcasgqe.html

Py:   async def f():⏎    await g()
来源：http://hz.yongpay.top/gtknonlxpo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nwbrower.top/gtqeobriug.html

JS:   async function f() { await g(); }
来源：http://hz.bjfxy.top/gtnooiseop.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.sufxvd.cn/gtxrvipvji.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.quarkkingdee.top/gtembazkpb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.chenlongwang.top/gtgiqixxcu.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cdnleiting.top/gtigccqdhx.html

C#:   async Task F() { await G(); }
来源：http://hz.daxiang520.top/gtafxsumeb.html

[O05] 并发执行并等待全部完成
来源：http://hz.sysykeji.top/gtqdkvmcxp.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jlsjyb.cn/gtkhukjnfe.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jianghu66.top/gtzassushi.html

JS:   await Promise.all(tasks)
来源：http://hz.jinyuanbaomall.cn/gtzikhczbb.html

TS:   await Promise.all(tasks)
来源：http://hz.yonumen.top/gtrufjjpat.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.pycfn.com/gtiyhfyaoq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xylfe.cn/gtxvihnwsc.html

Ruby: threads.map(&:join)
来源：http://hz.dashuyun.cn/gtmzpoosjw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinyuanbaomall.cn/gtkaaimfes.html

[O06] 使用进程池
来源：http://hz.nanxuanxn.top/gtwbigwfvl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yonumen.top/gtdrebeyot.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.52xcode.cn/gtlhzoiisa.html

JS:   // child_process / cluster 模块
来源：http://hz.52xcode.cn/gthjeaxncf.html

TS:   // child_process / cluster 模块
来源：http://hz.feifeiyinyue.top/gtndefzxfm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.nanxinkj.top/gtwffbodku.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yj20258888.top/gtlmyzswcl.html

Ruby: // fork 块
来源：http://hz.hnxiangtu.top/gtipixuxgo.html

C#:   Parallel.For
来源：http://hz.cheryme.top/gtaobdbvln.html

================================================================================
来源：http://hz.birdmap.top/gtsnkxxofi.html

P. 常用工具函数
来源：http://hz.jinqigufen.top/gtvzlpbqhf.html

================================================================================
来源：http://hz.zhijiandao.cn/gtcrnvirrk.html

[P01] 生成 UUID
来源：http://hz.jinghuilouyu.cn/gtdnyagote.html

Py:   str(uuid.uuid4())
来源：http://hz.zhengqikj.top/gtjrpbzndp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jqgfzy.top/gtaknytmkv.html

JS:   crypto.randomUUID()
来源：http://hz.shuidangran.top/gtmxixjndd.html

TS:   crypto.randomUUID()
来源：http://hz.pycfn.com/gtpfkfmfgg.html

Java: UUID.randomUUID().toString()
来源：http://hz.ivvv.top/gtnkozcpaf.html

Go:   // 用 github.com/google/uuid
来源：http://hz.chenlongwang.top/gtqynuwtte.html

Ruby: SecureRandom.uuid
来源：http://hz.jianghu66.top/gtotmdpmrs.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.quarkkingdee.top/gtbmaiobxy.html

[P02] MD5 / SHA256 摘要
来源：http://hz.smart0.xyz/gtqzmwxcnm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.tianlin.xyz/gtvyrumnmf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.aizwys.cn/gtsuqxcpeo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.andypj.xyz/gtyopmovur.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ywan-chungtsiang.top/gtuilssvnq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xziqi.cn/gtfxbgscws.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.fzhhl.top/gtwatoggvd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ywan-chungtsiang.top/gtxsiysakz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhoulong.xyz/gtwdcupjdx.html

[P03] 生成短随机字符串
来源：http://hz.havefunace.top/gtrrmhaitd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ydzc1.top/gtwjqhlmua.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.tanke756.top/gtyuaazkmv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.wangdashe.top/gtbpomzsvn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangkeji.top/gtyjrlhjoi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhiwuduotai.top/gttuubqvvt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.snrcjt.cn/gtzqbxhwdm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.chenjidiqi.icu/gtafmaaqsf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.chenzaomai.com/gtoqdicurk.html

[P04] 求长度
来源：http://hz.sufxvd.cn/gtipmbiifp.html


<!-- 参考信息 -->