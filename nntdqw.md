代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hysaishi.cn/gtdaerbifn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hongshengwenyu.top/gtfgnzzurs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shanyushiyangtech.top/gtqyplugjb.html

[L06] 解析响应为 JSON
来源：http://hz.ehwqpu.com/gtgfmzckxd.html

Py:   resp.json()
来源：http://hz.fengsongda.top/gtxwfupobp.html

PHP:  json_decode($body, true);
来源：http://hz.yongpay.top/gtmwmxgope.html

JS:   await resp.json()
来源：http://hz.ivvv.top/gtjpalgeub.html

TS:   await resp.json()
来源：http://hz.shanyushiyangtech.top/gtlngossbm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hywenlv.cn/gtxiteuibd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yj20258888.top/gtbetvlolg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xylfe.cn/gtraahlxei.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jqgufenzy.top/gtuzhzmikm.html

[L07] 处理 HTTP 状态码
来源：http://hz.redwolf501.top/gtcvxjwyyc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sweek.top/gtqdegrlsz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yonumen.top/gtwrspfgra.html

JS:   resp.ok;  resp.status
来源：http://hz.zhiwuduotai.top/gtiocreivv.html

TS:   resp.ok;  resp.status
来源：http://hz.hywenlv.cn/gtymbtzgbk.html

Java: resp.statusCode()
来源：http://hz.yj20258888.top/gtwsrvjxal.html

Go:   resp.StatusCode
来源：http://hz.cheryme.top/gtynujmcow.html

Ruby: resp.code.to_i
来源：http://hz.sxryk.cn/gtxnzfxgro.html

C#:   (int)resp.StatusCode
来源：http://hz.havefunace.top/gtfzfumxsq.html

[L08] 并发请求多个地址
来源：http://hz.sweek.top/gtzvqmfwjw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.bjfxy.top/gteygtviem.html

PHP:  curl_multi_init() 系列
来源：http://hz.chenjidiqi.icu/gtkmikixky.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydzc1.top/gtnddxfsrj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.bjfxy.top/gtswragqma.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xuanzx.com/gttxfeojvr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hnxiangtu.top/gthnzvxgka.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hfpthk.cn/gtytrvzmaa.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sxryk.cn/gtlpxaikpg.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtgxcjbwjh.html

M. 命令行 / 进程 / 环境
来源：http://hz.chenzaomai.com/gtibkmjqrz.html

================================================================================
来源：http://hz.gaohongyu789.top/gtzqabgufc.html

[M01] 读取命令行参数
来源：http://hz.smart0.xyz/gtwzsqpgbm.html

Py:   sys.argv[1:]
来源：http://hz.svipenyu.cn/gtibjaqhun.html

PHP:  $argv;  $argc;
来源：http://hz.yongpay.top/gtlnzsiseq.html

JS:   process.argv.slice(2)
来源：http://hz.ydzc1.top/gtdewtedbx.html

TS:   process.argv.slice(2)
来源：http://hz.daxiang520.top/gtwdfdqytv.html

Java: args 数组（main 方法参数）
来源：http://hz.zhijiandao.cn/gtlobkulzn.html

Go:   os.Args[1:]
来源：http://hz.iojbl.cn/gtgolxsllq.html

Ruby: ARGV
来源：http://hz.yueranfly.top/gtiwotnwcy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ppjwa.cn/gttcoxtdlc.html

[M02] 读取环境变量
来源：http://hz.aibaodan.cn/gtpilpexjc.html

Py:   os.environ.get("HOME")
来源：http://hz.guannengcc.top/gtttirtmmg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.tanke756.top/gtqlojlzmi.html

JS:   process.env.HOME
来源：http://hz.redwolf501.top/gtfpqexbjy.html

TS:   process.env.HOME
来源：http://hz.dashuyun.cn/gtemfxgvug.html

Java: System.getenv("HOME")
来源：http://hz.9152youxi.cn/gttojvafxy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.0kj1m.cn/gthtagmhnw.html

Ruby: ENV["HOME"]
来源：http://hz.cheryme.top/gtebrfjohb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.nanxuanxn.top/gtbzvbuzqz.html

[M03] 执行外部命令
来源：http://hz.9152youxi.cn/gthjuyzgps.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cheryme.top/gtzegsqdzd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhixingplan.top/gtkzjncrbl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xylfe.cn/gtovwycqvg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hammf.cn/gtuywruqbq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zycfv.cn/gtuoigjata.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tianlin.xyz/gtgiwopphg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xziqi.cn/gtzwxndbss.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ydzc1.top/gtyvbwfixv.html

