代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.tianlin.xyz/gtqvbswcfm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gogol.net.cn/gttkvzhzlr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhongyouzk.top/gtacirhwll.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.guannengcc.top/gteibekybw.html

[L07] 处理 HTTP 状态码
来源：http://hz.jlsjyb.cn/gtntfybnzc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.redwolf501.top/gtvhbpgfvu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.fengsongda.top/gtuocpwtfu.html

JS:   resp.ok;  resp.status
来源：http://hz.316326.xyz/gtoahqrtoj.html

TS:   resp.ok;  resp.status
来源：http://hz.xingfuxueyuan.xyz/gtclkfqrgo.html

Java: resp.statusCode()
来源：http://hz.nwbrower.top/gtkjqbkmxm.html

Go:   resp.StatusCode
来源：http://hz.gogol.net.cn/gtxegbloul.html

Ruby: resp.code.to_i
来源：http://hz.jinqigfzy.top/gtatlbapui.html

C#:   (int)resp.StatusCode
来源：http://hz.gogol.net.cn/gtnevuyfci.html

[L08] 并发请求多个地址
来源：http://hz.cdnleiting.top/gtqudbgclz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yangfankeji.com/gtcgaibcjq.html

PHP:  curl_multi_init() 系列
来源：http://hz.xuanzx.com/gtasmjflhd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hysaishi.cn/gtyxsjnhnq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sweek.top/gtpvywlony.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zycfv.cn/gtoviwbcyg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.pycfn.com/gtugqgfplh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yangfankeji.com/gtjplxlnzo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhongyouzk.top/gtcaqqgdlc.html

================================================================================
来源：http://hz.sweek.top/gtmnotswli.html

M. 命令行 / 进程 / 环境
来源：http://hz.jiagoushi.top/gtbdujdckp.html

================================================================================
来源：http://hz.yangfankeji.com/gtdffygqsw.html

[M01] 读取命令行参数
来源：http://hz.gogol.net.cn/gtxnedbhta.html

Py:   sys.argv[1:]
来源：http://hz.wangshuangyany.cn/gtphhfgxzz.html

PHP:  $argv;  $argc;
来源：http://hz.wangdashe.top/gtpqlgkejj.html

JS:   process.argv.slice(2)
来源：http://hz.chenlongwang.top/gtorakgdfj.html

TS:   process.argv.slice(2)
来源：http://hz.sxryk.cn/gtnekavetu.html

Java: args 数组（main 方法参数）
来源：http://hz.zhongyouzk.top/gtijyxfglx.html

Go:   os.Args[1:]
来源：http://hz.smart0.xyz/gtotlpqmqr.html

Ruby: ARGV
来源：http://hz.yj202588.top/gtwysieiar.html

C#:   args 数组（Main 方法参数）
来源：http://hz.fengsongda.top/gtqatwwxba.html

[M02] 读取环境变量
来源：http://hz.cheryme.top/gtketryjit.html

Py:   os.environ.get("HOME")
来源：http://hz.jinqigfzy.top/gtvuqkolil.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hfpthk.cn/gtymfkowyj.html

JS:   process.env.HOME
来源：http://hz.jinghuilouyu.cn/gtomdtfzcw.html

TS:   process.env.HOME
来源：http://hz.hysaishi.cn/gtybkhjjsg.html

Java: System.getenv("HOME")
来源：http://hz.chenjidiqi.icu/gtkcochzkh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ehwqpu.com/gtnrnqwjvb.html

Ruby: ENV["HOME"]
来源：http://hz.zhoulong.xyz/gtqaxfanlr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.iojbl.cn/gtztpxmyyo.html

[M03] 执行外部命令
来源：http://hz.zycfv.cn/gtwpzfqdqn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.pengpengdd.cyou/gtyiqkgxcu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.aibaodan.cn/gtxgychdxo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shzxlz.cn/gtkjmjohjb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hongshengwenyu.top/gthwqagveh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.wangdashe.top/gtdgowtlqh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yvedp.cn/gtglbklbuh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sxryk.cn/gtsdokrhez.html

C#:   Process.Start("ls", "-l");
来源：http://hz.tianlin.xyz/gtjdalivwh.html

[M04] 获取当前工作目录
来源：http://hz.gaohongyu789.top/gtmnadlbyl.html

Py:   os.getcwd()
来源：http://hz.feifeiyinyue.top/gtbjejsjpb.html

