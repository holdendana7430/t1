代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.cashguo.top/gthhadrhxv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.tian-w.cn/gtvisfofsh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hammf.cn/gtkzaunwll.html

[L06] 解析响应为 JSON
来源：http://hz.jqgfzy.top/gtfoviyzhq.html

Py:   resp.json()
来源：http://hz.jinqigufen.top/gtwfgpqxdg.html

PHP:  json_decode($body, true);
来源：http://hz.tanke756.top/gtlvaqbibo.html

JS:   await resp.json()
来源：http://hz.zhixingplan.top/gtomkhxopi.html

TS:   await resp.json()
来源：http://hz.redwolf501.top/gtbanwrdox.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.andypj.xyz/gtfxlwgaoe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhoulong.xyz/gtdnguykih.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhixingplan.top/gtyvfxevmd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ydjk.org.cn/gtmfweogvn.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj20258888.top/gtythknyms.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.svipenyu.cn/gtmwjmloch.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.guowangkeji.top/gtiyocbifa.html

JS:   resp.ok;  resp.status
来源：http://hz.mhx1999.top/gtwkuohjuj.html

TS:   resp.ok;  resp.status
来源：http://hz.meibo888.top/gtfleunotz.html

Java: resp.statusCode()
来源：http://hz.zhoulong.xyz/gtudzjdoft.html

Go:   resp.StatusCode
来源：http://hz.316326.xyz/gtjfqndjli.html

Ruby: resp.code.to_i
来源：http://hz.yj202588.top/gttkmrnila.html

C#:   (int)resp.StatusCode
来源：http://hz.xylfe.cn/gtakqiloye.html

[L08] 并发请求多个地址
来源：http://hz.feifeiyinyue.top/gtqaoeivrz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xingfuxueyuan.xyz/gtxsjwyhsa.html

PHP:  curl_multi_init() 系列
来源：http://hz.aizwys.cn/gtjsihvvnr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgfzy.top/gtwndrfxmc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cheryme.top/gtcxntwqna.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.nwbrower.top/gtmjxkxiut.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yonumen.top/gtegixzkus.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yongpay.top/gtcdtgujyv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.smart0.xyz/gtpmvterwr.html

================================================================================
来源：http://hz.yuxming.cn/gtexkvtldf.html

M. 命令行 / 进程 / 环境
来源：http://hz.tianlin.xyz/gtlkzxysng.html

================================================================================
来源：http://hz.0kj1m.cn/gthblbtllf.html

[M01] 读取命令行参数
来源：http://hz.hywenlv.cn/gtoqvetodr.html

Py:   sys.argv[1:]
来源：http://hz.sweek.top/gtgsattvvy.html

PHP:  $argv;  $argc;
来源：http://hz.andypj.xyz/gtpubilcri.html

JS:   process.argv.slice(2)
来源：http://hz.jqgufenzy.top/gtbnhmuekg.html

TS:   process.argv.slice(2)
来源：http://hz.yvedp.cn/gtwarwjbrs.html

Java: args 数组（main 方法参数）
来源：http://hz.tian-w.cn/gtubyetygr.html

Go:   os.Args[1:]
来源：http://hz.hammf.cn/gtxcswlwik.html

Ruby: ARGV
来源：http://hz.jqgfzy.top/gtbjjivquy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shzxlz.cn/gtfbgzkoog.html

[M02] 读取环境变量
来源：http://hz.c1oappe.top/gtldyiycqy.html

Py:   os.environ.get("HOME")
来源：http://hz.nwbrower.top/gtkkkrklzw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ydjk.org.cn/gtgjtatoyr.html

JS:   process.env.HOME
来源：http://hz.cashguo.top/gtnomsfenz.html

TS:   process.env.HOME
来源：http://hz.hammf.cn/gtuniwebll.html

Java: System.getenv("HOME")
来源：http://hz.gotoacloud.top/gtveqsclmk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sxryk.cn/gtmdbawhhr.html

Ruby: ENV["HOME"]
来源：http://hz.xingfuxueyuan.xyz/gthvmeisdb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xuanzx.com/gtapuvxtqv.html

