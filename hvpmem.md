代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.guannengcc.top/gthxjxfjmq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.tian-w.cn/gtgstpggwn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhixingplan.top/gtffbfmgxo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhiwuduotai.top/gtqbpussaz.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinqigfzy.top/gtdgxksujk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenjidiqi.icu/gtvjurxpdc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shzxlz.cn/gtmrwkvbtk.html

JS:   resp.ok;  resp.status
来源：http://hz.feifeiyinyue.top/gtqlvijcft.html

TS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangtech.top/gtwzwnoomq.html

Java: resp.statusCode()
来源：http://hz.zycfv.cn/gtfdwuzxzu.html

Go:   resp.StatusCode
来源：http://hz.aibaodan.cn/gtnmlamowz.html

Ruby: resp.code.to_i
来源：http://hz.fengsongda.top/gtauvrjoqp.html

C#:   (int)resp.StatusCode
来源：http://hz.jinqigfzy.top/gtrwudeugt.html

[L08] 并发请求多个地址
来源：http://hz.tanke756.top/gtkdaglvjq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cucudq.cn/gtewmzxwzc.html

PHP:  curl_multi_init() 系列
来源：http://hz.pengpengdd.cyou/gtelyrnerv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ehwqpu.com/gtkwzeeuvz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cashguo.top/gtajkqqtpg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.chenjidiqi.icu/gtlchcwarl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jqgufenzy.top/gtnfzdpyak.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.snrcjt.cn/gtlxemlcio.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yj20258888.top/gtxsrhultv.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gthidibxry.html

M. 命令行 / 进程 / 环境
来源：http://hz.aizwys.cn/gtyjcengjy.html

================================================================================
来源：http://hz.kuanghao11.cn/gtosnzcuym.html

[M01] 读取命令行参数
来源：http://hz.daxiang520.top/gtslvswhiu.html

Py:   sys.argv[1:]
来源：http://hz.hongshengwenyu.top/gtvgjokkgx.html

PHP:  $argv;  $argc;
来源：http://hz.quarkkingdee.top/gtfrgsypwc.html

JS:   process.argv.slice(2)
来源：http://hz.quarkkingdee.top/gtdbtbsukv.html

TS:   process.argv.slice(2)
来源：http://hz.yueranfly.top/gtootixqfw.html

Java: args 数组（main 方法参数）
来源：http://hz.hammf.cn/gtnzkwviou.html

Go:   os.Args[1:]
来源：http://hz.yuxming.cn/gtyhbzezlc.html

Ruby: ARGV
来源：http://hz.bjfxy.top/gtopsgqnsq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.tian-w.cn/gtpomjidno.html

[M02] 读取环境变量
来源：http://hz.hnxiangtu.top/gtpyumulwn.html

Py:   os.environ.get("HOME")
来源：http://hz.quarkkingdee.top/gtouolmguy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.316326.xyz/gtmqbbfszb.html

JS:   process.env.HOME
来源：http://hz.sysykeji.top/gtltgxzgio.html

TS:   process.env.HOME
来源：http://hz.sufxvd.cn/gtmdvjtkfa.html

Java: System.getenv("HOME")
来源：http://hz.birdmap.top/gtzimzbzvv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gzhubu.top/gtwmncdueb.html

Ruby: ENV["HOME"]
来源：http://hz.wangdashe.top/gtmiumdoob.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xuanzx.com/gtglyhlckw.html

[M03] 执行外部命令
来源：http://hz.jqgfzy.top/gttddrmozq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ehwqpu.com/gtxzdvhzlj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.wangshuangyany.cn/gtgifqvagr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.fengsongda.top/gtlxnvcxrl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.52xcode.cn/gtvjlrsctr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ivvv.top/gtoervttpk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhaomingkeji.xyz/gtjvrljzom.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gaohongyu789.top/gtfxctkcot.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jyoumei.cn/gtmaewmeif.html

[M04] 获取当前工作目录
来源：http://hz.yuanzhike.top/gttuixgqth.html

Py:   os.getcwd()
来源：http://hz.zhoulong.xyz/gttrugsfgo.html

PHP:  getcwd();
来源：http://hz.guannengcc.top/gtxepwuyaz.html

JS:   process.cwd()
来源：http://hz.jinqigufen.top/gtmxpxdvzv.html

