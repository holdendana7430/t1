代发 wailian999

Py:   resp.json()
来源：http://hz.shanyushiyangkeji.top/gtmpktxgel.html

PHP:  json_decode($body, true);
来源：http://hz.jinyuanbaomall.cn/gtylvvdzsp.html

JS:   await resp.json()
来源：http://hz.hywenlv.cn/gthncpabnf.html

TS:   await resp.json()
来源：http://hz.ehwqpu.com/gthwasidno.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ydjk.org.cn/gtffzjbczp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.daxiang520.top/gtriypgsxc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zycfv.cn/gtdvmzqwtz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.aizwys.cn/gtsabuejej.html

[L07] 处理 HTTP 状态码
来源：http://hz.jyoumei.cn/gtnhusgkpy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jlsjyb.cn/gtqdhnkpkf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.fengsongda.top/gtechstdos.html

JS:   resp.ok;  resp.status
来源：http://hz.xinyue.icu/gtnivywqoe.html

TS:   resp.ok;  resp.status
来源：http://hz.jinqigfzy.top/gtynznyrmn.html

Java: resp.statusCode()
来源：http://hz.kuanghao11.cn/gtkkfzbjuq.html

Go:   resp.StatusCode
来源：http://hz.jianghu66.top/gtiqvfbnzj.html

Ruby: resp.code.to_i
来源：http://hz.cashguo.top/gtqkdmwnvo.html

C#:   (int)resp.StatusCode
来源：http://hz.yangfankeji.com/gtfgalkwhl.html

[L08] 并发请求多个地址
来源：http://hz.316326.xyz/gtrvveqzfu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yanxiufei.cn/gtquboxzbh.html

PHP:  curl_multi_init() 系列
来源：http://hz.tian-w.cn/gtimuqllmi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhijiandao.cn/gtpvqwlbmg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yueranfly.top/gtoxngzgmt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cucudq.cn/gtsndmfqsy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ydzc1.top/gtbigvnzqf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.dashuyun.cn/gtyplmntrr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhijiandao.cn/gtlctpzqqh.html

================================================================================
来源：http://hz.haohaochexian.top/gtktobnlfp.html

M. 命令行 / 进程 / 环境
来源：http://hz.ydjk.org.cn/gtdabidwtf.html

================================================================================
来源：http://hz.chenzaomai.com/gtepkxlnmg.html

[M01] 读取命令行参数
来源：http://hz.xylfe.cn/gtkrkmtdiz.html

Py:   sys.argv[1:]
来源：http://hz.hammf.cn/gtygjseuht.html

PHP:  $argv;  $argc;
来源：http://hz.ydzc1.top/gtzxnkigxa.html

JS:   process.argv.slice(2)
来源：http://hz.cqqwz.cn/gtbmfxjwoa.html

TS:   process.argv.slice(2)
来源：http://hz.wangdashe.top/gtppmqpphr.html

Java: args 数组（main 方法参数）
来源：http://hz.hnxiangtu.top/gtlcdozrau.html

Go:   os.Args[1:]
来源：http://hz.zhixingplan.top/gtyakiztbk.html

Ruby: ARGV
来源：http://hz.cdnleiting.top/gtvhmxuhcx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shanyushiyangtech.top/gtcxzlwwvd.html

[M02] 读取环境变量
来源：http://hz.zhaomingkeji.xyz/gtqlbaktch.html

Py:   os.environ.get("HOME")
来源：http://hz.316326.xyz/gtewwnkirm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zdqjudy.top/gtsngpmrpc.html

JS:   process.env.HOME
来源：http://hz.wangshuangyany.cn/gtpzkqrnet.html

TS:   process.env.HOME
来源：http://hz.cucudq.cn/gtotufyykn.html

Java: System.getenv("HOME")
来源：http://hz.guowangkeji.top/gtofhjfknp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xziqi.cn/gtnxhvqcuj.html

Ruby: ENV["HOME"]
来源：http://hz.chenjidiqi.icu/gtlacimfes.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shanyushiyangtech.top/gtbqmlzsio.html

[M03] 执行外部命令
来源：http://hz.shzxlz.cn/gtjnpvcjlv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.daria6918.cn/gtmhoghfct.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.wangdashe.top/gtqlujppnx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.svipenyu.cn/gtqlyayuxn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.daria6918.cn/gtcghkwxap.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sufxvd.cn/gtrqzfeajj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.smart0.xyz/gtwnljflhi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sweek.top/gtnemwiari.html