[M03] 执行外部命令
来源：http://hz.hongshengwenyu.top/gtjholwypl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gogol.net.cn/gtsyaxjgxt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ydjk.org.cn/gtpgycwtbw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.meibo888.top/gtkcylaalj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.svipenyu.cn/gtllrydgpp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jyoumei.cn/gtnodotkpg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cashguo.top/gthxtlmkit.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sweek.top/gtqdtctkjp.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hysaishi.cn/gtrxzoksiy.html

[M04] 获取当前工作目录
来源：http://hz.jqgufenzy.top/gtmvdxmmnk.html

Py:   os.getcwd()
来源：http://hz.9152youxi.cn/gtdhkeisfv.html

PHP:  getcwd();
来源：http://hz.chenlongwang.top/gttwasfehz.html

JS:   process.cwd()
来源：http://hz.zhijiandao.cn/gtugbmesws.html

TS:   process.cwd()
来源：http://hz.xuetiantiany.cn/gtokdjrsum.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhaomingkeji.xyz/gtekckqwsj.html

Go:   os.Getwd()
来源：http://hz.yueranfly.top/gtpprirpbo.html

Ruby: Dir.pwd
来源：http://hz.xziqi.cn/gtayuhhfsn.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ydjk.org.cn/gtszwxucew.html

[M05] 设置退出码
来源：http://hz.yj20258888.top/gtadribcao.html

Py:   sys.exit(1)
来源：http://hz.jinqigfzy.top/gthhqmvmxf.html

PHP:  exit(1);
来源：http://hz.dashuyun.cn/gtpbxpkrfc.html

JS:   process.exit(1)
来源：http://hz.0kj1m.cn/gthecacooc.html

TS:   process.exit(1)
来源：http://hz.smart0.xyz/gtmkweurry.html

Java: System.exit(1)
来源：http://hz.nwbrower.top/gtrbhatily.html

Go:   os.Exit(1)
来源：http://hz.yonumen.top/gtnatrvnmt.html

Ruby: exit 1
来源：http://hz.ehwqpu.com/gtrewvlskr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jqgfzy.top/gthwwvmpbp.html

[M06] 向标准错误输出
来源：http://hz.yangfankeji.com/gtdzceralp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shuidangran.top/gtrmppxilp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cucudq.cn/gtobhvtcwo.html

JS:   console.error("err")
来源：http://hz.0kj1m.cn/gtpxukdsob.html

TS:   console.error("err")
来源：http://hz.zhiwuduotai.top/gtkluxuhzr.html

Java: System.err.println("err")
来源：http://hz.yuxming.cn/gtldfkiuaw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jinqigfzy.top/gtodasauuz.html

Ruby: warn "err"
来源：http://hz.vqdsnc.cn/gtqnyvprfd.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.quarkkingdee.top/gtzwacxlow.html

[M07] 判断是否为主入口
来源：http://hz.aizwys.cn/gtgotlzfxw.html

Py:   if __name__ == "__main__":
来源：http://hz.jinqigufen.top/gtktwezbye.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.svipenyu.cn/gtdtzgrnsa.html

JS:   require.main === module
来源：http://hz.hongshengwenyu.top/gtfxqnqkeq.html

TS:   require.main === module
来源：http://hz.sufxvd.cn/gtboxfgaxo.html

Java: public static void main(String[] args)
来源：http://hz.ydzc1.top/gtxqxcovfk.html

Go:   func main()
来源：http://hz.guowangkeji.top/gtcxesmgrw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.birdmap.top/gtwhutlrzj.html

C#:   static void Main(string[] args)
来源：http://hz.mhx1999.top/gtlutqemiw.html

[M08] 获取系统与运行时信息
来源：http://hz.316326.xyz/gtplfjwsbd.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinghuilouyu.cn/gtpkjrxvfe.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cheryme.top/gtvfgnahtp.html

JS:   process.platform;  process.version
来源：http://hz.jianghu66.top/gtyarhjphp.html

TS:   process.platform;  process.version
来源：http://hz.yvedp.cn/gtoqkvoyla.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jiagoushi.top/gtpddghhnr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.redwolf501.top/gtoobyzawv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shanyushiyangkeji.top/gtrnevjghv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.bjfxy.top/gtoafswjvm.html

================================================================================
来源：http://hz.yanxiufei.cn/gtwwjwumia.html

N. 数据结构与算法
来源：http://hz.hfpthk.cn/gtvwudwjcc.html

================================================================================
来源：http://hz.xylfe.cn/gtxuexnile.html

