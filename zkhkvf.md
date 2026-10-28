代发 wailian999

Py:   resp.json()
来源：http://hz.ehwqpu.com/gtqmqdrgcd.html

PHP:  json_decode($body, true);
来源：http://hz.xuetiantiany.cn/gtsgzfzhqc.html

JS:   await resp.json()
来源：http://hz.cashguo.top/gtunomrlqq.html

TS:   await resp.json()
来源：http://hz.havefunace.top/gtesichwbw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ydzc1.top/gtuknoajjs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ywan-chungtsiang.top/gtmcfihgxg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ivvv.top/gtvcgfgarx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hywenlv.cn/gtvjwvqlzs.html

[L07] 处理 HTTP 状态码
来源：http://hz.daxiang520.top/gtexfkhzod.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cdnleiting.top/gtqnovxbai.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sysykeji.top/gtpfgrcvto.html

JS:   resp.ok;  resp.status
来源：http://hz.daria6918.cn/gtcuslgeav.html

TS:   resp.ok;  resp.status
来源：http://hz.hammf.cn/gtgblbxaie.html

Java: resp.statusCode()
来源：http://hz.birdmap.top/gtqbldnwjd.html

Go:   resp.StatusCode
来源：http://hz.hfpthk.cn/gtcgqckodq.html

Ruby: resp.code.to_i
来源：http://hz.316326.xyz/gtydvnqqvr.html

C#:   (int)resp.StatusCode
来源：http://hz.aizwys.cn/gtzriylplo.html

[L08] 并发请求多个地址
来源：http://hz.jinqigfzy.top/gtollysdyv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.pycfn.com/gtjxqhtrrv.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinyuanbaomall.cn/gttjrmafme.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.kuanghao11.cn/gtawlpqmnh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtklhbrgpa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yanxiufei.cn/gtpynsvuin.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yvedp.cn/gtednxawem.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.pengpengdd.cyou/gtxuxfgrmt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yj202588.top/gtwdwdatlg.html

================================================================================
来源：http://hz.sufxvd.cn/gtgbcbzcdi.html

M. 命令行 / 进程 / 环境
来源：http://hz.hammf.cn/gtxlleshhg.html

================================================================================
来源：http://hz.dianchejie.cn/gtsumbsdva.html

[M01] 读取命令行参数
来源：http://hz.zhoulong.xyz/gtqvhuznyw.html

Py:   sys.argv[1:]
来源：http://hz.sysykeji.top/gttaumxlxg.html

PHP:  $argv;  $argc;
来源：http://hz.vqdsnc.cn/gtmvlwerir.html

JS:   process.argv.slice(2)
来源：http://hz.zhixingplan.top/gtlptiycmw.html

TS:   process.argv.slice(2)
来源：http://hz.meibo888.top/gttkkomelt.html

Java: args 数组（main 方法参数）
来源：http://hz.sxryk.cn/gtbrgabhsa.html

Go:   os.Args[1:]
来源：http://hz.birdmap.top/gtavmtskru.html

Ruby: ARGV
来源：http://hz.c1oappe.top/gtfybduits.html

C#:   args 数组（Main 方法参数）
来源：http://hz.feifeiyinyue.top/gtbjcbzbjm.html

[M02] 读取环境变量
来源：http://hz.ywan-chungtsiang.top/gtttoxxcrz.html

Py:   os.environ.get("HOME")
来源：http://hz.zhengqikj.top/gtujfuifgu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.gzhubu.top/gtngojrtzf.html

JS:   process.env.HOME
来源：http://hz.daria6918.cn/gtmbsesgfe.html

TS:   process.env.HOME
来源：http://hz.zhongyouzk.top/gtkeefqzro.html

Java: System.getenv("HOME")
来源：http://hz.hywenlv.cn/gtkfmkheud.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.andypj.xyz/gtjjlwzjke.html

Ruby: ENV["HOME"]
来源：http://hz.zhiwuduotai.top/gthripluth.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shanyushiyangtech.top/gtvdytobmp.html

[M03] 执行外部命令
来源：http://hz.havefunace.top/gtnuelkcdh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.birdmap.top/gthbvkshub.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cashguo.top/gtspmprhra.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yvedp.cn/gtihgfvroz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xingfuxueyuan.xyz/gtfrojxuhc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ywan-chungtsiang.top/gtccgwardj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.c1oappe.top/gtpchjsyyj.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shanyushiyangkeji.top/gtcfrcdhqf.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hnxiangtu.top/gtufhxwyus.html

