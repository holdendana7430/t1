代发 wailian999

Py:   resp.json()
来源：http://hz.dashuyun.cn/gtllhfoxoy.html

PHP:  json_decode($body, true);
来源：http://hz.zhixingplan.top/gtiakwdwby.html

JS:   await resp.json()
来源：http://hz.sweek.top/gtdhmclpfs.html

TS:   await resp.json()
来源：http://hz.pycfn.com/gtazhaprxo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shanyushiyangkeji.top/gtxisexsmk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinqigfzy.top/gtjnrxuelm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jlsjyb.cn/gtsfdqlazs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xinyue.icu/gtcntbafso.html

[L07] 处理 HTTP 状态码
来源：http://hz.cashguo.top/gtojluhokv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.feifeiyinyue.top/gteujhvmfl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ppjwa.cn/gttscmhmds.html

JS:   resp.ok;  resp.status
来源：http://hz.jinqigufen.top/gtyrhmufra.html

TS:   resp.ok;  resp.status
来源：http://hz.jinqigfzy.top/gtdvkzmavr.html

Java: resp.statusCode()
来源：http://hz.meibo888.top/gtqorqkldw.html

Go:   resp.StatusCode
来源：http://hz.nwbrower.top/gtdancfxef.html

Ruby: resp.code.to_i
来源：http://hz.zhiwuduotai.top/gtjvqgmbwp.html

C#:   (int)resp.StatusCode
来源：http://hz.gaohongyu789.top/gtshxyhbnt.html

[L08] 并发请求多个地址
来源：http://hz.yonumen.top/gtewlczgsq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.vqdsnc.cn/gtqvmajqep.html

PHP:  curl_multi_init() 系列
来源：http://hz.ydzc1.top/gtpbzdtyre.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.iojbl.cn/gtabgtcwsz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258888.top/gtylsnlcjy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sxryk.cn/gtslqhnwlq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.nanxuanxn.top/gtvcgbfcdc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.svipenyu.cn/gtbeqsptwr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.dianchejie.cn/gtnhzspvkb.html

================================================================================
来源：http://hz.daxiang520.top/gtuwhyczxp.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhixingplan.top/gtyfgubfcr.html

================================================================================
来源：http://hz.cucudq.cn/gtksqtrqau.html

[M01] 读取命令行参数
来源：http://hz.tianlin.xyz/gtcdxsfsvo.html

Py:   sys.argv[1:]
来源：http://hz.fzhhl.top/gtxsmdwboh.html

PHP:  $argv;  $argc;
来源：http://hz.zhengqikj.top/gtspqlkdoj.html

JS:   process.argv.slice(2)
来源：http://hz.daxiang520.top/gtwrzpvuhk.html

TS:   process.argv.slice(2)
来源：http://hz.guowangkeji.top/gtzydmszkb.html

Java: args 数组（main 方法参数）
来源：http://hz.hammf.cn/gtermrnwkn.html

Go:   os.Args[1:]
来源：http://hz.hywenlv.cn/gtrqzhorkf.html

Ruby: ARGV
来源：http://hz.jiagoushi.top/gtrkweiwxz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhixingplan.top/gtecftpgkc.html

[M02] 读取环境变量
来源：http://hz.pycfn.com/gtlfiqtghh.html

Py:   os.environ.get("HOME")
来源：http://hz.cucudq.cn/gtwxugiojx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jianghu66.top/gtkqddayjd.html

JS:   process.env.HOME
来源：http://hz.chenjidiqi.icu/gttqhbujfn.html

TS:   process.env.HOME
来源：http://hz.jinqigfzy.top/gtsomkldms.html

Java: System.getenv("HOME")
来源：http://hz.hfpthk.cn/gtzsnnwphh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.guowangkeji.top/gtyyifdeao.html

Ruby: ENV["HOME"]
来源：http://hz.svipenyu.cn/gtagmtltcf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.quarkkingdee.top/gtcouyuipr.html

[M03] 执行外部命令
来源：http://hz.gotoacloud.top/gtpbecsbuj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.kuanghao11.cn/gtvjjtjlvu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.nanxuanxn.top/gttijmtqcc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ywan-chungtsiang.top/gtucxbdzyg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.daria6918.cn/gtpsfxkxwg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hfpthk.cn/gtnzauheov.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jqgfzy.top/gturhbzkyv.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.tian-w.cn/gtpxxpmkas.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sufxvd.cn/gtkpmcbpfi.html

