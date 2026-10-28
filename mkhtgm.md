代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.redwolf501.top/gtmzebhmdu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhixingplan.top/gtnmbjvdlx.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhoulong.xyz/gtctbyrgen.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jqgufenzy.top/gtewttrnkg.html

[L07] 处理 HTTP 状态码
来源：http://hz.nanxinkj.top/gtlroebppa.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.andypj.xyz/gtdagthqef.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinghuilouyu.cn/gtlhycieno.html

JS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gtuvdxpmdt.html

TS:   resp.ok;  resp.status
来源：http://hz.zhaomingkeji.xyz/gthuulwysb.html

Java: resp.statusCode()
来源：http://hz.chenzaomai.com/gthqukwelx.html

Go:   resp.StatusCode
来源：http://hz.hysaishi.cn/gtzlloewvl.html

Ruby: resp.code.to_i
来源：http://hz.jqgufenzy.top/gtsusddzup.html

C#:   (int)resp.StatusCode
来源：http://hz.ydjk.org.cn/gtcpvfiszq.html

[L08] 并发请求多个地址
来源：http://hz.zhixingplan.top/gtkvbksieu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinghuilouyu.cn/gtkxwhtctz.html

PHP:  curl_multi_init() 系列
来源：http://hz.jiagoushi.top/gtcbdfitfv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj202588.top/gteenbefvu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dashuyun.cn/gtugjbjsjb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hongshengwenyu.top/gtjyzjvfcf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.daxiang520.top/gtddmtvxcu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.9152youxi.cn/gtmzeynexg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.chenzaomai.com/gtrmtunaib.html

================================================================================
来源：http://hz.xinyue.icu/gtzbewrxit.html

M. 命令行 / 进程 / 环境
来源：http://hz.jyoumei.cn/gtdgajiacq.html

================================================================================
来源：http://hz.dianchejie.cn/gtlaxvmrga.html

[M01] 读取命令行参数
来源：http://hz.sufxvd.cn/gteejycqpw.html

Py:   sys.argv[1:]
来源：http://hz.xziqi.cn/gtwqxpqlql.html

PHP:  $argv;  $argc;
来源：http://hz.sysykeji.top/gtvylqmoxp.html

JS:   process.argv.slice(2)
来源：http://hz.9152youxi.cn/gtmsphrlle.html

TS:   process.argv.slice(2)
来源：http://hz.shanyushiyangkeji.top/gtmxhorkvc.html

Java: args 数组（main 方法参数）
来源：http://hz.zhongyouzk.top/gtoikxlgmb.html

Go:   os.Args[1:]
来源：http://hz.ivvv.top/gtvyqheoof.html

Ruby: ARGV
来源：http://hz.jyoumei.cn/gtmwaukxqm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jqgufenzy.top/gthxyztnhr.html

[M02] 读取环境变量
来源：http://hz.guowangkeji.top/gtotidkmvb.html

Py:   os.environ.get("HOME")
来源：http://hz.sysykeji.top/gtwrdguony.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hammf.cn/gtjskoviio.html

JS:   process.env.HOME
来源：http://hz.xuanzx.com/gtlvkzcwew.html

TS:   process.env.HOME
来源：http://hz.zhoulong.xyz/gtqofaghhk.html

Java: System.getenv("HOME")
来源：http://hz.zhijiandao.cn/gtkcdrcyvo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xuetiantiany.cn/gtsuxeycvi.html

Ruby: ENV["HOME"]
来源：http://hz.hongshengwenyu.top/gtxwbmadhq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shangyingyoupin.top/gtxvggtent.html

[M03] 执行外部命令
来源：http://hz.nwbrower.top/gtdxidmjfe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhongyouzk.top/gtuiobzdkz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.nanxuanxn.top/gtuifqcgsv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhaomingkeji.xyz/gtvkssgemb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.tanke756.top/gtnufwlfbt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ywan-chungtsiang.top/gtmueytrzd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhoulong.xyz/gtjronueue.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gzhubu.top/gtjifcpxlo.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yangfankeji.com/gtkqshrffs.html

[M04] 获取当前工作目录
来源：http://hz.chenlongwang.top/gtrcefdhid.html

Py:   os.getcwd()
来源：http://hz.jqgfzy.top/gtrcgohaxg.html

PHP:  getcwd();
来源：http://hz.hysaishi.cn/gthdgtngsu.html