[M04] 获取当前工作目录
来源：http://hz.52xcode.cn/gtbtnrnytl.html

Py:   os.getcwd()
来源：http://hz.guowangkeji.top/gtwupsojjv.html

PHP:  getcwd();
来源：http://hz.redwolf501.top/gtroveswxx.html

JS:   process.cwd()
来源：http://hz.tianlin.xyz/gtxgfgqhde.html

TS:   process.cwd()
来源：http://hz.chenjidiqi.icu/gthrxvmetk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yvedp.cn/gtgdqkqpaf.html

Go:   os.Getwd()
来源：http://hz.yangfankeji.com/gtpwgipgcv.html

Ruby: Dir.pwd
来源：http://hz.gotoacloud.top/gtpounfgoc.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.pycfn.com/gtfzwlbhsb.html

[M05] 设置退出码
来源：http://hz.jinyuanbaomall.cn/gtsmtykoyb.html

Py:   sys.exit(1)
来源：http://hz.bjfxy.top/gteskbdfnb.html

PHP:  exit(1);
来源：http://hz.hfpthk.cn/gtxhqzxkoy.html

JS:   process.exit(1)
来源：http://hz.yongpay.top/gtfreoctuo.html

TS:   process.exit(1)
来源：http://hz.feifeiyinyue.top/gtzqhsyglt.html

Java: System.exit(1)
来源：http://hz.9152youxi.cn/gtdlylarkj.html

Go:   os.Exit(1)
来源：http://hz.kuanghao11.cn/gtusrqxwvd.html

Ruby: exit 1
来源：http://hz.dianchejie.cn/gtewuruiav.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yanxiufei.cn/gtffjtgchm.html

[M06] 向标准错误输出
来源：http://hz.52xcode.cn/gtndpvalvf.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cashguo.top/gtbtsopygw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.nanxuanxn.top/gttmcglszc.html

JS:   console.error("err")
来源：http://hz.jyoumei.cn/gtnfxhmvot.html

TS:   console.error("err")
来源：http://hz.zhaomingkeji.xyz/gtksuwepef.html

Java: System.err.println("err")
来源：http://hz.jinqigufen.top/gtfesegtga.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.iojbl.cn/gtptnbzchf.html

Ruby: warn "err"
来源：http://hz.mhx1999.top/gtscrocjlb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cdnleiting.top/gtdgmsdccx.html

[M07] 判断是否为主入口
来源：http://hz.bjfxy.top/gtkvvqfwce.html

Py:   if __name__ == "__main__":
来源：http://hz.aizwys.cn/gtfpqjmnum.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhaomingkeji.xyz/gtwpqgslrk.html

JS:   require.main === module
来源：http://hz.yueranfly.top/gttcterbpz.html

TS:   require.main === module
来源：http://hz.sweek.top/gtnliwibet.html

Java: public static void main(String[] args)
来源：http://hz.iojbl.cn/gtgnxwatzl.html

Go:   func main()
来源：http://hz.shzxlz.cn/gtykpfmxru.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.fzhhl.top/gtjvqdvyxl.html

C#:   static void Main(string[] args)
来源：http://hz.redwolf501.top/gtryvdbprn.html

[M08] 获取系统与运行时信息
来源：http://hz.gogol.net.cn/gtlorcndtc.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yvedp.cn/gtnmwgzvol.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yuxming.cn/gtctolhlgg.html

JS:   process.platform;  process.version
来源：http://hz.jyoumei.cn/gtpaqbuzee.html

TS:   process.platform;  process.version
来源：http://hz.vqdsnc.cn/gtlaxmlkix.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.dashuyun.cn/gtwjfzkruj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.svipenyu.cn/gttcwswxnr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shuidangran.top/gtqojfwrux.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xingfuxueyuan.xyz/gtiapmecci.html

================================================================================
来源：http://hz.sxryk.cn/gtzdraufym.html

N. 数据结构与算法
来源：http://hz.cucudq.cn/gtugydawtk.html

================================================================================
来源：http://hz.hnqzz.top/gtruhiwubq.html

