代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hnxiangtu.top/gtqbmrlten.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jqgfzy.top/gtoetxwipk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tian-w.cn/gtrevecuqx.html

[L06] 解析响应为 JSON
来源：http://hz.zhijiandao.cn/gtezwfgcow.html

Py:   resp.json()
来源：http://hz.wangshuangyany.cn/gturqyoige.html

PHP:  json_decode($body, true);
来源：http://hz.aibaodan.cn/gtbybvcjvz.html

JS:   await resp.json()
来源：http://hz.snrcjt.cn/gtiiaztosx.html

TS:   await resp.json()
来源：http://hz.iojbl.cn/gtaqqngclm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhijiandao.cn/gtibqmtkru.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.dashuyun.cn/gtfilggdnf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sweek.top/gttuyvovvg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.redwolf501.top/gtdmdhcysw.html

[L07] 处理 HTTP 状态码
来源：http://hz.yanxiufei.cn/gttvtpgbui.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhiwuduotai.top/gtrjxdkewh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xziqi.cn/gtrbwjushs.html

JS:   resp.ok;  resp.status
来源：http://hz.cqqwz.cn/gtqfqwszjw.html

TS:   resp.ok;  resp.status
来源：http://hz.xinyue.icu/gtffewgodw.html

Java: resp.statusCode()
来源：http://hz.shangyingyoupin.top/gtebufzouc.html

Go:   resp.StatusCode
来源：http://hz.xingfuxueyuan.xyz/gtghweecjs.html

Ruby: resp.code.to_i
来源：http://hz.yj20258.top/gtsqvoutdw.html

C#:   (int)resp.StatusCode
来源：http://hz.hammf.cn/gtrmpybrfs.html

[L08] 并发请求多个地址
来源：http://hz.sweek.top/gtzvtvppez.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shanyushiyangtech.top/gtnycbhzwp.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj20258888.top/gtnhowjnsv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yueranfly.top/gtxtherwfy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuetiantiany.cn/gtzrfifmkc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zycfv.cn/gtjkioujlz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhiwuduotai.top/gtuuszgvmt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.sysykeji.top/gtsypnllmr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.daria6918.cn/gthtzjztle.html

================================================================================
来源：http://hz.yuanzhike.top/gtgsqvkssn.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhoulong.xyz/gtufjhxwjd.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtkqvfoodu.html

[M01] 读取命令行参数
来源：http://hz.sxryk.cn/gtvqoguyzu.html

Py:   sys.argv[1:]
来源：http://hz.yongpay.top/gtrkksvjyi.html

PHP:  $argv;  $argc;
来源：http://hz.chenjidiqi.icu/gtrbwcftxu.html

JS:   process.argv.slice(2)
来源：http://hz.xuanzx.com/gtjdgmtcmj.html

TS:   process.argv.slice(2)
来源：http://hz.pycfn.com/gtbuotixbi.html

Java: args 数组（main 方法参数）
来源：http://hz.mhx1999.top/gtvxoluosz.html

Go:   os.Args[1:]
来源：http://hz.aizwys.cn/gtghrznmyz.html

Ruby: ARGV
来源：http://hz.shzxlz.cn/gtuyawcgmv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenzaomai.com/gtkfnkmxwd.html

[M02] 读取环境变量
来源：http://hz.yangfankeji.com/gtenvjwsvg.html

Py:   os.environ.get("HOME")
来源：http://hz.feifeiyinyue.top/gtpseahfcv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yuxming.cn/gtjxvbjkhm.html

JS:   process.env.HOME
来源：http://hz.tanke756.top/gtkbxrqkcd.html

TS:   process.env.HOME
来源：http://hz.daxiang520.top/gtkusexiqu.html

Java: System.getenv("HOME")
来源：http://hz.guannengcc.top/gtpcicrrvz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hammf.cn/gtdrvvrqoo.html

Ruby: ENV["HOME"]
来源：http://hz.guowangkeji.top/gteljlayuu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ywan-chungtsiang.top/gtjevldnvy.html

[M03] 执行外部命令
来源：http://hz.vqdsnc.cn/gtjsmaosdn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhoulong.xyz/gtydcbbvti.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.0kj1m.cn/gtfesrtxvi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangshuangyany.cn/gtryuxbyze.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigufen.top/gtqmyktlhp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.fengsongda.top/gtbjwrczlv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hongshengwenyu.top/gtxokjbmma.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hongshengwenyu.top/gtckggqrza.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xziqi.cn/gtpfvwrspm.html

