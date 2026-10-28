代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yanxiufei.cn/gtjtildzmd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinqigufen.top/gtfbgemtkj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.52xcode.cn/gtrpvzkeyz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.bjfxy.top/gtwdipmhag.html

[L07] 处理 HTTP 状态码
来源：http://hz.jqgfzy.top/gtulxthcxi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yuxming.cn/gtlzcrzjqd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinghuilouyu.cn/gtmwplbcfe.html

JS:   resp.ok;  resp.status
来源：http://hz.52xcode.cn/gthjeubuhr.html

TS:   resp.ok;  resp.status
来源：http://hz.xuanzx.com/gtmvhbzmdd.html

Java: resp.statusCode()
来源：http://hz.zhaomingkeji.xyz/gtevlaqwgx.html

Go:   resp.StatusCode
来源：http://hz.jinqigufen.top/gtvcqpaige.html

Ruby: resp.code.to_i
来源：http://hz.ppjwa.cn/gthwyjqdpg.html

C#:   (int)resp.StatusCode
来源：http://hz.hammf.cn/gtxfaucwpv.html

[L08] 并发请求多个地址
来源：http://hz.ehwqpu.com/gtqqroefcb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.dianchejie.cn/gtgioeyivz.html

PHP:  curl_multi_init() 系列
来源：http://hz.hnqzz.top/gtheopdaud.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dianchejie.cn/gtorxvwrhr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gtdnbawyvx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xylfe.cn/gtfhocafds.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.mhx1999.top/gtjnbbxflu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhaomingkeji.xyz/gtbnfnxokm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cqqwz.cn/gtuenfvvrv.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtmxtwxylg.html

M. 命令行 / 进程 / 环境
来源：http://hz.nanxinkj.top/gtmjhaptzd.html

================================================================================
来源：http://hz.ehwqpu.com/gtbsfenfpy.html

[M01] 读取命令行参数
来源：http://hz.snrcjt.cn/gtyskzcddl.html

Py:   sys.argv[1:]
来源：http://hz.xylfe.cn/gtdcbfdwvh.html

PHP:  $argv;  $argc;
来源：http://hz.zdqjudy.top/gtigzoqepc.html

JS:   process.argv.slice(2)
来源：http://hz.316326.xyz/gtjoygkdil.html

TS:   process.argv.slice(2)
来源：http://hz.yangfankeji.com/gtzqpvvpku.html

Java: args 数组（main 方法参数）
来源：http://hz.jqgfzy.top/gtezzevytu.html

Go:   os.Args[1:]
来源：http://hz.zhongyouzk.top/gtzciawwxc.html

Ruby: ARGV
来源：http://hz.havefunace.top/gtqkpovumc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shanyushiyangtech.top/gtrhxnlbdo.html

[M02] 读取环境变量
来源：http://hz.vqdsnc.cn/gtkxcgjbzy.html

Py:   os.environ.get("HOME")
来源：http://hz.haohaochexian.top/gtrmsipkgm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.pengpengdd.cyou/gtclbzgruu.html

JS:   process.env.HOME
来源：http://hz.tanke756.top/gtdxrpkyey.html

TS:   process.env.HOME
来源：http://hz.bjfxy.top/gtkxfayaes.html

Java: System.getenv("HOME")
来源：http://hz.fzhhl.top/gtqrmzmjip.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.kuanghao11.cn/gtyvayveui.html

Ruby: ENV["HOME"]
来源：http://hz.yongpay.top/gtlfgtgery.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ybcxt.top/gtulpxuyad.html

[M03] 执行外部命令
来源：http://hz.zhijiandao.cn/gtfjyjkdqa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.wangdashe.top/gtcrynftwv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinqigufen.top/gthxcxzlsi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.redwolf501.top/gtorqmupfk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.dianchejie.cn/gtcuhsscjv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.nwbrower.top/gtwgzdshmi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.aizwys.cn/gthsuuyncc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.iojbl.cn/gtmqtutcty.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ydjk.org.cn/gtwcemsldq.html

[M04] 获取当前工作目录
来源：http://hz.sysykeji.top/gtbgwyoxfb.html

Py:   os.getcwd()
来源：http://hz.yangfankeji.com/gtjafcdqlt.html

PHP:  getcwd();
来源：http://hz.yj20258.top/gtorsfvlpp.html

