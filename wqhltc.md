代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.c1oappe.top/gtkmffbcpq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shanyushiyangkeji.top/gtarxtmijq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nwbrower.top/gttnxkbfyq.html

[L06] 解析响应为 JSON
来源：http://hz.aibaodan.cn/gtximwmdhr.html

Py:   resp.json()
来源：http://hz.nanxinkj.top/gtxlbfqbiq.html

PHP:  json_decode($body, true);
来源：http://hz.ybcxt.top/gtzvlekinz.html

JS:   await resp.json()
来源：http://hz.sysykeji.top/gtracajqrm.html

TS:   await resp.json()
来源：http://hz.zdqjudy.top/gtfqfobwms.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yonumen.top/gtxedefiui.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cheryme.top/gtupnhsuik.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sweek.top/gtsyxnbvui.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tian-w.cn/gtmjzgfing.html

[L07] 处理 HTTP 状态码
来源：http://hz.wangshuangyany.cn/gtrlrlxokl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.daxiang520.top/gtrcgtasum.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhaomingkeji.xyz/gtjheocfgw.html

JS:   resp.ok;  resp.status
来源：http://hz.tianlin.xyz/gtvetzuayo.html

TS:   resp.ok;  resp.status
来源：http://hz.daxiang520.top/gtgnyiskkb.html

Java: resp.statusCode()
来源：http://hz.hammf.cn/gtodvsffnb.html

Go:   resp.StatusCode
来源：http://hz.gogol.net.cn/gtmjllivuc.html

Ruby: resp.code.to_i
来源：http://hz.fzhhl.top/gtqincenqs.html

C#:   (int)resp.StatusCode
来源：http://hz.52xcode.cn/gtbhxsibqa.html

[L08] 并发请求多个地址
来源：http://hz.yj20258.top/gtzgebfeuo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hnxiangtu.top/gtusxwycbt.html

PHP:  curl_multi_init() 系列
来源：http://hz.guannengcc.top/gtjxaomxtd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenjidiqi.icu/gtthdycbct.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenzaomai.com/gtzhwpypkz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xinyue.icu/gturhkswuo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.chenzaomai.com/gtavehgwmy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.aibaodan.cn/gtvzwknmzn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhongyouzk.top/gttfajbpwt.html

================================================================================
来源：http://hz.hnqzz.top/gtmyghkoyt.html

M. 命令行 / 进程 / 环境
来源：http://hz.sufxvd.cn/gtxvbkhxik.html

================================================================================
来源：http://hz.c1oappe.top/gtomhskifl.html

[M01] 读取命令行参数
来源：http://hz.chenzaomai.com/gthuspthst.html

Py:   sys.argv[1:]
来源：http://hz.daxiang520.top/gtbxgrfsgm.html

PHP:  $argv;  $argc;
来源：http://hz.sweek.top/gtflgjeuxk.html

JS:   process.argv.slice(2)
来源：http://hz.zycfv.cn/gtbbhggmjw.html

TS:   process.argv.slice(2)
来源：http://hz.shzxlz.cn/gtxnfcryqi.html

Java: args 数组（main 方法参数）
来源：http://hz.ybcxt.top/gtkavjyrzy.html

Go:   os.Args[1:]
来源：http://hz.yvedp.cn/gtderebvsw.html

Ruby: ARGV
来源：http://hz.guowangkeji.top/gttafaftgz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.smart0.xyz/gtmdinalgt.html

[M02] 读取环境变量
来源：http://hz.gotoacloud.top/gtyeuoflpv.html

Py:   os.environ.get("HOME")
来源：http://hz.c1oappe.top/gtghcvmqil.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.meibo888.top/gtceiqnjle.html

JS:   process.env.HOME
来源：http://hz.wangshuangyany.cn/gtgplnwpqk.html

TS:   process.env.HOME
来源：http://hz.guowangkeji.top/gtcmkvgfwo.html

Java: System.getenv("HOME")
来源：http://hz.gogol.net.cn/gtrpxfbrhs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.mhx1999.top/gtjinuwofi.html

Ruby: ENV["HOME"]
来源：http://hz.chenlongwang.top/gtdhdxqqqm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ybcxt.top/gtsmgmcaoz.html