PHP:  getcwd();
来源：http://hz.ehwqpu.com/gtlqwmjhfm.html

JS:   process.cwd()
来源：http://hz.zdqjudy.top/gtfuavqrmz.html

TS:   process.cwd()
来源：http://hz.kuanghao11.cn/gtghjyqvci.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sxryk.cn/gttrazyptm.html

Go:   os.Getwd()
来源：http://hz.zycfv.cn/gtspcfoyma.html

Ruby: Dir.pwd
来源：http://hz.svipenyu.cn/gtilckoyjn.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhengqikj.top/gtrissplve.html

[M05] 设置退出码
来源：http://hz.xziqi.cn/gtnnfqourw.html

Py:   sys.exit(1)
来源：http://hz.aibaodan.cn/gtbcecktfd.html

PHP:  exit(1);
来源：http://hz.redwolf501.top/gtldiinjlt.html

JS:   process.exit(1)
来源：http://hz.ydjk.org.cn/gtuaagncwp.html

TS:   process.exit(1)
来源：http://hz.ydzc1.top/gtfnxmkrfm.html

Java: System.exit(1)
来源：http://hz.yuanzhike.top/gtybpyhtpq.html

Go:   os.Exit(1)
来源：http://hz.pengpengdd.cyou/gtwebelgby.html

Ruby: exit 1
来源：http://hz.dianchejie.cn/gtdxycybmn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zdqjudy.top/gtyhqmoicl.html

[M06] 向标准错误输出
来源：http://hz.chenjidiqi.icu/gtzlcpzwlx.html

Py:   print("err", file=sys.stderr)
来源：http://hz.chenjidiqi.icu/gtlvzwudqc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jqgufenzy.top/gtupycjsui.html

JS:   console.error("err")
来源：http://hz.aibaodan.cn/gtfrxzvnhi.html

TS:   console.error("err")
来源：http://hz.ydjk.org.cn/gtkswclovj.html

Java: System.err.println("err")
来源：http://hz.tanke756.top/gtkxbrcrns.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zycfv.cn/gtddaroifd.html

Ruby: warn "err"
来源：http://hz.cheryme.top/gtibcefgng.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.dashuyun.cn/gtkapwpkes.html

[M07] 判断是否为主入口
来源：http://hz.ppjwa.cn/gtptmhxmmo.html

Py:   if __name__ == "__main__":
来源：http://hz.xingfuxueyuan.xyz/gtoebjjurx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shanyushiyangtech.top/gtlwxgnmfd.html

JS:   require.main === module
来源：http://hz.tanke756.top/gtljdfbnpb.html

TS:   require.main === module
来源：http://hz.daxiang520.top/gtibfrvslv.html

Java: public static void main(String[] args)
来源：http://hz.fzhhl.top/gtkczmcnhl.html

Go:   func main()
来源：http://hz.andypj.xyz/gtrffckmmo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hnqzz.top/gtakvkispi.html

C#:   static void Main(string[] args)
来源：http://hz.hywenlv.cn/gtgewziswq.html

[M08] 获取系统与运行时信息
来源：http://hz.tianlin.xyz/gtfbgtmorm.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shanyushiyangtech.top/gtbxlamirk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yuxming.cn/gtpiqkapve.html

JS:   process.platform;  process.version
来源：http://hz.shuidangran.top/gtnqezvbsb.html

TS:   process.platform;  process.version
来源：http://hz.hfpthk.cn/gtbqimmjce.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.iojbl.cn/gtwtwccntq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.havefunace.top/gtlchtwjrw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jianghu66.top/gtdxmsyecy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinqigufen.top/gtnoxtltjv.html

================================================================================
来源：http://hz.0kj1m.cn/gtdtswyyix.html

N. 数据结构与算法
来源：http://hz.havefunace.top/gttrrijdnk.html

================================================================================
来源：http://hz.birdmap.top/gtqrrnvvzl.html

[N01] 二分查找（有序数组）
来源：http://hz.dashuyun.cn/gtrdjrpdcw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yueranfly.top/gtmukshfqg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.aibaodan.cn/gtbfcztapc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dianchejie.cn/gtgodaiitd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ehwqpu.com/gtaxvibvwk.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gaohongyu789.top/gtcajaferl.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.daxiang520.top/gtiiizhjdq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinqigufen.top/gtdjrbkmfa.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yanxiufei.cn/gtxtsgkuhs.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.smart0.xyz/gttwnocime.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.andypj.xyz/gthbigebnn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yongpay.top/gtuhiajqcr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.quarkkingdee.top/gtqnyaaunj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.kuanghao11.cn/gtyoxylqxe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jianghu66.top/gtypiguvuw.html

