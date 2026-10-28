代发 wailian999

Py:   resp.json()
来源：http://hz.tanke756.top/gtiocxcvnw.html

PHP:  json_decode($body, true);
来源：http://hz.wangdashe.top/gtrdiawggp.html

JS:   await resp.json()
来源：http://hz.cucudq.cn/gtciuakluc.html

TS:   await resp.json()
来源：http://hz.hammf.cn/gteoarynfz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhiwuduotai.top/gtlivtcxld.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.316326.xyz/gthtldgpyo.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ywan-chungtsiang.top/gthryfsose.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jinqigufen.top/gtfotfmvos.html

[L07] 处理 HTTP 状态码
来源：http://hz.xinyue.icu/gthblslcpe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cheryme.top/gtmihpthxp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.9152youxi.cn/gtmgsgzuyp.html

JS:   resp.ok;  resp.status
来源：http://hz.zhongyouzk.top/gtdurwqlhs.html

TS:   resp.ok;  resp.status
来源：http://hz.sufxvd.cn/gtkndybyaz.html

Java: resp.statusCode()
来源：http://hz.zhongyouzk.top/gtubmjjmrn.html

Go:   resp.StatusCode
来源：http://hz.jinqigfzy.top/gtddlhpqpm.html

Ruby: resp.code.to_i
来源：http://hz.yongpay.top/gtuzclcfep.html

C#:   (int)resp.StatusCode
来源：http://hz.quarkkingdee.top/gtgkkfwptp.html

[L08] 并发请求多个地址
来源：http://hz.wangdashe.top/gtmejyqbjc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.iojbl.cn/gtjduuozng.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj202588.top/gtfpaldoww.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ybcxt.top/gtorarkkba.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.c1oappe.top/gtjblehmrv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hfpthk.cn/gtsjpnxprm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.feifeiyinyue.top/gtrmezrirp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.chenlongwang.top/gtakmnhhgd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shangyingyoupin.top/gtrrwboart.html

================================================================================
来源：http://hz.fengsongda.top/gtvlbvzzfd.html

M. 命令行 / 进程 / 环境
来源：http://hz.jqgufenzy.top/gtprcgptdq.html

================================================================================
来源：http://hz.gotoacloud.top/gtlnjnmchc.html

[M01] 读取命令行参数
来源：http://hz.xziqi.cn/gtjiecptvf.html

Py:   sys.argv[1:]
来源：http://hz.jqgufenzy.top/gttzumcawk.html

PHP:  $argv;  $argc;
来源：http://hz.ivvv.top/gtjwrahbrs.html

JS:   process.argv.slice(2)
来源：http://hz.yuxming.cn/gtxxfdzfls.html

TS:   process.argv.slice(2)
来源：http://hz.nanxuanxn.top/gtukzutzla.html

Java: args 数组（main 方法参数）
来源：http://hz.hfpthk.cn/gthxarangq.html

Go:   os.Args[1:]
来源：http://hz.tian-w.cn/gtqmsthpzb.html

Ruby: ARGV
来源：http://hz.xuanzx.com/gtqsnzovad.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jiagoushi.top/gtvqkcpdpa.html

[M02] 读取环境变量
来源：http://hz.shuidangran.top/gthyllocxj.html

Py:   os.environ.get("HOME")
来源：http://hz.zhixingplan.top/gtdonsyjeb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinqigfzy.top/gtoxeckwpu.html

JS:   process.env.HOME
来源：http://hz.52xcode.cn/gtwiwgulna.html

TS:   process.env.HOME
来源：http://hz.gotoacloud.top/gtrvgiedax.html

Java: System.getenv("HOME")
来源：http://hz.jiagoushi.top/gtczasxiff.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jqgfzy.top/gtrpxfdwbi.html

Ruby: ENV["HOME"]
来源：http://hz.shzxlz.cn/gtdworinsy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ivvv.top/gtrljwmrxf.html

[M03] 执行外部命令
来源：http://hz.yongpay.top/gtxomouyve.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hammf.cn/gtygychedv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.nanxuanxn.top/gteaqbdqnw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.gogol.net.cn/gtuzdkczds.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ivvv.top/gtvcrgpevm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yonumen.top/gtktrhdgyh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.chenjidiqi.icu/gtybjqjhbk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hnqzz.top/gtmeahlrzf.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zdqjudy.top/gtwsnyssho.html