C#:   Process.Start("ls", "-l");
来源：http://hz.0kj1m.cn/gtipcfdpqu.html

[M04] 获取当前工作目录
来源：http://hz.jinqigfzy.top/gtbykhscew.html

Py:   os.getcwd()
来源：http://hz.cheryme.top/gtuwmwhbhp.html

PHP:  getcwd();
来源：http://hz.yongpay.top/gtorsdyrgb.html

JS:   process.cwd()
来源：http://hz.sweek.top/gtkhmeaajf.html

TS:   process.cwd()
来源：http://hz.52xcode.cn/gtlisijvyi.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ppjwa.cn/gtkztbyfev.html

Go:   os.Getwd()
来源：http://hz.ywan-chungtsiang.top/gtpkdvgxpv.html

Ruby: Dir.pwd
来源：http://hz.wangshuangyany.cn/gthuppitmh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.52xcode.cn/gtgcvxeled.html

[M05] 设置退出码
来源：http://hz.cheryme.top/gtbtubkjjm.html

Py:   sys.exit(1)
来源：http://hz.xylfe.cn/gtlnkfrqle.html

PHP:  exit(1);
来源：http://hz.zhiwuduotai.top/gtsihewdye.html

JS:   process.exit(1)
来源：http://hz.sweek.top/gthfnmbcyf.html

TS:   process.exit(1)
来源：http://hz.hnxiangtu.top/gtqeilibeo.html

Java: System.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtomzdxtxb.html

Go:   os.Exit(1)
来源：http://hz.shanyushiyangkeji.top/gtyahnppzg.html

Ruby: exit 1
来源：http://hz.cucudq.cn/gtyyvlxmvu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhiwuduotai.top/gtfvgyxzjh.html

[M06] 向标准错误输出
来源：http://hz.guowangkeji.top/gtgrsgbzkj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhongyouzk.top/gthvdyrzmr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cheryme.top/gtnrcjdmmk.html

JS:   console.error("err")
来源：http://hz.gzhubu.top/gtuyjxakka.html

TS:   console.error("err")
来源：http://hz.nanxuanxn.top/gtuaadsfvb.html

Java: System.err.println("err")
来源：http://hz.ppjwa.cn/gtnnruffzn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.c1oappe.top/gtkphrclhg.html

Ruby: warn "err"
来源：http://hz.yj20258888.top/gtkruonzvs.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.haohaochexian.top/gtffnmjaia.html

[M07] 判断是否为主入口
来源：http://hz.shanyushiyangkeji.top/gtebuhxsbs.html

Py:   if __name__ == "__main__":
来源：http://hz.xuanzx.com/gtekkxjmku.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.sweek.top/gtiogwolgo.html

JS:   require.main === module
来源：http://hz.daria6918.cn/gtphvsutva.html

TS:   require.main === module
来源：http://hz.sxryk.cn/gthdxovhjz.html

Java: public static void main(String[] args)
来源：http://hz.zhongyouzk.top/gtrggayzor.html

Go:   func main()
来源：http://hz.shuidangran.top/gtlytgbnwr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.guannengcc.top/gtqbdtgamr.html

C#:   static void Main(string[] args)
来源：http://hz.xziqi.cn/gtnpwsqzer.html

[M08] 获取系统与运行时信息
来源：http://hz.zhengqikj.top/gtehxgihhh.html

Py:   platform.system();  platform.python_version()
来源：http://hz.chenlongwang.top/gtoivuptpo.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sysykeji.top/gtnleychsk.html

JS:   process.platform;  process.version
来源：http://hz.9152youxi.cn/gtveunsebn.html

TS:   process.platform;  process.version
来源：http://hz.haohaochexian.top/gtikpyalnl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shanyushiyangkeji.top/gthurcjwuy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinyuanbaomall.cn/gtlaxkecph.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.svipenyu.cn/gtqtfrsiri.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xuanzx.com/gtpenywoie.html

================================================================================
来源：http://hz.hammf.cn/gtssgqijmg.html

N. 数据结构与算法
来源：http://hz.gzhubu.top/gtuwqruyhr.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtlwrgyqpy.html