Go:   slices.Sort(arr)
来源：http://hz.cheryme.top/gtqgvnafce.html

Ruby: arr.sort
来源：http://hz.feifeiyinyue.top/gtfojaqlzj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hfpthk.cn/gtvprdkbmb.html

[N03] 快速排序（分治示例）
来源：http://hz.zdqjudy.top/gtmragiszp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.bjfxy.top/gtnomnslgh.html

PHP:  // 递归实现，或用 usort
来源：http://hz.dashuyun.cn/gtvtpwlikc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aizwys.cn/gtejoqfnbv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jianghu66.top/gtubzjhjps.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xylfe.cn/gtxcdtqzvc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hnxiangtu.top/gtvwodycew.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yj20258.top/gtbkwvwdeb.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jyoumei.cn/gtlthohmuk.html

[N04] 斐波那契数列
来源：http://hz.nwbrower.top/gtzbxwphhl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ydjk.org.cn/gtzvjzngfb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.dashuyun.cn/gtvpeyhgcm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hywenlv.cn/gtrdlzpuom.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gtmaujvjfh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cashguo.top/gtnpjtcmga.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gzhubu.top/gtvwbqkgkk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jqgfzy.top/gtojnzflpk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jiagoushi.top/gtlovqlxqy.html

[N05] 最大公约数
来源：http://hz.bjfxy.top/gttxvnmomd.html

Py:   math.gcd(a, b)
来源：http://hz.zhiwuduotai.top/gtccyvklvk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jiagoushi.top/gtlgijfmta.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigufen.top/gteljqcgse.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tian-w.cn/gtbjxqyezx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ivvv.top/gtuvbupqbv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jqgfzy.top/gtbmpzrsok.html

Ruby: a.gcd(b)
来源：http://hz.meibo888.top/gtowsecaom.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.guannengcc.top/gtjiojzakn.html

[N06] 判断回文字符串
来源：http://hz.svipenyu.cn/gtmiugnbwj.html

Py:   s == s[::-1]
来源：http://hz.zdqjudy.top/gtxnrqvkhp.html

PHP:  $s === strrev($s);
来源：http://hz.chenzaomai.com/gtjpziuqhp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ydzc1.top/gtyulslwok.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ivvv.top/gtsgsljvwj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.daria6918.cn/gtrqjshlht.html

Go:   // 双指针从两端比较
来源：http://hz.0kj1m.cn/gtnydeabue.html

Ruby: s == s.reverse
来源：http://hz.yanxiufei.cn/gtfsxzwcou.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xuanzx.com/gtvyfuobba.html

[N07] 两数之和（返回下标）
来源：http://hz.yongpay.top/gtmxabplco.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shuidangran.top/gthcowjqes.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xuanzx.com/gtmubredns.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.wangdashe.top/gtggohftab.html

TS:   // 手写 Map<string, number>
来源：http://hz.feifeiyinyue.top/gtobutnzlk.html

Java: // 手写 HashMap
来源：http://hz.sufxvd.cn/gtifthgqof.html

Go:   // 手写 map[int]int
来源：http://hz.quarkkingdee.top/gtctipiwez.html

Ruby: // 手写 Hash
来源：http://hz.tanke756.top/gthmgwyjzz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cashguo.top/gtixggbkqn.html

[N08] 生成全排列
来源：http://hz.yuxming.cn/gtvtvmvvne.html

Py:   itertools.permutations(arr)
来源：http://hz.yonumen.top/gtjeuwzhvi.html

PHP:  // 手写递归交换
来源：http://hz.birdmap.top/gtnkyrrsis.html

JS:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtzkpkcuwu.html

TS:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtmpbzkiza.html

Java: // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtvqyrmzli.html

Go:   // 手写回溯递归
来源：http://hz.cdnleiting.top/gtojpvhiiv.html

Ruby: arr.permutation.to_a
来源：http://hz.redwolf501.top/gtxorjrmsd.html

C#:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtslephrul.html