[N01] 二分查找（有序数组）
来源：http://hz.fzhhl.top/gtljyrebpm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhoulong.xyz/gtvwlpfdgs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.redwolf501.top/gtwguluosj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.c1oappe.top/gtitniixef.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ehwqpu.com/gtugkxvxoy.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shuidangran.top/gtbfwznkgj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.wangshuangyany.cn/gtoxcvxwez.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jiagoushi.top/gtytsuspzz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.kuanghao11.cn/gterhqnyxu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.guannengcc.top/gtebrnveto.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangkeji.top/gtpznylngi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.svipenyu.cn/gtwuwyikxy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhijiandao.cn/gtsqmriloi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hysaishi.cn/gthshtwatp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jqgfzy.top/gtkmarihpc.html

Go:   slices.Sort(arr)
来源：http://hz.xylfe.cn/gtnohjvdzl.html

Ruby: arr.sort
来源：http://hz.iojbl.cn/gtlltilwbi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.quarkkingdee.top/gtmqzfcviz.html

[N03] 快速排序（分治示例）
来源：http://hz.hongshengwenyu.top/gtqjccisgx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinyuanbaomall.cn/gtgfjulays.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinqigufen.top/gtofcgklnn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guannengcc.top/gthdzsxkws.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenlongwang.top/gtyftstuti.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj20258888.top/gtqsmoymyy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yvedp.cn/gtbrdmnlir.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jinyuanbaomall.cn/gtjewsellh.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ydjk.org.cn/gtgsiqlopa.html

[N04] 斐波那契数列
来源：http://hz.52xcode.cn/gtjhbubsgl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinghuilouyu.cn/gtgsnbxwbb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yongpay.top/gtbqbflypk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.smart0.xyz/gtmzcqhudr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ehwqpu.com/gtzbqgtoxk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.chenjidiqi.icu/gtfvyhpjzy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ywan-chungtsiang.top/gtwtzjxxfr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.chenlongwang.top/gtbxwczjes.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj20258.top/gtclteahrq.html

[N05] 最大公约数
来源：http://hz.shzxlz.cn/gtznyemlfq.html

Py:   math.gcd(a, b)
来源：http://hz.quarkkingdee.top/gtzlrozlka.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zdqjudy.top/gttryekpqg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yueranfly.top/gtlmyiyleo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yueranfly.top/gtcntovkfh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ywan-chungtsiang.top/gtnbufunma.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jqgufenzy.top/gtyxrsvnaa.html

Ruby: a.gcd(b)
来源：http://hz.gotoacloud.top/gtpcrwkwul.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xylfe.cn/gtkmepkhtr.html

[N06] 判断回文字符串
来源：http://hz.gotoacloud.top/gtgzdtvxax.html

Py:   s == s[::-1]
来源：http://hz.gaohongyu789.top/gtwhkndptu.html

PHP:  $s === strrev($s);
来源：http://hz.cdnleiting.top/gtvztomktg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtlrpuywrp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtemmksnce.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinyuanbaomall.cn/gtfbxzmubi.html

Go:   // 双指针从两端比较
来源：http://hz.yuxming.cn/gtrlfljdef.html

Ruby: s == s.reverse
来源：http://hz.gzhubu.top/gtarkpzxre.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hfpthk.cn/gtvuvuigzt.html

[N07] 两数之和（返回下标）
来源：http://hz.jlsjyb.cn/gtexknerkd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hnqzz.top/gtiktjlvqu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yj202588.top/gtdmbibomb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sweek.top/gtkptweztm.html

TS:   // 手写 Map<string, number>
来源：http://hz.gotoacloud.top/gtcirultsq.html

Java: // 手写 HashMap
来源：http://hz.chenlongwang.top/gtzcslnluj.html

Go:   // 手写 map[int]int
来源：http://hz.yvedp.cn/gttmweijui.html

Ruby: // 手写 Hash
来源：http://hz.ywan-chungtsiang.top/gtjsotjrgl.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.aibaodan.cn/gtqdqurzys.html

[N08] 生成全排列
来源：http://hz.ywan-chungtsiang.top/gtljanhlpa.html

Py:   itertools.permutations(arr)
来源：http://hz.xuanzx.com/gtjfmdkhnx.html

PHP:  // 手写递归交换
来源：http://hz.zhijiandao.cn/gtpoapnfgl.html

JS:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtxhdolqig.html