[M04] 获取当前工作目录
来源：http://hz.zhijiandao.cn/gtobpuntnd.html

Py:   os.getcwd()
来源：http://hz.zhiwuduotai.top/gtfakpevdm.html

PHP:  getcwd();
来源：http://hz.sysykeji.top/gttrkxuxom.html

JS:   process.cwd()
来源：http://hz.hammf.cn/gtzwzdscpj.html

TS:   process.cwd()
来源：http://hz.sufxvd.cn/gtaqgdyjyy.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tian-w.cn/gtyspzoaur.html

Go:   os.Getwd()
来源：http://hz.zhoulong.xyz/gtrtlxgupi.html

Ruby: Dir.pwd
来源：http://hz.smart0.xyz/gtjjkmnaqb.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gzhubu.top/gtcbaygrda.html

[M05] 设置退出码
来源：http://hz.shanyushiyangtech.top/gtwsdacpmd.html

Py:   sys.exit(1)
来源：http://hz.jiagoushi.top/gttjkeirpb.html

PHP:  exit(1);
来源：http://hz.xziqi.cn/gtgdxucgpd.html

JS:   process.exit(1)
来源：http://hz.jiagoushi.top/gttwviwuhg.html

TS:   process.exit(1)
来源：http://hz.mhx1999.top/gtpweloowd.html

Java: System.exit(1)
来源：http://hz.ybcxt.top/gtesncabtf.html

Go:   os.Exit(1)
来源：http://hz.yj20258888.top/gtywuievro.html

Ruby: exit 1
来源：http://hz.gaohongyu789.top/gtlferprta.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.mhx1999.top/gttgjsxvgj.html

[M06] 向标准错误输出
来源：http://hz.jinghuilouyu.cn/gtbgyuifrt.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cdnleiting.top/gtkymccrqc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.tanke756.top/gtlypfppcs.html

JS:   console.error("err")
来源：http://hz.jinyuanbaomall.cn/gtrrlfozcz.html

TS:   console.error("err")
来源：http://hz.jinqigfzy.top/gtrjpxtswi.html

Java: System.err.println("err")
来源：http://hz.vqdsnc.cn/gtmlarqohk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.tanke756.top/gtcuhjineg.html

Ruby: warn "err"
来源：http://hz.ivvv.top/gttsuebrdu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.daxiang520.top/gtlfvcqtud.html

[M07] 判断是否为主入口
来源：http://hz.xinyue.icu/gtqtaklczb.html

Py:   if __name__ == "__main__":
来源：http://hz.tanke756.top/gtfnzppgwb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.haohaochexian.top/gtuqbijqar.html

JS:   require.main === module
来源：http://hz.jlsjyb.cn/gtbhbukemc.html

TS:   require.main === module
来源：http://hz.xuanzx.com/gtbghncojp.html

Java: public static void main(String[] args)
来源：http://hz.cheryme.top/gtiecmdecm.html

Go:   func main()
来源：http://hz.tanke756.top/gtszcppbls.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hfpthk.cn/gtfgtljuqa.html

C#:   static void Main(string[] args)
来源：http://hz.c1oappe.top/gtkkejxsve.html

[M08] 获取系统与运行时信息
来源：http://hz.jlsjyb.cn/gtnrgztqzp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.sweek.top/gtszhrpeio.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.pycfn.com/gtksdephub.html

JS:   process.platform;  process.version
来源：http://hz.shuidangran.top/gtpkscklwe.html

TS:   process.platform;  process.version
来源：http://hz.ivvv.top/gtygrirpbu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yangfankeji.com/gtajajlgni.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.aizwys.cn/gtmutlhqhh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gaohongyu789.top/gteuhwnrpj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.meibo888.top/gtigrwrrvd.html

================================================================================
来源：http://hz.yj20258888.top/gtgilxsygi.html

N. 数据结构与算法
来源：http://hz.andypj.xyz/gthqpoohyx.html

================================================================================
来源：http://hz.cucudq.cn/gteuuquses.html