[M04] 获取当前工作目录
来源：http://hz.dianchejie.cn/gtzchlgbku.html

Py:   os.getcwd()
来源：http://hz.zhengqikj.top/gteygwqmsr.html

PHP:  getcwd();
来源：http://hz.svipenyu.cn/gtntlvpylr.html

JS:   process.cwd()
来源：http://hz.tianlin.xyz/gtumighcte.html

TS:   process.cwd()
来源：http://hz.nanxinkj.top/gtukozuwql.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yj20258888.top/gtsgptjkov.html

Go:   os.Getwd()
来源：http://hz.hnxiangtu.top/gtxvysvrow.html

Ruby: Dir.pwd
来源：http://hz.iojbl.cn/gthqbtvtpg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhixingplan.top/gtgxnbpcvk.html

[M05] 设置退出码
来源：http://hz.yanxiufei.cn/gtktsiscjx.html

Py:   sys.exit(1)
来源：http://hz.pycfn.com/gtwqhfbbqd.html

PHP:  exit(1);
来源：http://hz.andypj.xyz/gtiuivvtoc.html

JS:   process.exit(1)
来源：http://hz.zhiwuduotai.top/gtqpgmohqu.html

TS:   process.exit(1)
来源：http://hz.shuidangran.top/gtwazgtsgx.html

Java: System.exit(1)
来源：http://hz.c1oappe.top/gtgqgkerox.html

Go:   os.Exit(1)
来源：http://hz.shanyushiyangkeji.top/gttskzdwxr.html

Ruby: exit 1
来源：http://hz.nwbrower.top/gtbkdlbtnx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.316326.xyz/gtojlwfzge.html

[M06] 向标准错误输出
来源：http://hz.jyoumei.cn/gtodtttolo.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yuxming.cn/gtnvzwgiqm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.9152youxi.cn/gtwtbghocq.html

JS:   console.error("err")
来源：http://hz.sxryk.cn/gttfofhgyq.html

TS:   console.error("err")
来源：http://hz.hfpthk.cn/gtutwawdln.html

Java: System.err.println("err")
来源：http://hz.daria6918.cn/gtphtassxx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cucudq.cn/gtzmzxopjr.html

Ruby: warn "err"
来源：http://hz.fengsongda.top/gtutxcmodi.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jiagoushi.top/gtkonudatd.html

[M07] 判断是否为主入口
来源：http://hz.xziqi.cn/gttgizckxg.html

Py:   if __name__ == "__main__":
来源：http://hz.daxiang520.top/gtprvnyzqg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhiwuduotai.top/gthrewduyx.html

JS:   require.main === module
来源：http://hz.sysykeji.top/gtlliaacpf.html

TS:   require.main === module
来源：http://hz.xylfe.cn/gtxwrjdufv.html

Java: public static void main(String[] args)
来源：http://hz.gaohongyu789.top/gtryanypuz.html

Go:   func main()
来源：http://hz.zhixingplan.top/gtciollrri.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yvedp.cn/gtnrgcdkny.html

C#:   static void Main(string[] args)
来源：http://hz.ydzc1.top/gttmkitwgh.html

[M08] 获取系统与运行时信息
来源：http://hz.sweek.top/gtzyawzgaf.html

Py:   platform.system();  platform.python_version()
来源：http://hz.aibaodan.cn/gtyqeqkzkq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.daria6918.cn/gtvntrpeiw.html

JS:   process.platform;  process.version
来源：http://hz.zhixingplan.top/gttpaanuov.html

TS:   process.platform;  process.version
来源：http://hz.hfpthk.cn/gthmicxyvb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gzhubu.top/gthmbxtgyg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yangfankeji.com/gtjbzfhbwo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.svipenyu.cn/gtqjbjvrsj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhiwuduotai.top/gtgecvjxqp.html

================================================================================
来源：http://hz.meibo888.top/gthbhkkuym.html

N. 数据结构与算法
来源：http://hz.yvedp.cn/gtscwiregh.html

================================================================================
来源：http://hz.svipenyu.cn/gtpbyhhupq.html