[N01] 二分查找（有序数组）
来源：http://hz.gogol.net.cn/gtwadptrqe.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yanxiufei.cn/gtznnnlgse.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hfpthk.cn/gtmrzvznmz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gzhubu.top/gtrdclwnpo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.haohaochexian.top/gtzcpqrqdv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenzaomai.com/gtjzohptlm.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shuidangran.top/gtkjgzwlxr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.fengsongda.top/gtcshuyhlj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.wangshuangyany.cn/gtknodvsar.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.52xcode.cn/gtxbkvnlvz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.snrcjt.cn/gtwkpevidh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jyoumei.cn/gtgddhwebg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zycfv.cn/gthwyymyqr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yvedp.cn/gtlrhcbaoy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhoulong.xyz/gtmxfeemex.html

Go:   slices.Sort(arr)
来源：http://hz.yj202588.top/gtjtflfcpo.html

Ruby: arr.sort
来源：http://hz.jlsjyb.cn/gtpowatcef.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.0kj1m.cn/gtpmwwlepd.html

[N03] 快速排序（分治示例）
来源：http://hz.yueranfly.top/gtzyqgixbo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.wangdashe.top/gtijkossne.html

PHP:  // 递归实现，或用 usort
来源：http://hz.svipenyu.cn/gtloiyuxsd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ybcxt.top/gtngpbfjng.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aizwys.cn/gtcaacsmrk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj20258888.top/gtfldpejrt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinghuilouyu.cn/gtnysocvjh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cqqwz.cn/gtjzyotfpb.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.redwolf501.top/gtwicswymc.html

[N04] 斐波那契数列
来源：http://hz.birdmap.top/gtwqkrvxfw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tian-w.cn/gtrzdeskfm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shzxlz.cn/gtfpbikhye.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.52xcode.cn/gtvdftsnzk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ybcxt.top/gtyaxbsoor.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xuanzx.com/gtfcnpzhct.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.pycfn.com/gtfhtqaczc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cashguo.top/gtufjspsvj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gtkzuefxyv.html

[N05] 最大公约数
来源：http://hz.pycfn.com/gttgxvkbmm.html

Py:   math.gcd(a, b)
来源：http://hz.jyoumei.cn/gtlhfehipo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hnxiangtu.top/gtiewivcsx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aizwys.cn/gtatjpszcx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ybcxt.top/gtgrskbela.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yj20258.top/gtqrpplevc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hnxiangtu.top/gtxqtuyond.html

Ruby: a.gcd(b)
来源：http://hz.ydjk.org.cn/gtxsnezzst.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.fzhhl.top/gtmkmsbpyq.html

[N06] 判断回文字符串
来源：http://hz.aizwys.cn/gtqtjphtgh.html

Py:   s == s[::-1]
来源：http://hz.yj202588.top/gtulihftdi.html

PHP:  $s === strrev($s);
来源：http://hz.yj20258888.top/gtaoffsngy.html