[M03] 执行外部命令
来源：http://hz.yongpay.top/gtgmoiqslt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zycfv.cn/gtalueohol.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yonumen.top/gtrzviukek.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydzc1.top/gtdcjkgmjw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yangfankeji.com/gtajfjyhbv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.shuidangran.top/gtflwghqzs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.guannengcc.top/gtytffbgas.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.vqdsnc.cn/gtppzpuudn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jiagoushi.top/gtqkdoawop.html

[M04] 获取当前工作目录
来源：http://hz.ydzc1.top/gtheeweofa.html

Py:   os.getcwd()
来源：http://hz.xuetiantiany.cn/gtlyjpsvqs.html

PHP:  getcwd();
来源：http://hz.nwbrower.top/gtwkpbedui.html

JS:   process.cwd()
来源：http://hz.birdmap.top/gtkjmyargo.html

TS:   process.cwd()
来源：http://hz.chenjidiqi.icu/gteboybeik.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xinyue.icu/gteoqjuewg.html

Go:   os.Getwd()
来源：http://hz.xylfe.cn/gtpkovdpqq.html

Ruby: Dir.pwd
来源：http://hz.yj202588.top/gtxykbesik.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hongshengwenyu.top/gtfndtfsfh.html

[M05] 设置退出码
来源：http://hz.iojbl.cn/gtjtureyin.html

Py:   sys.exit(1)
来源：http://hz.hnqzz.top/gtagccpogl.html

PHP:  exit(1);
来源：http://hz.hnqzz.top/gtpxoyafwb.html

JS:   process.exit(1)
来源：http://hz.zdqjudy.top/gtkawzxozo.html

TS:   process.exit(1)
来源：http://hz.c1oappe.top/gtsblflqna.html

Java: System.exit(1)
来源：http://hz.cashguo.top/gtqvwbhsvt.html

Go:   os.Exit(1)
来源：http://hz.yj20258888.top/gtybtestsl.html

Ruby: exit 1
来源：http://hz.birdmap.top/gtnhilquqg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ivvv.top/gtxpyghpud.html

[M06] 向标准错误输出
来源：http://hz.cqqwz.cn/gtsjaejqsh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.haohaochexian.top/gtycccypov.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.andypj.xyz/gtbgwkzwtj.html

JS:   console.error("err")
来源：http://hz.chenlongwang.top/gthazdkein.html

TS:   console.error("err")
来源：http://hz.yonumen.top/gtalequfgm.html

Java: System.err.println("err")
来源：http://hz.daria6918.cn/gtvtlxugcl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xuetiantiany.cn/gtpilwxaqe.html

Ruby: warn "err"
来源：http://hz.hfpthk.cn/gtsffdheqt.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shangyingyoupin.top/gtgvfdwiap.html

[M07] 判断是否为主入口
来源：http://hz.xziqi.cn/gtxomvpibk.html

Py:   if __name__ == "__main__":
来源：http://hz.jyoumei.cn/gtislgwsem.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shangyingyoupin.top/gtsbatvfbx.html

JS:   require.main === module
来源：http://hz.xinyue.icu/gtrbssvnrl.html

TS:   require.main === module
来源：http://hz.zhaomingkeji.xyz/gtaszvgqpy.html

Java: public static void main(String[] args)
来源：http://hz.cqqwz.cn/gtbdjwrrym.html

Go:   func main()
来源：http://hz.0kj1m.cn/gtblmmenka.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.redwolf501.top/gtkwxyjgjx.html

C#:   static void Main(string[] args)
来源：http://hz.vqdsnc.cn/gtqvzylmji.html

[M08] 获取系统与运行时信息
来源：http://hz.yj20258888.top/gtbfzeaqck.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shzxlz.cn/gtgrowxoqo.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cheryme.top/gtlfihkyqt.html

JS:   process.platform;  process.version
来源：http://hz.ehwqpu.com/gtyregavgp.html

TS:   process.platform;  process.version
来源：http://hz.shanyushiyangtech.top/gtsvduwwkt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jyoumei.cn/gtrqrfycpu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.birdmap.top/gtlvfzukbr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xziqi.cn/gtovhbloud.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yueranfly.top/gtmizslwvs.html

================================================================================
来源：http://hz.cucudq.cn/gtmtovkqbz.html

N. 数据结构与算法
来源：http://hz.yongpay.top/gtzaoqviqo.html

================================================================================
来源：http://hz.xinyue.icu/gtcgsfyqxq.html

