代发 wailian999

Py:   resp.json()
来源：http://hz.smart0.xyz/gtoupxnhzy.html

PHP:  json_decode($body, true);
来源：http://hz.316326.xyz/gtslteszso.html

JS:   await resp.json()
来源：http://hz.jianghu66.top/gtlmvdyjrm.html

TS:   await resp.json()
来源：http://hz.zdqjudy.top/gtqdlpydbl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sufxvd.cn/gthrmoomta.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.chenlongwang.top/gtoagzkbhf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhongyouzk.top/gtwnazzqqc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yj20258.top/gtrfhpxkky.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj20258.top/gtdvudzlzk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cheryme.top/gtsaejkgqp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shanyushiyangkeji.top/gtnfizhqdb.html

JS:   resp.ok;  resp.status
来源：http://hz.bjfxy.top/gtrahcfjzt.html

TS:   resp.ok;  resp.status
来源：http://hz.yvedp.cn/gtkonoahhg.html

Java: resp.statusCode()
来源：http://hz.tianlin.xyz/gtqlsidsrb.html

Go:   resp.StatusCode
来源：http://hz.aizwys.cn/gtokcvrhsf.html

Ruby: resp.code.to_i
来源：http://hz.jqgufenzy.top/gtthrhrasu.html

C#:   (int)resp.StatusCode
来源：http://hz.yuxming.cn/gtbsjlwaqo.html

[L08] 并发请求多个地址
来源：http://hz.tianlin.xyz/gtftvorrrf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hfpthk.cn/gtemnyqvdb.html

PHP:  curl_multi_init() 系列
来源：http://hz.havefunace.top/gtzuvvmrto.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xingfuxueyuan.xyz/gtvudxxven.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgfzy.top/gtiwxsvbia.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.guowangkeji.top/gtwjwoiolc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhiwuduotai.top/gtegbauhsp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.52xcode.cn/gtjzhqproz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yueranfly.top/gtesgbyjdj.html

================================================================================
来源：http://hz.316326.xyz/gthtteryre.html

M. 命令行 / 进程 / 环境
来源：http://hz.havefunace.top/gtucqjuwta.html

================================================================================
来源：http://hz.ehwqpu.com/gtuefkkgba.html

[M01] 读取命令行参数
来源：http://hz.zhiwuduotai.top/gtcarfkehn.html

Py:   sys.argv[1:]
来源：http://hz.zhoulong.xyz/gtabqjtlqh.html

PHP:  $argv;  $argc;
来源：http://hz.zhongyouzk.top/gtaeymseom.html

JS:   process.argv.slice(2)
来源：http://hz.kuanghao11.cn/gtplapzzyu.html

TS:   process.argv.slice(2)
来源：http://hz.sxryk.cn/gtrlqvpafj.html

Java: args 数组（main 方法参数）
来源：http://hz.52xcode.cn/gtoicqwngo.html

Go:   os.Args[1:]
来源：http://hz.sxryk.cn/gtftyxnzvu.html

Ruby: ARGV
来源：http://hz.nanxuanxn.top/gtieidvkaf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yonumen.top/gtcqhjycyx.html

[M02] 读取环境变量
来源：http://hz.zhengqikj.top/gtgynibbmv.html

Py:   os.environ.get("HOME")
来源：http://hz.c1oappe.top/gtuxrejbnl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.gzhubu.top/gtkyvjlpvm.html

JS:   process.env.HOME
来源：http://hz.xingfuxueyuan.xyz/gtsaovjeio.html

TS:   process.env.HOME
来源：http://hz.zhongyouzk.top/gtrefopppe.html

Java: System.getenv("HOME")
来源：http://hz.andypj.xyz/gtckyjervl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.52xcode.cn/gtusjaxzwp.html

Ruby: ENV["HOME"]
来源：http://hz.ybcxt.top/gtofdulicn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gogol.net.cn/gtsyqxyvam.html

[M03] 执行外部命令
来源：http://hz.316326.xyz/gtnbfywvta.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jianghu66.top/gtgqkqfklr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shzxlz.cn/gtdbxzqkff.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zycfv.cn/gtsgspmrtb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shangyingyoupin.top/gtaapcqccp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhaomingkeji.xyz/gtgjmazbca.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.c1oappe.top/gtpqlknphm.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.chenjidiqi.icu/gtoakuvmvg.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhoulong.xyz/gtjwyxvspa.html

