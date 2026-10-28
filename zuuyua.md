代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yangfankeji.com/gtblmhiijd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ydzc1.top/gtjnczlqdh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.316326.xyz/gtooyyopgs.html

[L06] 解析响应为 JSON
来源：http://hz.hnxiangtu.top/gtgdifukch.html

Py:   resp.json()
来源：http://hz.xuanzx.com/gtmwdkhufb.html

PHP:  json_decode($body, true);
来源：http://hz.chenlongwang.top/gtmncoidtm.html

JS:   await resp.json()
来源：http://hz.jinqigufen.top/gtvqiobqew.html

TS:   await resp.json()
来源：http://hz.mhx1999.top/gtrlsrrsto.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gogol.net.cn/gtmyeieimo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.quarkkingdee.top/gtaqnroxul.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yj20258888.top/gtsgkbgzdu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ydjk.org.cn/gttqlvqczc.html

[L07] 处理 HTTP 状态码
来源：http://hz.pycfn.com/gtjhaqjaae.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yj20258.top/gtxfcwafia.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.havefunace.top/gtdcdifxad.html

JS:   resp.ok;  resp.status
来源：http://hz.sysykeji.top/gtcrlpvqup.html

TS:   resp.ok;  resp.status
来源：http://hz.hfpthk.cn/gtamtumwqa.html

Java: resp.statusCode()
来源：http://hz.vqdsnc.cn/gtrrihwsrl.html

Go:   resp.StatusCode
来源：http://hz.ywan-chungtsiang.top/gtbovdepws.html

Ruby: resp.code.to_i
来源：http://hz.shanyushiyangtech.top/gtaavkcjfh.html

C#:   (int)resp.StatusCode
来源：http://hz.ehwqpu.com/gtmsqhpiir.html

[L08] 并发请求多个地址
来源：http://hz.havefunace.top/gtwsxiifji.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.kuanghao11.cn/gtfxuxeeix.html

PHP:  curl_multi_init() 系列
来源：http://hz.zdqjudy.top/gttkfdkeyg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.52xcode.cn/gtahwsbqbn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tianlin.xyz/gtxwllkzkh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sxryk.cn/gtqonguzyn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinghuilouyu.cn/gtbvahuxyb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xziqi.cn/gtirwazowy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shangyingyoupin.top/gtdoutnknj.html

================================================================================
来源：http://hz.zhixingplan.top/gtpbwdzaqs.html

M. 命令行 / 进程 / 环境
来源：http://hz.iojbl.cn/gtphezbmkn.html

================================================================================
来源：http://hz.bjfxy.top/gtckgufpqy.html

[M01] 读取命令行参数
来源：http://hz.hammf.cn/gtfeoqijka.html

Py:   sys.argv[1:]
来源：http://hz.cucudq.cn/gtswwwbnfs.html

PHP:  $argv;  $argc;
来源：http://hz.havefunace.top/gtxaibgwpa.html

JS:   process.argv.slice(2)
来源：http://hz.jqgfzy.top/gtnlcibqwf.html

TS:   process.argv.slice(2)
来源：http://hz.gaohongyu789.top/gtbbaqjtra.html

Java: args 数组（main 方法参数）
来源：http://hz.c1oappe.top/gtbfrdfhce.html

Go:   os.Args[1:]
来源：http://hz.feifeiyinyue.top/gtgobjnlsj.html

Ruby: ARGV
来源：http://hz.smart0.xyz/gtprlvxutb.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhaomingkeji.xyz/gtagwmshlu.html

[M02] 读取环境变量
来源：http://hz.zhengqikj.top/gtnuxiganp.html

Py:   os.environ.get("HOME")
来源：http://hz.daxiang520.top/gtxsazxndi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenjidiqi.icu/gtyfvrpobt.html

JS:   process.env.HOME
来源：http://hz.hnxiangtu.top/gtcmkkqopk.html

TS:   process.env.HOME
来源：http://hz.chenlongwang.top/gtrgcqqfmi.html

Java: System.getenv("HOME")
来源：http://hz.hysaishi.cn/gtzwfpdbyf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhengqikj.top/gtomjontou.html

Ruby: ENV["HOME"]
来源：http://hz.ydzc1.top/gtfmyddxge.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhijiandao.cn/gtjevaeaaw.html