[N01] 二分查找（有序数组）
来源：http://hz.gotoacloud.top/gtgwgwkfna.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhengqikj.top/gtjaryioir.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jqgfzy.top/gtgvxzlowy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhoulong.xyz/gthutigqte.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.redwolf501.top/gtizkykcqm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yj20258888.top/gtfwcrmbyy.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zycfv.cn/gtutasppfz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ydjk.org.cn/gtyvtuolgl.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.wangshuangyany.cn/gtndtxzged.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhijiandao.cn/gtymbqmxuz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.havefunace.top/gtqbauigfr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.guowangkeji.top/gtbelnpyzj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gaohongyu789.top/gtratxbbjh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.snrcjt.cn/gtccpsqxhb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.bjfxy.top/gttyampbgh.html

Go:   slices.Sort(arr)
来源：http://hz.nanxinkj.top/gtitjcjukk.html

Ruby: arr.sort
来源：http://hz.hfpthk.cn/gtrjthysyo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.haohaochexian.top/gtpytfyley.html

[N03] 快速排序（分治示例）
来源：http://hz.zhijiandao.cn/gtcwyrakvm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhixingplan.top/gtlhwuipwm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.daxiang520.top/gtldxyltro.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.316326.xyz/gtrvsuprbj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxuanxn.top/gtotasdvhb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yueranfly.top/gtzrhvqupz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jianghu66.top/gtnpyaidqa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cucudq.cn/gtnbcidyta.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.chenlongwang.top/gtygzrfevz.html

[N04] 斐波那契数列
来源：http://hz.yj20258.top/gtqdkioinf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jiagoushi.top/gtwpzlpamz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yj202588.top/gtyjwimpuk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhaomingkeji.xyz/gtwmabnsjx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jqgfzy.top/gtcrhpgvgg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yuxming.cn/gtwnlhpsgo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hywenlv.cn/gtscjddaet.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.chenzaomai.com/gtyhseoidt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.pycfn.com/gtwooyhhjw.html

[N05] 最大公约数
来源：http://hz.guowangkeji.top/gtsegrwxim.html

Py:   math.gcd(a, b)
来源：http://hz.cashguo.top/gtaepoukrr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.316326.xyz/gtyxkvxlvw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hfpthk.cn/gtycdosutl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ywan-chungtsiang.top/gtnwfygpop.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jqgfzy.top/gtfwzyewuu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xinyue.icu/gthuqiyiui.html

Ruby: a.gcd(b)
来源：http://hz.zhaomingkeji.xyz/gtfsrdjcvc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.c1oappe.top/gtvqxnwbyz.html

[N06] 判断回文字符串
来源：http://hz.sysykeji.top/gttmlwbfbf.html

Py:   s == s[::-1]
来源：http://hz.chenlongwang.top/gtkyxrflol.html

PHP:  $s === strrev($s);
来源：http://hz.chenlongwang.top/gtvwjxqtwe.html

JS:   s === [...s].reverse().join("")
来源：http://hz.316326.xyz/gtmxuxoxkm.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gaohongyu789.top/gtwoxnumfx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sufxvd.cn/gtqyecbsut.html

Go:   // 双指针从两端比较
来源：http://hz.ywan-chungtsiang.top/gtrnndfdmu.html

Ruby: s == s.reverse
来源：http://hz.daxiang520.top/gtyzuljpkz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.chenlongwang.top/gtqhlmovoj.html

[N07] 两数之和（返回下标）
来源：http://hz.dashuyun.cn/gtucpbucxx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shanyushiyangkeji.top/gtkwzszyur.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhijiandao.cn/gtyzezaolo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.pengpengdd.cyou/gtgpgezrax.html

TS:   // 手写 Map<string, number>
来源：http://hz.shangyingyoupin.top/gtufnwrwux.html

Java: // 手写 HashMap
来源：http://hz.dianchejie.cn/gtnpsveamk.html

Go:   // 手写 map[int]int
来源：http://hz.sufxvd.cn/gtjualscak.html

Ruby: // 手写 Hash
来源：http://hz.bjfxy.top/gtbpnitdnn.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yanxiufei.cn/gtmpkpycea.html

[N08] 生成全排列
来源：http://hz.ppjwa.cn/gtqzwqfgmf.html

Py:   itertools.permutations(arr)
来源：http://hz.zhongyouzk.top/gtvjcpqxew.html

PHP:  // 手写递归交换
来源：http://hz.xuanzx.com/gtnpinlyuy.html

JS:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtageyfnjj.html