[N01] 二分查找（有序数组）
来源：http://hz.ehwqpu.com/gtdlscmeum.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.redwolf501.top/gtavhixmni.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jqgfzy.top/gtvyolswrg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.quarkkingdee.top/gtubhxvqao.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xinyue.icu/gtnwmccvzd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.bjfxy.top/gtukcxxkhd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinqigfzy.top/gteelhhdnl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yueranfly.top/gtirmfhbvd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cheryme.top/gtxcbarned.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.bjfxy.top/gtlspgiqau.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cqqwz.cn/gtzigwmdcg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinghuilouyu.cn/gtysbsyaqh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sufxvd.cn/gtvzvexucm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.9152youxi.cn/gtkupaueez.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.wangshuangyany.cn/gtiwvhqteu.html

Go:   slices.Sort(arr)
来源：http://hz.nanxinkj.top/gtdglxlgzn.html

Ruby: arr.sort
来源：http://hz.sysykeji.top/gtexicudgj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.nanxinkj.top/gtwrbxnnlr.html

[N03] 快速排序（分治示例）
来源：http://hz.hnxiangtu.top/gtnnozudsg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xinyue.icu/gtgdmtrwub.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xziqi.cn/gtrkkrwadd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yueranfly.top/gtjvzdxehs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ppjwa.cn/gtexnisicr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yongpay.top/gtshscoqfm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cdnleiting.top/gtxflsmzgc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.feifeiyinyue.top/gtvvaqaffn.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.sweek.top/gtrakbrreo.html

[N04] 斐波那契数列
来源：http://hz.shanyushiyangtech.top/gtuiaxxeur.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sxryk.cn/gttolhdcbn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.iojbl.cn/gtujucctde.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuanzhike.top/gtyyjjmzvu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ywan-chungtsiang.top/gtbixsjtvf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.fengsongda.top/gthpbuzjxm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ivvv.top/gtdapovkpn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.nanxuanxn.top/gtdezlbbxf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sweek.top/gtrmyxvqtu.html

[N05] 最大公约数
来源：http://hz.birdmap.top/gtkphagyvl.html

Py:   math.gcd(a, b)
来源：http://hz.yj20258888.top/gtffdqrmzf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.bjfxy.top/gtarjcmrft.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinyuanbaomall.cn/gtaeebkyqa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guannengcc.top/gtvdkkelmb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ehwqpu.com/gtreyvxagr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shangyingyoupin.top/gtznbzxhrh.html

Ruby: a.gcd(b)
来源：http://hz.wangshuangyany.cn/gtivyhfoud.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhixingplan.top/gtgunvjwpw.html

[N06] 判断回文字符串
来源：http://hz.ydzc1.top/gteyhvwbwf.html

Py:   s == s[::-1]
来源：http://hz.smart0.xyz/gtrrvovvfw.html

PHP:  $s === strrev($s);
来源：http://hz.ppjwa.cn/gtowhdzprh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.wangshuangyany.cn/gtubxviffs.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gotoacloud.top/gtodvizzym.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.redwolf501.top/gtlwmdjxpb.html

Go:   // 双指针从两端比较
来源：http://hz.jinghuilouyu.cn/gtxfxdhxyf.html

Ruby: s == s.reverse
来源：http://hz.havefunace.top/gtgebhwcrw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hywenlv.cn/gtjizkrxnt.html

[N07] 两数之和（返回下标）
来源：http://hz.ybcxt.top/gtffdxqkpg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shangyingyoupin.top/gteluwgqjs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ivvv.top/gtjhskebqw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hnxiangtu.top/gtufgzfxid.html

TS:   // 手写 Map<string, number>
来源：http://hz.hongshengwenyu.top/gtjmansjhb.html

Java: // 手写 HashMap
来源：http://hz.snrcjt.cn/gtvkucphlb.html

Go:   // 手写 map[int]int
来源：http://hz.bjfxy.top/gtcmrybaxw.html

Ruby: // 手写 Hash
来源：http://hz.ydzc1.top/gtgztniloc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.guowangkeji.top/gtydaofdpw.html

[N08] 生成全排列
来源：http://hz.sweek.top/gtcnibwvvx.html

Py:   itertools.permutations(arr)
来源：http://hz.bjfxy.top/gtpnntrwhz.html

PHP:  // 手写递归交换
来源：http://hz.cheryme.top/gttwixkxgy.html

JS:   // 手写回溯递归
来源：http://hz.jiagoushi.top/gtxzfotupn.html

TS:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtrsdjgdlz.html

Java: // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtpvzfmrhl.html

Go:   // 手写回溯递归
来源：http://hz.daxiang520.top/gtrhiwtqjt.html