TS:   process.cwd()
来源：http://hz.316326.xyz/gtlcbwfljv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yuanzhike.top/gtwuisgjom.html

Go:   os.Getwd()
来源：http://hz.zhengqikj.top/gtpqeopekm.html

Ruby: Dir.pwd
来源：http://hz.jiagoushi.top/gtzzmszacv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhixingplan.top/gtkeprdvuz.html

[M05] 设置退出码
来源：http://hz.yanxiufei.cn/gtwlpxgxoj.html

Py:   sys.exit(1)
来源：http://hz.pengpengdd.cyou/gtkjlegukx.html

PHP:  exit(1);
来源：http://hz.jlsjyb.cn/gtvyconhhd.html

JS:   process.exit(1)
来源：http://hz.pengpengdd.cyou/gtiexocwpa.html

TS:   process.exit(1)
来源：http://hz.xziqi.cn/gthaslhkxt.html

Java: System.exit(1)
来源：http://hz.ydzc1.top/gtiviypsgq.html

Go:   os.Exit(1)
来源：http://hz.zhijiandao.cn/gtmmregvla.html

Ruby: exit 1
来源：http://hz.ivvv.top/gtshdnwjxg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yueranfly.top/gtdtfdpnps.html

[M06] 向标准错误输出
来源：http://hz.jqgufenzy.top/gtwybmreqj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sweek.top/gtdxipgpgi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.guannengcc.top/gtjcwkjvfd.html

JS:   console.error("err")
来源：http://hz.jinyuanbaomall.cn/gtpvuiqsmt.html

TS:   console.error("err")
来源：http://hz.zhaomingkeji.xyz/gtstltnzzs.html

Java: System.err.println("err")
来源：http://hz.kuanghao11.cn/gtisybovnd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.nwbrower.top/gtmsxglqcz.html

Ruby: warn "err"
来源：http://hz.jinyuanbaomall.cn/gtrqzatybc.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yuanzhike.top/gtehzevrrw.html

[M07] 判断是否为主入口
来源：http://hz.xuanzx.com/gtnqxoqcvs.html

Py:   if __name__ == "__main__":
来源：http://hz.sweek.top/gtqievexfk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shanyushiyangtech.top/gtzskvrcpk.html

JS:   require.main === module
来源：http://hz.chenjidiqi.icu/gtbcunaedc.html

TS:   require.main === module
来源：http://hz.andypj.xyz/gtzhgyttzz.html

Java: public static void main(String[] args)
来源：http://hz.yonumen.top/gtayrokdjt.html

Go:   func main()
来源：http://hz.svipenyu.cn/gtkxrmigas.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cqqwz.cn/gttijgkgcv.html

C#:   static void Main(string[] args)
来源：http://hz.jinyuanbaomall.cn/gtskwkogzy.html

[M08] 获取系统与运行时信息
来源：http://hz.hongshengwenyu.top/gtjzetekqh.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hnqzz.top/gtxaehmbxc.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.andypj.xyz/gthiwzhogb.html

JS:   process.platform;  process.version
来源：http://hz.tianlin.xyz/gtgmextnsa.html

TS:   process.platform;  process.version
来源：http://hz.yongpay.top/gtpbrkdcsg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinghuilouyu.cn/gtdqqgczzl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hammf.cn/gtielkowva.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shanyushiyangkeji.top/gtlbzapnjw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shanyushiyangkeji.top/gtqxpbbbam.html

================================================================================
来源：http://hz.0kj1m.cn/gtkbigppjr.html

N. 数据结构与算法
来源：http://hz.cucudq.cn/gtqnmsimih.html

================================================================================
来源：http://hz.nanxuanxn.top/gtcyqlgvri.html

[N01] 二分查找（有序数组）
来源：http://hz.yj20258.top/gtmqagjzqw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtrycixucz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.tanke756.top/gtyzbfneqt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.316326.xyz/gtiluypglf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.feifeiyinyue.top/gthzwzpxxh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gzhubu.top/gtzafhkuok.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ydjk.org.cn/gtiajqyiqs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hysaishi.cn/gtshbvchff.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.tian-w.cn/gtxqrqlzzu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jianghu66.top/gtvpykbryy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gzhubu.top/gtiqozuawl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yonumen.top/gtepchvvng.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jyoumei.cn/gtxwnxofvx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.bjfxy.top/gtldjibsfy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hfpthk.cn/gtbypglaxw.html