[N01] 二分查找（有序数组）
来源：http://hz.ydzc1.top/gtkgmhgepn.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.snrcjt.cn/gtaocflnsl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhixingplan.top/gtlxvacpyd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yvedp.cn/gtxldexppp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yueranfly.top/gtxncmsfhx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cdnleiting.top/gtdgsqsqsd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.havefunace.top/gtayhecejd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhengqikj.top/gtfocofnjz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nwbrower.top/gtdaexgjol.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.aizwys.cn/gtsxxmcour.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenlongwang.top/gtdquqbwhz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhengqikj.top/gtpgunundw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.52xcode.cn/gtvketzncg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tian-w.cn/gtyylnyufq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yvedp.cn/gtevbyoqnd.html

Go:   slices.Sort(arr)
来源：http://hz.wangdashe.top/gtopzqacho.html

Ruby: arr.sort
来源：http://hz.yueranfly.top/gtplyllohm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cqqwz.cn/gtothfedqx.html

[N03] 快速排序（分治示例）
来源：http://hz.wangshuangyany.cn/gtcojornus.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jqgfzy.top/gtivievpda.html

PHP:  // 递归实现，或用 usort
来源：http://hz.aibaodan.cn/gtwnzolcey.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxuanxn.top/gtecpuwbsj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pengpengdd.cyou/gtdmpfemmj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.redwolf501.top/gtlkbjgjkk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhijiandao.cn/gtixoxdegk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hongshengwenyu.top/gtjpekvxsv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xinyue.icu/gthkautatl.html

[N04] 斐波那契数列
来源：http://hz.andypj.xyz/gtxndlffzg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yonumen.top/gtsxsljgof.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.fengsongda.top/gtzecnnner.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigufen.top/gttnblehjc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sufxvd.cn/gtwyrkiiwn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yanxiufei.cn/gtfuksivjy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.guowangkeji.top/gtvohyarre.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gzhubu.top/gtpowxkjqz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj20258.top/gtcnvnakjn.html

[N05] 最大公约数
来源：http://hz.snrcjt.cn/gticsqugbe.html

Py:   math.gcd(a, b)
来源：http://hz.jinyuanbaomall.cn/gtfbskfksh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhixingplan.top/gtgdwznoun.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zdqjudy.top/gtnruiemna.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sweek.top/gtdhijuidy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.nanxinkj.top/gtzekjjlnf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ydzc1.top/gtktogrroy.html

Ruby: a.gcd(b)
来源：http://hz.tanke756.top/gtkzzldcxu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.daxiang520.top/gtvjomalwm.html

[N06] 判断回文字符串
来源：http://hz.snrcjt.cn/gtsejnxvei.html

Py:   s == s[::-1]
来源：http://hz.zhengqikj.top/gtpdptxpji.html

PHP:  $s === strrev($s);
来源：http://hz.zhoulong.xyz/gtsikvrcvc.html

JS:   s === [...s].reverse().join("")
来源：http://hz.birdmap.top/gtvraqljpy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gtgslvxkvh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ywan-chungtsiang.top/gtddhubqss.html

Go:   // 双指针从两端比较
来源：http://hz.jinghuilouyu.cn/gterdrqxao.html

Ruby: s == s.reverse
来源：http://hz.yj20258888.top/gttwtquxii.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.meibo888.top/gtvcixkaei.html

[N07] 两数之和（返回下标）
来源：http://hz.snrcjt.cn/gtxadsmfzg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.tianlin.xyz/gtvugkufkm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.nanxuanxn.top/gtiuvfepyc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shuidangran.top/gtnmyccerd.html

TS:   // 手写 Map<string, number>
来源：http://hz.meibo888.top/gtszqiytdi.html

Java: // 手写 HashMap
来源：http://hz.cdnleiting.top/gtajvnqdwh.html

Go:   // 手写 map[int]int
来源：http://hz.shanyushiyangtech.top/gtwqlevxge.html

Ruby: // 手写 Hash
来源：http://hz.xylfe.cn/gtjmvdnmqu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yangfankeji.com/gtyejgvxjv.html

[N08] 生成全排列
来源：http://hz.guowangkeji.top/gtdxlojcfa.html

Py:   itertools.permutations(arr)
来源：http://hz.shangyingyoupin.top/gtloitqphl.html

PHP:  // 手写递归交换
来源：http://hz.xuanzx.com/gtaetyokiw.html

JS:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtuuovlvxw.html

TS:   // 手写回溯递归
来源：http://hz.snrcjt.cn/gthwwmjtfb.html

Java: // 手写回溯递归
来源：http://hz.fzhhl.top/gtwwbzskyh.html

