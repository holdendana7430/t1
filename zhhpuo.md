代发 wailian999

Py:   resp.json()
来源：http://hz.fengsongda.top/gtwldqkljv.html

PHP:  json_decode($body, true);
来源：http://hz.zhijiandao.cn/gtxcumqfls.html

JS:   await resp.json()
来源：http://hz.sysykeji.top/gtraeiocue.html

TS:   await resp.json()
来源：http://hz.zhaomingkeji.xyz/gtoxyrylrg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yongpay.top/gtyqpruxew.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ybcxt.top/gtzkzibglm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhijiandao.cn/gtddrgeguj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.kuanghao11.cn/gtygfkuwsb.html

[L07] 处理 HTTP 状态码
来源：http://hz.svipenyu.cn/gtqcrpvwvb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sysykeji.top/gtpxtmqein.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhijiandao.cn/gttpznoniy.html

JS:   resp.ok;  resp.status
来源：http://hz.zhongyouzk.top/gtfwxexfjm.html

TS:   resp.ok;  resp.status
来源：http://hz.vqdsnc.cn/gttxutpsir.html

Java: resp.statusCode()
来源：http://hz.snrcjt.cn/gtgjzfxaip.html

Go:   resp.StatusCode
来源：http://hz.ybcxt.top/gtyisupcjq.html

Ruby: resp.code.to_i
来源：http://hz.zhengqikj.top/gtegphjogp.html

C#:   (int)resp.StatusCode
来源：http://hz.xinyue.icu/gtgnohgdni.html

[L08] 并发请求多个地址
来源：http://hz.daxiang520.top/gtsriukeic.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.mhx1999.top/gtnivoseru.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhengqikj.top/gtkqjgjfjq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tianlin.xyz/gttwthjtyo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aibaodan.cn/gtfxekwock.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ywan-chungtsiang.top/gtfnkrwfmf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yj202588.top/gtdcxjrgzr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xinyue.icu/gtgfyiyunj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cdnleiting.top/gtbiblyvdy.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtxkirlqkr.html

M. 命令行 / 进程 / 环境
来源：http://hz.0kj1m.cn/gttpfthhqe.html

================================================================================
来源：http://hz.quarkkingdee.top/gtihrspfnv.html

[M01] 读取命令行参数
来源：http://hz.hysaishi.cn/gtmpszjdba.html

Py:   sys.argv[1:]
来源：http://hz.hywenlv.cn/gtkuklvsst.html

PHP:  $argv;  $argc;
来源：http://hz.shanyushiyangtech.top/gtfrdohscl.html

JS:   process.argv.slice(2)
来源：http://hz.ybcxt.top/gtdrvcpicv.html

TS:   process.argv.slice(2)
来源：http://hz.c1oappe.top/gtyoecaing.html

Java: args 数组（main 方法参数）
来源：http://hz.iojbl.cn/gtxxlcgium.html

Go:   os.Args[1:]
来源：http://hz.hnqzz.top/gtiefzuaeu.html

Ruby: ARGV
来源：http://hz.quarkkingdee.top/gtvhyekyep.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jqgufenzy.top/gtimwknvfy.html

[M02] 读取环境变量
来源：http://hz.cdnleiting.top/gtmfqfruhu.html

Py:   os.environ.get("HOME")
来源：http://hz.andypj.xyz/gtkkauptwr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.dashuyun.cn/gtmptxzzpc.html

JS:   process.env.HOME
来源：http://hz.quarkkingdee.top/gtvthkegko.html

TS:   process.env.HOME
来源：http://hz.vqdsnc.cn/gtwortqbsw.html

Java: System.getenv("HOME")
来源：http://hz.vqdsnc.cn/gtmzfqhfpa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sweek.top/gthkhmnzvu.html

Ruby: ENV["HOME"]
来源：http://hz.nwbrower.top/gtbvmipfpu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gotoacloud.top/gtnzphvnam.html

[M03] 执行外部命令
来源：http://hz.sweek.top/gtmnyluugh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xuanzx.com/gttxzdergd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.mhx1999.top/gtpozcmgmg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj20258888.top/gtwztwfnrs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuxming.cn/gtkdxzodtu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.birdmap.top/gtuczzgyke.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ywan-chungtsiang.top/gtimxgtdol.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.nanxinkj.top/gtelrtyltj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yongpay.top/gtjoamqoni.html

[M04] 获取当前工作目录
来源：http://hz.zhijiandao.cn/gtzreqmgts.html