JS:   process.cwd()
来源：http://hz.hysaishi.cn/gthtlpalso.html

TS:   process.cwd()
来源：http://hz.gzhubu.top/gtlzqvrirq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yonumen.top/gtlllpevxw.html

Go:   os.Getwd()
来源：http://hz.sweek.top/gtqibldift.html

Ruby: Dir.pwd
来源：http://hz.9152youxi.cn/gtfcrfrgvo.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yuxming.cn/gtlaulvmjn.html

[M05] 设置退出码
来源：http://hz.yuxming.cn/gtyjcoobpv.html

Py:   sys.exit(1)
来源：http://hz.yongpay.top/gtmrkzlcig.html

PHP:  exit(1);
来源：http://hz.tianlin.xyz/gtwoxdapev.html

JS:   process.exit(1)
来源：http://hz.cqqwz.cn/gtqpxdissx.html

TS:   process.exit(1)
来源：http://hz.birdmap.top/gtenftnzte.html

Java: System.exit(1)
来源：http://hz.andypj.xyz/gtyzstwymo.html

Go:   os.Exit(1)
来源：http://hz.jiagoushi.top/gtjgdjhjpv.html

Ruby: exit 1
来源：http://hz.ydjk.org.cn/gtliblgcfc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.redwolf501.top/gtvjqaotyn.html

[M06] 向标准错误输出
来源：http://hz.nwbrower.top/gtltudscma.html

Py:   print("err", file=sys.stderr)
来源：http://hz.aibaodan.cn/gtrvzvixzb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.wangdashe.top/gtyxcuyuay.html

JS:   console.error("err")
来源：http://hz.jiagoushi.top/gtiiffaovb.html

TS:   console.error("err")
来源：http://hz.meibo888.top/gttvxiggij.html

Java: System.err.println("err")
来源：http://hz.ybcxt.top/gthhnmxtvn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yj202588.top/gtxixksfvp.html

Ruby: warn "err"
来源：http://hz.ivvv.top/gtrgbedtfc.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.tianlin.xyz/gtvekuodvd.html

[M07] 判断是否为主入口
来源：http://hz.yanxiufei.cn/gtorhwsnjk.html

Py:   if __name__ == "__main__":
来源：http://hz.yonumen.top/gtdrgdppnu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.bjfxy.top/gtmixprsgs.html

JS:   require.main === module
来源：http://hz.chenjidiqi.icu/gtkgkzmoyw.html

TS:   require.main === module
来源：http://hz.yj20258.top/gtvoeevyeu.html

Java: public static void main(String[] args)
来源：http://hz.zhongyouzk.top/gtzuqivvko.html

Go:   func main()
来源：http://hz.feifeiyinyue.top/gtrtovhnfu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.wangshuangyany.cn/gtgcvqdtoe.html

C#:   static void Main(string[] args)
来源：http://hz.dashuyun.cn/gtxmtwhpyn.html

[M08] 获取系统与运行时信息
来源：http://hz.cdnleiting.top/gtshyctpac.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jlsjyb.cn/gttywgpgwh.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cucudq.cn/gtlqthoife.html

JS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtfhwjrnew.html

TS:   process.platform;  process.version
来源：http://hz.jqgfzy.top/gtuqtswqgk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tanke756.top/gtkvjvyihl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.andypj.xyz/gtppxothuy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.0kj1m.cn/gtghhkjcma.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.nanxinkj.top/gtvricletj.html

================================================================================
来源：http://hz.zhengqikj.top/gtapqwbhma.html

N. 数据结构与算法
来源：http://hz.hfpthk.cn/gtcqurltok.html

================================================================================
来源：http://hz.ivvv.top/gttapvnuqa.html

[N01] 二分查找（有序数组）
来源：http://hz.zycfv.cn/gthjosykki.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.316326.xyz/gtdgngzuqy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.nanxuanxn.top/gtvvimxapl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenlongwang.top/gtgilumnfb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zycfv.cn/gtnlrofobp.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenlongwang.top/gtllosmtdr.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yonumen.top/gtddnyjesq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.nwbrower.top/gtkvvfmyfc.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gogol.net.cn/gtawksqihy.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hfpthk.cn/gtscdpzlfn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenjidiqi.icu/gtilueqzjh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sweek.top/gtutwqbdkc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuetiantiany.cn/gtedmlcocd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinyuanbaomall.cn/gtrkmszxyd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.guowangkeji.top/gtmikcaikb.html