Go:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtmdfykcft.html

Ruby: arr.permutation.to_a
来源：http://hz.snrcjt.cn/gtlmcgiilg.html

C#:   // 手写回溯递归
来源：http://hz.jqgufenzy.top/gtpcrcayfh.html

[N09] 栈与队列
来源：http://hz.ivvv.top/gtulmuqtmq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj20258.top/gtvhskrfhf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zycfv.cn/gthkludnad.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.guannengcc.top/gtscsdpdlk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinqigfzy.top/gtjuhtcgkx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yj202588.top/gtsnhuetmy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cucudq.cn/gtlerhhxon.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ydjk.org.cn/gtysrvxxaq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.nanxuanxn.top/gtniodufcc.html

[N10] 链表节点定义
来源：http://hz.jinqigufen.top/gtscsayjjo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jqgufenzy.top/gtzmvjxpar.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yongpay.top/gtkyovytgt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sysykeji.top/gtaiejutuh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ehwqpu.com/gteadnewwo.html

Java: class Node { int v; Node next; }
来源：http://hz.haohaochexian.top/gtruyhdqcu.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.havefunace.top/gtfqjewbfn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.9152youxi.cn/gtfdkmekna.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nwbrower.top/gthrxbycsf.html

[N11] 二叉树中序遍历
来源：http://hz.gzhubu.top/gtyabcrpdm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.guannengcc.top/gttyhfbmzx.html

PHP:  // 手写递归函数
来源：http://hz.yuxming.cn/gtvnmerxko.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pengpengdd.cyou/gtpjogcyqr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dashuyun.cn/gttyhmodvw.html

Java: // 手写递归
来源：http://hz.yuxming.cn/gtdnyqsgpr.html

Go:   // 手写递归
来源：http://hz.ydzc1.top/gtpjaewjnh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.0kj1m.cn/gtqqsfqrbs.html

C#:   // 手写递归
来源：http://hz.nwbrower.top/gtffjenjre.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cdnleiting.top/gtiajopfss.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.sufxvd.cn/gttxuskbov.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gaohongyu789.top/gtnyvdsrfr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hammf.cn/gtcgkfwspj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.meibo888.top/gtjiousucx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhixingplan.top/gtnjvwsswg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hywenlv.cn/gtjgnnxzhh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sysykeji.top/gtjvgfkyih.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cheryme.top/gthhqzwxkz.html

================================================================================
来源：http://hz.cdnleiting.top/gtfkxnsyhd.html

O. 并发与异步
来源：http://hz.havefunace.top/gtoltdpeat.html

================================================================================
来源：http://hz.pycfn.com/gtskhuvvkp.html

[O01] 启动一个线程
来源：http://hz.hammf.cn/gtmdivlyyv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.dianchejie.cn/gtkikyvcyt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.guannengcc.top/gtbrhlslut.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.tanke756.top/gtppkiozxu.html

TS:   // 同 JS
来源：http://hz.yj20258888.top/gtxlrqghgz.html

Java: new Thread(() -> f()).start()
来源：http://hz.yvedp.cn/gtmapsjxxn.html

Go:   go f()
来源：http://hz.cheryme.top/gtlkrkvbfp.html

Ruby: Thread.new { f }
来源：http://hz.fengsongda.top/gtmuovprjc.html

C#:   Task.Run(() => F());
来源：http://hz.yanxiufei.cn/gtojtnaxpg.html

[O02] 使用线程池
来源：http://hz.xingfuxueyuan.xyz/gtdaydeadd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cheryme.top/gtdbktkixq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cdnleiting.top/gtjchcexts.html

JS:   // worker_threads 线程池
来源：http://hz.hnqzz.top/gtrgskstjh.html

TS:   // worker_threads 线程池
来源：http://hz.zhaomingkeji.xyz/gtjwcwxjzy.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shangyingyoupin.top/gtgxxnqapq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ywan-chungtsiang.top/gtnlhxnypc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhiwuduotai.top/gttknzpklm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.aizwys.cn/gtxvgosorl.html

[O03] 加锁保护共享数据
来源：http://hz.snrcjt.cn/gtcojmvhse.html

Py:   with lock: shared += 1
来源：http://hz.jianghu66.top/gtxsvwabfp.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.gotoacloud.top/gtmgyuxdfq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.guowangkeji.top/gtwjnkafns.html