JS:   process.cwd()
来源：http://hz.shuidangran.top/gtpyjhhgah.html

TS:   process.cwd()
来源：http://hz.nwbrower.top/gtpkvwduyk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.wangshuangyany.cn/gtywtcghjc.html

Go:   os.Getwd()
来源：http://hz.gogol.net.cn/gthshoapqv.html

Ruby: Dir.pwd
来源：http://hz.tanke756.top/gtborylxdg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.tian-w.cn/gthchnomin.html

[M05] 设置退出码
来源：http://hz.nanxinkj.top/gtkmktxdru.html

Py:   sys.exit(1)
来源：http://hz.ydjk.org.cn/gtyrkvfotp.html

PHP:  exit(1);
来源：http://hz.xinyue.icu/gtogtinnbx.html

JS:   process.exit(1)
来源：http://hz.yj20258888.top/gtvhjkalsy.html

TS:   process.exit(1)
来源：http://hz.zhaomingkeji.xyz/gtlqwgazxc.html

Java: System.exit(1)
来源：http://hz.hammf.cn/gtgyyupbak.html

Go:   os.Exit(1)
来源：http://hz.guowangkeji.top/gtifyqspur.html

Ruby: exit 1
来源：http://hz.cheryme.top/gtblplwcyr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hywenlv.cn/gtgahjprmn.html

[M06] 向标准错误输出
来源：http://hz.hnqzz.top/gtcketplzo.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nanxuanxn.top/gtnphmnxox.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.nanxuanxn.top/gtsnfpyqta.html

JS:   console.error("err")
来源：http://hz.52xcode.cn/gtnzyhekkw.html

TS:   console.error("err")
来源：http://hz.cucudq.cn/gtpyxrcwpm.html

Java: System.err.println("err")
来源：http://hz.xingfuxueyuan.xyz/gtsqtklzpa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.c1oappe.top/gtghrpizon.html

Ruby: warn "err"
来源：http://hz.cheryme.top/gtsnljygsa.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.gogol.net.cn/gtkmbcrula.html

[M07] 判断是否为主入口
来源：http://hz.zhijiandao.cn/gtkuqcgunn.html

Py:   if __name__ == "__main__":
来源：http://hz.jyoumei.cn/gtuunwcfso.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinqigfzy.top/gttuhsudyn.html

JS:   require.main === module
来源：http://hz.hammf.cn/gtugkfrnbn.html

TS:   require.main === module
来源：http://hz.shzxlz.cn/gtiqkbrpyx.html

Java: public static void main(String[] args)
来源：http://hz.bjfxy.top/gtecxoiios.html

Go:   func main()
来源：http://hz.yj20258888.top/gtcooohxwd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.nwbrower.top/gtjwvlahql.html

C#:   static void Main(string[] args)
来源：http://hz.quarkkingdee.top/gtjqzwbafz.html

[M08] 获取系统与运行时信息
来源：http://hz.c1oappe.top/gtnhupdziq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhoulong.xyz/gtcbchrtji.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.quarkkingdee.top/gtlxqgdgbt.html

JS:   process.platform;  process.version
来源：http://hz.yj20258.top/gtjxawnqyx.html

TS:   process.platform;  process.version
来源：http://hz.svipenyu.cn/gtlqizqwls.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ehwqpu.com/gtlydniudv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xuetiantiany.cn/gtgvciumfi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ybcxt.top/gtkkbxwyxy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xuetiantiany.cn/gtlivxrckq.html

================================================================================
来源：http://hz.havefunace.top/gtgzepeksa.html

N. 数据结构与算法
来源：http://hz.snrcjt.cn/gtyfwmvghf.html

================================================================================
来源：http://hz.mhx1999.top/gtgsmopnbm.html

[N01] 二分查找（有序数组）
来源：http://hz.nanxuanxn.top/gtuhfygidr.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.birdmap.top/gtqyqfhtxb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ivvv.top/gtmueyofym.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sweek.top/gtzrsagyrt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.c1oappe.top/gtghlspxyw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.sufxvd.cn/gtzcthiogk.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.wangshuangyany.cn/gtalxrtdxf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hnxiangtu.top/gtjwqfdeyv.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.guowangkeji.top/gtinsoprxr.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ydzc1.top/gtekgevhrq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sufxvd.cn/gtnfhklrxy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.guannengcc.top/gtqyvaqbdw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tanke756.top/gtokqgeoox.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuanzhike.top/gtjzwfcrai.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.gogol.net.cn/gtoanyzadw.html