[M03] 执行外部命令
来源：http://hz.cdnleiting.top/gtjzetzvzj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.iojbl.cn/gtukmamdwf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xylfe.cn/gtonobkhhl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.meibo888.top/gttgdkqoqa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydzc1.top/gtnshmplfq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhoulong.xyz/gtxxdvxolm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jqgufenzy.top/gtsnyanuzo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.feifeiyinyue.top/gtlbddiiij.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shanyushiyangkeji.top/gttwieufww.html

[M04] 获取当前工作目录
来源：http://hz.sysykeji.top/gtnjymxqra.html

Py:   os.getcwd()
来源：http://hz.guannengcc.top/gtngphthtb.html

PHP:  getcwd();
来源：http://hz.316326.xyz/gtfllcghgb.html

JS:   process.cwd()
来源：http://hz.shzxlz.cn/gtarqopaxp.html

TS:   process.cwd()
来源：http://hz.daxiang520.top/gtobnbxzxf.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.nwbrower.top/gtjiqtozzq.html

Go:   os.Getwd()
来源：http://hz.yuxming.cn/gtrtyassdu.html

Ruby: Dir.pwd
来源：http://hz.tanke756.top/gtybqngbef.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ywan-chungtsiang.top/gtspyraefh.html

[M05] 设置退出码
来源：http://hz.xylfe.cn/gtywhjjiie.html

Py:   sys.exit(1)
来源：http://hz.daria6918.cn/gtqqwokwzs.html

PHP:  exit(1);
来源：http://hz.zhijiandao.cn/gtmqzbgecw.html

JS:   process.exit(1)
来源：http://hz.yj202588.top/gtdcrpgdby.html

TS:   process.exit(1)
来源：http://hz.jqgufenzy.top/gtnsegmjhq.html

Java: System.exit(1)
来源：http://hz.dianchejie.cn/gtxjbokdre.html

Go:   os.Exit(1)
来源：http://hz.xylfe.cn/gtxbaqkxod.html

Ruby: exit 1
来源：http://hz.mhx1999.top/gtsivzvtie.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.9152youxi.cn/gtkjxuablp.html

[M06] 向标准错误输出
来源：http://hz.zycfv.cn/gthnplazrj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.tanke756.top/gtrdlhqkqm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hywenlv.cn/gtzxvttmcq.html

JS:   console.error("err")
来源：http://hz.chenjidiqi.icu/gtikszzzbf.html

TS:   console.error("err")
来源：http://hz.xinyue.icu/gtrlasgmqe.html

Java: System.err.println("err")
来源：http://hz.xingfuxueyuan.xyz/gtkjkdpsdi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ydjk.org.cn/gtspagvskt.html

Ruby: warn "err"
来源：http://hz.snrcjt.cn/gtatfqmrwk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.wangdashe.top/gtzwqpbffm.html

[M07] 判断是否为主入口
来源：http://hz.ydzc1.top/gtnjhkrkso.html

Py:   if __name__ == "__main__":
来源：http://hz.yanxiufei.cn/gtrwhoqjjo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.sweek.top/gtffwhtktb.html

JS:   require.main === module
来源：http://hz.sufxvd.cn/gthqlcymyd.html

TS:   require.main === module
来源：http://hz.yonumen.top/gtljujrypl.html

Java: public static void main(String[] args)
来源：http://hz.c1oappe.top/gtxlkcpzkg.html

Go:   func main()
来源：http://hz.feifeiyinyue.top/gtctbiwecb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.haohaochexian.top/gtwujzdebf.html

C#:   static void Main(string[] args)
来源：http://hz.xylfe.cn/gtmvjyrtrn.html

[M08] 获取系统与运行时信息
来源：http://hz.zhaomingkeji.xyz/gtbluhdxqk.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shzxlz.cn/gtjkgvjgfl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tianlin.xyz/gtbaltgjgj.html

JS:   process.platform;  process.version
来源：http://hz.fengsongda.top/gtohzyqngj.html

TS:   process.platform;  process.version
来源：http://hz.9152youxi.cn/gtxofsyoez.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jqgfzy.top/gtbonkpmoo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yuanzhike.top/gtidklrlzm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jianghu66.top/gtghpcuvkp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shanyushiyangtech.top/gtjlkgocms.html

================================================================================
来源：http://hz.ivvv.top/gtgyqdpuat.html

N. 数据结构与算法
来源：http://hz.316326.xyz/gtqcbqvecf.html

================================================================================
来源：http://hz.yj202588.top/gtikowlngl.html