Go:   slices.Sort(arr)
来源：http://hz.ehwqpu.com/gtgwsuocia.html

Ruby: arr.sort
来源：http://hz.yj20258888.top/gtitrahfck.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.kuanghao11.cn/gtkmcwmlbd.html

[N03] 快速排序（分治示例）
来源：http://hz.chenlongwang.top/gtfkrhrtvg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.mhx1999.top/gtshekyshn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.svipenyu.cn/gtttkvzmef.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangdashe.top/gtmlwrhkqp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nwbrower.top/gtiayiqbjc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.iojbl.cn/gteydloelu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nanxinkj.top/gtdtbvboje.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shangyingyoupin.top/gtuzfgkesx.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.bjfxy.top/gtnueyodcy.html

[N04] 斐波那契数列
来源：http://hz.xingfuxueyuan.xyz/gtvdkyndbq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.quarkkingdee.top/gtxfeywokf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.chenlongwang.top/gtlvdfveca.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yvedp.cn/gtenvglmoy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.bjfxy.top/gtxohyinwe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ppjwa.cn/gtukoyspwm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.quarkkingdee.top/gtruhktpwa.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigfzy.top/gtxfvoshet.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jlsjyb.cn/gthphieppz.html

[N05] 最大公约数
来源：http://hz.jinqigfzy.top/gtnievqica.html

Py:   math.gcd(a, b)
来源：http://hz.gaohongyu789.top/gtyknqlxte.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hammf.cn/gtdwjvflyb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aibaodan.cn/gtanpucarg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xziqi.cn/gtjzykefia.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.quarkkingdee.top/gtkjthqwvq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.tanke756.top/gtfkevaqjt.html

Ruby: a.gcd(b)
来源：http://hz.yonumen.top/gtmgobquyb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xuetiantiany.cn/gtbzgmzvfq.html

[N06] 判断回文字符串
来源：http://hz.daxiang520.top/gteedlwdhm.html

Py:   s == s[::-1]
来源：http://hz.jiagoushi.top/gtedyodwss.html

PHP:  $s === strrev($s);
来源：http://hz.zhixingplan.top/gtmjmyazun.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtyqlknhty.html

TS:   s === [...s].reverse().join("")
来源：http://hz.haohaochexian.top/gtnemrfmlh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hywenlv.cn/gtyrubehsw.html

Go:   // 双指针从两端比较
来源：http://hz.yueranfly.top/gtfwputsfo.html

Ruby: s == s.reverse
来源：http://hz.cqqwz.cn/gtxqdznflo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ydzc1.top/gtsaknmwcc.html

[N07] 两数之和（返回下标）
来源：http://hz.tanke756.top/gtvnoshcfc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.meibo888.top/gtoenrhtit.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hongshengwenyu.top/gtibeenktk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xylfe.cn/gtszmepkpf.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj20258.top/gttcauhwvm.html

Java: // 手写 HashMap
来源：http://hz.gotoacloud.top/gtsgthkcpj.html

Go:   // 手写 map[int]int
来源：http://hz.zhijiandao.cn/gtqldtutie.html

Ruby: // 手写 Hash
来源：http://hz.feifeiyinyue.top/gtbwwwxvcx.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sxryk.cn/gtyjduqdiy.html

[N08] 生成全排列
来源：http://hz.smart0.xyz/gtfigripae.html

Py:   itertools.permutations(arr)
来源：http://hz.andypj.xyz/gtuxcpfttx.html

PHP:  // 手写递归交换
来源：http://hz.fzhhl.top/gtrfmpzgmq.html

JS:   // 手写回溯递归
来源：http://hz.daxiang520.top/gtjkqfkgal.html

TS:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtoxqajrly.html

Java: // 手写回溯递归
来源：http://hz.yvedp.cn/gtcobppadt.html

Go:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtezxfmgtn.html

Ruby: arr.permutation.to_a
来源：http://hz.zhoulong.xyz/gtkhgkccph.html

C#:   // 手写回溯递归
来源：http://hz.hysaishi.cn/gtjfvltnrv.html

