代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhaomingkeji.xyz/gtquvwswvy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.andypj.xyz/gttrsavimy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.nwbrower.top/gtgydyykpn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.redwolf501.top/gtdabalkvf.html

[L07] 处理 HTTP 状态码
来源：http://hz.sysykeji.top/gtkwidqgfk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.c1oappe.top/gtcnuhdpri.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xuanzx.com/gtjraqzaez.html

JS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gtecoiikkx.html

TS:   resp.ok;  resp.status
来源：http://hz.gaohongyu789.top/gtgejnvoka.html

Java: resp.statusCode()
来源：http://hz.yanxiufei.cn/gtrxyekluo.html

Go:   resp.StatusCode
来源：http://hz.ywan-chungtsiang.top/gtntqvohyt.html

Ruby: resp.code.to_i
来源：http://hz.cashguo.top/gttjyehyip.html

C#:   (int)resp.StatusCode
来源：http://hz.zhongyouzk.top/gttwrfkfno.html

[L08] 并发请求多个地址
来源：http://hz.zhijiandao.cn/gtysfwuwqf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.wangshuangyany.cn/gtutnkftdt.html

PHP:  curl_multi_init() 系列
来源：http://hz.yuxming.cn/gtqncgzdmt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhijiandao.cn/gtugdooeiv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.c1oappe.top/gtxoazwfaa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xuetiantiany.cn/gtogmrsblu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zycfv.cn/gtkcvsypnz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinghuilouyu.cn/gtasrkndla.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jianghu66.top/gtoodwpmmx.html

================================================================================
来源：http://hz.cheryme.top/gtvzdrikik.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhongyouzk.top/gtmrjpgjti.html

================================================================================
来源：http://hz.c1oappe.top/gtftakdeou.html

[M01] 读取命令行参数
来源：http://hz.feifeiyinyue.top/gtsoptiwps.html

Py:   sys.argv[1:]
来源：http://hz.gotoacloud.top/gtmtgjoxcl.html

PHP:  $argv;  $argc;
来源：http://hz.zhiwuduotai.top/gtvqlprcpr.html

JS:   process.argv.slice(2)
来源：http://hz.ydjk.org.cn/gtraoqvgue.html

TS:   process.argv.slice(2)
来源：http://hz.fzhhl.top/gtwvoxghor.html

Java: args 数组（main 方法参数）
来源：http://hz.zdqjudy.top/gtupevxxnd.html

Go:   os.Args[1:]
来源：http://hz.zhiwuduotai.top/gtlktjlixp.html

Ruby: ARGV
来源：http://hz.cdnleiting.top/gtpfxwkuii.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shuidangran.top/gtyaabegci.html

[M02] 读取环境变量
来源：http://hz.shanyushiyangkeji.top/gtzsxqheeh.html

Py:   os.environ.get("HOME")
来源：http://hz.gaohongyu789.top/gtdhxakbhb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sysykeji.top/gtfeitmbma.html

JS:   process.env.HOME
来源：http://hz.smart0.xyz/gtpcxwabni.html

TS:   process.env.HOME
来源：http://hz.xinyue.icu/gttcfiqlbj.html

Java: System.getenv("HOME")
来源：http://hz.ppjwa.cn/gtnyyjmgxy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hysaishi.cn/gtptoacoqu.html

Ruby: ENV["HOME"]
来源：http://hz.yuxming.cn/gtxgptgogf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.52xcode.cn/gtgngdufcr.html

[M03] 执行外部命令
来源：http://hz.jiagoushi.top/gtdirvrmzo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.52xcode.cn/gtaumtmayq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yangfankeji.com/gtwcfyhchm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.tanke756.top/gtuaabdsro.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zdqjudy.top/gtntvkeuji.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinqigfzy.top/gttlylqtwu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hongshengwenyu.top/gtlxonzekl.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shangyingyoupin.top/gtyaedmvhb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xingfuxueyuan.xyz/gtzuskbamz.html

[M04] 获取当前工作目录
来源：http://hz.daxiang520.top/gtdbrczrwy.html

Py:   os.getcwd()
来源：http://hz.tian-w.cn/gtfzjxwubx.html

PHP:  getcwd();
来源：http://hz.yanxiufei.cn/gtmptbbtzw.html

JS:   process.cwd()
来源：http://hz.hywenlv.cn/gthrujonrf.html