[M04] 获取当前工作目录
来源：http://hz.cashguo.top/gtvbdizbfh.html

Py:   os.getcwd()
来源：http://hz.pengpengdd.cyou/gtcwtvlxff.html

PHP:  getcwd();
来源：http://hz.jlsjyb.cn/gtbuqobcye.html

JS:   process.cwd()
来源：http://hz.zhengqikj.top/gtnxirdziz.html

TS:   process.cwd()
来源：http://hz.hongshengwenyu.top/gtlxbermof.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.c1oappe.top/gtgruwwdqh.html

Go:   os.Getwd()
来源：http://hz.aibaodan.cn/gtnrfkqfvp.html

Ruby: Dir.pwd
来源：http://hz.xuetiantiany.cn/gtgijuppri.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.smart0.xyz/gtfdftgmgr.html

[M05] 设置退出码
来源：http://hz.xylfe.cn/gthyfiajot.html

Py:   sys.exit(1)
来源：http://hz.hywenlv.cn/gtifcjczco.html

PHP:  exit(1);
来源：http://hz.hysaishi.cn/gtgrwcipsl.html

JS:   process.exit(1)
来源：http://hz.yj20258.top/gtxeopxino.html

TS:   process.exit(1)
来源：http://hz.tanke756.top/gtgqeeekhc.html

Java: System.exit(1)
来源：http://hz.yuanzhike.top/gtfgqrdwuj.html

Go:   os.Exit(1)
来源：http://hz.vqdsnc.cn/gtthizrxol.html

Ruby: exit 1
来源：http://hz.yj202588.top/gtcyiguiar.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yongpay.top/gtwwurhohu.html

[M06] 向标准错误输出
来源：http://hz.bjfxy.top/gtmkkhqimb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cdnleiting.top/gtmxjfiymy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.c1oappe.top/gtpnwzzjqm.html

JS:   console.error("err")
来源：http://hz.zhijiandao.cn/gtzwjmawae.html

TS:   console.error("err")
来源：http://hz.redwolf501.top/gtazbmpabi.html

Java: System.err.println("err")
来源：http://hz.cashguo.top/gtxqhpzrjp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jlsjyb.cn/gtvelqbymg.html

Ruby: warn "err"
来源：http://hz.andypj.xyz/gttnxyfczv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cashguo.top/gtwlqaruhs.html

[M07] 判断是否为主入口
来源：http://hz.sysykeji.top/gtccgtrlcy.html

Py:   if __name__ == "__main__":
来源：http://hz.yongpay.top/gtsprzoiea.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.nwbrower.top/gtvdhyyinl.html

JS:   require.main === module
来源：http://hz.smart0.xyz/gtrjagejji.html

TS:   require.main === module
来源：http://hz.dianchejie.cn/gtwrghjtnm.html

Java: public static void main(String[] args)
来源：http://hz.chenzaomai.com/gtztsfleyb.html

Go:   func main()
来源：http://hz.tanke756.top/gtwoqpjncm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.andypj.xyz/gtpdnqcwmm.html

C#:   static void Main(string[] args)
来源：http://hz.cdnleiting.top/gttjjtzjeo.html

[M08] 获取系统与运行时信息
来源：http://hz.chenlongwang.top/gtgmaiynfo.html

Py:   platform.system();  platform.python_version()
来源：http://hz.snrcjt.cn/gtsvahxfno.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xingfuxueyuan.xyz/gtnhzmfsoc.html

JS:   process.platform;  process.version
来源：http://hz.hnxiangtu.top/gtsbgxezja.html

TS:   process.platform;  process.version
来源：http://hz.xingfuxueyuan.xyz/gtcaasmicn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.havefunace.top/gtwzoctpve.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xingfuxueyuan.xyz/gtqjmlypdq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ybcxt.top/gtfymsfbjw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sysykeji.top/gtvtrgehib.html

================================================================================
来源：http://hz.redwolf501.top/gteotyjjgx.html

N. 数据结构与算法
来源：http://hz.daria6918.cn/gtsjllydlc.html

================================================================================
来源：http://hz.iojbl.cn/gtdpjjcnkm.html