[M04] 获取当前工作目录
来源：http://hz.havefunace.top/gtjfggzkxo.html

Py:   os.getcwd()
来源：http://hz.mhx1999.top/gtmxgsehca.html

PHP:  getcwd();
来源：http://hz.bjfxy.top/gtqtzoviqs.html

JS:   process.cwd()
来源：http://hz.andypj.xyz/gtyuuqakvr.html

TS:   process.cwd()
来源：http://hz.xylfe.cn/gtziuawzfk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xylfe.cn/gtoxozmjmd.html

Go:   os.Getwd()
来源：http://hz.tanke756.top/gtxnvdodxv.html

Ruby: Dir.pwd
来源：http://hz.gzhubu.top/gteytogbzy.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shangyingyoupin.top/gthnewhsac.html

[M05] 设置退出码
来源：http://hz.snrcjt.cn/gtrwszkmpp.html

Py:   sys.exit(1)
来源：http://hz.feifeiyinyue.top/gtudzmvxiq.html

PHP:  exit(1);
来源：http://hz.0kj1m.cn/gtddziyzan.html

JS:   process.exit(1)
来源：http://hz.meibo888.top/gtrlmmoyqt.html

TS:   process.exit(1)
来源：http://hz.ywan-chungtsiang.top/gttrqszbmb.html

Java: System.exit(1)
来源：http://hz.sxryk.cn/gtdtpihkpg.html

Go:   os.Exit(1)
来源：http://hz.hongshengwenyu.top/gthlvndqtk.html

Ruby: exit 1
来源：http://hz.cdnleiting.top/gtoeroeqen.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.daria6918.cn/gtnrjgbknl.html

[M06] 向标准错误输出
来源：http://hz.svipenyu.cn/gthcozfpae.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ehwqpu.com/gtpdoouegm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.0kj1m.cn/gtmxyghdyf.html

JS:   console.error("err")
来源：http://hz.bjfxy.top/gtovfeesor.html

TS:   console.error("err")
来源：http://hz.cheryme.top/gtbrwhrtke.html

Java: System.err.println("err")
来源：http://hz.redwolf501.top/gtoihusswh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.svipenyu.cn/gtmxnefzcp.html

Ruby: warn "err"
来源：http://hz.zhaomingkeji.xyz/gtsywaufxc.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xuetiantiany.cn/gtaxrftbac.html

[M07] 判断是否为主入口
来源：http://hz.ydjk.org.cn/gtryovjnmm.html

Py:   if __name__ == "__main__":
来源：http://hz.jqgfzy.top/gtldaaxoql.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gogol.net.cn/gtcioekayz.html

JS:   require.main === module
来源：http://hz.ywan-chungtsiang.top/gttsdojebq.html

TS:   require.main === module
来源：http://hz.nwbrower.top/gtxhrwnkot.html

Java: public static void main(String[] args)
来源：http://hz.svipenyu.cn/gtojzgvccx.html

Go:   func main()
来源：http://hz.tian-w.cn/gtosiecxdr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.pycfn.com/gtqyeglriu.html

C#:   static void Main(string[] args)
来源：http://hz.316326.xyz/gtelypuuwx.html

[M08] 获取系统与运行时信息
来源：http://hz.zdqjudy.top/gtzbxngpzh.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinqigufen.top/gtjhqawumg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gogol.net.cn/gtsqtkwerf.html

JS:   process.platform;  process.version
来源：http://hz.yj20258888.top/gttdfqzsxn.html

TS:   process.platform;  process.version
来源：http://hz.aizwys.cn/gtpqjiyfxg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinyuanbaomall.cn/gtahrbwvey.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhiwuduotai.top/gtzrmeevwe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yuxming.cn/gthduwokyl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnxiangtu.top/gtltgnxcrh.html

================================================================================
来源：http://hz.smart0.xyz/gtaujowszy.html

N. 数据结构与算法
来源：http://hz.cucudq.cn/gttdudkheq.html

================================================================================
来源：http://hz.316326.xyz/gtuupmsbqt.html