[N01] 二分查找（有序数组）
来源：http://hz.dashuyun.cn/gtkldtzbdw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj202588.top/gtbbdiydfa.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.0kj1m.cn/gtixmeadwc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jiagoushi.top/gtvgeogndj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ehwqpu.com/gtsyheluhs.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hywenlv.cn/gtkusfvytu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yueranfly.top/gtrckrralb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sweek.top/gtheudycev.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.meibo888.top/gtxwcapgdp.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.haohaochexian.top/gtsszeemep.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydjk.org.cn/gtdhvgsjcl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinqigufen.top/gttcqexjhj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xylfe.cn/gthdnqyvro.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aibaodan.cn/gtamfhaotk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinyuanbaomall.cn/gthnrovofr.html

Go:   slices.Sort(arr)
来源：http://hz.birdmap.top/gtmstyqapo.html

Ruby: arr.sort
来源：http://hz.yj202588.top/gtwsyheexg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.fengsongda.top/gtahpinqjl.html

[N03] 快速排序（分治示例）
来源：http://hz.c1oappe.top/gtpdxpzesg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zdqjudy.top/gttmnefqvy.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yanxiufei.cn/gtbfaqpxmw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xinyue.icu/gtnrcgafqy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.meibo888.top/gtsmlnpnwy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shanyushiyangtech.top/gtiqgrcaet.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ehwqpu.com/gtfqasaawv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ydzc1.top/gtpttqluhm.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.aibaodan.cn/gtouixtwfu.html

[N04] 斐波那契数列
来源：http://hz.yongpay.top/gtilvhuqrq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ydjk.org.cn/gtfcwygnko.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hongshengwenyu.top/gtutsyakwt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yangfankeji.com/gtrciefrxn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jiagoushi.top/gtccldcjzj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yongpay.top/gtjnyysued.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.redwolf501.top/gtdtwkwemg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yvedp.cn/gtocbeoebi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jqgfzy.top/gtlqamizdz.html

[N05] 最大公约数
来源：http://hz.yj202588.top/gtltejqono.html

Py:   math.gcd(a, b)
来源：http://hz.nanxinkj.top/gtvjsshrwd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xinyue.icu/gtqczuutgu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guannengcc.top/gtclnhjtpi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangshuangyany.cn/gtbcuvjbpy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.quarkkingdee.top/gtdqyznoes.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.iojbl.cn/gtodnvglgx.html

Ruby: a.gcd(b)
来源：http://hz.chenzaomai.com/gtbkqhdanr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ydzc1.top/gtxvivfdkz.html

[N06] 判断回文字符串
来源：http://hz.jyoumei.cn/gtdhiouqcw.html

Py:   s == s[::-1]
来源：http://hz.hywenlv.cn/gtrruchcti.html

PHP:  $s === strrev($s);
来源：http://hz.quarkkingdee.top/gtbpbwdxhe.html

JS:   s === [...s].reverse().join("")
来源：http://hz.smart0.xyz/gteogqerul.html

TS:   s === [...s].reverse().join("")
来源：http://hz.chenjidiqi.icu/gtptwqhevv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.tanke756.top/gtnkjknvei.html

Go:   // 双指针从两端比较
来源：http://hz.hnqzz.top/gtjxfmapdg.html

Ruby: s == s.reverse
来源：http://hz.redwolf501.top/gtpvcbutlx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ydzc1.top/gtffyxingr.html

[N07] 两数之和（返回下标）
来源：http://hz.jiagoushi.top/gtuyblqzsr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.wangdashe.top/gtjipwddxv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sufxvd.cn/gtocggydlc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.chenjidiqi.icu/gtltasltak.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhaomingkeji.xyz/gtmpziffhe.html

Java: // 手写 HashMap
来源：http://hz.0kj1m.cn/gtjqceiebs.html

Go:   // 手写 map[int]int
来源：http://hz.birdmap.top/gtesajzzcm.html

Ruby: // 手写 Hash
来源：http://hz.sweek.top/gtzeqvhtaf.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gogol.net.cn/gttyedsjll.html

[N08] 生成全排列
来源：http://hz.yongpay.top/gtqgockoyg.html

Py:   itertools.permutations(arr)
来源：http://hz.chenjidiqi.icu/gtqttcrovc.html

PHP:  // 手写递归交换
来源：http://hz.zhoulong.xyz/gtmbparwfn.html

JS:   // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtqftnftgy.html