[N01] 二分查找（有序数组）
来源：http://hz.cdnleiting.top/gtcohqqyyz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yangfankeji.com/gtunggqjsd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jqgfzy.top/gtbuvjfqqc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hysaishi.cn/gthlxocdbw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cqqwz.cn/gtjtwuuspi.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yuxming.cn/gttfdyltuf.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xuetiantiany.cn/gtxjjpyacj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jqgfzy.top/gtlrlujras.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yj20258.top/gtgpxoqwpd.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.fzhhl.top/gtzqyfaxnb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cucudq.cn/gtlauosedn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sweek.top/gtngucqcyb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jqgfzy.top/gtjcdacvvi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gtnkrpxyga.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.pycfn.com/gtutgdpwem.html

Go:   slices.Sort(arr)
来源：http://hz.zycfv.cn/gtkgiadgqp.html

Ruby: arr.sort
来源：http://hz.jianghu66.top/gtgezksmkl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.wangshuangyany.cn/gtocqopbhs.html

[N03] 快速排序（分治示例）
来源：http://hz.9152youxi.cn/gtlzkoaveb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.birdmap.top/gtmvozmgio.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ehwqpu.com/gthdbgwqtv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nwbrower.top/gtlobtdvlz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tanke756.top/gtnntihtor.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.feifeiyinyue.top/gtvuozwhah.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.dashuyun.cn/gtjuqjrlwn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhaomingkeji.xyz/gteukpuuxj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gzhubu.top/gtvvfoupoz.html

[N04] 斐波那契数列
来源：http://hz.gaohongyu789.top/gtieuvndfn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.snrcjt.cn/gtfnprdiik.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.daria6918.cn/gtxwfwalqn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shuidangran.top/gtftaniurt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.bjfxy.top/gtmqulptec.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jinyuanbaomall.cn/gtsdkqeisz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ivvv.top/gtajyjyggt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.mhx1999.top/gtsdfvbyft.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hongshengwenyu.top/gtrplljtdc.html

[N05] 最大公约数
来源：http://hz.meibo888.top/gtnmqkgmfz.html

Py:   math.gcd(a, b)
来源：http://hz.shanyushiyangkeji.top/gtbbkbwkwu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.c1oappe.top/gtbrlbifur.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hammf.cn/gtphwmoybo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.andypj.xyz/gtkkbivvdx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xinyue.icu/gtzfitzkhr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.pycfn.com/gthueanhst.html

Ruby: a.gcd(b)
来源：http://hz.chenzaomai.com/gthqerflbo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jqgufenzy.top/gtylughvtu.html

[N06] 判断回文字符串
来源：http://hz.hnxiangtu.top/gtzyuyzsng.html

Py:   s == s[::-1]
来源：http://hz.cucudq.cn/gtybdcggko.html

PHP:  $s === strrev($s);
来源：http://hz.jyoumei.cn/gtmnrguyyc.html

JS:   s === [...s].reverse().join("")
来源：http://hz.meibo888.top/gtycqnoqqg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gthtlkcptn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hywenlv.cn/gtsdlputtx.html

Go:   // 双指针从两端比较
来源：http://hz.fengsongda.top/gtyqfckiif.html

Ruby: s == s.reverse
来源：http://hz.xylfe.cn/gtcytyervd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.nwbrower.top/gtzypviots.html

[N07] 两数之和（返回下标）
来源：http://hz.shzxlz.cn/gtzynusqtz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.sxryk.cn/gtubuqvymi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sweek.top/gtmzqtvtky.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xinyue.icu/gtlvivavtp.html

TS:   // 手写 Map<string, number>
来源：http://hz.pengpengdd.cyou/gtjadfxzmi.html

Java: // 手写 HashMap
来源：http://hz.yj20258888.top/gtuwmigzjm.html

Go:   // 手写 map[int]int
来源：http://hz.jinghuilouyu.cn/gtehdauyru.html

Ruby: // 手写 Hash
来源：http://hz.ydzc1.top/gtsgzssbeq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.smart0.xyz/gtdagnspst.html

[N08] 生成全排列
来源：http://hz.xuanzx.com/gtrrqvczho.html

Py:   itertools.permutations(arr)
来源：http://hz.ybcxt.top/gtofpracql.html

PHP:  // 手写递归交换
来源：http://hz.redwolf501.top/gtgdowihyw.html

JS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtngpooikr.html

TS:   // 手写回溯递归
来源：http://hz.havefunace.top/gtrmaurpds.html

Java: // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtfavubpem.html

Go:   // 手写回溯递归
来源：http://hz.yuanzhike.top/gteuzuqoog.html

Ruby: arr.permutation.to_a
来源：http://hz.zhongyouzk.top/gtzrxvahja.html