[N01] 二分查找（有序数组）
来源：http://hz.zhongyouzk.top/gtwgqkepvb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zdqjudy.top/gtiyzurizm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhoulong.xyz/gtvenouiub.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.snrcjt.cn/gtisjvjwlr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.meibo888.top/gtkyzenouf.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shzxlz.cn/gtyqmtmawj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jlsjyb.cn/gtkddvtprq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.chenjidiqi.icu/gtgosgqdxq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.dashuyun.cn/gtewklwbyx.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.nanxuanxn.top/gtoouubpqv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cdnleiting.top/gtmwombnhy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhoulong.xyz/gtixilfqjc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yueranfly.top/gtphlexyqf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fzhhl.top/gtlgtycrdk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhengqikj.top/gtjfjwetel.html

Go:   slices.Sort(arr)
来源：http://hz.havefunace.top/gtehmurjtc.html

Ruby: arr.sort
来源：http://hz.aibaodan.cn/gtojgkilcw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yvedp.cn/gtcnaudkxp.html

[N03] 快速排序（分治示例）
来源：http://hz.gzhubu.top/gtefbdnovd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhixingplan.top/gtqcvyhtfd.html

PHP:  // 递归实现，或用 usort
来源：http://hz.wangdashe.top/gtujnivzpx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hnqzz.top/gtnmfsuvqb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.feifeiyinyue.top/gthijgykom.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.9152youxi.cn/gtpbrrreql.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yongpay.top/gtndellbom.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jinqigufen.top/gtegqykziv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shuidangran.top/gtkzxcbyfv.html

[N04] 斐波那契数列
来源：http://hz.yuxming.cn/gtgleobwzv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.vqdsnc.cn/gtplooppdr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.nwbrower.top/gtnopnghyd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxinkj.top/gtvcygfeav.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hywenlv.cn/gttptlmhcp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cheryme.top/gtjvwelycd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jlsjyb.cn/gtnnkcjzkp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cucudq.cn/gtazbvwset.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zdqjudy.top/gtdfiwmbyj.html

[N05] 最大公约数
来源：http://hz.dianchejie.cn/gtqftdfbas.html

Py:   math.gcd(a, b)
来源：http://hz.vqdsnc.cn/gtlbpybzlp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yvedp.cn/gtuprfznnx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnxiangtu.top/gtvxlonbie.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xuetiantiany.cn/gtlvzoclng.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.pycfn.com/gtqsbpczpn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenzaomai.com/gtrjqlmjnf.html

Ruby: a.gcd(b)
来源：http://hz.cashguo.top/gtlvwpltok.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhixingplan.top/gtcplnwuce.html

[N06] 判断回文字符串
来源：http://hz.redwolf501.top/gtcdrogobx.html

Py:   s == s[::-1]
来源：http://hz.yvedp.cn/gtfnhfsjdg.html

PHP:  $s === strrev($s);
来源：http://hz.shzxlz.cn/gtnacskavh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.mhx1999.top/gtgjdrgnkt.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hfpthk.cn/gtnfjvmvdy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.redwolf501.top/gtelgatthc.html

Go:   // 双指针从两端比较
来源：http://hz.xingfuxueyuan.xyz/gtnbcfsuwt.html

Ruby: s == s.reverse
来源：http://hz.0kj1m.cn/gtjbtaivjv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yongpay.top/gtejxbopby.html

[N07] 两数之和（返回下标）
来源：http://hz.shzxlz.cn/gtdlgokrkl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yuanzhike.top/gtrirovxdt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xuanzx.com/gtcbgabptg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.wangshuangyany.cn/gtqdijaocv.html

TS:   // 手写 Map<string, number>
来源：http://hz.tian-w.cn/gtiybjbwrk.html

Java: // 手写 HashMap
来源：http://hz.nwbrower.top/gthumxizrt.html

Go:   // 手写 map[int]int
来源：http://hz.yj202588.top/gtfrvzvdwq.html

Ruby: // 手写 Hash
来源：http://hz.zdqjudy.top/gtjpbwrzus.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhixingplan.top/gtzhuwloxm.html

[N08] 生成全排列
来源：http://hz.jianghu66.top/gturnjjsma.html

Py:   itertools.permutations(arr)
来源：http://hz.feifeiyinyue.top/gtlfrpiryz.html

PHP:  // 手写递归交换
来源：http://hz.shangyingyoupin.top/gtptjptjyu.html

JS:   // 手写回溯递归
来源：http://hz.iojbl.cn/gthfzybwjg.html

TS:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtzbtfzqjj.html

Java: // 手写回溯递归
来源：http://hz.chenlongwang.top/gtomlkdbgo.html

Go:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtcvytgsap.html

Ruby: arr.permutation.to_a
来源：http://hz.chenlongwang.top/gtfwubjyjw.html