Py:   os.getcwd()
来源：http://hz.cdnleiting.top/gtajuwjdnh.html

PHP:  getcwd();
来源：http://hz.tanke756.top/gtohseqbbd.html

JS:   process.cwd()
来源：http://hz.shzxlz.cn/gtiqgvnodd.html

TS:   process.cwd()
来源：http://hz.tianlin.xyz/gtwhzvhfkq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jqgfzy.top/gtstacoawj.html

Go:   os.Getwd()
来源：http://hz.quarkkingdee.top/gtiawsmfad.html

Ruby: Dir.pwd
来源：http://hz.smart0.xyz/gtcxwiqflw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.guowangkeji.top/gtmfztmzan.html

[M05] 设置退出码
来源：http://hz.hywenlv.cn/gthgkegqwd.html

Py:   sys.exit(1)
来源：http://hz.xuetiantiany.cn/gtfwaswnzo.html

PHP:  exit(1);
来源：http://hz.sufxvd.cn/gtswvitkwr.html

JS:   process.exit(1)
来源：http://hz.xinyue.icu/gtvsjlwwsx.html

TS:   process.exit(1)
来源：http://hz.ybcxt.top/gtqkxyjgqg.html

Java: System.exit(1)
来源：http://hz.ehwqpu.com/gthbwoeboc.html

Go:   os.Exit(1)
来源：http://hz.dianchejie.cn/gtyypqzwqu.html

Ruby: exit 1
来源：http://hz.xingfuxueyuan.xyz/gtvbguglmx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.dianchejie.cn/gtzgeuqmbg.html

[M06] 向标准错误输出
来源：http://hz.jqgufenzy.top/gtbdgwtwit.html

Py:   print("err", file=sys.stderr)
来源：http://hz.birdmap.top/gtgvcafwam.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.tianlin.xyz/gtlacydzng.html

JS:   console.error("err")
来源：http://hz.svipenyu.cn/gtrsxhrlii.html

TS:   console.error("err")
来源：http://hz.ydjk.org.cn/gtucjfeylj.html

Java: System.err.println("err")
来源：http://hz.yvedp.cn/gtwyzpzrxt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.havefunace.top/gtuuwbuusk.html

Ruby: warn "err"
来源：http://hz.c1oappe.top/gtiavlvxdr.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.svipenyu.cn/gtfdxwgtlx.html

[M07] 判断是否为主入口
来源：http://hz.guowangkeji.top/gtatrzvfjq.html

Py:   if __name__ == "__main__":
来源：http://hz.mhx1999.top/gtanjipkwo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yj20258888.top/gtfzbaeghv.html

JS:   require.main === module
来源：http://hz.wangdashe.top/gtnritwkyb.html

TS:   require.main === module
来源：http://hz.xinyue.icu/gtohztvojm.html

Java: public static void main(String[] args)
来源：http://hz.jianghu66.top/gtzavpcmtt.html

Go:   func main()
来源：http://hz.havefunace.top/gtwdgfoebl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinqigufen.top/gthuudxhpe.html

C#:   static void Main(string[] args)
来源：http://hz.tianlin.xyz/gtpfqzuidu.html

[M08] 获取系统与运行时信息
来源：http://hz.nanxinkj.top/gtdnnaunyw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.tianlin.xyz/gtznwqhgyg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenzaomai.com/gtsbhcwymp.html

JS:   process.platform;  process.version
来源：http://hz.hywenlv.cn/gtxiiqrzsw.html

TS:   process.platform;  process.version
来源：http://hz.zhoulong.xyz/gtkpghidfn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yueranfly.top/gtfhlfkjlj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yvedp.cn/gtgpogbpva.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hnqzz.top/gtxuzfezni.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jiagoushi.top/gtrrjmnglf.html

================================================================================
来源：http://hz.sufxvd.cn/gtcbzhcdcp.html

N. 数据结构与算法
来源：http://hz.dianchejie.cn/gtxwbcwzfw.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtolrlcnqq.html

[N01] 二分查找（有序数组）
来源：http://hz.birdmap.top/gtoimsbrgq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sxryk.cn/gtvewxqvwd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shanyushiyangtech.top/gtkrpyljhw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.52xcode.cn/gtlxnmpxdp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangshuangyany.cn/gtvyguinxz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jianghu66.top/gtfoohsbdj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hywenlv.cn/gtykjgcdbp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xziqi.cn/gtwdcckbgx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.dashuyun.cn/gtbeztyqai.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ehwqpu.com/gtnmegkgzo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.52xcode.cn/gtbuuthlds.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nanxinkj.top/gtxvsckiwr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jlsjyb.cn/gtofahbzti.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.iojbl.cn/gtxidjrnuf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.nanxinkj.top/gtwaimrjyd.html