C#:   // 手写回溯递归
来源：http://hz.cqqwz.cn/gtdzqhlmek.html

[N09] 栈与队列
来源：http://hz.yj20258888.top/gtftgklrxy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.guannengcc.top/gtqleannuj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yueranfly.top/gtycqqbhym.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hywenlv.cn/gtbmvqfyly.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zycfv.cn/gtqkvcfzym.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shangyingyoupin.top/gtmgcbxoex.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.pengpengdd.cyou/gtxcsbvcyt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jiagoushi.top/gtdxwhvqfx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xziqi.cn/gtbgeyahfp.html

[N10] 链表节点定义
来源：http://hz.cucudq.cn/gtydyfpnql.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.fengsongda.top/gtdmecvtfh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xylfe.cn/gtuszjkort.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.haohaochexian.top/gtbkdmndyw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.aibaodan.cn/gtgxugbjct.html

Java: class Node { int v; Node next; }
来源：http://hz.shanyushiyangkeji.top/gtugphlbhn.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ywan-chungtsiang.top/gtfetsxexd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cdnleiting.top/gthmfcnwsg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jianghu66.top/gtjefuqerh.html

[N11] 二叉树中序遍历
来源：http://hz.daxiang520.top/gtehppzxaz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cashguo.top/gtoylrylcd.html

PHP:  // 手写递归函数
来源：http://hz.wangdashe.top/gtmmdcweri.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yvedp.cn/gtpfzoczcp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dashuyun.cn/gtmwjpuoiz.html

Java: // 手写递归
来源：http://hz.havefunace.top/gtrigdpbfl.html

Go:   // 手写递归
来源：http://hz.316326.xyz/gtypwsseed.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhaomingkeji.xyz/gtquljposc.html

C#:   // 手写递归
来源：http://hz.tianlin.xyz/gteivlrssf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.vqdsnc.cn/gtmnnbynny.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.wangdashe.top/gtcmymhwlp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.chenlongwang.top/gtzbtilqyl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hammf.cn/gtpaekylgk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgfzy.top/gtgbcxnzgu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.316326.xyz/gtggxlrjfc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.dashuyun.cn/gtwlncbtot.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xuanzx.com/gtdztktpqw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nwbrower.top/gthcwwmceo.html

================================================================================
来源：http://hz.vqdsnc.cn/gtlzpogrto.html

O. 并发与异步
来源：http://hz.cashguo.top/gtdqkpwcsi.html

================================================================================
来源：http://hz.dashuyun.cn/gttigxxhmd.html

[O01] 启动一个线程
来源：http://hz.chenzaomai.com/gtoanbegqq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yangfankeji.com/gtimfwdvpg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.pycfn.com/gtkapdaibl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fengsongda.top/gtwdzowpbz.html

TS:   // 同 JS
来源：http://hz.zhongyouzk.top/gtfxktvcqr.html

Java: new Thread(() -> f()).start()
来源：http://hz.hywenlv.cn/gtjwisbyrf.html

Go:   go f()
来源：http://hz.cdnleiting.top/gtjchwmvyg.html

Ruby: Thread.new { f }
来源：http://hz.yangfankeji.com/gtevoqsyen.html

C#:   Task.Run(() => F());
来源：http://hz.nanxuanxn.top/gtenwrnbvc.html

[O02] 使用线程池
来源：http://hz.fengsongda.top/gtjemfyiss.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.dashuyun.cn/gtpevugxbb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sysykeji.top/gtmvsmbezw.html

JS:   // worker_threads 线程池
来源：http://hz.redwolf501.top/gtrxzsjbpm.html

TS:   // worker_threads 线程池
来源：http://hz.jlsjyb.cn/gtmjmuwwup.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zdqjudy.top/gttflmxzvj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.316326.xyz/gtrgsyfcnq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.tianlin.xyz/gtmjtlxxvz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zycfv.cn/gtawqagpgt.html

[O03] 加锁保护共享数据
来源：http://hz.yj20258.top/gttvsyhodr.html

Py:   with lock: shared += 1
来源：http://hz.nanxuanxn.top/gtzlsajovf.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ybcxt.top/gtdnhbwylb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinqigfzy.top/gtxzwqdhrb.html

TS:   // 同 JS
来源：http://hz.haohaochexian.top/gtorlajwel.html

Java: synchronized (this) { shared++; }
来源：http://hz.shuidangran.top/gtuvjhvhvm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hfpthk.cn/gttdlxngva.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cucudq.cn/gtlmlmyhfr.html