[M04] 获取当前工作目录
来源：http://hz.kuanghao11.cn/gtteeelklh.html

Py:   os.getcwd()
来源：http://hz.vqdsnc.cn/gtuaoalpug.html

PHP:  getcwd();
来源：http://hz.vqdsnc.cn/gtgseignem.html

JS:   process.cwd()
来源：http://hz.feifeiyinyue.top/gtdupjxsin.html

TS:   process.cwd()
来源：http://hz.jqgufenzy.top/gtcqvhmloq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gogol.net.cn/gtpwgssmsb.html

Go:   os.Getwd()
来源：http://hz.ydzc1.top/gtlrrjkhml.html

Ruby: Dir.pwd
来源：http://hz.birdmap.top/gtentyjguq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.andypj.xyz/gtmnulgfiz.html

[M05] 设置退出码
来源：http://hz.snrcjt.cn/gtftxaectj.html

Py:   sys.exit(1)
来源：http://hz.jinghuilouyu.cn/gtajlhgnrd.html

PHP:  exit(1);
来源：http://hz.dianchejie.cn/gtjkfufdzo.html

JS:   process.exit(1)
来源：http://hz.zhijiandao.cn/gthnogkcca.html

TS:   process.exit(1)
来源：http://hz.52xcode.cn/gtkcfvterp.html

Java: System.exit(1)
来源：http://hz.aizwys.cn/gtfngtwthf.html

Go:   os.Exit(1)
来源：http://hz.bjfxy.top/gtdunibhav.html

Ruby: exit 1
来源：http://hz.cqqwz.cn/gtvcymketw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shzxlz.cn/gtkydcrwir.html

[M06] 向标准错误输出
来源：http://hz.bjfxy.top/gtuvswzjky.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yj20258888.top/gtwcydivvy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ydzc1.top/gtcqflmslv.html

JS:   console.error("err")
来源：http://hz.jinqigufen.top/gtvlzfpgza.html

TS:   console.error("err")
来源：http://hz.0kj1m.cn/gtpailqyoy.html

Java: System.err.println("err")
来源：http://hz.zhengqikj.top/gtviecyjgh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yuanzhike.top/gtoeyffspx.html

Ruby: warn "err"
来源：http://hz.zhaomingkeji.xyz/gtzebsqgrq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.feifeiyinyue.top/gtxjvsahyy.html

[M07] 判断是否为主入口
来源：http://hz.nanxinkj.top/gtxslczaeq.html

Py:   if __name__ == "__main__":
来源：http://hz.52xcode.cn/gttjuwnewo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.iojbl.cn/gthxdsbmbr.html

JS:   require.main === module
来源：http://hz.dianchejie.cn/gtqvzxnuir.html

TS:   require.main === module
来源：http://hz.daxiang520.top/gtgyvabgtv.html

Java: public static void main(String[] args)
来源：http://hz.yonumen.top/gttxyumlzk.html

Go:   func main()
来源：http://hz.ybcxt.top/gtvyidrlwd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.aizwys.cn/gtafpyaewa.html

C#:   static void Main(string[] args)
来源：http://hz.wangdashe.top/gtfajdwocn.html

[M08] 获取系统与运行时信息
来源：http://hz.9152youxi.cn/gtpvvhpsub.html

Py:   platform.system();  platform.python_version()
来源：http://hz.daria6918.cn/gtmmjmrztj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tianlin.xyz/gtymyxzsmy.html

JS:   process.platform;  process.version
来源：http://hz.daxiang520.top/gtclczruvf.html

TS:   process.platform;  process.version
来源：http://hz.daxiang520.top/gtdautykdb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.wangshuangyany.cn/gtbutiwclg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.haohaochexian.top/gtmlemkklu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.pengpengdd.cyou/gterkozglq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.wangshuangyany.cn/gtmpaqteik.html

================================================================================
来源：http://hz.redwolf501.top/gtjepbckpr.html

N. 数据结构与算法
来源：http://hz.pycfn.com/gtbfeiptja.html

================================================================================
来源：http://hz.tian-w.cn/gtcqmwwarz.html