TS:   process.cwd()
来源：http://hz.jianghu66.top/gthdgwhsfs.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.fzhhl.top/gttfbhwfhk.html

Go:   os.Getwd()
来源：http://hz.iojbl.cn/gtpvucvfdw.html

Ruby: Dir.pwd
来源：http://hz.jianghu66.top/gtcuyghhoc.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xylfe.cn/gtjeemkasu.html

[M05] 设置退出码
来源：http://hz.bjfxy.top/gtvebkjfii.html

Py:   sys.exit(1)
来源：http://hz.316326.xyz/gtybqrhgof.html

PHP:  exit(1);
来源：http://hz.ppjwa.cn/gtrpfucnfu.html

JS:   process.exit(1)
来源：http://hz.jinghuilouyu.cn/gtmobeifzy.html

TS:   process.exit(1)
来源：http://hz.nanxuanxn.top/gtsrjaizvt.html

Java: System.exit(1)
来源：http://hz.ybcxt.top/gtduqoqspn.html

Go:   os.Exit(1)
来源：http://hz.cqqwz.cn/gtkffksobl.html

Ruby: exit 1
来源：http://hz.zhoulong.xyz/gtqtncimfz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.c1oappe.top/gtkuibuqoz.html

[M06] 向标准错误输出
来源：http://hz.hywenlv.cn/gtajgecdxr.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinghuilouyu.cn/gtujmztuzc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.aibaodan.cn/gtremjhwqd.html

JS:   console.error("err")
来源：http://hz.zdqjudy.top/gtyemqfrpx.html

TS:   console.error("err")
来源：http://hz.guowangkeji.top/gtdhmrfyhf.html

Java: System.err.println("err")
来源：http://hz.cucudq.cn/gtoqoglqmo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.9152youxi.cn/gtqvtzzorw.html

Ruby: warn "err"
来源：http://hz.yonumen.top/gtldjjrvqn.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.316326.xyz/gthurjxgvn.html

[M07] 判断是否为主入口
来源：http://hz.xziqi.cn/gtvarkswlm.html

Py:   if __name__ == "__main__":
来源：http://hz.bjfxy.top/gtuauxdykk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhongyouzk.top/gtxddrxacr.html

JS:   require.main === module
来源：http://hz.jinqigfzy.top/gtlphpezld.html

TS:   require.main === module
来源：http://hz.quarkkingdee.top/gtocjhvxwg.html

Java: public static void main(String[] args)
来源：http://hz.yuxming.cn/gtfdjcknbx.html

Go:   func main()
来源：http://hz.xinyue.icu/gtpqkhnwme.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhoulong.xyz/gtfidhztnc.html

C#:   static void Main(string[] args)
来源：http://hz.hongshengwenyu.top/gtdmthorvq.html

[M08] 获取系统与运行时信息
来源：http://hz.quarkkingdee.top/gtbkjipjur.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ywan-chungtsiang.top/gtcqovqegb.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jqgufenzy.top/gtfotfdmqq.html

JS:   process.platform;  process.version
来源：http://hz.zycfv.cn/gtzunmrqyj.html

TS:   process.platform;  process.version
来源：http://hz.daria6918.cn/gtgvbochbb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tanke756.top/gteyiawniz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jianghu66.top/gtdwnywnje.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jyoumei.cn/gtjbnhbeny.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.tanke756.top/gtdcugouiv.html

================================================================================
来源：http://hz.cheryme.top/gtjzmsodge.html

N. 数据结构与算法
来源：http://hz.iojbl.cn/gtdspwjmui.html

================================================================================
来源：http://hz.chenlongwang.top/gtxyjijauv.html

[N01] 二分查找（有序数组）
来源：http://hz.wangdashe.top/gtwhhfdwhe.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sxryk.cn/gtyptqjjqd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sufxvd.cn/gtshwkqhyn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.birdmap.top/gtgbacvbcn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nwbrower.top/gtowggussd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hywenlv.cn/gtgmngyoea.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jqgufenzy.top/gtciucwugk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yangfankeji.com/gtqpfjimtn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.chenlongwang.top/gtrgpxlzgn.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.nanxinkj.top/gtyayfqzyo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigfzy.top/gtwcdquhmk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yuxming.cn/gtkyekbvax.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yvedp.cn/gtogwbsrxt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gtpujmurmq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yj202588.top/gtinkwxhmj.html