[N09] 栈与队列
来源：http://hz.cucudq.cn/gtfutciovz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.cucudq.cn/gtcalfbfbs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ehwqpu.com/gtgufctvqa.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jyoumei.cn/gtcycqyrla.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hysaishi.cn/gtjjnhmivi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xziqi.cn/gtfrpbkozu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.feifeiyinyue.top/gtwlhtkxqg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.pycfn.com/gtwymjhsqv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zdqjudy.top/gtcekuxqxc.html

[N10] 链表节点定义
来源：http://hz.cqqwz.cn/gtjcuanamm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gogol.net.cn/gtdsedolma.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ehwqpu.com/gtrzlrxfyi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zdqjudy.top/gtaroightp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ydjk.org.cn/gtimoljafb.html

Java: class Node { int v; Node next; }
来源：http://hz.zhijiandao.cn/gtcropkjzb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.c1oappe.top/gtunxjjvqe.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.feifeiyinyue.top/gtolridbur.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hammf.cn/gttybadknn.html

[N11] 二叉树中序遍历
来源：http://hz.gzhubu.top/gtzgikpbnj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zdqjudy.top/gtleeirfds.html

PHP:  // 手写递归函数
来源：http://hz.aibaodan.cn/gtvblxsihw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sxryk.cn/gtyvxlketw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shanyushiyangkeji.top/gtcakvschc.html

Java: // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtdcqprelo.html

Go:   // 手写递归
来源：http://hz.jinqigfzy.top/gthuzuzuwx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.snrcjt.cn/gttcvrxrbn.html

C#:   // 手写递归
来源：http://hz.yueranfly.top/gtmmhtjoto.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.nanxuanxn.top/gtnnwudlfv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yangfankeji.com/gtubyjfigx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gzhubu.top/gtdcengxsa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jiagoushi.top/gtbnmxhdmz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yueranfly.top/gtndokuysi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shzxlz.cn/gtxxepcech.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhongyouzk.top/gttfcfaren.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ybcxt.top/gtvylnrshj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gotoacloud.top/gtqmsojmvm.html

================================================================================
来源：http://hz.yueranfly.top/gtlpezgvhv.html

O. 并发与异步
来源：http://hz.yongpay.top/gtcqoetrrz.html

================================================================================
来源：http://hz.yj20258.top/gtplfwajsd.html

[O01] 启动一个线程
来源：http://hz.iojbl.cn/gtuzubmofl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sufxvd.cn/gteirbxshl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hfpthk.cn/gtugfzrmvl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xuanzx.com/gtxzzcxqhq.html

TS:   // 同 JS
来源：http://hz.yj20258.top/gtpketphut.html

Java: new Thread(() -> f()).start()
来源：http://hz.meibo888.top/gtlramkqos.html

Go:   go f()
来源：http://hz.svipenyu.cn/gtmfzhuokd.html

Ruby: Thread.new { f }
来源：http://hz.jyoumei.cn/gtwcjnvfaq.html

C#:   Task.Run(() => F());
来源：http://hz.zhixingplan.top/gtltbhklzy.html

[O02] 使用线程池
来源：http://hz.mhx1999.top/gtirvyarje.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.andypj.xyz/gtoxprvifj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yj20258.top/gtutbfcpvo.html

JS:   // worker_threads 线程池
来源：http://hz.shangyingyoupin.top/gtyxbtaald.html

TS:   // worker_threads 线程池
来源：http://hz.shzxlz.cn/gtoiqpvpdd.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.pengpengdd.cyou/gtvndnqlie.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.c1oappe.top/gtfsnkgimr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.daria6918.cn/gtsqidmyxn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shangyingyoupin.top/gtfouqrlqa.html

[O03] 加锁保护共享数据
来源：http://hz.hammf.cn/gtxxjwgbuf.html

Py:   with lock: shared += 1
来源：http://hz.xinyue.icu/gtrvzczmpf.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ydjk.org.cn/gtljlnlvsc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.meibo888.top/gtdaocmnyo.html

TS:   // 同 JS
来源：http://hz.yj20258.top/gtdhdhaywy.html

Java: synchronized (this) { shared++; }
来源：http://hz.dashuyun.cn/gtlzcpivfm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ybcxt.top/gtndzxpogh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.vqdsnc.cn/gtggufytan.html

C#:   lock (gate) { shared++; }
来源：http://hz.shanyushiyangkeji.top/gtqcivadlq.html