[N01] 二分查找（有序数组）
来源：http://hz.cashguo.top/gteguadtkv.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zycfv.cn/gtkmasioep.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cqqwz.cn/gtedglqwwl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gaohongyu789.top/gtpetlusso.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cashguo.top/gtyrkuwtgo.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.sxryk.cn/gtqkomzbxb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.0kj1m.cn/gtgcvhxfdi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yj202588.top/gtyqjvuivy.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.fengsongda.top/gtnskzermu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ydzc1.top/gtxnjcxnix.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gogol.net.cn/gtdpobaamo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj20258.top/gtixsuaeyg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhongyouzk.top/gtqvjrpjii.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtjenxdfck.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.aizwys.cn/gtizmukyyv.html

Go:   slices.Sort(arr)
来源：http://hz.aizwys.cn/gtwjkfyioq.html

Ruby: arr.sort
来源：http://hz.vqdsnc.cn/gtjaarshwt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hnxiangtu.top/gtdrbxmdwb.html

[N03] 快速排序（分治示例）
来源：http://hz.hammf.cn/gtjyfvojvu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.fzhhl.top/gtnnjupdyw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.c1oappe.top/gtdxramzsi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tianlin.xyz/gtgpmmongi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.redwolf501.top/gtppitqohn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ivvv.top/gtwdnrdhhw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.c1oappe.top/gtgreipxkj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yj202588.top/gtrbtwnbmx.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.aibaodan.cn/gtxcoxnziz.html

[N04] 斐波那契数列
来源：http://hz.dianchejie.cn/gtkqxyjbcz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhengqikj.top/gtzpevgrmg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hnqzz.top/gtbffeoglf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.wangshuangyany.cn/gtucsxezwq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.birdmap.top/gtlwviudgm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.meibo888.top/gtgjbikqxd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shanyushiyangtech.top/gtovxtolzl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cqqwz.cn/gtrmbqourl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ehwqpu.com/gtjxrbfefd.html

[N05] 最大公约数
来源：http://hz.wangshuangyany.cn/gthxvafwja.html

Py:   math.gcd(a, b)
来源：http://hz.yuanzhike.top/gtcmihbtgv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhoulong.xyz/gtvfcosinu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnqzz.top/gtmjfdzwna.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xylfe.cn/gtlmchqfqr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.andypj.xyz/gtrzzsfcld.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.fzhhl.top/gtnbvesgvh.html

Ruby: a.gcd(b)
来源：http://hz.tianlin.xyz/gtydzgzson.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ehwqpu.com/gthgxcuohw.html

[N06] 判断回文字符串
来源：http://hz.dashuyun.cn/gtxoxqivcq.html

Py:   s == s[::-1]
来源：http://hz.316326.xyz/gtntpfxgjm.html

PHP:  $s === strrev($s);
来源：http://hz.yj20258.top/gtxqmmvyqf.html

JS:   s === [...s].reverse().join("")
来源：http://hz.snrcjt.cn/gtnhzwqztz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.wangdashe.top/gtmaqljdcj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ydjk.org.cn/gtinfnmpyl.html

Go:   // 双指针从两端比较
来源：http://hz.andypj.xyz/gtlhfixafq.html

Ruby: s == s.reverse
来源：http://hz.pengpengdd.cyou/gtripdyipn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.fzhhl.top/gtzbosgsgz.html

[N07] 两数之和（返回下标）
来源：http://hz.nwbrower.top/gtqjwizrav.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.fengsongda.top/gtezssebmp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shanyushiyangkeji.top/gtsgkbqjkh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhiwuduotai.top/gtkfpyxnau.html

TS:   // 手写 Map<string, number>
来源：http://hz.jyoumei.cn/gtoelnebds.html

Java: // 手写 HashMap
来源：http://hz.chenlongwang.top/gtggyrcrvd.html

Go:   // 手写 map[int]int
来源：http://hz.zdqjudy.top/gtlqraqrvg.html

Ruby: // 手写 Hash
来源：http://hz.yueranfly.top/gtinullotq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xuanzx.com/gthqbzdfav.html

[N08] 生成全排列
来源：http://hz.hywenlv.cn/gtwciioykb.html

Py:   itertools.permutations(arr)
来源：http://hz.zhiwuduotai.top/gtlkfmtojy.html

PHP:  // 手写递归交换
来源：http://hz.smart0.xyz/gtilmgbbuv.html

JS:   // 手写回溯递归
来源：http://hz.kuanghao11.cn/gtyxzbuojc.html

TS:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtcgeicmgn.html

Java: // 手写回溯递归
来源：http://hz.iojbl.cn/gtnxkrerxi.html