Go:   slices.Sort(arr)
来源：http://hz.xziqi.cn/gthuskoicw.html

Ruby: arr.sort
来源：http://hz.yuxming.cn/gtaypfvbja.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sufxvd.cn/gtwlclgrre.html

[N03] 快速排序（分治示例）
来源：http://hz.jianghu66.top/gtwpuvrglt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ybcxt.top/gtnxzslzfo.html

PHP:  // 递归实现，或用 usort
来源：http://hz.wangdashe.top/gtxebbakjp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jianghu66.top/gtlwfojvpv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gaohongyu789.top/gtnliuqwvx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cucudq.cn/gtsiwwesvv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xziqi.cn/gtebwwjjmm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.smart0.xyz/gtfufassaj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.316326.xyz/gthvubtsvz.html

[N04] 斐波那契数列
来源：http://hz.vqdsnc.cn/gtnwqpxqxo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shuidangran.top/gtpuavtcqb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.guowangkeji.top/gtiqznfbau.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.9152youxi.cn/gtmydmwiem.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangtech.top/gtbtkbswtk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.meibo888.top/gtuwqhudcg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.nanxuanxn.top/gtzvezjyob.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hnqzz.top/gtkhkqqcbt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.316326.xyz/gtqksfdmqq.html

[N05] 最大公约数
来源：http://hz.yuxming.cn/gthortizcc.html

Py:   math.gcd(a, b)
来源：http://hz.sxryk.cn/gtnkuxhens.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhengqikj.top/gtbpqskemy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgufenzy.top/gtuxjyfbhv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.birdmap.top/gtzwuhhvti.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.redwolf501.top/gtoyqzhkmz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jianghu66.top/gtcunxaver.html

Ruby: a.gcd(b)
来源：http://hz.cashguo.top/gtznikxbtg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhengqikj.top/gtzsgfwjez.html

[N06] 判断回文字符串
来源：http://hz.pycfn.com/gtuuugsozb.html

Py:   s == s[::-1]
来源：http://hz.jqgfzy.top/gtsptkdmpk.html

PHP:  $s === strrev($s);
来源：http://hz.sufxvd.cn/gtxsputovk.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sweek.top/gtpkaadryq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtuvtznzea.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhixingplan.top/gtncjznpuq.html

Go:   // 双指针从两端比较
来源：http://hz.snrcjt.cn/gtkziookzb.html

Ruby: s == s.reverse
来源：http://hz.gogol.net.cn/gtizftksjz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.daxiang520.top/gtkqfxpmnb.html

[N07] 两数之和（返回下标）
来源：http://hz.ydzc1.top/gtbeplefhs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yonumen.top/gtokvplsyb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gotoacloud.top/gtyflkwoky.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhijiandao.cn/gtmturyaco.html

TS:   // 手写 Map<string, number>
来源：http://hz.nanxinkj.top/gtykhiubap.html

Java: // 手写 HashMap
来源：http://hz.yuanzhike.top/gtwpbnblqu.html

Go:   // 手写 map[int]int
来源：http://hz.hnqzz.top/gtcyvuqjiw.html

Ruby: // 手写 Hash
来源：http://hz.chenlongwang.top/gtlsgatpob.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.0kj1m.cn/gtkjebflwh.html

[N08] 生成全排列
来源：http://hz.fzhhl.top/gtckbcnjnh.html

Py:   itertools.permutations(arr)
来源：http://hz.snrcjt.cn/gttzlllitz.html

PHP:  // 手写递归交换
来源：http://hz.xuanzx.com/gthtgizxao.html

JS:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtsaoptgsq.html

TS:   // 手写回溯递归
来源：http://hz.xinyue.icu/gthfvbrktd.html

Java: // 手写回溯递归
来源：http://hz.c1oappe.top/gtajjhhcmo.html

Go:   // 手写回溯递归
来源：http://hz.fzhhl.top/gthnsaxtye.html

Ruby: arr.permutation.to_a
来源：http://hz.316326.xyz/gtmeeuhkfi.html

C#:   // 手写回溯递归
来源：http://hz.316326.xyz/gtamchljqb.html