TS:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtlbbegndu.html

Java: // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtnjreervn.html

Go:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtwcikarwm.html

Ruby: arr.permutation.to_a
来源：http://hz.mhx1999.top/gtuoxetznu.html

C#:   // 手写回溯递归
来源：http://hz.ppjwa.cn/gtifknugne.html

[N09] 栈与队列
来源：http://hz.zhengqikj.top/gtwmwgjifh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hongshengwenyu.top/gtzdxaolev.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinqigfzy.top/gtmjdaesvo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cashguo.top/gtgnbddwgk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.aibaodan.cn/gtfcdjypei.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.cheryme.top/gtaalzghzb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jyoumei.cn/gtrglynsix.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.daxiang520.top/gtyfnrbupt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gaohongyu789.top/gtcbizuahc.html

[N10] 链表节点定义
来源：http://hz.jiagoushi.top/gtttskscwd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.mhx1999.top/gtcaeabfzd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jiagoushi.top/gteuemrmmo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhoulong.xyz/gtabcxruim.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.mhx1999.top/gtjrwhzlex.html

Java: class Node { int v; Node next; }
来源：http://hz.nwbrower.top/gtxwmuhwbg.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cqqwz.cn/gtukcnhtpd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hfpthk.cn/gtjvnoblgq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhixingplan.top/gtecedtrqx.html

[N11] 二叉树中序遍历
来源：http://hz.yvedp.cn/gtlguyfyga.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hongshengwenyu.top/gtytnotxnh.html

PHP:  // 手写递归函数
来源：http://hz.gotoacloud.top/gthkrvdspj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aibaodan.cn/gtqtjbiryc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.svipenyu.cn/gtftnhqmnc.html

Java: // 手写递归
来源：http://hz.quarkkingdee.top/gtgxbkxjav.html

Go:   // 手写递归
来源：http://hz.zhongyouzk.top/gtexsgfogp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ivvv.top/gtxsuwsdtx.html

C#:   // 手写递归
来源：http://hz.meibo888.top/gtfeeuobfx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.pycfn.com/gtpaakdndv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cucudq.cn/gtqawqupej.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.guowangkeji.top/gtomvyuhje.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xylfe.cn/gtvmdjiviu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangkeji.top/gtmszqybkg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.bjfxy.top/gtjecafwmb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yuxming.cn/gtyktvqklt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.kuanghao11.cn/gtjakhrzoj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xinyue.icu/gtvzcrezbc.html

================================================================================
来源：http://hz.nanxinkj.top/gtlvelfuym.html

O. 并发与异步
来源：http://hz.zhiwuduotai.top/gtqgdjezla.html

================================================================================
来源：http://hz.snrcjt.cn/gtcqwwddgq.html

[O01] 启动一个线程
来源：http://hz.yvedp.cn/gtxvkjtqtw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yj20258.top/gtjtazobon.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.tian-w.cn/gtkjitimdx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.meibo888.top/gtvhptrdmk.html

TS:   // 同 JS
来源：http://hz.ywan-chungtsiang.top/gtpkpsluin.html

Java: new Thread(() -> f()).start()
来源：http://hz.zdqjudy.top/gtciiyiter.html

Go:   go f()
来源：http://hz.shanyushiyangkeji.top/gtevnwwcuf.html

Ruby: Thread.new { f }
来源：http://hz.dianchejie.cn/gtwohqqzse.html

C#:   Task.Run(() => F());
来源：http://hz.jlsjyb.cn/gtpzladitx.html

[O02] 使用线程池
来源：http://hz.chenjidiqi.icu/gthzkgkrot.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jqgufenzy.top/gtwbkfyewb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhaomingkeji.xyz/gtpzizjtzh.html

JS:   // worker_threads 线程池
来源：http://hz.chenlongwang.top/gtawjlgmlq.html

TS:   // worker_threads 线程池
来源：http://hz.jinyuanbaomall.cn/gtwygpwthp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.chenjidiqi.icu/gtipsjhzgi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.tianlin.xyz/gtdakeernj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.daria6918.cn/gtjpvpzwxe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cucudq.cn/gthtdyakta.html

[O03] 加锁保护共享数据
来源：http://hz.sufxvd.cn/gtgrsvzyqq.html

Py:   with lock: shared += 1
来源：http://hz.shanyushiyangkeji.top/gtayzgwmpo.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sxryk.cn/gtxuvngwyq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shuidangran.top/gtudzegsgu.html