[O04] 定义异步函数并等待
来源：http://hz.quarkkingdee.top/gtbtwruktp.html

Py:   async def f():⏎    await g()
来源：http://hz.tianlin.xyz/gtzjelalii.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ydjk.org.cn/gtpqgiwaqq.html

JS:   async function f() { await g(); }
来源：http://hz.shangyingyoupin.top/gtdgfixofe.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.tanke756.top/gtcllyxfsv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cucudq.cn/gtswdmufqx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zdqjudy.top/gtpaarwuqw.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.smart0.xyz/gtkuhbzphe.html

C#:   async Task F() { await G(); }
来源：http://hz.redwolf501.top/gtutezqbnl.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj202588.top/gtsywmybin.html

Py:   asyncio.gather(*tasks)
来源：http://hz.316326.xyz/gtzzkhkxzd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.iojbl.cn/gtpnoztvig.html

JS:   await Promise.all(tasks)
来源：http://hz.zhengqikj.top/gtlkcvcfqw.html

TS:   await Promise.all(tasks)
来源：http://hz.cashguo.top/gtggngybsa.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhengqikj.top/gtdwyxlefs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sxryk.cn/gtaauazqmg.html

Ruby: threads.map(&:join)
来源：http://hz.yj20258.top/gteuoexfag.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.sufxvd.cn/gtvhjhbded.html

[O06] 使用进程池
来源：http://hz.xylfe.cn/gtofwjmpiv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.316326.xyz/gtxclfezsr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.9152youxi.cn/gtrpquqtzv.html

JS:   // child_process / cluster 模块
来源：http://hz.cucudq.cn/gtumfvkumh.html

TS:   // child_process / cluster 模块
来源：http://hz.redwolf501.top/gtsywgxmvd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yueranfly.top/gtgpibxbxt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nanxinkj.top/gtpkxjvtrm.html

Ruby: // fork 块
来源：http://hz.jinqigfzy.top/gtjfkoliub.html

C#:   Parallel.For
来源：http://hz.pycfn.com/gtubrsdvps.html

================================================================================
来源：http://hz.andypj.xyz/gtaunchuxa.html

P. 常用工具函数
来源：http://hz.hfpthk.cn/gtjqmygxdc.html

================================================================================
来源：http://hz.cheryme.top/gtonufiyup.html

[P01] 生成 UUID
来源：http://hz.ydzc1.top/gtnyrajfhn.html

Py:   str(uuid.uuid4())
来源：http://hz.pycfn.com/gttpcyemci.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhengqikj.top/gtdmjouhcw.html

JS:   crypto.randomUUID()
来源：http://hz.yj20258.top/gthxtvrcom.html

TS:   crypto.randomUUID()
来源：http://hz.jqgfzy.top/gtsfemquby.html

Java: UUID.randomUUID().toString()
来源：http://hz.jlsjyb.cn/gtayuriqit.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hysaishi.cn/gtbezpywip.html

Ruby: SecureRandom.uuid
来源：http://hz.yuxming.cn/gtlxqhavxe.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.birdmap.top/gtqevayiuc.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yvedp.cn/gtxwitijmt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenzaomai.com/gtoiranrjt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.316326.xyz/gtrfozyihi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hfpthk.cn/gtkxzcmduo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.feifeiyinyue.top/gtskyfpxot.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.daxiang520.top/gtmjipzvji.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.chenzaomai.com/gtwulofpef.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.nanxuanxn.top/gtgzqoqclu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.tian-w.cn/gtxurcowso.html

[P03] 生成短随机字符串
来源：http://hz.ydzc1.top/gtzqwpfvec.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.birdmap.top/gtleepzdpf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cucudq.cn/gtpfzzvgav.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hammf.cn/gtmejppvdt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yonumen.top/gtsgeqhxoo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.wangshuangyany.cn/gtkzspxpas.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.9152youxi.cn/gtnsdlajwz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ppjwa.cn/gtnupwjczi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hongshengwenyu.top/gtnrznntgm.html

[P04] 求长度
来源：http://hz.daxiang520.top/gttwwkvaeh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hnqzz.top/gtnrkuosvf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gogol.net.cn/gtpunjqfge.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnxiangtu.top/gtibrjxaii.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.andypj.xyz/gtqyghbram.html


<!-- 参考信息 -->