[N09] 栈与队列
来源：http://hz.shangyingyoupin.top/gtajvmmomd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yueranfly.top/gtdfistcvd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cashguo.top/gtoalzbjtb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ehwqpu.com/gtgvupnxfc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cqqwz.cn/gtjrqbauko.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ivvv.top/gtixeocjzv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sufxvd.cn/gtheqifcnh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yueranfly.top/gtybbjckcg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinghuilouyu.cn/gtszgppxxg.html

[N10] 链表节点定义
来源：http://hz.svipenyu.cn/gtexbuaqeh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jinqigufen.top/gtgxxzumny.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xingfuxueyuan.xyz/gtdkbnoobj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yvedp.cn/gthaiucdop.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jinghuilouyu.cn/gtmncxpcth.html

Java: class Node { int v; Node next; }
来源：http://hz.mhx1999.top/gthedmiyon.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cheryme.top/gtpbnygsfq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.c1oappe.top/gtysoihziw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.fzhhl.top/gtlnxuwpzv.html

[N11] 二叉树中序遍历
来源：http://hz.zhiwuduotai.top/gtytcvsadn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.snrcjt.cn/gtcuvzbqed.html

PHP:  // 手写递归函数
来源：http://hz.zhixingplan.top/gtuylxurmf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tianlin.xyz/gtbwmnhjij.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tanke756.top/gtdeveclve.html

Java: // 手写递归
来源：http://hz.mhx1999.top/gtuloozjja.html

Go:   // 手写递归
来源：http://hz.xylfe.cn/gtidgiwssu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.sweek.top/gtnqtwiivw.html

C#:   // 手写递归
来源：http://hz.9152youxi.cn/gtkjfuiixo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.bjfxy.top/gtszwrguwu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hysaishi.cn/gtmzoggipi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xziqi.cn/gtupqisoym.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.haohaochexian.top/gtykoiodap.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jianghu66.top/gtbdtksldt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.mhx1999.top/gtsahzflmk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.redwolf501.top/gtuevnnxlk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.wangdashe.top/gtgrswmbqu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ivvv.top/gtyuiuafuk.html

================================================================================
来源：http://hz.yanxiufei.cn/gtnryzdpyj.html

O. 并发与异步
来源：http://hz.smart0.xyz/gtwnlropid.html

================================================================================
来源：http://hz.zhongyouzk.top/gttvvxtzkf.html

[O01] 启动一个线程
来源：http://hz.iojbl.cn/gtrnkvotai.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gogol.net.cn/gtslepvkuu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.snrcjt.cn/gtntqrrdyk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jyoumei.cn/gtgnoprpqd.html

TS:   // 同 JS
来源：http://hz.xuanzx.com/gttygsqjll.html

Java: new Thread(() -> f()).start()
来源：http://hz.gogol.net.cn/gtqyxptrog.html

Go:   go f()
来源：http://hz.wangdashe.top/gtatusomxy.html

Ruby: Thread.new { f }
来源：http://hz.iojbl.cn/gteknsgonz.html

C#:   Task.Run(() => F());
来源：http://hz.bjfxy.top/gtvefoebhm.html

[O02] 使用线程池
来源：http://hz.zhijiandao.cn/gtynctxljf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shanyushiyangtech.top/gtadfbcgwg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.havefunace.top/gtwxjeplup.html

JS:   // worker_threads 线程池
来源：http://hz.jqgfzy.top/gtcbztwufy.html

TS:   // worker_threads 线程池
来源：http://hz.guowangkeji.top/gtelpbmxoz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jiagoushi.top/gtvgyqsrra.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.aibaodan.cn/gtrhcovymk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zycfv.cn/gtserwnoii.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cheryme.top/gtxxhumjwi.html

[O03] 加锁保护共享数据
来源：http://hz.yueranfly.top/gtgdsszqhm.html

Py:   with lock: shared += 1
来源：http://hz.jqgfzy.top/gtbciepneh.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhongyouzk.top/gtcfweznun.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shanyushiyangkeji.top/gtznellmib.html

TS:   // 同 JS
来源：http://hz.hysaishi.cn/gtxznwnhxl.html

Java: synchronized (this) { shared++; }
来源：http://hz.daria6918.cn/gtfekxygxa.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.andypj.xyz/gtzhqlntot.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhoulong.xyz/gtslflzuyu.html

C#:   lock (gate) { shared++; }
来源：http://hz.0kj1m.cn/gtznawzmjg.html