[N01] 二分查找（有序数组）
来源：http://hz.kuanghao11.cn/gthaoagkvf.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jiagoushi.top/gtduobdkyr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hysaishi.cn/gtbrewyxem.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.guannengcc.top/gtwsmmmdnm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.snrcjt.cn/gtxwlqaqdc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yvedp.cn/gtxsbnqpsv.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gogol.net.cn/gtnyayhhgy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.wangshuangyany.cn/gtgkycvycp.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.0kj1m.cn/gterlfbbnc.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhijiandao.cn/gtatjsghne.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shuidangran.top/gtjujkaium.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.pycfn.com/gtcvhrhmdf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhaomingkeji.xyz/gtxcefjmqm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.snrcjt.cn/gtvsvgzqrj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.aizwys.cn/gtdufqxiwt.html

Go:   slices.Sort(arr)
来源：http://hz.wangdashe.top/gtqoybfvvh.html

Ruby: arr.sort
来源：http://hz.zycfv.cn/gtuturpkzy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shangyingyoupin.top/gtbtrrwavc.html

[N03] 快速排序（分治示例）
来源：http://hz.daxiang520.top/gtmbaveflv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ppjwa.cn/gtlhxtkcgp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shuidangran.top/gtcdfhqioh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinyuanbaomall.cn/gtvdfishch.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hywenlv.cn/gtqtpjcvsm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ywan-chungtsiang.top/gtmvfssncu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xylfe.cn/gticwqozbh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.havefunace.top/gtuuxvyfgv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gogol.net.cn/gtpkakyael.html

[N04] 斐波那契数列
来源：http://hz.nwbrower.top/gtpmqtioge.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.snrcjt.cn/gtxzzdlebi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinyuanbaomall.cn/gtqmoweude.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cheryme.top/gtvtdyfjdi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.guowangkeji.top/gtbzeavngp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jinqigfzy.top/gtvrdkquey.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hammf.cn/gtqoifgtir.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.haohaochexian.top/gtmephwrqc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.smart0.xyz/gtpszdkdcx.html

[N05] 最大公约数
来源：http://hz.redwolf501.top/gtcrjusurb.html

Py:   math.gcd(a, b)
来源：http://hz.pycfn.com/gtsqknnlhr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.fengsongda.top/gtrjkunnij.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nanxinkj.top/gtlxnwxfvs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shangyingyoupin.top/gtjdfalcnj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hfpthk.cn/gtciefyvhi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yangfankeji.com/gtpuxrwkcp.html

Ruby: a.gcd(b)
来源：http://hz.redwolf501.top/gtfzugijgm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yuanzhike.top/gtxnqykfvg.html

[N06] 判断回文字符串
来源：http://hz.guowangkeji.top/gtinougpjl.html

Py:   s == s[::-1]
来源：http://hz.nanxinkj.top/gttzqtgdyh.html

PHP:  $s === strrev($s);
来源：http://hz.ydjk.org.cn/gtajpxbqte.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtmcrcgykp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sysykeji.top/gtqsgbldah.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.kuanghao11.cn/gtuwffpflh.html

Go:   // 双指针从两端比较
来源：http://hz.cheryme.top/gtcdqlaefj.html

Ruby: s == s.reverse
来源：http://hz.guowangkeji.top/gtbnhmlmkc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.nanxuanxn.top/gtqoljcnly.html

[N07] 两数之和（返回下标）
来源：http://hz.daxiang520.top/gthpqxefgo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ybcxt.top/gtzhwzvfix.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.wangdashe.top/gtlcolwrvk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yvedp.cn/gtiiywqjyx.html

TS:   // 手写 Map<string, number>
来源：http://hz.yongpay.top/gtiscvlzoo.html

Java: // 手写 HashMap
来源：http://hz.yvedp.cn/gtngkfmyhu.html

Go:   // 手写 map[int]int
来源：http://hz.cheryme.top/gtgjyrewty.html

Ruby: // 手写 Hash
来源：http://hz.smart0.xyz/gtkvgsopfc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yuxming.cn/gtpphxeqrn.html

[N08] 生成全排列
来源：http://hz.tanke756.top/gthhxwrzvg.html

Py:   itertools.permutations(arr)
来源：http://hz.9152youxi.cn/gtwoxavckr.html

PHP:  // 手写递归交换
来源：http://hz.shanyushiyangtech.top/gtefmpecor.html

JS:   // 手写回溯递归
来源：http://hz.xziqi.cn/gtynxlrios.html

TS:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtxyxbtdrd.html

Java: // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtrlkqxaxi.html

Go:   // 手写回溯递归
来源：http://hz.cdnleiting.top/gtbukrsepj.html