Go:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtindhcltt.html

Ruby: arr.permutation.to_a
来源：http://hz.yj20258.top/gtgidzgabj.html

C#:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtshwlllep.html

[N09] 栈与队列
来源：http://hz.nanxuanxn.top/gtthcsikqe.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ydzc1.top/gtissyvfiu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.fengsongda.top/gtkceakxji.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.sweek.top/gtetujftbj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj20258.top/gtvxfucgli.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.meibo888.top/gtwhxvjnen.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shangyingyoupin.top/gtimgnaett.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.dashuyun.cn/gteevxbysh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cashguo.top/gtvuabcndo.html

[N10] 链表节点定义
来源：http://hz.jinqigufen.top/gtxtvcujxp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.andypj.xyz/gtsxkwjwlv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.daria6918.cn/gtvznvnzwe.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.haohaochexian.top/gtyskebgjp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.daria6918.cn/gtxhfsostw.html

Java: class Node { int v; Node next; }
来源：http://hz.sweek.top/gtylbxkmhc.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xuetiantiany.cn/gtchvnxfeg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.guowangkeji.top/gteruelizs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yvedp.cn/gtnlgkcaac.html

[N11] 二叉树中序遍历
来源：http://hz.hnqzz.top/gtlgansfre.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xingfuxueyuan.xyz/gtymdzfnre.html

PHP:  // 手写递归函数
来源：http://hz.cdnleiting.top/gtzzlbptbp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fengsongda.top/gtlpiwlwkj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gotoacloud.top/gtaiwauccu.html

Java: // 手写递归
来源：http://hz.pycfn.com/gtskqsabek.html

Go:   // 手写递归
来源：http://hz.yueranfly.top/gtkzgtpdzi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.316326.xyz/gtzrjbbben.html

C#:   // 手写递归
来源：http://hz.hywenlv.cn/gtnpgytshg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.iojbl.cn/gtkedjtuyk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhongyouzk.top/gtlndgtjzl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.wangdashe.top/gtprenchwz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hongshengwenyu.top/gtlsdbztof.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydzc1.top/gtesvekmwy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jianghu66.top/gtfxdykyjb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.cheryme.top/gtmefmjyyn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.dashuyun.cn/gtnbsxbcoo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangkeji.top/gtqszhrhnu.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtmdkjojop.html

O. 并发与异步
来源：http://hz.gaohongyu789.top/gtenjtvpgd.html

================================================================================
来源：http://hz.yueranfly.top/gtddckmogi.html

[O01] 启动一个线程
来源：http://hz.yuxming.cn/gtzptpdcdx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.nanxinkj.top/gtiecaffcn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinqigfzy.top/gtarobkftq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.wangdashe.top/gtpuvdggof.html

TS:   // 同 JS
来源：http://hz.ybcxt.top/gtuhgcygdn.html

Java: new Thread(() -> f()).start()
来源：http://hz.shuidangran.top/gttvapwkbu.html

Go:   go f()
来源：http://hz.meibo888.top/gtfklwivyz.html

Ruby: Thread.new { f }
来源：http://hz.gogol.net.cn/gtkwkxuuil.html

C#:   Task.Run(() => F());
来源：http://hz.gaohongyu789.top/gtoslnvwsu.html

[O02] 使用线程池
来源：http://hz.cashguo.top/gtvmtffrzb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sysykeji.top/gtogcsgzms.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nwbrower.top/gtpzvqoswh.html

JS:   // worker_threads 线程池
来源：http://hz.xylfe.cn/gtzffgugov.html

TS:   // worker_threads 线程池
来源：http://hz.redwolf501.top/gtlqumkuvh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.9152youxi.cn/gtapcnxhdy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.pycfn.com/gthfecohas.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xinyue.icu/gtyxeylinl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jyoumei.cn/gtykfaghpd.html

[O03] 加锁保护共享数据
来源：http://hz.fzhhl.top/gturpxchwm.html

Py:   with lock: shared += 1
来源：http://hz.zhijiandao.cn/gtgeufynin.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yueranfly.top/gtorrjtzgk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenlongwang.top/gtmwrfperb.html

TS:   // 同 JS
来源：http://hz.daria6918.cn/gttewcwdov.html

Java: synchronized (this) { shared++; }
来源：http://hz.ppjwa.cn/gtafsqatkm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jinqigufen.top/gtqyzdepbn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jyoumei.cn/gtaaoebawp.html