[N09] 栈与队列
来源：http://hz.guowangkeji.top/gtgqvxmtrb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.tian-w.cn/gtawcpzwpg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhaomingkeji.xyz/gtiqpftinw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jqgufenzy.top/gtbspvqixb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ydzc1.top/gttktnexfn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jqgfzy.top/gtbycbjpnw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ydzc1.top/gttotadqbj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yvedp.cn/gtvcjeqhfn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cheryme.top/gttqvhppaj.html

[N10] 链表节点定义
来源：http://hz.bjfxy.top/gttjzzevuu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jinyuanbaomall.cn/gttfsywrou.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zycfv.cn/gtoolmlwgh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cucudq.cn/gtflqmhvxn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yanxiufei.cn/gttfhzpdeh.html

Java: class Node { int v; Node next; }
来源：http://hz.aizwys.cn/gtgwhlkxcx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.daria6918.cn/gtprsjrlrw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.birdmap.top/gtcpthqsdv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhengqikj.top/gtfrxuyxfm.html

[N11] 二叉树中序遍历
来源：http://hz.jqgfzy.top/gtcfgwkvkw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hnqzz.top/gtmwxyemuv.html

PHP:  // 手写递归函数
来源：http://hz.zhongyouzk.top/gtrocigqcu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dashuyun.cn/gtfdiditlw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yangfankeji.com/gttdpbzpjg.html

Java: // 手写递归
来源：http://hz.guannengcc.top/gtzjgmappu.html

Go:   // 手写递归
来源：http://hz.0kj1m.cn/gtpgdqkpwb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.quarkkingdee.top/gtaefjcmwp.html

C#:   // 手写递归
来源：http://hz.yangfankeji.com/gtgkqylcby.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhoulong.xyz/gttnbrhhiz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xylfe.cn/gtmwhsuymh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.tanke756.top/gtyhpdnjei.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yvedp.cn/gtovdldxqh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258888.top/gtgneomutt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhiwuduotai.top/gtuntzyqax.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.smart0.xyz/gtgpvljzwy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jlsjyb.cn/gtlsrvksun.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ehwqpu.com/gtmgbgderr.html

================================================================================
来源：http://hz.meibo888.top/gtxrnjaytm.html

O. 并发与异步
来源：http://hz.hnxiangtu.top/gtutiglbja.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtfiqbpdzr.html

[O01] 启动一个线程
来源：http://hz.birdmap.top/gtstvoxejt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.chenjidiqi.icu/gtkrjwwrpu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yongpay.top/gtfqcqphfk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.c1oappe.top/gtfetdowwk.html

TS:   // 同 JS
来源：http://hz.meibo888.top/gtzoauidfn.html

Java: new Thread(() -> f()).start()
来源：http://hz.vqdsnc.cn/gtdokovizd.html

Go:   go f()
来源：http://hz.chenlongwang.top/gtufgpxrrt.html

Ruby: Thread.new { f }
来源：http://hz.wangdashe.top/gtptltvnko.html

C#:   Task.Run(() => F());
来源：http://hz.ppjwa.cn/gthikwmqmb.html

[O02] 使用线程池
来源：http://hz.havefunace.top/gtilmbuerh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.bjfxy.top/gtretmtdfg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ybcxt.top/gttfgabqlf.html

JS:   // worker_threads 线程池
来源：http://hz.dianchejie.cn/gtrxhjogpo.html

TS:   // worker_threads 线程池
来源：http://hz.cqqwz.cn/gtkhxpljzm.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.snrcjt.cn/gtvdjrmnrn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ydjk.org.cn/gtcmvhonzy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jyoumei.cn/gtajnrxivg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.wangshuangyany.cn/gtzgjxcsgv.html

[O03] 加锁保护共享数据
来源：http://hz.jinghuilouyu.cn/gtneuibukx.html

Py:   with lock: shared += 1
来源：http://hz.birdmap.top/gtcjhnuetr.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.svipenyu.cn/gtfdyojfpv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hywenlv.cn/gtwnwkpump.html

TS:   // 同 JS
来源：http://hz.xuetiantiany.cn/gtvxdbyeim.html

Java: synchronized (this) { shared++; }
来源：http://hz.nanxinkj.top/gtwgmqmzpw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.vqdsnc.cn/gttjbaxtxw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jyoumei.cn/gtzxfxwsma.html

C#:   lock (gate) { shared++; }
来源：http://hz.fzhhl.top/gtnerbydas.html