Go:   slices.Sort(arr)
来源：http://hz.ydzc1.top/gtdcneydff.html

Ruby: arr.sort
来源：http://hz.aibaodan.cn/gtggyoapnl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ivvv.top/gtbnxumnvr.html

[N03] 快速排序（分治示例）
来源：http://hz.xingfuxueyuan.xyz/gtcqlwhcxz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hammf.cn/gtdtgwpkma.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xuetiantiany.cn/gtmcwgfwyn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.52xcode.cn/gtnxbdezih.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pycfn.com/gtlpznxlcm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinghuilouyu.cn/gtefkjxlky.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zycfv.cn/gtrfkfcuuc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhijiandao.cn/gtzxihrdso.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.316326.xyz/gtoubbgbmn.html

[N04] 斐波那契数列
来源：http://hz.bjfxy.top/gtwosmexlo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sysykeji.top/gtmfujakyj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhiwuduotai.top/gtfngclefn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fengsongda.top/gtkrctrhdb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jqgufenzy.top/gtqsmhufkw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xinyue.icu/gtrpnniups.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hnxiangtu.top/gtmihsuliu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.mhx1999.top/gtahitgayd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gtqebppndx.html

[N05] 最大公约数
来源：http://hz.iojbl.cn/gtbjzpxlrg.html

Py:   math.gcd(a, b)
来源：http://hz.zhoulong.xyz/gtfrbczptq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.dianchejie.cn/gtnxwbismy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhixingplan.top/gtdmwrbqdn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gtkgprmcfh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhiwuduotai.top/gtmibjmkax.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhengqikj.top/gtbyulwixm.html

Ruby: a.gcd(b)
来源：http://hz.vqdsnc.cn/gtdaxulylz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jlsjyb.cn/gtydryfqxk.html

[N06] 判断回文字符串
来源：http://hz.shangyingyoupin.top/gttzwqkbcj.html

Py:   s == s[::-1]
来源：http://hz.chenjidiqi.icu/gtaesyfprv.html

PHP:  $s === strrev($s);
来源：http://hz.nwbrower.top/gtauaixwrl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtdjhtixnx.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtwpfzlxuk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shuidangran.top/gtonvdqrde.html

Go:   // 双指针从两端比较
来源：http://hz.jinqigufen.top/gtwymlctet.html

Ruby: s == s.reverse
来源：http://hz.c1oappe.top/gtpycklfin.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ybcxt.top/gtuxgyxhpp.html

[N07] 两数之和（返回下标）
来源：http://hz.sxryk.cn/gttrigsgyz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.guowangkeji.top/gtvmrilbsa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.fengsongda.top/gthoqcffqm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xuanzx.com/gtxotwsknk.html

TS:   // 手写 Map<string, number>
来源：http://hz.yonumen.top/gtywsffjxv.html

Java: // 手写 HashMap
来源：http://hz.52xcode.cn/gtqtizcaic.html

Go:   // 手写 map[int]int
来源：http://hz.sxryk.cn/gthmrqobte.html

Ruby: // 手写 Hash
来源：http://hz.nanxuanxn.top/gtunyndtlc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhoulong.xyz/gthqmoobmj.html

[N08] 生成全排列
来源：http://hz.xziqi.cn/gtgupdwnna.html

Py:   itertools.permutations(arr)
来源：http://hz.jinyuanbaomall.cn/gtwqqujqox.html

PHP:  // 手写递归交换
来源：http://hz.nanxinkj.top/gtzbtoeuwi.html

JS:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtajglhuve.html

TS:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtvhrdkkfa.html

Java: // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtuwdgnmxc.html

Go:   // 手写回溯递归
来源：http://hz.ybcxt.top/gtxqrkadhs.html

Ruby: arr.permutation.to_a
来源：http://hz.jyoumei.cn/gtspefsnct.html

C#:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gttvusxoxy.html