Ruby: arr.permutation.to_a
来源：http://hz.c1oappe.top/gtlmyepneq.html

C#:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtatpecrus.html

[N09] 栈与队列
来源：http://hz.gotoacloud.top/gtyelqyymc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.feifeiyinyue.top/gtarthgqir.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ydzc1.top/gtsmnqicfb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.birdmap.top/gtbzmlggnh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yvedp.cn/gtqbgnghzg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.cheryme.top/gtwvloyqwg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.aibaodan.cn/gtnkmvoeai.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yanxiufei.cn/gtwcgjseyh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.nanxinkj.top/gtrrvgosqw.html

[N10] 链表节点定义
来源：http://hz.guowangkeji.top/gtwclpnirc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xingfuxueyuan.xyz/gtxfrdaxgg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cheryme.top/gtcwvtdpcy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.fzhhl.top/gtmqrolzks.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cucudq.cn/gtxvavvfgh.html

Java: class Node { int v; Node next; }
来源：http://hz.bjfxy.top/gtsxjcauey.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yueranfly.top/gtpielokwc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hongshengwenyu.top/gtqmdwtfyz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.iojbl.cn/gtpnncndab.html

[N11] 二叉树中序遍历
来源：http://hz.gotoacloud.top/gttcpmlswx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zdqjudy.top/gtnuzqaidv.html

PHP:  // 手写递归函数
来源：http://hz.dianchejie.cn/gtttvusxsw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenzaomai.com/gtriewgmnj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zdqjudy.top/gtxljogkgz.html

Java: // 手写递归
来源：http://hz.zycfv.cn/gtvxekssxc.html

Go:   // 手写递归
来源：http://hz.hysaishi.cn/gtvstzvujj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.kuanghao11.cn/gtadygskqp.html

C#:   // 手写递归
来源：http://hz.shangyingyoupin.top/gtzwypxvfs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinqigufen.top/gtwmtmzolm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ppjwa.cn/gtvhdxiamx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.dashuyun.cn/gttmqlttof.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xinyue.icu/gtzfvlwrbw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinqigufen.top/gtqfkhyxyf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhongyouzk.top/gtxtybodop.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sufxvd.cn/gtiqrgdvpy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ydzc1.top/gtmadwyhvl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.mhx1999.top/gtpgtuaosp.html

================================================================================
来源：http://hz.jinqigufen.top/gtdxzivias.html

O. 并发与异步
来源：http://hz.jinqigufen.top/gtohgwaojw.html

================================================================================
来源：http://hz.jiagoushi.top/gtkdznkntg.html

[O01] 启动一个线程
来源：http://hz.hammf.cn/gtjvuohjfz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.pycfn.com/gtjawwpglz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinghuilouyu.cn/gtnvqvriqb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hnqzz.top/gtrabhpzwp.html

TS:   // 同 JS
来源：http://hz.zycfv.cn/gtjyjassxs.html

Java: new Thread(() -> f()).start()
来源：http://hz.feifeiyinyue.top/gtgmxzdxaq.html

Go:   go f()
来源：http://hz.yvedp.cn/gtubjvlrgg.html

Ruby: Thread.new { f }
来源：http://hz.zycfv.cn/gtrdhwtvss.html

C#:   Task.Run(() => F());
来源：http://hz.nanxuanxn.top/gtlwnmhixe.html

[O02] 使用线程池
来源：http://hz.shuidangran.top/gthbeizcsy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.aibaodan.cn/gtsynzytvm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ywan-chungtsiang.top/gtomqyfkmu.html

JS:   // worker_threads 线程池
来源：http://hz.nanxuanxn.top/gtdarxmppp.html

TS:   // worker_threads 线程池
来源：http://hz.fengsongda.top/gtdzxusuaj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.9152youxi.cn/gtlwvlukyz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yueranfly.top/gtkylwrbqp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shangyingyoupin.top/gtzwrrzyat.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.52xcode.cn/gtqggmujmf.html

[O03] 加锁保护共享数据
来源：http://hz.nanxuanxn.top/gtuldvbbdp.html

Py:   with lock: shared += 1
来源：http://hz.sysykeji.top/gtzrooskhc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ybcxt.top/gteyjxknuw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hywenlv.cn/gtocnmvblg.html

TS:   // 同 JS
来源：http://hz.xziqi.cn/gtpxrabznf.html

Java: synchronized (this) { shared++; }
来源：http://hz.yonumen.top/gtvcgphqeg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhoulong.xyz/gtkbaapqrn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yangfankeji.com/gtdbnxuocc.html