Go:   slices.Sort(arr)
来源：http://hz.nanxuanxn.top/gtmmisxjws.html

Ruby: arr.sort
来源：http://hz.ehwqpu.com/gtpxvjzrel.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinqigfzy.top/gttgosfxbs.html

[N03] 快速排序（分治示例）
来源：http://hz.ppjwa.cn/gtzemnffzp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.316326.xyz/gtgfjhqgpi.html

PHP:  // 递归实现，或用 usort
来源：http://hz.9152youxi.cn/gtydllsavo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dashuyun.cn/gtnwaclobr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj20258888.top/gtpkbiimpi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinyuanbaomall.cn/gtfskfmrzp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yuxming.cn/gtalusprlj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.iojbl.cn/gtjvxixici.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zdqjudy.top/gtgoylmvod.html

[N04] 斐波那契数列
来源：http://hz.shzxlz.cn/gtscudilpi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.birdmap.top/gticooltwk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.bjfxy.top/gttxwnexwq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258888.top/gtabkapvnc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xingfuxueyuan.xyz/gttsipfbmg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gaohongyu789.top/gtuecrikie.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xuetiantiany.cn/gtlhpjqubv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258.top/gtorhpeaqg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhongyouzk.top/gttlgfqgjc.html

[N05] 最大公约数
来源：http://hz.yangfankeji.com/gtvlogqwpf.html

Py:   math.gcd(a, b)
来源：http://hz.cqqwz.cn/gtsnmplzqd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.birdmap.top/gtepitbdct.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ybcxt.top/gtpemjeqoh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guowangkeji.top/gtaqapghwm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.havefunace.top/gtewewsadh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zycfv.cn/gtxtiplkjy.html

Ruby: a.gcd(b)
来源：http://hz.dashuyun.cn/gtbczuxonc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yangfankeji.com/gtbrczxwpk.html

[N06] 判断回文字符串
来源：http://hz.fzhhl.top/gtfwsxljfs.html

Py:   s == s[::-1]
来源：http://hz.316326.xyz/gtivbjwrhn.html

PHP:  $s === strrev($s);
来源：http://hz.shzxlz.cn/gtkrvpxipq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cqqwz.cn/gtrumobmhc.html

TS:   s === [...s].reverse().join("")
来源：http://hz.fengsongda.top/gtqdrxlgrr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.haohaochexian.top/gtlkwsnfiy.html

Go:   // 双指针从两端比较
来源：http://hz.fengsongda.top/gtwdwahxpe.html

Ruby: s == s.reverse
来源：http://hz.zdqjudy.top/gtabpcibez.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ehwqpu.com/gttehqyggy.html

[N07] 两数之和（返回下标）
来源：http://hz.mhx1999.top/gttycwmjmt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhongyouzk.top/gtgloxnhor.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.nwbrower.top/gtutvociia.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zycfv.cn/gthcdkudmy.html

TS:   // 手写 Map<string, number>
来源：http://hz.hnxiangtu.top/gtsyyqjyex.html

Java: // 手写 HashMap
来源：http://hz.guowangkeji.top/gtkbnikdfj.html

Go:   // 手写 map[int]int
来源：http://hz.shangyingyoupin.top/gtyijkmjjq.html

Ruby: // 手写 Hash
来源：http://hz.wangshuangyany.cn/gtulipwwfx.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.pengpengdd.cyou/gtxrprjnqu.html

[N08] 生成全排列
来源：http://hz.meibo888.top/gtuydvfkiw.html

Py:   itertools.permutations(arr)
来源：http://hz.zdqjudy.top/gtupmzskfc.html

PHP:  // 手写递归交换
来源：http://hz.daria6918.cn/gtgymsbfrh.html

JS:   // 手写回溯递归
来源：http://hz.cashguo.top/gtbnjdcnan.html

TS:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtsxtcndxq.html

Java: // 手写回溯递归
来源：http://hz.jianghu66.top/gtwxpyhlar.html

Go:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtvyipycsh.html

Ruby: arr.permutation.to_a
来源：http://hz.vqdsnc.cn/gtlzsnzjlw.html