[N09] 栈与队列
来源：http://hz.zdqjudy.top/gtztxasfud.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ppjwa.cn/gtndjvmojr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hammf.cn/gtdfjungks.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jqgufenzy.top/gtgyjbsqeb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.guowangkeji.top/gtejqjgmew.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhengqikj.top/gtedrwaufz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xinyue.icu/gtdrwliwfh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jinghuilouyu.cn/gtbxebqlcy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xziqi.cn/gtyzgjiwrn.html

[N10] 链表节点定义
来源：http://hz.cqqwz.cn/gtkrsrxtom.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gaohongyu789.top/gtofcougzy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shanyushiyangkeji.top/gthfqsatwg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xingfuxueyuan.xyz/gthdcboepp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.aizwys.cn/gtywdluvek.html

Java: class Node { int v; Node next; }
来源：http://hz.gzhubu.top/gtvcbvicea.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.fzhhl.top/gtdmwvjzlb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shzxlz.cn/gtjnstrvfb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ehwqpu.com/gtdwrgcgjo.html

[N11] 二叉树中序遍历
来源：http://hz.jyoumei.cn/gtbljknbou.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shuidangran.top/gtulzcotqo.html

PHP:  // 手写递归函数
来源：http://hz.ybcxt.top/gtqailgyzi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ywan-chungtsiang.top/gthdadzzpx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.kuanghao11.cn/gtashiyyaa.html

Java: // 手写递归
来源：http://hz.hfpthk.cn/gtlttzauay.html

Go:   // 手写递归
来源：http://hz.9152youxi.cn/gtwbcmdipx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.wangshuangyany.cn/gtcihzzcyf.html

C#:   // 手写递归
来源：http://hz.hysaishi.cn/gtjrhkzrhl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xuetiantiany.cn/gtyhqgzhrn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ywan-chungtsiang.top/gtjobvxlbb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.andypj.xyz/gtsmqnlgjy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shangyingyoupin.top/gtzzgbffcf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hfpthk.cn/gtqacptarp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yvedp.cn/gtadkbxwqm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.pycfn.com/gtvaqulqre.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.gogol.net.cn/gtwnpogifs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhiwuduotai.top/gtxxazxsjo.html

================================================================================
来源：http://hz.hfpthk.cn/gtapmotdhq.html

O. 并发与异步
来源：http://hz.gogol.net.cn/gtdkqntajj.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gttngxifim.html

[O01] 启动一个线程
来源：http://hz.nanxuanxn.top/gtqumlkita.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ywan-chungtsiang.top/gtgialrnow.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.dashuyun.cn/gtzioqefkb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.pycfn.com/gtfvvnnkix.html

TS:   // 同 JS
来源：http://hz.yuxming.cn/gtchoutmcx.html

Java: new Thread(() -> f()).start()
来源：http://hz.yanxiufei.cn/gtpkjpgokt.html

Go:   go f()
来源：http://hz.xziqi.cn/gtdtliqacj.html

Ruby: Thread.new { f }
来源：http://hz.zdqjudy.top/gtevzqmnho.html

C#:   Task.Run(() => F());
来源：http://hz.chenlongwang.top/gtvkvowpkf.html

[O02] 使用线程池
来源：http://hz.yueranfly.top/gtkbjshndh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shzxlz.cn/gtvwkvsauc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.dashuyun.cn/gtyofxnvjr.html

JS:   // worker_threads 线程池
来源：http://hz.svipenyu.cn/gtevfdkhjl.html

TS:   // worker_threads 线程池
来源：http://hz.vqdsnc.cn/gtolzhxsls.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hywenlv.cn/gtmvgjdilt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xuetiantiany.cn/gtqudzgrrs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.chenlongwang.top/gtykyadakh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.sysykeji.top/gtyjelbblj.html

[O03] 加锁保护共享数据
来源：http://hz.andypj.xyz/gtnqjcytxh.html

Py:   with lock: shared += 1
来源：http://hz.tian-w.cn/gtvsfvpmig.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.nanxuanxn.top/gthrrdkbds.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hammf.cn/gtyatiojwy.html

TS:   // 同 JS
来源：http://hz.dianchejie.cn/gtwvechiql.html

Java: synchronized (this) { shared++; }
来源：http://hz.sufxvd.cn/gtaehliuws.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jinghuilouyu.cn/gtzxansiyy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yvedp.cn/gtedyeqxzp.html

C#:   lock (gate) { shared++; }
来源：http://hz.yongpay.top/gtwwwsxjhm.html