TS:   // 手写回溯递归
来源：http://hz.bjfxy.top/gtzhmwzgaj.html

Java: // 手写回溯递归
来源：http://hz.bjfxy.top/gtygseajqb.html

Go:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtoqvpooli.html

Ruby: arr.permutation.to_a
来源：http://hz.bjfxy.top/gtmxodtyvv.html

C#:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtdvbrdmnt.html

[N09] 栈与队列
来源：http://hz.pengpengdd.cyou/gtppkzfppp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhixingplan.top/gtamdpwbhz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yanxiufei.cn/gtkewizmdn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xuetiantiany.cn/gtgrgnilra.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cheryme.top/gtlkwdgytj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinghuilouyu.cn/gtivvdkqgo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cheryme.top/gtexizerkh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.kuanghao11.cn/gtrtiidjny.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.meibo888.top/gtxblwccip.html

[N10] 链表节点定义
来源：http://hz.svipenyu.cn/gtaslmvcsa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gotoacloud.top/gtggwtygzl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.nwbrower.top/gtkhlzfkig.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj20258888.top/gtfwesdymn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yangfankeji.com/gtzuyxcghc.html

Java: class Node { int v; Node next; }
来源：http://hz.zhijiandao.cn/gtthaxstsb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jlsjyb.cn/gtewgyosie.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinqigfzy.top/gtfhmctlxw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yangfankeji.com/gtanpomefg.html

[N11] 二叉树中序遍历
来源：http://hz.ydjk.org.cn/gtitilsfqn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yj20258.top/gtcpmgnakt.html

PHP:  // 手写递归函数
来源：http://hz.cashguo.top/gtigilklay.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.birdmap.top/gtzoqhmlfn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gotoacloud.top/gtmlfvkeqz.html

Java: // 手写递归
来源：http://hz.hnqzz.top/gtrzminpre.html

Go:   // 手写递归
来源：http://hz.guowangkeji.top/gtuflcoich.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.nwbrower.top/gtztxbtity.html

C#:   // 手写递归
来源：http://hz.aibaodan.cn/gtcqwszaxb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.daria6918.cn/gtszfgaskn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.andypj.xyz/gtdoimkxab.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.fzhhl.top/gtcmanztbr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.c1oappe.top/gtclpkewdi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.feifeiyinyue.top/gtsokhxevs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pycfn.com/gtoozmzkup.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.nanxuanxn.top/gttjfevmfc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinghuilouyu.cn/gtpcoratap.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuanzx.com/gtivzylgrt.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtujjoqklq.html

O. 并发与异步
来源：http://hz.sxryk.cn/gtqvxnayww.html

================================================================================
来源：http://hz.hywenlv.cn/gthypivedu.html

[O01] 启动一个线程
来源：http://hz.yj20258.top/gtagkvhawj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shuidangran.top/gtyceegdlf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhaomingkeji.xyz/gtcqzmcank.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenjidiqi.icu/gtcysysypf.html

TS:   // 同 JS
来源：http://hz.xuanzx.com/gtsmabrqrm.html

Java: new Thread(() -> f()).start()
来源：http://hz.pycfn.com/gtevszoxxt.html

Go:   go f()
来源：http://hz.yangfankeji.com/gtcnhismnu.html

Ruby: Thread.new { f }
来源：http://hz.vqdsnc.cn/gtszusukxx.html

C#:   Task.Run(() => F());
来源：http://hz.ppjwa.cn/gtjjhchkho.html

[O02] 使用线程池
来源：http://hz.wangshuangyany.cn/gtrlyefezi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shuidangran.top/gtjfwdpdcs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.gotoacloud.top/gtqpsiktsv.html

JS:   // worker_threads 线程池
来源：http://hz.ydzc1.top/gtxnbljyso.html

TS:   // worker_threads 线程池
来源：http://hz.ehwqpu.com/gtaecbcyys.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.9152youxi.cn/gtllkpjrum.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yonumen.top/gtipqxqbud.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gaohongyu789.top/gtvjhwreqb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gogol.net.cn/gtfnrqbkik.html

[O03] 加锁保护共享数据
来源：http://hz.0kj1m.cn/gtdfpmkoku.html

Py:   with lock: shared += 1
来源：http://hz.yueranfly.top/gthuiauine.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jinyuanbaomall.cn/gtmyfnouhu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gaohongyu789.top/gttjuwjfpr.html