[O04] 定义异步函数并等待
来源：http://hz.havefunace.top/gtohgxqqaq.html

Py:   async def f():⏎    await g()
来源：http://hz.shangyingyoupin.top/gtmspxrbgn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.pycfn.com/gtueqvkveq.html

JS:   async function f() { await g(); }
来源：http://hz.tianlin.xyz/gtuqqmnlft.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.kuanghao11.cn/gtogyivwvp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.9152youxi.cn/gtoynzicew.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xuetiantiany.cn/gtkxoxppya.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shangyingyoupin.top/gteqnuaqqo.html

C#:   async Task F() { await G(); }
来源：http://hz.cqqwz.cn/gtcgmybprv.html

[O05] 并发执行并等待全部完成
来源：http://hz.52xcode.cn/gtwmqijctk.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cheryme.top/gtcnbtraaj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hysaishi.cn/gtjydhrlhu.html

JS:   await Promise.all(tasks)
来源：http://hz.yj202588.top/gtwzuqpwaq.html

TS:   await Promise.all(tasks)
来源：http://hz.ivvv.top/gtzvoegpxg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinyuanbaomall.cn/gtefxbvgvj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhiwuduotai.top/gtxbmvjpar.html

Ruby: threads.map(&:join)
来源：http://hz.yvedp.cn/gtncjzuesj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hnqzz.top/gtcgmhcxxx.html

[O06] 使用进程池
来源：http://hz.hnxiangtu.top/gtzbcafgpj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xuanzx.com/gtfklnprej.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xingfuxueyuan.xyz/gtmsyvbibj.html

JS:   // child_process / cluster 模块
来源：http://hz.zhixingplan.top/gtzmwhztid.html

TS:   // child_process / cluster 模块
来源：http://hz.iojbl.cn/gtvmlrwyfz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jlsjyb.cn/gthfjaglcb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.chenlongwang.top/gtokfmkjaz.html

Ruby: // fork 块
来源：http://hz.birdmap.top/gtxpggmyrc.html

C#:   Parallel.For
来源：http://hz.havefunace.top/gtvqnztmsz.html

================================================================================
来源：http://hz.dashuyun.cn/gtlusrtpxw.html

P. 常用工具函数
来源：http://hz.cucudq.cn/gtjnloyncn.html

================================================================================
来源：http://hz.jlsjyb.cn/gtpjjzkjdt.html

[P01] 生成 UUID
来源：http://hz.chenzaomai.com/gtyjsifmak.html

Py:   str(uuid.uuid4())
来源：http://hz.tian-w.cn/gtliimynbo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xuetiantiany.cn/gtggexamwx.html

JS:   crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtmyydjqio.html

TS:   crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtjacameha.html

Java: UUID.randomUUID().toString()
来源：http://hz.jinqigfzy.top/gtrxeblqqo.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ybcxt.top/gtwduhvbcr.html

Ruby: SecureRandom.uuid
来源：http://hz.jinqigfzy.top/gtilicmpuv.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.havefunace.top/gtfpilgmro.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jiagoushi.top/gtyowlwasd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenzaomai.com/gtqyfxrvyt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.sweek.top/gtvmimjeuc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hongshengwenyu.top/gtisrjfpcu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xziqi.cn/gtkegjnuit.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hywenlv.cn/gtzprijhwi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jinyuanbaomall.cn/gtgkesuzxi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ywan-chungtsiang.top/gtlcslqmxn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yuanzhike.top/gtsgzaalkv.html

[P03] 生成短随机字符串
来源：http://hz.yueranfly.top/gtsabtasxl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.aibaodan.cn/gtqpckctxf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gogol.net.cn/gtfxlfwpmc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigufen.top/gtrktwdjxx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangtech.top/gtlkjgwjtd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.sysykeji.top/gtpffensoh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xziqi.cn/gtswnjusde.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhoulong.xyz/gtdoesfvez.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.redwolf501.top/gtqxqtvztp.html

[P04] 求长度
来源：http://hz.nanxinkj.top/gtkbydsdyl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jqgufenzy.top/gtcmkfgiya.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhongyouzk.top/gtkytxkuwa.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuanzhike.top/gtwnaupmdv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ybcxt.top/gtqcnodyme.html


<!-- 参考信息 -->