[O04] 定义异步函数并等待
来源：http://hz.zhaomingkeji.xyz/gtkxhyfwox.html

Py:   async def f():⏎    await g()
来源：http://hz.tianlin.xyz/gtxemeoapx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jianghu66.top/gtogqxfdkk.html

JS:   async function f() { await g(); }
来源：http://hz.feifeiyinyue.top/gtloadyooa.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ivvv.top/gtpatewgjc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.0kj1m.cn/gtwfgtmdqn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.mhx1999.top/gtmybultwt.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gotoacloud.top/gtfpgceqkc.html

C#:   async Task F() { await G(); }
来源：http://hz.cheryme.top/gtxkpkxdry.html

[O05] 并发执行并等待全部完成
来源：http://hz.nanxinkj.top/gtyqufrdho.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cdnleiting.top/gtphqsalhf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gotoacloud.top/gtupmduglt.html

JS:   await Promise.all(tasks)
来源：http://hz.xuanzx.com/gtoxldrfqh.html

TS:   await Promise.all(tasks)
来源：http://hz.jlsjyb.cn/gtdxdnizbn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.aizwys.cn/gtdajmtutk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sufxvd.cn/gtbzgasdiy.html

Ruby: threads.map(&:join)
来源：http://hz.wangdashe.top/gtysegsxul.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.andypj.xyz/gtgfxhzadq.html

[O06] 使用进程池
来源：http://hz.c1oappe.top/gtccithybp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.havefunace.top/gtwlmnpisa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cucudq.cn/gtdewqakkv.html

JS:   // child_process / cluster 模块
来源：http://hz.tianlin.xyz/gtpyaaiprt.html

TS:   // child_process / cluster 模块
来源：http://hz.redwolf501.top/gttwrecjiw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.guowangkeji.top/gtbpoixrbk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.meibo888.top/gtxcgteuxj.html

Ruby: // fork 块
来源：http://hz.jinqigufen.top/gtfvkuifxo.html

C#:   Parallel.For
来源：http://hz.fengsongda.top/gtupmqkmoe.html

================================================================================
来源：http://hz.zhongyouzk.top/gtarssgved.html

P. 常用工具函数
来源：http://hz.ywan-chungtsiang.top/gtokutvytm.html

================================================================================
来源：http://hz.sweek.top/gtfhvihkbi.html

[P01] 生成 UUID
来源：http://hz.hongshengwenyu.top/gtuvekvbzg.html

Py:   str(uuid.uuid4())
来源：http://hz.shuidangran.top/gtuekmzwtl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xziqi.cn/gtjltbwvco.html

JS:   crypto.randomUUID()
来源：http://hz.yuxming.cn/gtimwnszyk.html

TS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtvfpkunyh.html

Java: UUID.randomUUID().toString()
来源：http://hz.jianghu66.top/gtgpmylubo.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jinqigfzy.top/gtjwdpuone.html

Ruby: SecureRandom.uuid
来源：http://hz.jinyuanbaomall.cn/gtsuvvydhm.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shuidangran.top/gtuqtwhmvn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yanxiufei.cn/gtbggjapwe.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gotoacloud.top/gtsmasebts.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.cucudq.cn/gtffswjuiw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shzxlz.cn/gtemlaxnqj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xingfuxueyuan.xyz/gtqtrvaqsb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.dianchejie.cn/gthpnmyicl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhaomingkeji.xyz/gtvumxnkid.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xziqi.cn/gteqxqjeas.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yanxiufei.cn/gtvljvbeux.html

[P03] 生成短随机字符串
来源：http://hz.guowangkeji.top/gtdlsrxtqc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ivvv.top/gtjsnkqkef.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shangyingyoupin.top/gttjzsuenv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenjidiqi.icu/gtwzdnfzpk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jlsjyb.cn/gtjoukfcfd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hywenlv.cn/gtigqsdmcm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.gotoacloud.top/gtgrczxbef.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhoulong.xyz/gttcdexwda.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.pycfn.com/gtgkbfrlzo.html

[P04] 求长度
来源：http://hz.cucudq.cn/gtqnftxdcr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gotoacloud.top/gtuukfudov.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuanzx.com/gtgygmqmwn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jyoumei.cn/gtnuzxcshz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jqgufenzy.top/gtmskjuqrw.html


<!-- 参考信息 -->