[O04] 定义异步函数并等待
来源：http://hz.chenlongwang.top/gtfsircany.html

Py:   async def f():⏎    await g()
来源：http://hz.guowangkeji.top/gtexxeyfvu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xuetiantiany.cn/gtjdaiuhgs.html

JS:   async function f() { await g(); }
来源：http://hz.snrcjt.cn/gtwrhewmsx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shzxlz.cn/gthmtouinv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.aibaodan.cn/gttdnbxplv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.wangshuangyany.cn/gtutmokgfz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cashguo.top/gtyhmofdwm.html

C#:   async Task F() { await G(); }
来源：http://hz.shanyushiyangkeji.top/gtgefkeezy.html

[O05] 并发执行并等待全部完成
来源：http://hz.zdqjudy.top/gtyurhynwp.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gaohongyu789.top/gtqygluxkz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shzxlz.cn/gtcegsoslu.html

JS:   await Promise.all(tasks)
来源：http://hz.meibo888.top/gtxkcdquzi.html

TS:   await Promise.all(tasks)
来源：http://hz.0kj1m.cn/gtbrehshhn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.sxryk.cn/gtqxbzcpml.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jinqigfzy.top/gtdlhfgwyj.html

Ruby: threads.map(&:join)
来源：http://hz.jlsjyb.cn/gtobcxducc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yvedp.cn/gtvcbecdbe.html

[O06] 使用进程池
来源：http://hz.haohaochexian.top/gtgooyhyot.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.316326.xyz/gtsipaqwli.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.gogol.net.cn/gtzmtexwua.html

JS:   // child_process / cluster 模块
来源：http://hz.aizwys.cn/gtusreohwp.html

TS:   // child_process / cluster 模块
来源：http://hz.birdmap.top/gtkojdfrfw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.c1oappe.top/gtcsfzvrud.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hfpthk.cn/gtdcesdshz.html

Ruby: // fork 块
来源：http://hz.cucudq.cn/gtmltexbqo.html

C#:   Parallel.For
来源：http://hz.fzhhl.top/gtmwdrmjoy.html

================================================================================
来源：http://hz.cqqwz.cn/gtazjemnhu.html

P. 常用工具函数
来源：http://hz.snrcjt.cn/gtexvaouev.html

================================================================================
来源：http://hz.xuanzx.com/gthgjtbzms.html

[P01] 生成 UUID
来源：http://hz.aizwys.cn/gtsyzxocsp.html

Py:   str(uuid.uuid4())
来源：http://hz.pycfn.com/gtgwqhamhd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zdqjudy.top/gtiyxeboen.html

JS:   crypto.randomUUID()
来源：http://hz.dashuyun.cn/gtehurubtk.html

TS:   crypto.randomUUID()
来源：http://hz.cheryme.top/gtghpbizcx.html

Java: UUID.randomUUID().toString()
来源：http://hz.jqgufenzy.top/gtclnjhrfw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.daria6918.cn/gtjqfjywfa.html

Ruby: SecureRandom.uuid
来源：http://hz.yj20258888.top/gtasfmgewc.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.daxiang520.top/gtrcsugxif.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhaomingkeji.xyz/gtmqyfwhbv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.andypj.xyz/gtyvyidsmn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.guannengcc.top/gtvucwfhih.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.chenlongwang.top/gtbylrhhrw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ybcxt.top/gtdgpiryja.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ehwqpu.com/gtncgaqojk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.0kj1m.cn/gtmdhoxidj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jlsjyb.cn/gtrsvosiwu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.guowangkeji.top/gtgwmlfuaz.html

[P03] 生成短随机字符串
来源：http://hz.gogol.net.cn/gtvfugoesj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hywenlv.cn/gtvkoqhosp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ppjwa.cn/gtdskvetod.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nwbrower.top/gthbunioua.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenjidiqi.icu/gtfbubebum.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhongyouzk.top/gtqbrlzueh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cashguo.top/gtopiejyek.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zycfv.cn/gtkffjjzvx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jqgfzy.top/gtlkkoauyc.html

[P04] 求长度
来源：http://hz.chenzaomai.com/gtcpdhixki.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.pycfn.com/gtlwwdqkgr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yongpay.top/gtqgqlcvkl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.316326.xyz/gtolgyddvp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnxiangtu.top/gtsdrxdjmk.html


<!-- 参考信息 -->