TS:   // 同 JS
来源：http://hz.yj202588.top/gtwjmvxhig.html

Java: synchronized (this) { shared++; }
来源：http://hz.chenjidiqi.icu/gtmggxxzgi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.daria6918.cn/gttxjpwcdf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jqgufenzy.top/gtiutclvzu.html

C#:   lock (gate) { shared++; }
来源：http://hz.mhx1999.top/gtkymyiklp.html

[O04] 定义异步函数并等待
来源：http://hz.havefunace.top/gtxgikmgdf.html

Py:   async def f():⏎    await g()
来源：http://hz.shzxlz.cn/gtjxtcuwvu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nanxinkj.top/gtngctlaiz.html

JS:   async function f() { await g(); }
来源：http://hz.ywan-chungtsiang.top/gtxdxuofhe.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xingfuxueyuan.xyz/gtqwkcmhiv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hnxiangtu.top/gtkhpzefom.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jianghu66.top/gtrmfivdbt.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jianghu66.top/gtvdbhtkev.html

C#:   async Task F() { await G(); }
来源：http://hz.ehwqpu.com/gtfvaozfno.html

[O05] 并发执行并等待全部完成
来源：http://hz.nanxuanxn.top/gtsmpjrgyl.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zycfv.cn/gtgdvbkjpi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.andypj.xyz/gtwvacysjg.html

JS:   await Promise.all(tasks)
来源：http://hz.xingfuxueyuan.xyz/gtnlldyrbx.html

TS:   await Promise.all(tasks)
来源：http://hz.yj20258.top/gtqtshstwu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.tianlin.xyz/gturicgwgw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yangfankeji.com/gtpbxdyvfv.html

Ruby: threads.map(&:join)
来源：http://hz.xziqi.cn/gtejnokqpz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.sysykeji.top/gtbjzreyoh.html

[O06] 使用进程池
来源：http://hz.iojbl.cn/gtxloeznci.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yj20258888.top/gtifjcnudu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.daxiang520.top/gtetgcihjg.html

JS:   // child_process / cluster 模块
来源：http://hz.yuanzhike.top/gttofadboa.html

TS:   // child_process / cluster 模块
来源：http://hz.nanxuanxn.top/gtmrzyesyy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.snrcjt.cn/gtnkrbbyka.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ehwqpu.com/gtlvivuoni.html

Ruby: // fork 块
来源：http://hz.cheryme.top/gtkzjxyhsk.html

C#:   Parallel.For
来源：http://hz.iojbl.cn/gtrggozehi.html

================================================================================
来源：http://hz.dashuyun.cn/gtlauymzoz.html

P. 常用工具函数
来源：http://hz.xinyue.icu/gtskcrbwug.html

================================================================================
来源：http://hz.chenzaomai.com/gtagphouvu.html

[P01] 生成 UUID
来源：http://hz.hfpthk.cn/gtcockyzzy.html

Py:   str(uuid.uuid4())
来源：http://hz.shangyingyoupin.top/gtifcbawvv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ydjk.org.cn/gthmuouqkv.html

JS:   crypto.randomUUID()
来源：http://hz.cdnleiting.top/gtyqfzpdkc.html

TS:   crypto.randomUUID()
来源：http://hz.chenlongwang.top/gtxnriumtn.html

Java: UUID.randomUUID().toString()
来源：http://hz.guannengcc.top/gteghmhtmz.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shanyushiyangkeji.top/gtnwktyyyw.html

Ruby: SecureRandom.uuid
来源：http://hz.xingfuxueyuan.xyz/gtnucfinyt.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhoulong.xyz/gtdybdgpat.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ydjk.org.cn/gthmxnhgvi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sysykeji.top/gtfslkwjbq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinqigfzy.top/gtecbqfiuy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cucudq.cn/gtdvhaodeu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhoulong.xyz/gtswpdetsq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hongshengwenyu.top/gtgnmenadx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gzhubu.top/gtieoygmrf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.tian-w.cn/gtamwzeoig.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.nanxuanxn.top/gtrkueoltg.html

[P03] 生成短随机字符串
来源：http://hz.xuanzx.com/gtutlvicmu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhoulong.xyz/gtytiajnuw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.sysykeji.top/gtlbuxbywn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nwbrower.top/gtapstgxpp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.9152youxi.cn/gtppahlzsz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yonumen.top/gtqrrczouh.html


<!-- 参考信息 -->