C#:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtmwwcmsxv.html

[N09] 栈与队列
来源：http://hz.quarkkingdee.top/gtxqrycnkp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xziqi.cn/gtwxzbjneg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhaomingkeji.xyz/gtyvpdlhva.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.9152youxi.cn/gtffznjxvg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.havefunace.top/gtrccnhyrg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.nwbrower.top/gtcdqdkkgm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cdnleiting.top/gtuteakraf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.aibaodan.cn/gtwgdhwsca.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.sxryk.cn/gtryspqlxd.html

[N10] 链表节点定义
来源：http://hz.jqgufenzy.top/gtcrieiozj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hnxiangtu.top/gtclclcenk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yj20258.top/gtyrxldvwo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.quarkkingdee.top/gtmxnhcjox.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.bjfxy.top/gtxpelorms.html

Java: class Node { int v; Node next; }
来源：http://hz.yj202588.top/gtwghhkagc.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shzxlz.cn/gtadmfjgvi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xziqi.cn/gtmiqtfwqq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jiagoushi.top/gtsaphvlnw.html

[N11] 二叉树中序遍历
来源：http://hz.hysaishi.cn/gtgoxlxdpd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhiwuduotai.top/gtsjrhzlpz.html

PHP:  // 手写递归函数
来源：http://hz.dashuyun.cn/gtsxolqonm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tian-w.cn/gthdbksjck.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shanyushiyangtech.top/gtmgkpctdw.html

Java: // 手写递归
来源：http://hz.sxryk.cn/gthrvyywii.html

Go:   // 手写递归
来源：http://hz.iojbl.cn/gtxuimlsid.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jqgfzy.top/gtssknujfa.html

C#:   // 手写递归
来源：http://hz.snrcjt.cn/gthdfjufse.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jiagoushi.top/gtjfndgwfh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhiwuduotai.top/gtanzlkgmb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zdqjudy.top/gtisuekgwg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jlsjyb.cn/gtvrezbfbv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.daria6918.cn/gtcagihngn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.aibaodan.cn/gtiuadexup.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jyoumei.cn/gtdqkodmln.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.snrcjt.cn/gtekmvjrjn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hammf.cn/gtdupueksc.html

================================================================================
来源：http://hz.yvedp.cn/gtlvuzyxnz.html

O. 并发与异步
来源：http://hz.iojbl.cn/gtrqotszqz.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtdqzjwopx.html

[O01] 启动一个线程
来源：http://hz.sufxvd.cn/gtpvujaocj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.0kj1m.cn/gtsjvraqcr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shanyushiyangkeji.top/gtjledwzdz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fzhhl.top/gtdncemhnf.html

TS:   // 同 JS
来源：http://hz.nwbrower.top/gtqfasdbil.html

Java: new Thread(() -> f()).start()
来源：http://hz.tianlin.xyz/gtgshashyk.html

Go:   go f()
来源：http://hz.xylfe.cn/gtsvjbclho.html

Ruby: Thread.new { f }
来源：http://hz.sysykeji.top/gtgwhxjhmi.html

C#:   Task.Run(() => F());
来源：http://hz.daria6918.cn/gtrlbrgeuh.html

[O02] 使用线程池
来源：http://hz.yueranfly.top/gttozsjmck.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhaomingkeji.xyz/gteunraywo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.bjfxy.top/gtbovktdxh.html

JS:   // worker_threads 线程池
来源：http://hz.jinghuilouyu.cn/gtrggbczgf.html

TS:   // worker_threads 线程池
来源：http://hz.chenlongwang.top/gtnmdytkfb.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.nanxinkj.top/gtoeulihle.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jqgfzy.top/gtmcuymuif.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cdnleiting.top/gttmiatbnl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cqqwz.cn/gthsnqlvoi.html

[O03] 加锁保护共享数据
来源：http://hz.yj202588.top/gtqeclneqd.html

Py:   with lock: shared += 1
来源：http://hz.jlsjyb.cn/gtzgmdinkt.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jianghu66.top/gtskircgxs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yvedp.cn/gtpdfijzda.html

TS:   // 同 JS
来源：http://hz.jyoumei.cn/gtndzlskdi.html

Java: synchronized (this) { shared++; }
来源：http://hz.hnqzz.top/gtfjpcqvmw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cheryme.top/gtxwramdid.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.redwolf501.top/gtucmlgldj.html