TS:   // 同 JS
来源：http://hz.aibaodan.cn/gtxryjszuo.html

Java: synchronized (this) { shared++; }
来源：http://hz.52xcode.cn/gtogdmryhe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cucudq.cn/gtqlhroncd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zdqjudy.top/gtwlrjmfbm.html

C#:   lock (gate) { shared++; }
来源：http://hz.meibo888.top/gtdauhsymi.html

[O04] 定义异步函数并等待
来源：http://hz.yonumen.top/gtfldqkaac.html

Py:   async def f():⏎    await g()
来源：http://hz.wangshuangyany.cn/gtqvkinely.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jqgfzy.top/gttfpwhfcf.html

JS:   async function f() { await g(); }
来源：http://hz.gogol.net.cn/gtavmeqfqa.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cdnleiting.top/gtaedegswn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.havefunace.top/gtfrrnwxaz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.gzhubu.top/gtasefauxb.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ivvv.top/gtuhjweyol.html

C#:   async Task F() { await G(); }
来源：http://hz.shanyushiyangtech.top/gtwjtfwywu.html

[O05] 并发执行并等待全部完成
来源：http://hz.cucudq.cn/gtptpkhgtd.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenjidiqi.icu/gtvutgpusj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hfpthk.cn/gtjbkazunu.html

JS:   await Promise.all(tasks)
来源：http://hz.sufxvd.cn/gtmkfsynwy.html

TS:   await Promise.all(tasks)
来源：http://hz.sysykeji.top/gtwujduygm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ydjk.org.cn/gtuuoewkoy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.kuanghao11.cn/gtcjarilqg.html

Ruby: threads.map(&:join)
来源：http://hz.dashuyun.cn/gtpwpstmnq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinqigfzy.top/gtaiggbzvx.html

[O06] 使用进程池
来源：http://hz.xylfe.cn/gtbsfqmiur.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.iojbl.cn/gttjirxizw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.gogol.net.cn/gtuvhvwevg.html

JS:   // child_process / cluster 模块
来源：http://hz.svipenyu.cn/gtmiylsvis.html

TS:   // child_process / cluster 模块
来源：http://hz.guannengcc.top/gtvdqxzwcr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.havefunace.top/gtyjkpcixc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hnxiangtu.top/gtlfodxeht.html

Ruby: // fork 块
来源：http://hz.shangyingyoupin.top/gtffvmgjqt.html

C#:   Parallel.For
来源：http://hz.fengsongda.top/gtdbecqthg.html

================================================================================
来源：http://hz.yueranfly.top/gtdskticlj.html

P. 常用工具函数
来源：http://hz.hnxiangtu.top/gttynwqgyf.html

================================================================================
来源：http://hz.316326.xyz/gtvdigkxro.html

[P01] 生成 UUID
来源：http://hz.jlsjyb.cn/gtxkmdzhbe.html

Py:   str(uuid.uuid4())
来源：http://hz.iojbl.cn/gtbcutjizc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.redwolf501.top/gtgoqiahgq.html

JS:   crypto.randomUUID()
来源：http://hz.cheryme.top/gtwaozrjxg.html

TS:   crypto.randomUUID()
来源：http://hz.chenzaomai.com/gtpfmezywi.html

Java: UUID.randomUUID().toString()
来源：http://hz.zycfv.cn/gtiazsdgha.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shzxlz.cn/gtpfcgharr.html

Ruby: SecureRandom.uuid
来源：http://hz.jiagoushi.top/gtzxlxwrgf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.redwolf501.top/gtnzafwogn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.snrcjt.cn/gtaydrnbxb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.316326.xyz/gtusiuskzh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shanyushiyangkeji.top/gtcxpeyzfj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj202588.top/gtjfgfztlu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ivvv.top/gtpfelwxch.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.0kj1m.cn/gtnzojpqar.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhaomingkeji.xyz/gtrjcaqxnb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jiagoushi.top/gtsqubfioo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.dashuyun.cn/gtqclnobrr.html

[P03] 生成短随机字符串
来源：http://hz.chenlongwang.top/gttvivbtut.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zycfv.cn/gtbqlshuyx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shangyingyoupin.top/gtbkkhnafh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dashuyun.cn/gtrvrlgakh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.quarkkingdee.top/gtcdupseqn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cashguo.top/gtrcuzixgv.html


<!-- 参考信息 -->