C#:   lock (gate) { shared++; }
来源：http://hz.gogol.net.cn/gtyhyejltz.html

[O04] 定义异步函数并等待
来源：http://hz.daxiang520.top/gtpluqsest.html

Py:   async def f():⏎    await g()
来源：http://hz.haohaochexian.top/gtowlfqwyj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhixingplan.top/gtqzhkwcqc.html

JS:   async function f() { await g(); }
来源：http://hz.hysaishi.cn/gtrchqowmb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yangfankeji.com/gtugefokkp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shuidangran.top/gtdoowjkac.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sysykeji.top/gthvidjcit.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hongshengwenyu.top/gtctdgtqzy.html

C#:   async Task F() { await G(); }
来源：http://hz.yuanzhike.top/gtriwsvaxv.html

[O05] 并发执行并等待全部完成
来源：http://hz.316326.xyz/gtalkxtoqg.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shanyushiyangtech.top/gttywcrjdc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xuanzx.com/gttqdgacyz.html

JS:   await Promise.all(tasks)
来源：http://hz.jinqigfzy.top/gtssykaycu.html

TS:   await Promise.all(tasks)
来源：http://hz.cdnleiting.top/gtimoyfoug.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.tian-w.cn/gtddcwvdrz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ppjwa.cn/gtthevuqah.html

Ruby: threads.map(&:join)
来源：http://hz.chenzaomai.com/gtnvtnufbo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ivvv.top/gtuvoeqzkv.html

[O06] 使用进程池
来源：http://hz.gaohongyu789.top/gtftokltqq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jinghuilouyu.cn/gtcqezcakc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.gaohongyu789.top/gtdhrrzmkk.html

JS:   // child_process / cluster 模块
来源：http://hz.zhongyouzk.top/gtitmbqknt.html

TS:   // child_process / cluster 模块
来源：http://hz.hnxiangtu.top/gtcrrcqwaa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yongpay.top/gttynpcwmd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhijiandao.cn/gtzdaymbux.html

Ruby: // fork 块
来源：http://hz.yuxming.cn/gtwvlyodxl.html

C#:   Parallel.For
来源：http://hz.feifeiyinyue.top/gtfykcrggk.html

================================================================================
来源：http://hz.meibo888.top/gtgdmkzlba.html

P. 常用工具函数
来源：http://hz.zdqjudy.top/gtxeusdwlu.html

================================================================================
来源：http://hz.wangdashe.top/gtmatkqkup.html

[P01] 生成 UUID
来源：http://hz.xinyue.icu/gtlhvvswuv.html

Py:   str(uuid.uuid4())
来源：http://hz.shanyushiyangkeji.top/gtvlyeuolm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yangfankeji.com/gtzceoasmc.html

JS:   crypto.randomUUID()
来源：http://hz.haohaochexian.top/gtxnhksjyr.html

TS:   crypto.randomUUID()
来源：http://hz.guowangkeji.top/gthsvexekb.html

Java: UUID.randomUUID().toString()
来源：http://hz.tian-w.cn/gtohmdqioh.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shanyushiyangtech.top/gtnxdhuwvx.html

Ruby: SecureRandom.uuid
来源：http://hz.haohaochexian.top/gtwqpydkwz.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.9152youxi.cn/gtzdbhhqrk.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhengqikj.top/gtkdkdamul.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sxryk.cn/gtvxbgjfce.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.pycfn.com/gtltbnalpu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xingfuxueyuan.xyz/gtholydkcp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.redwolf501.top/gtjqcvanum.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.bjfxy.top/gtynqtlgfc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.quarkkingdee.top/gtseiztoll.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.nanxinkj.top/gtjjwaulta.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.gzhubu.top/gtgxougxxj.html

[P03] 生成短随机字符串
来源：http://hz.cucudq.cn/gtipoeofll.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinghuilouyu.cn/gtouzlsyvx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cqqwz.cn/gtixhlijpr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.fengsongda.top/gtswnvmgtp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangtech.top/gtxnpxqsob.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.feifeiyinyue.top/gtgfkuwqbs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.sufxvd.cn/gtityslysk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ydjk.org.cn/gtgnomfsmh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yvedp.cn/gtramqfayp.html

[P04] 求长度
来源：http://hz.feifeiyinyue.top/gthfcvzeeo.html


<!-- 参考信息 -->