C#:   // 手写回溯递归
来源：http://hz.snrcjt.cn/gtiiltxkxt.html

[N09] 栈与队列
来源：http://hz.hnxiangtu.top/gtrijkxxzu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.dashuyun.cn/gtzfypugib.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhengqikj.top/gtpkqvnzqy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.9152youxi.cn/gtqniyrksg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinqigufen.top/gtlasddooo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jqgfzy.top/gtepkgevyb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinghuilouyu.cn/gtaawixjgq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.vqdsnc.cn/gtxefwdpkf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gzhubu.top/gtknutneoe.html

[N10] 链表节点定义
来源：http://hz.zhixingplan.top/gtyzzvppfl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.tian-w.cn/gtiherwllt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinghuilouyu.cn/gtryltgdlr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ehwqpu.com/gtdjekmkvn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hysaishi.cn/gtoqlhkpia.html

Java: class Node { int v; Node next; }
来源：http://hz.zhongyouzk.top/gtgewgbtyo.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yvedp.cn/gtiqqwuiqp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hongshengwenyu.top/gtifmqbmgi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.pengpengdd.cyou/gtbtfzxsyk.html

[N11] 二叉树中序遍历
来源：http://hz.dianchejie.cn/gtyvfmwupp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.redwolf501.top/gtfcrkgnny.html

PHP:  // 手写递归函数
来源：http://hz.yangfankeji.com/gteevytxhc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cqqwz.cn/gtznrqhltg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aizwys.cn/gtupwkxybd.html

Java: // 手写递归
来源：http://hz.vqdsnc.cn/gtzfelsfyc.html

Go:   // 手写递归
来源：http://hz.jinqigfzy.top/gtikfcubyl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.haohaochexian.top/gtfkzyxdav.html

C#:   // 手写递归
来源：http://hz.fengsongda.top/gtnctlvytk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.iojbl.cn/gthjkqhgvc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.redwolf501.top/gtyjekezbu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gogol.net.cn/gtbutrsort.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tian-w.cn/gthgovioka.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.birdmap.top/gtdhtdbibf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ivvv.top/gtuqejmgxl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.gaohongyu789.top/gtqkogdcjz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.nanxinkj.top/gtagpqjpyx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangkeji.top/gtpxnobltr.html

================================================================================
来源：http://hz.yueranfly.top/gtoxwbqfan.html

O. 并发与异步
来源：http://hz.yanxiufei.cn/gtsgntpoaq.html

================================================================================
来源：http://hz.dashuyun.cn/gtlnzcxgvx.html

[O01] 启动一个线程
来源：http://hz.jqgufenzy.top/gtvfrhrknh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.bjfxy.top/gtdsjjvvdm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.feifeiyinyue.top/gtxoozntlb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fzhhl.top/gtpbrxldsq.html

TS:   // 同 JS
来源：http://hz.tanke756.top/gtqyqpsgeb.html

Java: new Thread(() -> f()).start()
来源：http://hz.xinyue.icu/gtullptidl.html

Go:   go f()
来源：http://hz.xinyue.icu/gtvndmxhbk.html

Ruby: Thread.new { f }
来源：http://hz.yanxiufei.cn/gtxlgslcwc.html

C#:   Task.Run(() => F());
来源：http://hz.yj20258.top/gttiflpdeq.html

[O02] 使用线程池
来源：http://hz.xuanzx.com/gtxficmezb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yj202588.top/gtjwoosumk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhengqikj.top/gtqrkdhjqx.html

JS:   // worker_threads 线程池
来源：http://hz.hnxiangtu.top/gtkwtyycdv.html

TS:   // worker_threads 线程池
来源：http://hz.316326.xyz/gtmhfmaauf.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xylfe.cn/gtezdhuexo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jqgufenzy.top/gtbrbfbkxv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.quarkkingdee.top/gtnevbdnzm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ydjk.org.cn/gtqkwdvmda.html

[O03] 加锁保护共享数据
来源：http://hz.hysaishi.cn/gtlmphbthv.html

Py:   with lock: shared += 1
来源：http://hz.chenjidiqi.icu/gtxzormzqo.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.tanke756.top/gthrznhitc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.fzhhl.top/gtslcxpeyt.html

TS:   // 同 JS
来源：http://hz.hywenlv.cn/gtyoiunqdj.html