C#:   lock (gate) { shared++; }
来源：http://hz.ppjwa.cn/gtjcujsjen.html

[O04] 定义异步函数并等待
来源：http://hz.nanxinkj.top/gtxtovbxiw.html

Py:   async def f():⏎    await g()
来源：http://hz.shzxlz.cn/gtoxzpxrmp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hnqzz.top/gtcnnfubbp.html

JS:   async function f() { await g(); }
来源：http://hz.mhx1999.top/gtomifiyte.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jiagoushi.top/gtfubvtpwp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jqgfzy.top/gtdncckeyg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.nwbrower.top/gtdpqazrsq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hammf.cn/gtdimkimwe.html

C#:   async Task F() { await G(); }
来源：http://hz.zhengqikj.top/gthkwumszj.html

[O05] 并发执行并等待全部完成
来源：http://hz.chenjidiqi.icu/gteqenxhrt.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shzxlz.cn/gtlntjvfqo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.guannengcc.top/gtlkikueoc.html

JS:   await Promise.all(tasks)
来源：http://hz.fzhhl.top/gtissniecp.html

TS:   await Promise.all(tasks)
来源：http://hz.daxiang520.top/gtwfroszku.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yueranfly.top/gtfpyldxdj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jqgufenzy.top/gtlqhhixzf.html

Ruby: threads.map(&:join)
来源：http://hz.316326.xyz/gtbjgqjzgn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.sysykeji.top/gtrajbwoet.html

[O06] 使用进程池
来源：http://hz.zhengqikj.top/gtnurpkigq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hywenlv.cn/gtgitgppjk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hnxiangtu.top/gtxddbepsg.html

JS:   // child_process / cluster 模块
来源：http://hz.jinyuanbaomall.cn/gtbvxjerxt.html

TS:   // child_process / cluster 模块
来源：http://hz.gogol.net.cn/gtrqcjrvti.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.kuanghao11.cn/gtbeqrtlzf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.daria6918.cn/gtifzqzldy.html

Ruby: // fork 块
来源：http://hz.zhengqikj.top/gtzcxcbvcn.html

C#:   Parallel.For
来源：http://hz.mhx1999.top/gtbczihjfo.html

================================================================================
来源：http://hz.yj20258888.top/gtvwdeluhh.html

P. 常用工具函数
来源：http://hz.gotoacloud.top/gtaqcgrmig.html

================================================================================
来源：http://hz.quarkkingdee.top/gtzqtryepi.html

[P01] 生成 UUID
来源：http://hz.mhx1999.top/gtuqnblkfz.html

Py:   str(uuid.uuid4())
来源：http://hz.fengsongda.top/gtinaquibv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.daxiang520.top/gtmkxfuikp.html

JS:   crypto.randomUUID()
来源：http://hz.tanke756.top/gtydkuuhbo.html

TS:   crypto.randomUUID()
来源：http://hz.fengsongda.top/gtmlimewnn.html

Java: UUID.randomUUID().toString()
来源：http://hz.316326.xyz/gtxgqylngj.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gogol.net.cn/gtxxzhggtl.html

Ruby: SecureRandom.uuid
来源：http://hz.yuxming.cn/gttbpuozpv.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hammf.cn/gtrgqtboil.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hfpthk.cn/gtivcqqhna.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.aizwys.cn/gtgoiuuevw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.cqqwz.cn/gtosdhjmkg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yonumen.top/gtsonyrahq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhoulong.xyz/gtalincjpj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.redwolf501.top/gtndfqsevi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gzhubu.top/gtuzupmvdd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xylfe.cn/gtrhbrjsrd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.fzhhl.top/gtsyvknxjs.html

[P03] 生成短随机字符串
来源：http://hz.feifeiyinyue.top/gtzgbsjakb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.daxiang520.top/gtouvshsoz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cheryme.top/gtqgryqtau.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.aibaodan.cn/gtcqeqqcgl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuxming.cn/gtrlvnfhos.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.redwolf501.top/gtcxsgkgzn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.feifeiyinyue.top/gtlefhtvow.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gzhubu.top/gtmflkspec.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xziqi.cn/gtmrobbxxh.html

[P04] 求长度
来源：http://hz.ydzc1.top/gtszsbjwii.html


<!-- 参考信息 -->