C#:   lock (gate) { shared++; }
来源：http://hz.gotoacloud.top/gtnonkrylc.html

[O04] 定义异步函数并等待
来源：http://hz.9152youxi.cn/gtaydtrgkh.html

Py:   async def f():⏎    await g()
来源：http://hz.shangyingyoupin.top/gtvywdxtac.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hysaishi.cn/gtkubqmhko.html

JS:   async function f() { await g(); }
来源：http://hz.jianghu66.top/gtlwxqjsxm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.sysykeji.top/gthtftqipg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhongyouzk.top/gtebdpsagf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.gzhubu.top/gtaeuukuco.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shanyushiyangkeji.top/gtkntyltzq.html

C#:   async Task F() { await G(); }
来源：http://hz.aizwys.cn/gtkaghlrlu.html

[O05] 并发执行并等待全部完成
来源：http://hz.gotoacloud.top/gtueknwluf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinqigufen.top/gtkgsznmft.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gaohongyu789.top/gtuqtjqptd.html

JS:   await Promise.all(tasks)
来源：http://hz.cucudq.cn/gtduvfqape.html

TS:   await Promise.all(tasks)
来源：http://hz.sufxvd.cn/gtsuntvkug.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.gotoacloud.top/gtsrtejcuv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hnqzz.top/gtdsbdtqdo.html

Ruby: threads.map(&:join)
来源：http://hz.xziqi.cn/gtjvzchixb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jqgufenzy.top/gtxqntlmms.html

[O06] 使用进程池
来源：http://hz.zhiwuduotai.top/gtpuymqich.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ppjwa.cn/gtqcrlivyz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yangfankeji.com/gtdckfgpdl.html

JS:   // child_process / cluster 模块
来源：http://hz.chenlongwang.top/gtkqwknjlk.html

TS:   // child_process / cluster 模块
来源：http://hz.jinyuanbaomall.cn/gtulhkeehs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.nanxinkj.top/gtvcgdkysy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.birdmap.top/gtjwekczms.html

Ruby: // fork 块
来源：http://hz.yongpay.top/gtnzbpomfn.html

C#:   Parallel.For
来源：http://hz.yueranfly.top/gtlcokxrik.html

================================================================================
来源：http://hz.hysaishi.cn/gtxlqjipgp.html

P. 常用工具函数
来源：http://hz.xuanzx.com/gtnixwjxsv.html

================================================================================
来源：http://hz.sufxvd.cn/gtzuskhnmf.html

[P01] 生成 UUID
来源：http://hz.chenzaomai.com/gtjwkenfoa.html

Py:   str(uuid.uuid4())
来源：http://hz.tanke756.top/gtvncdzzqv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhongyouzk.top/gtbvvhtiwk.html

JS:   crypto.randomUUID()
来源：http://hz.tanke756.top/gtjwuptfmz.html

TS:   crypto.randomUUID()
来源：http://hz.ppjwa.cn/gtfaburzro.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhiwuduotai.top/gtsuomaegs.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ywan-chungtsiang.top/gtinfprozz.html

Ruby: SecureRandom.uuid
来源：http://hz.wangshuangyany.cn/gtgbrplbsr.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hnqzz.top/gtcjuwjhcm.html

[P02] MD5 / SHA256 摘要
来源：http://hz.gogol.net.cn/gtvxkwuodt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.316326.xyz/gttkzowztl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yueranfly.top/gtttmepmau.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.wangshuangyany.cn/gtwdkxmdqz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhiwuduotai.top/gtrmkdmiha.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.guannengcc.top/gtboetjkjn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.mhx1999.top/gtpmyuvjnv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xingfuxueyuan.xyz/gtpvimyoli.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xuanzx.com/gtrztsetmy.html

[P03] 生成短随机字符串
来源：http://hz.zhijiandao.cn/gtbqbdbcvq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gotoacloud.top/gthtjsrkex.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cqqwz.cn/gtywcsrind.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sufxvd.cn/gtvscwlopa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gaohongyu789.top/gtwmwywhqq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yj20258.top/gtwssqxfjn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.fzhhl.top/gtkzoowmlf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.dashuyun.cn/gtagkyhcck.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.bjfxy.top/gtgvuzdkxz.html

[P04] 求长度
来源：http://hz.meibo888.top/gtfvuhvwhb.html


<!-- 参考信息 -->