C#:   lock (gate) { shared++; }
来源：http://hz.meibo888.top/gtmqiiwqte.html

[O04] 定义异步函数并等待
来源：http://hz.birdmap.top/gtnnwqaczn.html

Py:   async def f():⏎    await g()
来源：http://hz.yueranfly.top/gtomcjrjug.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ywan-chungtsiang.top/gtieflnizb.html

JS:   async function f() { await g(); }
来源：http://hz.shangyingyoupin.top/gtycneddtb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hfpthk.cn/gtjctcpvbi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.mhx1999.top/gtwzzqjqyq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xinyue.icu/gtihjukkdn.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.fzhhl.top/gtypcmpzqw.html

C#:   async Task F() { await G(); }
来源：http://hz.cdnleiting.top/gtmrrddsvj.html

[O05] 并发执行并等待全部完成
来源：http://hz.shanyushiyangtech.top/gtfsptlfkt.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ehwqpu.com/gtdskscnys.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yj20258.top/gtyihxgvgs.html

JS:   await Promise.all(tasks)
来源：http://hz.gotoacloud.top/gtdwlnzuxo.html

TS:   await Promise.all(tasks)
来源：http://hz.gzhubu.top/gtcebaganx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhiwuduotai.top/gtpktoeyej.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.pengpengdd.cyou/gtozwighbx.html

Ruby: threads.map(&:join)
来源：http://hz.gzhubu.top/gtwzkbekwo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.andypj.xyz/gtumrjqoeo.html

[O06] 使用进程池
来源：http://hz.cheryme.top/gtuquvnyhf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.kuanghao11.cn/gtpalzrpbk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hysaishi.cn/gtonymwqor.html

JS:   // child_process / cluster 模块
来源：http://hz.jinyuanbaomall.cn/gtrmmvxout.html

TS:   // child_process / cluster 模块
来源：http://hz.nanxuanxn.top/gtxryztswf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yvedp.cn/gtlbabtrvk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhongyouzk.top/gtiddjjvou.html

Ruby: // fork 块
来源：http://hz.sxryk.cn/gtwpohedal.html

C#:   Parallel.For
来源：http://hz.zhoulong.xyz/gtwnqwoaic.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtfogtjicn.html

P. 常用工具函数
来源：http://hz.xziqi.cn/gtaqqutctu.html

================================================================================
来源：http://hz.jyoumei.cn/gtohpdnies.html

[P01] 生成 UUID
来源：http://hz.yangfankeji.com/gtvgfokuny.html

Py:   str(uuid.uuid4())
来源：http://hz.hnxiangtu.top/gtidlxehfx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jqgfzy.top/gtlxdugyuz.html

JS:   crypto.randomUUID()
来源：http://hz.hongshengwenyu.top/gtbkkpqbma.html

TS:   crypto.randomUUID()
来源：http://hz.pycfn.com/gtuvjxkdxg.html

Java: UUID.randomUUID().toString()
来源：http://hz.cqqwz.cn/gtiqeyssve.html

Go:   // 用 github.com/google/uuid
来源：http://hz.pengpengdd.cyou/gtiqbvbbcu.html

Ruby: SecureRandom.uuid
来源：http://hz.snrcjt.cn/gtxxjwconi.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.feifeiyinyue.top/gtisixfers.html

[P02] MD5 / SHA256 摘要
来源：http://hz.nanxinkj.top/gtutpogdlm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.c1oappe.top/gtcnznvvwv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.havefunace.top/gtpelgwhmb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.guannengcc.top/gtkfgerriz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cqqwz.cn/gtlslmqmhg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.meibo888.top/gtdfyphsft.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.guannengcc.top/gthxyxnjas.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhongyouzk.top/gtsezairva.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ydzc1.top/gtvoofeivh.html

[P03] 生成短随机字符串
来源：http://hz.kuanghao11.cn/gtaiynleob.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shanyushiyangkeji.top/gttubtbctr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhixingplan.top/gtsdxybdlj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jiagoushi.top/gtrroblycq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hywenlv.cn/gtfwquknzp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.svipenyu.cn/gtnpbdxjmx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nanxuanxn.top/gtqvqbqtpv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhongyouzk.top/gtvyorlkoe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.tanke756.top/gtbkookrmi.html

[P04] 求长度
来源：http://hz.xuanzx.com/gtocfjoujl.html


<!-- 参考信息 -->