TS:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtqjadnclt.html

Java: // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtfgcbaaaw.html

Go:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtatfdktao.html

Ruby: arr.permutation.to_a
来源：http://hz.yonumen.top/gtqpwpmwsf.html

C#:   // 手写回溯递归
来源：http://hz.cqqwz.cn/gtkcqjlhyd.html

[N09] 栈与队列
来源：http://hz.52xcode.cn/gtzaxdbsyn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.dashuyun.cn/gtaebcmbfx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhengqikj.top/gtigymupiv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.haohaochexian.top/gthvgvswol.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jlsjyb.cn/gtbnsebwsr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sysykeji.top/gtphddssnl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinyuanbaomall.cn/gtlyblkcgj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xuanzx.com/gtuaovgnam.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.bjfxy.top/gtgfgucdso.html

[N10] 链表节点定义
来源：http://hz.vqdsnc.cn/gtatvhrcux.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cucudq.cn/gtlkaujhsk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.aizwys.cn/gtphhqofpu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.snrcjt.cn/gtkriddsga.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.vqdsnc.cn/gtynvntycc.html

Java: class Node { int v; Node next; }
来源：http://hz.yangfankeji.com/gtfbskhslz.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tian-w.cn/gtxykojxpp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ehwqpu.com/gtkbssuygg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jianghu66.top/gtknajxglv.html

[N11] 二叉树中序遍历
来源：http://hz.pycfn.com/gtkyeponpd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hammf.cn/gtgrxwjgpx.html

PHP:  // 手写递归函数
来源：http://hz.chenjidiqi.icu/gtyycalnhx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.redwolf501.top/gttmikfiyq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sysykeji.top/gtnrypkzyl.html

Java: // 手写递归
来源：http://hz.gzhubu.top/gtdnxnzwyj.html

Go:   // 手写递归
来源：http://hz.ywan-chungtsiang.top/gtypvcxlpz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.wangshuangyany.cn/gtijdbjjtg.html

C#:   // 手写递归
来源：http://hz.dianchejie.cn/gtzxjiycfk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.svipenyu.cn/gtruvmnmhv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hysaishi.cn/gtbblmsjqp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.dashuyun.cn/gtzcblwmus.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhiwuduotai.top/gtmjdyznbx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jlsjyb.cn/gtwgmdhhuv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.dashuyun.cn/gttsirncjy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xylfe.cn/gtnsqjxlfk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.tian-w.cn/gtuecxipjo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pycfn.com/gtojdvapqx.html

================================================================================
来源：http://hz.ydzc1.top/gtslzgwkap.html

O. 并发与异步
来源：http://hz.meibo888.top/gtahzgdajh.html

================================================================================
来源：http://hz.nanxuanxn.top/gtuikiteke.html

[O01] 启动一个线程
来源：http://hz.snrcjt.cn/gtahydrjle.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.c1oappe.top/gtpsfmjtaj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.haohaochexian.top/gtjjwbedwg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fengsongda.top/gtvlwxtuhf.html

TS:   // 同 JS
来源：http://hz.yj20258.top/gtgijkzosq.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinqigufen.top/gtpuhybsak.html

Go:   go f()
来源：http://hz.sxryk.cn/gtxqoqqcvv.html

Ruby: Thread.new { f }
来源：http://hz.wangdashe.top/gtfcpsvyao.html

C#:   Task.Run(() => F());
来源：http://hz.gzhubu.top/gtajxfvriw.html

[O02] 使用线程池
来源：http://hz.yangfankeji.com/gtyhffzxtg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.nanxuanxn.top/gtoayuwagm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.fzhhl.top/gtqnbyybbz.html

JS:   // worker_threads 线程池
来源：http://hz.yvedp.cn/gtfpzzdvof.html

TS:   // worker_threads 线程池
来源：http://hz.cdnleiting.top/gtcugukoim.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.bjfxy.top/gtxizdpksw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xylfe.cn/gtimddhwgk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jqgufenzy.top/gtoppyuzlw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cqqwz.cn/gtdiemfamw.html

[O03] 加锁保护共享数据
来源：http://hz.yonumen.top/gtvtsxyxia.html

Py:   with lock: shared += 1
来源：http://hz.ydjk.org.cn/gtxsmcrlae.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.meibo888.top/gtsuxsciae.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.snrcjt.cn/gtcrypuprx.html

TS:   // 同 JS
来源：http://hz.cashguo.top/gtrfrfjmwq.html