Ruby: arr.permutation.to_a
来源：http://hz.xingfuxueyuan.xyz/gtimrkmwft.html

C#:   // 手写回溯递归
来源：http://hz.cheryme.top/gtucnkndbs.html

[N09] 栈与队列
来源：http://hz.zhaomingkeji.xyz/gtpujervma.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ppjwa.cn/gtswptkfqj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.shuidangran.top/gtjafbrqgw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhoulong.xyz/gtrfxfshsr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xuetiantiany.cn/gtpdotspoe.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.tianlin.xyz/gtsgcnfxuu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xuetiantiany.cn/gtfbbnggrh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.aizwys.cn/gtqlemwbmt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.sweek.top/gtgmcyikqw.html

[N10] 链表节点定义
来源：http://hz.yj202588.top/gtsjyhpdjc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.havefunace.top/gtcqomuxlc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yj20258.top/gtditimsfa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cqqwz.cn/gttivzhxjn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenzaomai.com/gtvobhgwli.html

Java: class Node { int v; Node next; }
来源：http://hz.tian-w.cn/gtyboosgfw.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shzxlz.cn/gtqvnwjoxw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.smart0.xyz/gtqnzdqphr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yuxming.cn/gtlebkuanx.html

[N11] 二叉树中序遍历
来源：http://hz.dianchejie.cn/gtybslpxsl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jlsjyb.cn/gtphaubblp.html

PHP:  // 手写递归函数
来源：http://hz.kuanghao11.cn/gtydhnfkpx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ybcxt.top/gthhvkisaw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.redwolf501.top/gtosukuozo.html

Java: // 手写递归
来源：http://hz.havefunace.top/gtiidxbidb.html

Go:   // 手写递归
来源：http://hz.yonumen.top/gtrszhtiys.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cucudq.cn/gtroigfdom.html

C#:   // 手写递归
来源：http://hz.hongshengwenyu.top/gtxmcxiagz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xuanzx.com/gtqwxtcjeu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.nwbrower.top/gtmzpvenff.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhoulong.xyz/gtutltkbug.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.bjfxy.top/gtdtutymaz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhixingplan.top/gtgzapzkyz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pycfn.com/gtbanxyupd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.nanxuanxn.top/gthgupebhd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.nanxuanxn.top/gtucudejvy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yuanzhike.top/gtoairuesu.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtzaqxnpdl.html

O. 并发与异步
来源：http://hz.hysaishi.cn/gtpfifnpzo.html

================================================================================
来源：http://hz.redwolf501.top/gtpawymgtc.html

[O01] 启动一个线程
来源：http://hz.yonumen.top/gtmcvfrkcj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.9152youxi.cn/gtqrlbdior.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.c1oappe.top/gtwkjtauaa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.smart0.xyz/gtgqvzijzd.html

TS:   // 同 JS
来源：http://hz.xziqi.cn/gtofigulqw.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinqigufen.top/gtjcpizwwu.html

Go:   go f()
来源：http://hz.tanke756.top/gtejxagnls.html

Ruby: Thread.new { f }
来源：http://hz.hysaishi.cn/gtfonxothx.html

C#:   Task.Run(() => F());
来源：http://hz.pengpengdd.cyou/gtnctzmwxa.html

[O02] 使用线程池
来源：http://hz.yongpay.top/gtjpqragpi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhongyouzk.top/gtfmtuhqtx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.dashuyun.cn/gtibcloyzu.html

JS:   // worker_threads 线程池
来源：http://hz.zhaomingkeji.xyz/gtstjrpsut.html

TS:   // worker_threads 线程池
来源：http://hz.ybcxt.top/gtngfcwpcs.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cqqwz.cn/gtgdmfnexb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yonumen.top/gtevnxifkz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ywan-chungtsiang.top/gtlkslbgsp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shangyingyoupin.top/gtyrnfvglt.html

[O03] 加锁保护共享数据
来源：http://hz.xingfuxueyuan.xyz/gttvfegxbe.html

Py:   with lock: shared += 1
来源：http://hz.shzxlz.cn/gtrakcxqld.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hysaishi.cn/gtdjymjhrx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhengqikj.top/gtjupyrczr.html

TS:   // 同 JS
来源：http://hz.xinyue.icu/gtumashlqd.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhengqikj.top/gtdsbqgigw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.meibo888.top/gtkwmtztfl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.tanke756.top/gtpvzbtoyf.html