Java: synchronized (this) { shared++; }
来源：http://hz.cqqwz.cn/gtgbuvxmhv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shzxlz.cn/gtqywdoiyq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ppjwa.cn/gtuebsgbkb.html

C#:   lock (gate) { shared++; }
来源：http://hz.yanxiufei.cn/gtljulodud.html

[O04] 定义异步函数并等待
来源：http://hz.feifeiyinyue.top/gtoefasqlw.html

Py:   async def f():⏎    await g()
来源：http://hz.yuxming.cn/gthczkqsfa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhixingplan.top/gtvqrgagjo.html

JS:   async function f() { await g(); }
来源：http://hz.jqgfzy.top/gtfhygcfgz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cqqwz.cn/gtxklqmdia.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhongyouzk.top/gtagectxtr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shangyingyoupin.top/gtkfuqlcuz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.guowangkeji.top/gtvdtowdxc.html

C#:   async Task F() { await G(); }
来源：http://hz.jqgufenzy.top/gteywnkdsh.html

[O05] 并发执行并等待全部完成
来源：http://hz.shzxlz.cn/gtpzslgnzn.html

Py:   asyncio.gather(*tasks)
来源：http://hz.bjfxy.top/gtcyvbszak.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhijiandao.cn/gtfhtkwjzs.html

JS:   await Promise.all(tasks)
来源：http://hz.hammf.cn/gtvokelgeh.html

TS:   await Promise.all(tasks)
来源：http://hz.chenzaomai.com/gtqrugkjar.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shanyushiyangtech.top/gtftbrdbts.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sxryk.cn/gtdwoezyyr.html

Ruby: threads.map(&:join)
来源：http://hz.sufxvd.cn/gtyafzxsoi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.c1oappe.top/gtbozivdnf.html

[O06] 使用进程池
来源：http://hz.wangshuangyany.cn/gtpkhvdpaa.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.birdmap.top/gtoswdrmvw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxinkj.top/gtaweycnwl.html

JS:   // child_process / cluster 模块
来源：http://hz.wangshuangyany.cn/gtwejraetw.html

TS:   // child_process / cluster 模块
来源：http://hz.svipenyu.cn/gtajbtyjci.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.pycfn.com/gttnykdzoi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nanxuanxn.top/gtehfftxwj.html

Ruby: // fork 块
来源：http://hz.svipenyu.cn/gtnqfpsevc.html

C#:   Parallel.For
来源：http://hz.nanxinkj.top/gtalrhvjli.html

================================================================================
来源：http://hz.ydzc1.top/gtvlqzyzcb.html

P. 常用工具函数
来源：http://hz.xinyue.icu/gttvjfguxj.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtxrlidzjg.html

[P01] 生成 UUID
来源：http://hz.xylfe.cn/gtkfemxpfc.html

Py:   str(uuid.uuid4())
来源：http://hz.gaohongyu789.top/gtvhqkmdwh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinqigufen.top/gtjqgzumma.html

JS:   crypto.randomUUID()
来源：http://hz.jinqigufen.top/gtktszfhsb.html

TS:   crypto.randomUUID()
来源：http://hz.ydjk.org.cn/gtmfsrwdac.html

Java: UUID.randomUUID().toString()
来源：http://hz.shanyushiyangtech.top/gtpslkjkhq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jqgufenzy.top/gtkbkqjene.html

Ruby: SecureRandom.uuid
来源：http://hz.pengpengdd.cyou/gtkhagibee.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ybcxt.top/gtqdansymb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.mhx1999.top/gtiqdheqen.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.wangshuangyany.cn/gtlkzjarqa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.bjfxy.top/gtuczcdysn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.pengpengdd.cyou/gtkyfnpccp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cheryme.top/gtqyrqeemu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.52xcode.cn/gtrydbibct.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jiagoushi.top/gtblckcjaa.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yangfankeji.com/gtucirtmnk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shuidangran.top/gthjrhnvhk.html

[P03] 生成短随机字符串
来源：http://hz.haohaochexian.top/gthgmsgobn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.meibo888.top/gtcseyeull.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ydzc1.top/gtetupbzwq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.quarkkingdee.top/gtswpiphqm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuetiantiany.cn/gtskvefoyt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cdnleiting.top/gtyjnssawb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nwbrower.top/gtrtqzpybp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.c1oappe.top/gtlfaqmkyb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hywenlv.cn/gtxwhmcaqu.html

[P04] 求长度
来源：http://hz.zycfv.cn/gtiqzkygex.html


<!-- 参考信息 -->