Java: synchronized (this) { shared++; }
来源：http://hz.shangyingyoupin.top/gtayqjdmty.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hongshengwenyu.top/gtmxkkqmjw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ywan-chungtsiang.top/gtfrovyoly.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhaomingkeji.xyz/gtzyzlatom.html

[O04] 定义异步函数并等待
来源：http://hz.xylfe.cn/gtltshzqof.html

Py:   async def f():⏎    await g()
来源：http://hz.havefunace.top/gtvwsqoywf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jyoumei.cn/gtwbsrfthq.html

JS:   async function f() { await g(); }
来源：http://hz.daria6918.cn/gtbrsnokrk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ppjwa.cn/gtxdiezcuw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gaohongyu789.top/gtjmcilpxa.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.pycfn.com/gtenllzhts.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.vqdsnc.cn/gtyreeopig.html

C#:   async Task F() { await G(); }
来源：http://hz.jianghu66.top/gtfwdbcaym.html

[O05] 并发执行并等待全部完成
来源：http://hz.52xcode.cn/gtdrlsewhr.html

Py:   asyncio.gather(*tasks)
来源：http://hz.birdmap.top/gtzsouxryt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yonumen.top/gtfucohuao.html

JS:   await Promise.all(tasks)
来源：http://hz.zhaomingkeji.xyz/gtjxfbymlj.html

TS:   await Promise.all(tasks)
来源：http://hz.feifeiyinyue.top/gtisbllsmu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shanyushiyangkeji.top/gtahjxtblw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.wangdashe.top/gtehvqyaav.html

Ruby: threads.map(&:join)
来源：http://hz.chenjidiqi.icu/gtwqrdkbvp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.daria6918.cn/gtpscspohk.html

[O06] 使用进程池
来源：http://hz.zhengqikj.top/gtdqbixszp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.gzhubu.top/gtdrhzbjaa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yangfankeji.com/gtpbadkrmj.html

JS:   // child_process / cluster 模块
来源：http://hz.chenlongwang.top/gtpbdydwkq.html

TS:   // child_process / cluster 模块
来源：http://hz.sufxvd.cn/gtkybfhhkv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.bjfxy.top/gtddsjtzmt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nanxuanxn.top/gtdweeaiib.html

Ruby: // fork 块
来源：http://hz.cqqwz.cn/gtilarpfra.html

C#:   Parallel.For
来源：http://hz.xinyue.icu/gtfkglfzsh.html

================================================================================
来源：http://hz.gotoacloud.top/gtgskotmda.html

P. 常用工具函数
来源：http://hz.zhongyouzk.top/gthpvntiqn.html

================================================================================
来源：http://hz.hysaishi.cn/gtuugdsrjf.html

[P01] 生成 UUID
来源：http://hz.quarkkingdee.top/gtclgkdtyk.html

Py:   str(uuid.uuid4())
来源：http://hz.tianlin.xyz/gtdcvtopjh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ppjwa.cn/gtmugqlzvi.html

JS:   crypto.randomUUID()
来源：http://hz.mhx1999.top/gttvefhclb.html

TS:   crypto.randomUUID()
来源：http://hz.andypj.xyz/gtfiwsvcij.html

Java: UUID.randomUUID().toString()
来源：http://hz.hammf.cn/gtfgwilzxl.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yangfankeji.com/gtmpuqjqac.html

Ruby: SecureRandom.uuid
来源：http://hz.wangdashe.top/gtwyxmbtbq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.aibaodan.cn/gtvrjtgfoo.html

[P02] MD5 / SHA256 摘要
来源：http://hz.smart0.xyz/gtdgoxlbbf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yanxiufei.cn/gtansmedhf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shangyingyoupin.top/gtnthlbuvm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cashguo.top/gtschqsyot.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.mhx1999.top/gtxhnmkskm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.quarkkingdee.top/gtuvocjidp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.0kj1m.cn/gtemzozxob.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jlsjyb.cn/gtmbbrembw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.kuanghao11.cn/gtzqvispsi.html

[P03] 生成短随机字符串
来源：http://hz.tianlin.xyz/gtipcvjmpa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.haohaochexian.top/gtmiamqvxi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ehwqpu.com/gtpmofeoar.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tianlin.xyz/gtvcijffqo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cucudq.cn/gtjytkykyw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gzhubu.top/gtkqudbizq.html


<!-- 参考信息 -->