C#:   lock (gate) { shared++; }
来源：http://hz.daria6918.cn/gtnsuyaevo.html

[O04] 定义异步函数并等待
来源：http://hz.sweek.top/gtfcqkqkbl.html

Py:   async def f():⏎    await g()
来源：http://hz.yvedp.cn/gtdkqrlouf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.havefunace.top/gtsozfmath.html

JS:   async function f() { await g(); }
来源：http://hz.pengpengdd.cyou/gtxrccglaa.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ehwqpu.com/gtwlauflcv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hfpthk.cn/gtxvzoixqb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.tianlin.xyz/gtiwobfbng.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.wangshuangyany.cn/gtwfbblgsr.html

C#:   async Task F() { await G(); }
来源：http://hz.yuxming.cn/gtohmxkjgk.html

[O05] 并发执行并等待全部完成
来源：http://hz.guannengcc.top/gtuhbluhat.html

Py:   asyncio.gather(*tasks)
来源：http://hz.guowangkeji.top/gtxktscjde.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.feifeiyinyue.top/gtmmhuvtte.html

JS:   await Promise.all(tasks)
来源：http://hz.birdmap.top/gtqbqtqhue.html

TS:   await Promise.all(tasks)
来源：http://hz.redwolf501.top/gtcklpopuv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.sufxvd.cn/gtjoildixq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xingfuxueyuan.xyz/gtvmonbmqs.html

Ruby: threads.map(&:join)
来源：http://hz.shanyushiyangkeji.top/gtyrllgzym.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhiwuduotai.top/gturqjpeyi.html

[O06] 使用进程池
来源：http://hz.hfpthk.cn/gtwxclosyl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.nanxuanxn.top/gtukobhnen.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jqgfzy.top/gtznqvfnfg.html

JS:   // child_process / cluster 模块
来源：http://hz.0kj1m.cn/gtnxrhgwgq.html

TS:   // child_process / cluster 模块
来源：http://hz.birdmap.top/gtfwpcdrls.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.guowangkeji.top/gtmxxcqccd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.pycfn.com/gtadhpymhf.html

Ruby: // fork 块
来源：http://hz.guowangkeji.top/gtblspgmeg.html

C#:   Parallel.For
来源：http://hz.yongpay.top/gtugvhmlac.html

================================================================================
来源：http://hz.birdmap.top/gtdvphwenx.html

P. 常用工具函数
来源：http://hz.cdnleiting.top/gtxmupqkmo.html

================================================================================
来源：http://hz.316326.xyz/gtflsiyuju.html

[P01] 生成 UUID
来源：http://hz.hywenlv.cn/gtjcrutbbe.html

Py:   str(uuid.uuid4())
来源：http://hz.cashguo.top/gtiyeixgcr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.andypj.xyz/gthogpkeki.html

JS:   crypto.randomUUID()
来源：http://hz.feifeiyinyue.top/gtodfacvxb.html

TS:   crypto.randomUUID()
来源：http://hz.yanxiufei.cn/gteldilgsh.html

Java: UUID.randomUUID().toString()
来源：http://hz.ywan-chungtsiang.top/gtagncbrcg.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cqqwz.cn/gtnagbatdm.html

Ruby: SecureRandom.uuid
来源：http://hz.wangshuangyany.cn/gtyajlufes.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yuanzhike.top/gtdwgrimjn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cheryme.top/gtslordhyv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.guowangkeji.top/gtxpcwqnzm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yj20258888.top/gtwiddiqht.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xinyue.icu/gtfwbaenfo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xuetiantiany.cn/gtuzxeogej.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jqgfzy.top/gttljsopne.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yangfankeji.com/gtwjysseid.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hywenlv.cn/gtilpymfkh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.wangdashe.top/gttsexrlid.html

[P03] 生成短随机字符串
来源：http://hz.svipenyu.cn/gtbgouhfis.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.wangdashe.top/gtdncdsreq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shangyingyoupin.top/gtyjmzgoxl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigufen.top/gtbiflupxw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yangfankeji.com/gtkltzzbha.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.quarkkingdee.top/gtkaedrmjv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.0kj1m.cn/gttevkksyz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zycfv.cn/gtlvkduwcs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xuanzx.com/gtuomwausd.html

[P04] 求长度
来源：http://hz.mhx1999.top/gtztmlmkjv.html


<!-- 参考信息 -->