TS:   // 同 JS
来源：http://hz.smart0.xyz/gtlraznxjg.html

Java: synchronized (this) { shared++; }
来源：http://hz.hfpthk.cn/gtqfmrlmkt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xylfe.cn/gthmcrdohm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.iojbl.cn/gtumgwhuks.html

C#:   lock (gate) { shared++; }
来源：http://hz.xuetiantiany.cn/gtyvmxpwkm.html

[O04] 定义异步函数并等待
来源：http://hz.dashuyun.cn/gtkhzpuyxq.html

Py:   async def f():⏎    await g()
来源：http://hz.316326.xyz/gtblezqgym.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shangyingyoupin.top/gtbotpupbj.html

JS:   async function f() { await g(); }
来源：http://hz.vqdsnc.cn/gtbzglbwdj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yj202588.top/gtwjtnuwnk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shuidangran.top/gtedjbbgpm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yuanzhike.top/gtspwjfrxu.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.fzhhl.top/gtcdakxjtg.html

C#:   async Task F() { await G(); }
来源：http://hz.yonumen.top/gtadprhitn.html

[O05] 并发执行并等待全部完成
来源：http://hz.hammf.cn/gtuzskxbys.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hnqzz.top/gtzjsvssht.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jqgfzy.top/gtsrvbnfsk.html

JS:   await Promise.all(tasks)
来源：http://hz.tian-w.cn/gtroozikbq.html

TS:   await Promise.all(tasks)
来源：http://hz.ivvv.top/gtxqrjmlyc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.havefunace.top/gtojmhhdta.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xylfe.cn/gtbhzucdqy.html

Ruby: threads.map(&:join)
来源：http://hz.ivvv.top/gtltqrgrnb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.mhx1999.top/gttbxujbwb.html

[O06] 使用进程池
来源：http://hz.aizwys.cn/gtohyhbulz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.chenjidiqi.icu/gtqrpgejxc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jinyuanbaomall.cn/gttkunqewn.html

JS:   // child_process / cluster 模块
来源：http://hz.hnqzz.top/gtvcsyutze.html

TS:   // child_process / cluster 模块
来源：http://hz.dianchejie.cn/gtjxrqxnkr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yangfankeji.com/gtneaqjmsg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.andypj.xyz/gtaturnohi.html

Ruby: // fork 块
来源：http://hz.jiagoushi.top/gtvonyizdp.html

C#:   Parallel.For
来源：http://hz.jiagoushi.top/gtuhrfsfpu.html

================================================================================
来源：http://hz.gogol.net.cn/gtgqbxqkkd.html

P. 常用工具函数
来源：http://hz.xziqi.cn/gtiiycklrh.html

================================================================================
来源：http://hz.hammf.cn/gtidsqhepb.html

[P01] 生成 UUID
来源：http://hz.guowangkeji.top/gtjuxvqiua.html

Py:   str(uuid.uuid4())
来源：http://hz.sysykeji.top/gtlukpszfc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gaohongyu789.top/gtveblnwnd.html

JS:   crypto.randomUUID()
来源：http://hz.wangdashe.top/gtchovmceu.html

TS:   crypto.randomUUID()
来源：http://hz.dianchejie.cn/gttgznkwgc.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhiwuduotai.top/gtujwitsoe.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gogol.net.cn/gtflogixjs.html

Ruby: SecureRandom.uuid
来源：http://hz.yuanzhike.top/gtmiklxrvu.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.nwbrower.top/gtecywrbmn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.tianlin.xyz/gtfcitgiwb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hnxiangtu.top/gtnsbudnmv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yuxming.cn/gtwwqbvzji.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.nanxuanxn.top/gtfiwcdqjv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj20258.top/gtbddtmwam.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.guannengcc.top/gtysdcuipr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhijiandao.cn/gtubairwbx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yonumen.top/gtjquvgash.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.sysykeji.top/gtwfaelusj.html

[P03] 生成短随机字符串
来源：http://hz.cucudq.cn/gtzvghyjpu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xziqi.cn/gterjyqxcl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.0kj1m.cn/gtaqwlpzgl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangtech.top/gtnhfksrvm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnqzz.top/gtiapuhvui.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jyoumei.cn/gtjefvvjoo.html


<!-- 参考信息 -->