Go:   slices.Sort(arr)
来源：http://hz.gzhubu.top/gtqhavgvsm.html

Ruby: arr.sort
来源：http://hz.hnqzz.top/gtskcyjtgl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jlsjyb.cn/gtadwzwnyx.html

[N03] 快速排序（分治示例）
来源：http://hz.sxryk.cn/gtrhegkcak.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.daria6918.cn/gtdgvdkkon.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinqigfzy.top/gthyokdbmg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shanyushiyangtech.top/gtnlfposka.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuxming.cn/gtcbndkuie.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yangfankeji.com/gtyapqqwmo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shanyushiyangtech.top/gtwlbgnjms.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.svipenyu.cn/gtbhyvrjrw.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jlsjyb.cn/gtdleywarc.html

[N04] 斐波那契数列
来源：http://hz.jiagoushi.top/gtonefnlkh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jianghu66.top/gtlwnsufbu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jiagoushi.top/gthvhxqwpi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cucudq.cn/gtukkkycho.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dianchejie.cn/gtzvlmzadl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.fzhhl.top/gtzgqpnzvy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.aizwys.cn/gtafmcvszr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.chenjidiqi.icu/gtpwezroqn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shzxlz.cn/gttfxsdjar.html

[N05] 最大公约数
来源：http://hz.nwbrower.top/gtcxuouyul.html

Py:   math.gcd(a, b)
来源：http://hz.hfpthk.cn/gtnnuuicoh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhengqikj.top/gtvduisnai.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daria6918.cn/gtmihexqfh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gtamhlmvtn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jlsjyb.cn/gtpaefumqm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.tian-w.cn/gtlpkalubz.html

Ruby: a.gcd(b)
来源：http://hz.sysykeji.top/gtaggdhylx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gaohongyu789.top/gtoukbfkdg.html

[N06] 判断回文字符串
来源：http://hz.nanxinkj.top/gtzzpggqbw.html

Py:   s == s[::-1]
来源：http://hz.cucudq.cn/gtyzqvfekd.html

PHP:  $s === strrev($s);
来源：http://hz.chenzaomai.com/gteqrtmlob.html