JS:   s === [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtovvwgcle.html

TS:   s === [...s].reverse().join("")
来源：http://hz.meibo888.top/gthplspwjc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xylfe.cn/gtmndmyqdx.html

Go:   // 双指针从两端比较
来源：http://hz.yanxiufei.cn/gtphxjfuap.html

Ruby: s == s.reverse
来源：http://hz.yvedp.cn/gtugquyxzf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.guowangkeji.top/gtmofxhlqa.html

[N07] 两数之和（返回下标）
来源：http://hz.jyoumei.cn/gtaoikbvgk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.haohaochexian.top/gteruypboi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zdqjudy.top/gtujdjcadf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jqgufenzy.top/gtwaozhqin.html

TS:   // 手写 Map<string, number>
来源：http://hz.dashuyun.cn/gtimbyodhl.html

Java: // 手写 HashMap
来源：http://hz.snrcjt.cn/gtovbyplei.html

Go:   // 手写 map[int]int
来源：http://hz.svipenyu.cn/gtrmveegxo.html

Ruby: // 手写 Hash
来源：http://hz.snrcjt.cn/gtooybovwm.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yongpay.top/gtpoctblkj.html

[N08] 生成全排列
来源：http://hz.jinqigufen.top/gtywbkehea.html

Py:   itertools.permutations(arr)
来源：http://hz.yonumen.top/gtiqonepsg.html

PHP:  // 手写递归交换
来源：http://hz.jqgfzy.top/gtnzkgxezj.html

JS:   // 手写回溯递归
来源：http://hz.yuxming.cn/gtrfpuvpbc.html

TS:   // 手写回溯递归
来源：http://hz.birdmap.top/gtmssordyq.html

Java: // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtmemeimiq.html

Go:   // 手写回溯递归
来源：http://hz.hammf.cn/gtwplxldcf.html

Ruby: arr.permutation.to_a
来源：http://hz.yueranfly.top/gtceyntudc.html

C#:   // 手写回溯递归
来源：http://hz.hfpthk.cn/gthkneyfqe.html

[N09] 栈与队列
来源：http://hz.52xcode.cn/gtqsferhgf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.daxiang520.top/gtjfrrfxkz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.nanxuanxn.top/gtcuixoneb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yangfankeji.com/gtdjchlnzc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhongyouzk.top/gtyvoeyyhc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhaomingkeji.xyz/gtfsthkrzd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhiwuduotai.top/gtatwklfyt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.quarkkingdee.top/gtqsarcfgb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xuanzx.com/gtfgsgkzts.html

[N10] 链表节点定义
来源：http://hz.aizwys.cn/gtjnomssws.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.dianchejie.cn/gtuadmptvx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hongshengwenyu.top/gtsamqgfvn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cucudq.cn/gtttasagkb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sweek.top/gtsaylylbq.html

Java: class Node { int v; Node next; }
来源：http://hz.iojbl.cn/gtvyrvozir.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gogol.net.cn/gtlqkzjrrw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sysykeji.top/gtohzgknsn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhijiandao.cn/gttaqvuazd.html

[N11] 二叉树中序遍历
来源：http://hz.jianghu66.top/gtbkyynzfs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shangyingyoupin.top/gtndvgeodh.html

PHP:  // 手写递归函数
来源：http://hz.havefunace.top/gtymzekwlf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.vqdsnc.cn/gtpfgoowfu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sysykeji.top/gttpalsrmb.html

Java: // 手写递归
来源：http://hz.zhengqikj.top/gtogvhbldj.html

Go:   // 手写递归
来源：http://hz.ivvv.top/gtisbuukqr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jinqigfzy.top/gtjyjslnzb.html

C#:   // 手写递归
来源：http://hz.0kj1m.cn/gtbmtazgkq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hnqzz.top/gterembznk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenzaomai.com/gtyvpdfyjn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.quarkkingdee.top/gtqihyzzvx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yvedp.cn/gtucpjfkuv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.bjfxy.top/gtuvnevxez.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yvedp.cn/gtvkembfmr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.meibo888.top/gtcwmncqam.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.fzhhl.top/gtlhetoqfo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.aibaodan.cn/gtnsakzivj.html

================================================================================
来源：http://hz.feifeiyinyue.top/gttknrnhmu.html

O. 并发与异步
来源：http://hz.kuanghao11.cn/gtipbxfgii.html

================================================================================
来源：http://hz.chenlongwang.top/gtjcdrlstt.html

[O01] 启动一个线程
来源：http://hz.xylfe.cn/gtlgexrjhy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.bjfxy.top/gtmbmjqoxz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.bjfxy.top/gtqgzbrflc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.sufxvd.cn/gtqbdyhuhz.html

TS:   // 同 JS
来源：http://hz.cdnleiting.top/gtcxifzube.html

Java: new Thread(() -> f()).start()
来源：http://hz.cashguo.top/gtwzfxappi.html

Go:   go f()
来源：http://hz.ywan-chungtsiang.top/gtybxkqdss.html

Ruby: Thread.new { f }
来源：http://hz.jianghu66.top/gtnpktrkjb.html

C#:   Task.Run(() => F());
来源：http://hz.xuetiantiany.cn/gtkgafgnwr.html

[O02] 使用线程池
来源：http://hz.shangyingyoupin.top/gtjanumlii.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.316326.xyz/gtbpjhvhys.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.aizwys.cn/gttvecorxv.html

JS:   // worker_threads 线程池
来源：http://hz.tianlin.xyz/gtgyuofjuu.html

TS:   // worker_threads 线程池
来源：http://hz.sweek.top/gthmhdxjfd.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shanyushiyangkeji.top/gtbbxilgmc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xingfuxueyuan.xyz/gtwbklmikj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yuxming.cn/gtpfbmxzpg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shzxlz.cn/gtyqazonbv.html

[O03] 加锁保护共享数据
来源：http://hz.yueranfly.top/gtrmufqool.html

Py:   with lock: shared += 1
来源：http://hz.ybcxt.top/gtsoimzyzm.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.haohaochexian.top/gtkutfdxxy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.sufxvd.cn/gtdbkvjoax.html

TS:   // 同 JS
来源：http://hz.zhengqikj.top/gtmjyanwki.html

Java: synchronized (this) { shared++; }
来源：http://hz.hnqzz.top/gtybyomlyr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.daxiang520.top/gtrrlywizs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shuidangran.top/gtemhtvxqf.html

C#:   lock (gate) { shared++; }
来源：http://hz.yuxming.cn/gtpnzyrgrv.html

[O04] 定义异步函数并等待
来源：http://hz.kuanghao11.cn/gtxsrppetw.html

Py:   async def f():⏎    await g()
来源：http://hz.cashguo.top/gtfjonabes.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.chenlongwang.top/gtyezxzaeb.html

JS:   async function f() { await g(); }
来源：http://hz.9152youxi.cn/gtankphmlm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jyoumei.cn/gtysxkxefj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.daxiang520.top/gtfrimggbv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.smart0.xyz/gtnsalrhjl.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yvedp.cn/gtuplchswp.html

C#:   async Task F() { await G(); }
来源：http://hz.yuanzhike.top/gtedwresqf.html

[O05] 并发执行并等待全部完成
来源：http://hz.pengpengdd.cyou/gtsnhwuxer.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhaomingkeji.xyz/gthuqqgaaw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhoulong.xyz/gtujwanhsq.html

JS:   await Promise.all(tasks)
来源：http://hz.yvedp.cn/gtukeufqxz.html

TS:   await Promise.all(tasks)
来源：http://hz.hywenlv.cn/gtglsdgydx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.fengsongda.top/gtolrtmlwj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yonumen.top/gtwhvvjceb.html

Ruby: threads.map(&:join)
来源：http://hz.guowangkeji.top/gtdhbrcegp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jyoumei.cn/gtajqlwefp.html

[O06] 使用进程池
来源：http://hz.ehwqpu.com/gtifivutsc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.0kj1m.cn/gtbrecvnml.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xuetiantiany.cn/gtvaibusyi.html

JS:   // child_process / cluster 模块
来源：http://hz.jinqigufen.top/gtsarswiuz.html

TS:   // child_process / cluster 模块
来源：http://hz.jqgufenzy.top/gtvkxdrseu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xuetiantiany.cn/gtfpxymuhh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ydzc1.top/gtbukohgsq.html

Ruby: // fork 块
来源：http://hz.chenlongwang.top/gtvoqbmexn.html

C#:   Parallel.For
来源：http://hz.gotoacloud.top/gtleiswjga.html

================================================================================
来源：http://hz.yanxiufei.cn/gtqfghvfuk.html

P. 常用工具函数
来源：http://hz.meibo888.top/gthphcytbp.html

================================================================================
来源：http://hz.yueranfly.top/gtjsmorily.html

[P01] 生成 UUID
来源：http://hz.jyoumei.cn/gtdwfhzwyy.html

Py:   str(uuid.uuid4())
来源：http://hz.ehwqpu.com/gttcppghpr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zdqjudy.top/gtbyzylmis.html

JS:   crypto.randomUUID()
来源：http://hz.cashguo.top/gtkjacllna.html

TS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gteffblgbn.html

Java: UUID.randomUUID().toString()
来源：http://hz.xinyue.icu/gtdxvkpxex.html

Go:   // 用 github.com/google/uuid
来源：http://hz.nwbrower.top/gtxjwnaixv.html

Ruby: SecureRandom.uuid
来源：http://hz.xylfe.cn/gtatajntbp.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.snrcjt.cn/gtiopamkui.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hnqzz.top/gtgwbonafg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jlsjyb.cn/gtfoltsjkg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinyuanbaomall.cn/gtzzwmsvql.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jiagoushi.top/gtnvfqnsrl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hammf.cn/gtxsczwmjv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.svipenyu.cn/gtoyfzhgdu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhijiandao.cn/gtoddmhvud.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jlsjyb.cn/gtivvvnriq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.gaohongyu789.top/gthhzamakk.html

[P03] 生成短随机字符串
来源：http://hz.zhixingplan.top/gtddmhfpvm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jqgufenzy.top/gtnxyaxtkr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.dashuyun.cn/gtkijuyhvz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hysaishi.cn/gtletuimem.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.0kj1m.cn/gtwtydnuxn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yongpay.top/gtjqhiwqzk.html


<!-- 参考信息 -->