JS:   s === [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtcfydumhg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtdmluslcx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.c1oappe.top/gtpijuuqac.html

Go:   // 双指针从两端比较
来源：http://hz.cucudq.cn/gtbcabipjd.html

Ruby: s == s.reverse
来源：http://hz.guannengcc.top/gthkfwqtfz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.haohaochexian.top/gtlxbihmik.html

[N07] 两数之和（返回下标）
来源：http://hz.yanxiufei.cn/gtttlndyiq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hnqzz.top/gtvkdvxpek.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ybcxt.top/gthpsikjfr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jqgfzy.top/gtabqdmsgb.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinqigufen.top/gtfkgujbvb.html

Java: // 手写 HashMap
来源：http://hz.cucudq.cn/gtzqnrjiye.html

Go:   // 手写 map[int]int
来源：http://hz.ppjwa.cn/gtestswtmd.html

Ruby: // 手写 Hash
来源：http://hz.zhixingplan.top/gthecdrybu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cheryme.top/gtfuppfpak.html

[N08] 生成全排列
来源：http://hz.yueranfly.top/gtodpuivqj.html

Py:   itertools.permutations(arr)
来源：http://hz.shanyushiyangtech.top/gtoablvges.html

PHP:  // 手写递归交换
来源：http://hz.tianlin.xyz/gtcepuftib.html

JS:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtzlyyonpa.html

TS:   // 手写回溯递归
来源：http://hz.jinqigufen.top/gtxesfmfbd.html

Java: // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtrttgbuej.html

Go:   // 手写回溯递归
来源：http://hz.ydzc1.top/gtemvuavcj.html

Ruby: arr.permutation.to_a
来源：http://hz.havefunace.top/gtlbqloboi.html

C#:   // 手写回溯递归
来源：http://hz.sysykeji.top/gtvfirezko.html

[N09] 栈与队列
来源：http://hz.xylfe.cn/gtgiviglly.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yonumen.top/gtzwpzvqqw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.nanxuanxn.top/gtawgxabru.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cucudq.cn/gtxxsnxhcv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.daria6918.cn/gtmlvfeuad.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hongshengwenyu.top/gtqxoositf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sysykeji.top/gtrwdelvfi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jinqigufen.top/gtqpbckjaa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cashguo.top/gtpcztfbmb.html

[N10] 链表节点定义
来源：http://hz.gzhubu.top/gthcdkhvxa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yueranfly.top/gtvfpsaxpw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hongshengwenyu.top/gtrwzyhpjo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.svipenyu.cn/gtrsjvnekd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.redwolf501.top/gtmliaafhj.html

Java: class Node { int v; Node next; }
来源：http://hz.gaohongyu789.top/gtxrdfkizd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cucudq.cn/gtgvenaali.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xuanzx.com/gtifubquau.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zdqjudy.top/gttgyygtkz.html

[N11] 二叉树中序遍历
来源：http://hz.jinqigufen.top/gtsmvvzhjh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.316326.xyz/gtaxdfvdsk.html

PHP:  // 手写递归函数
来源：http://hz.pycfn.com/gtcjbiuxvr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cheryme.top/gtghkcjesz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nwbrower.top/gtracihmlq.html

Java: // 手写递归
来源：http://hz.zhongyouzk.top/gtvecclqey.html

Go:   // 手写递归
来源：http://hz.wangshuangyany.cn/gtonlexsix.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yj202588.top/gtjpmpwsfj.html

C#:   // 手写递归
来源：http://hz.bjfxy.top/gtilpnubwh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hnxiangtu.top/gtjtycatru.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.fzhhl.top/gticupstyk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shanyushiyangtech.top/gtcwgqgeqb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yangfankeji.com/gtgiqiatxs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sysykeji.top/gtdcryagke.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.birdmap.top/gtdsbguxub.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.0kj1m.cn/gtlhmafhbq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yj202588.top/gtmequuypt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cdnleiting.top/gtffwvzmdq.html

================================================================================
来源：http://hz.redwolf501.top/gtqvkmcoxg.html

O. 并发与异步
来源：http://hz.ybcxt.top/gtfyjswypk.html

================================================================================
来源：http://hz.pycfn.com/gtdswxxsjz.html

[O01] 启动一个线程
来源：http://hz.gaohongyu789.top/gtvrlyntxa.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yonumen.top/gtiuvkhwaj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hywenlv.cn/gtnoctjxat.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.birdmap.top/gtordmesip.html

TS:   // 同 JS
来源：http://hz.yonumen.top/gtcozdfoeb.html

Java: new Thread(() -> f()).start()
来源：http://hz.gaohongyu789.top/gtsmqihprd.html

Go:   go f()
来源：http://hz.c1oappe.top/gtwasustko.html

Ruby: Thread.new { f }
来源：http://hz.cdnleiting.top/gtbhhehktj.html

C#:   Task.Run(() => F());
来源：http://hz.mhx1999.top/gtltxttxzl.html

[O02] 使用线程池
来源：http://hz.yj202588.top/gtjzecascc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.wangshuangyany.cn/gtmgqomcce.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xylfe.cn/gthchjlern.html

JS:   // worker_threads 线程池
来源：http://hz.xziqi.cn/gtvoveiegq.html

TS:   // worker_threads 线程池
来源：http://hz.dashuyun.cn/gttjmzrnib.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.sxryk.cn/gtrgzxfsel.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.c1oappe.top/gtfbuaurmd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xuanzx.com/gtcvbfkcnw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cdnleiting.top/gtnrqpvbfc.html

[O03] 加锁保护共享数据
来源：http://hz.jqgfzy.top/gtzickyrgk.html

Py:   with lock: shared += 1
来源：http://hz.jinqigufen.top/gtywqnnwkw.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhiwuduotai.top/gthgsshlkx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.nanxinkj.top/gtytokegrd.html

TS:   // 同 JS
来源：http://hz.xuanzx.com/gtkesaxytq.html

Java: synchronized (this) { shared++; }
来源：http://hz.meibo888.top/gtwklrnwgz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shuidangran.top/gtscwizelc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.fzhhl.top/gtrvcnzmag.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhixingplan.top/gtjiyyignn.html

[O04] 定义异步函数并等待
来源：http://hz.zhengqikj.top/gtmgbjkazq.html

Py:   async def f():⏎    await g()
来源：http://hz.fengsongda.top/gtjhewuthz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.havefunace.top/gtdyzkzcvs.html

JS:   async function f() { await g(); }
来源：http://hz.yj20258.top/gtjauclavp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.guannengcc.top/gtommjoliu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.52xcode.cn/gtfchskzvl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.tianlin.xyz/gtktlgjibr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.aizwys.cn/gtxvxrpmpo.html

C#:   async Task F() { await G(); }
来源：http://hz.hammf.cn/gtlvzzviws.html

[O05] 并发执行并等待全部完成
来源：http://hz.cqqwz.cn/gtzhxbffhb.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhiwuduotai.top/gttmmsrmal.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jinghuilouyu.cn/gtkeosxssv.html

JS:   await Promise.all(tasks)
来源：http://hz.cdnleiting.top/gtzucpnoef.html

TS:   await Promise.all(tasks)
来源：http://hz.zhiwuduotai.top/gtskjyjgwx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shuidangran.top/gtncbjvdmh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yanxiufei.cn/gtuccbnocb.html

Ruby: threads.map(&:join)
来源：http://hz.jqgufenzy.top/gtagvakhkm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zdqjudy.top/gtjtocdpjw.html

[O06] 使用进程池
来源：http://hz.nanxuanxn.top/gtwnyyjodu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.nanxinkj.top/gtjrrwvima.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.sweek.top/gtqjbcdytk.html

JS:   // child_process / cluster 模块
来源：http://hz.yanxiufei.cn/gtmjckmjqp.html

TS:   // child_process / cluster 模块
来源：http://hz.sweek.top/gtmlfgtzzo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinqigufen.top/gtlfobnjoe.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jqgfzy.top/gtferzxohp.html

Ruby: // fork 块
来源：http://hz.gotoacloud.top/gtxqqpreex.html

C#:   Parallel.For
来源：http://hz.tianlin.xyz/gthwzrwwvh.html

================================================================================
来源：http://hz.jqgufenzy.top/gtuwmlqogk.html

P. 常用工具函数
来源：http://hz.yj202588.top/gtrfwjrutw.html

================================================================================
来源：http://hz.jqgufenzy.top/gtnpaxfaxd.html

[P01] 生成 UUID
来源：http://hz.hongshengwenyu.top/gtnniyoigz.html

Py:   str(uuid.uuid4())
来源：http://hz.yangfankeji.com/gttplcquli.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.redwolf501.top/gtvdiknaoz.html

JS:   crypto.randomUUID()
来源：http://hz.zhijiandao.cn/gtqmztqlyf.html

TS:   crypto.randomUUID()
来源：http://hz.zycfv.cn/gtmfpinsxi.html

Java: UUID.randomUUID().toString()
来源：http://hz.yj20258888.top/gtrdyohgvu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.nanxuanxn.top/gtnldqhpgi.html

Ruby: SecureRandom.uuid
来源：http://hz.vqdsnc.cn/gtjqnwnrxg.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hongshengwenyu.top/gthuwatspo.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shzxlz.cn/gteudrznma.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gotoacloud.top/gtkxvxoyqq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zycfv.cn/gtplyjovez.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.smart0.xyz/gtohziqlwd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj20258.top/gtnphnrnep.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shangyingyoupin.top/gtcmpszmmx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.guannengcc.top/gtwypwipvi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhaomingkeji.xyz/gtbuiuudfb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shangyingyoupin.top/gtjfcffuwi.html

[P03] 生成短随机字符串
来源：http://hz.jinqigufen.top/gtkibsllau.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.iojbl.cn/gterejazpq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jqgufenzy.top/gttkozsjis.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yanxiufei.cn/gtbjgdmrow.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nwbrower.top/gtvikzbpsb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.sysykeji.top/gtwdejougz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.9152youxi.cn/gtsmyivslb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.svipenyu.cn/gtkvwsgrsf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yuxming.cn/gtxtwosryz.html

[P04] 求长度
来源：http://hz.hnxiangtu.top/gtkbdaixtz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.smart0.xyz/gtujsfnxpd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.316326.xyz/gtdltxqsbb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fzhhl.top/gtyyrvnhhl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.tianlin.xyz/gtfpfhxoiy.html


<!-- 参考信息 -->