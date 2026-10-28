代发 wailian999

Py:   resp.json()
来源：http://hz.gzhubu.top/gteoqqeodt.html

PHP:  json_decode($body, true);
来源：http://hz.chenzaomai.com/gtimhtsgqo.html

JS:   await resp.json()
来源：http://hz.ywan-chungtsiang.top/gtkcuavsmi.html

TS:   await resp.json()
来源：http://hz.hysaishi.cn/gttlmcxynl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nanxuanxn.top/gtukqfvyfz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hysaishi.cn/gtpikmarnm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.kuanghao11.cn/gtaxaigrec.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hywenlv.cn/gticzrjesa.html

[L07] 处理 HTTP 状态码
来源：http://hz.daxiang520.top/gtsjskeyda.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xziqi.cn/gtwrdrfboz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.52xcode.cn/gtetnixmlo.html

JS:   resp.ok;  resp.status
来源：http://hz.haohaochexian.top/gtrmzklucw.html

TS:   resp.ok;  resp.status
来源：http://hz.0kj1m.cn/gtqgomqcme.html

Java: resp.statusCode()
来源：http://hz.shzxlz.cn/gtcwinopgf.html

Go:   resp.StatusCode
来源：http://hz.52xcode.cn/gtbblsatub.html

Ruby: resp.code.to_i
来源：http://hz.zhengqikj.top/gtatvhhsuy.html

C#:   (int)resp.StatusCode
来源：http://hz.tianlin.xyz/gtekmxsnwh.html

[L08] 并发请求多个地址
来源：http://hz.shuidangran.top/gtfyfucobn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.bjfxy.top/gthtkussvr.html

PHP:  curl_multi_init() 系列
来源：http://hz.vqdsnc.cn/gtfaghfwwl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jiagoushi.top/gtrmfnzgcp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtojtjaguz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xuanzx.com/gtepxzasin.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.daxiang520.top/gtrgxkvpaq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ivvv.top/gtfrjpdgmu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.nanxinkj.top/gtvonnzzym.html

================================================================================
来源：http://hz.redwolf501.top/gtlmeknwjp.html

M. 命令行 / 进程 / 环境
来源：http://hz.wangdashe.top/gtsyiswxzf.html

================================================================================
来源：http://hz.tianlin.xyz/gtjzaludei.html

[M01] 读取命令行参数
来源：http://hz.feifeiyinyue.top/gtyiiexdaj.html

Py:   sys.argv[1:]
来源：http://hz.snrcjt.cn/gtxfingpuz.html

PHP:  $argv;  $argc;
来源：http://hz.cucudq.cn/gtzwjbwfsy.html

JS:   process.argv.slice(2)
来源：http://hz.zhixingplan.top/gtbvinakwb.html

TS:   process.argv.slice(2)
来源：http://hz.zdqjudy.top/gtnbloktcm.html

Java: args 数组（main 方法参数）
来源：http://hz.gotoacloud.top/gttbimhgks.html

Go:   os.Args[1:]
来源：http://hz.chenjidiqi.icu/gtzktfszsl.html

Ruby: ARGV
来源：http://hz.yuanzhike.top/gtjpjnjjdr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jianghu66.top/gtbalemuon.html

[M02] 读取环境变量
来源：http://hz.cucudq.cn/gtqwxvnegg.html

Py:   os.environ.get("HOME")
来源：http://hz.zhixingplan.top/gtbadmckrj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.9152youxi.cn/gtvqudbfll.html

JS:   process.env.HOME
来源：http://hz.yj202588.top/gtxtoxdmwr.html

TS:   process.env.HOME
来源：http://hz.zhixingplan.top/gtktmslboo.html

Java: System.getenv("HOME")
来源：http://hz.aibaodan.cn/gtiqwpvjvx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cqqwz.cn/gtfawgrdio.html

Ruby: ENV["HOME"]
来源：http://hz.hfpthk.cn/gtbpivvxkk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yj20258.top/gtuxoyohqi.html

[M03] 执行外部命令
来源：http://hz.birdmap.top/gtojhvdrmk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhijiandao.cn/gtgmmiauro.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ywan-chungtsiang.top/gtxivedwls.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.haohaochexian.top/gtvhvcpndf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.iojbl.cn/gtoxuegavr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.shzxlz.cn/gthmnilbzc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.daxiang520.top/gtraoamgsf.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jyoumei.cn/gtytjddtjw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jianghu66.top/gtxtnxeujd.html

[M04] 获取当前工作目录
来源：http://hz.yanxiufei.cn/gtvoylaung.html

Py:   os.getcwd()
来源：http://hz.yanxiufei.cn/gtjyjtspfo.html

PHP:  getcwd();
来源：http://hz.zhaomingkeji.xyz/gtsnjemziz.html

JS:   process.cwd()
来源：http://hz.wangshuangyany.cn/gtvivzjrbn.html

TS:   process.cwd()
来源：http://hz.jianghu66.top/gtfglmlffg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sxryk.cn/gtklaoshct.html

Go:   os.Getwd()
来源：http://hz.ehwqpu.com/gtvtqgrgoh.html

Ruby: Dir.pwd
来源：http://hz.jinghuilouyu.cn/gtbvwyulug.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ywan-chungtsiang.top/gtjszcxslb.html

[M05] 设置退出码
来源：http://hz.jlsjyb.cn/gteoykqcdj.html

Py:   sys.exit(1)
来源：http://hz.jqgfzy.top/gtfwsksmxe.html

PHP:  exit(1);
来源：http://hz.daxiang520.top/gtcubywrno.html

JS:   process.exit(1)
来源：http://hz.yangfankeji.com/gtvhoqwuia.html

TS:   process.exit(1)
来源：http://hz.zhengqikj.top/gttfruggxs.html

Java: System.exit(1)
来源：http://hz.jlsjyb.cn/gtoqeqneup.html

Go:   os.Exit(1)
来源：http://hz.shzxlz.cn/gtjthaqnew.html

Ruby: exit 1
来源：http://hz.sufxvd.cn/gtcmxfaahc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hongshengwenyu.top/gtoiagulxy.html

[M06] 向标准错误输出
来源：http://hz.yuanzhike.top/gtiamrcers.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yongpay.top/gtfngfcufj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yuanzhike.top/gtewwabyyu.html

JS:   console.error("err")
来源：http://hz.shzxlz.cn/gtqllgsoeg.html

TS:   console.error("err")
来源：http://hz.xylfe.cn/gtpiubvjsf.html

Java: System.err.println("err")
来源：http://hz.zhongyouzk.top/gtdxqhplwx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ivvv.top/gtqrhhragk.html

Ruby: warn "err"
来源：http://hz.smart0.xyz/gtxbzfmbdq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.pycfn.com/gtiqkkclqo.html

[M07] 判断是否为主入口
来源：http://hz.zhijiandao.cn/gtuzvfwnsq.html

Py:   if __name__ == "__main__":
来源：http://hz.pengpengdd.cyou/gtxtvvudkg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shzxlz.cn/gteehmmmkd.html

JS:   require.main === module
来源：http://hz.sysykeji.top/gtebdrjznc.html

TS:   require.main === module
来源：http://hz.haohaochexian.top/gtawvcbtii.html

Java: public static void main(String[] args)
来源：http://hz.hywenlv.cn/gtineoqfqp.html

Go:   func main()
来源：http://hz.zhoulong.xyz/gtqwsrazgh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhoulong.xyz/gtwooegmed.html

C#:   static void Main(string[] args)
来源：http://hz.yvedp.cn/gtrcrtzxom.html

[M08] 获取系统与运行时信息
来源：http://hz.dianchejie.cn/gtwpuvvxfi.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hnxiangtu.top/gtjvrzpnny.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.bjfxy.top/gtdznevjcb.html

JS:   process.platform;  process.version
来源：http://hz.tanke756.top/gtxjtenidd.html

TS:   process.platform;  process.version
来源：http://hz.gotoacloud.top/gteymyfash.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.iojbl.cn/gturwunbdq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xylfe.cn/gtmevelmta.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jqgufenzy.top/gthnrvvbsh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yuxming.cn/gtkeshopun.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtxrodlbme.html

N. 数据结构与算法
来源：http://hz.tanke756.top/gtrwkpcxrt.html

================================================================================
来源：http://hz.hywenlv.cn/gtdbxlyimq.html

[N01] 二分查找（有序数组）
来源：http://hz.gaohongyu789.top/gtpgamqcgy.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shangyingyoupin.top/gtanjfkfzl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.chenjidiqi.icu/gtwxfoakct.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.svipenyu.cn/gtfqycermv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.andypj.xyz/gtetcojrwb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jianghu66.top/gttffrbufv.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shanyushiyangtech.top/gtqahtrxja.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.quarkkingdee.top/gtvjmfsdqo.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtlgapdkdz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.svipenyu.cn/gtadsszcfz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xziqi.cn/gtbatkagmn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.chenlongwang.top/gtjfiqsajw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.birdmap.top/gtbohgqygj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuanzhike.top/gttzuwfhcz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ivvv.top/gtsbbhtbuk.html

Go:   slices.Sort(arr)
来源：http://hz.zhixingplan.top/gtrulangny.html

Ruby: arr.sort
来源：http://hz.jyoumei.cn/gtiztjsarz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ydzc1.top/gtuedxrxkg.html

[N03] 快速排序（分治示例）
来源：http://hz.zhengqikj.top/gtdsjluotw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hongshengwenyu.top/gtfotrnatk.html

PHP:  // 递归实现，或用 usort
来源：http://hz.dashuyun.cn/gtizhvnrdg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhixingplan.top/gtkqttcjuo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hammf.cn/gtnxuperni.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cqqwz.cn/gtphnwjbno.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yj20258888.top/gtmvjvaztr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cashguo.top/gtxdssnrks.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gotoacloud.top/gtrwhmezmg.html

[N04] 斐波那契数列
来源：http://hz.hammf.cn/gtohapxyjh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ywan-chungtsiang.top/gtblncnpdp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.daxiang520.top/gtxghhdyky.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hysaishi.cn/gtvpdxrmvu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnxiangtu.top/gtgqsjrdih.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.birdmap.top/gtzdzyhyiv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhongyouzk.top/gtrykntuam.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cqqwz.cn/gtymmgxxpo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.quarkkingdee.top/gtlyszrpat.html

[N05] 最大公约数
来源：http://hz.jianghu66.top/gtcwzbafeo.html

Py:   math.gcd(a, b)
来源：http://hz.yj20258888.top/gtqvcqafkm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhoulong.xyz/gtviexbzfc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hywenlv.cn/gtwhyvglun.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guannengcc.top/gtjikttlpc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.svipenyu.cn/gttjiieoxl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.guannengcc.top/gtwlhblzbv.html

Ruby: a.gcd(b)
来源：http://hz.birdmap.top/gtyhilbzck.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jianghu66.top/gtbpoajczf.html

[N06] 判断回文字符串
来源：http://hz.sweek.top/gtuvidkxju.html

Py:   s == s[::-1]
来源：http://hz.yuanzhike.top/gtdxsccsqu.html

PHP:  $s === strrev($s);
来源：http://hz.316326.xyz/gtwhsarxmh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.guowangkeji.top/gtnjfibenv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hnqzz.top/gtoaaadzhf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.gzhubu.top/gtwrrstjmb.html

Go:   // 双指针从两端比较
来源：http://hz.smart0.xyz/gtltcgdnkd.html

Ruby: s == s.reverse
来源：http://hz.0kj1m.cn/gtyviqrijh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.fengsongda.top/gtaliakqvq.html

[N07] 两数之和（返回下标）
来源：http://hz.vqdsnc.cn/gtpxgitegd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.vqdsnc.cn/gtssnrxrvo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hysaishi.cn/gtzbogclxh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yonumen.top/gtqsehujof.html

TS:   // 手写 Map<string, number>
来源：http://hz.chenlongwang.top/gtimoowfpg.html

Java: // 手写 HashMap
来源：http://hz.smart0.xyz/gtwdpbtqgi.html

Go:   // 手写 map[int]int
来源：http://hz.yanxiufei.cn/gthehbjszc.html

Ruby: // 手写 Hash
来源：http://hz.dianchejie.cn/gtmljsqzzs.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hfpthk.cn/gtvmvzzysi.html

[N08] 生成全排列
来源：http://hz.svipenyu.cn/gtdozoswuo.html

Py:   itertools.permutations(arr)
来源：http://hz.gogol.net.cn/gtnyczaerk.html

PHP:  // 手写递归交换
来源：http://hz.yj202588.top/gtzysnnxtn.html

JS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gthfcrssjg.html

TS:   // 手写回溯递归
来源：http://hz.pycfn.com/gtjwdgvrdk.html

Java: // 手写回溯递归
来源：http://hz.hnqzz.top/gtlpofpols.html

Go:   // 手写回溯递归
来源：http://hz.snrcjt.cn/gtkhshnqol.html

Ruby: arr.permutation.to_a
来源：http://hz.xuetiantiany.cn/gtuyblsrpb.html

C#:   // 手写回溯递归
来源：http://hz.cheryme.top/gtjeliimky.html

[N09] 栈与队列
来源：http://hz.pengpengdd.cyou/gtkplhatbm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.quarkkingdee.top/gtvghdgamr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ybcxt.top/gtnwyacryk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yanxiufei.cn/gtkanjjzva.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yongpay.top/gtmrqalvkf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.aibaodan.cn/gtofvxkzgy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shangyingyoupin.top/gtymcgwghx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yonumen.top/gtysulyglg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.vqdsnc.cn/gtujrtsrxu.html

[N10] 链表节点定义
来源：http://hz.jqgfzy.top/gtudoutztd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hongshengwenyu.top/gtrvooomym.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hnxiangtu.top/gtmkguulnl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cashguo.top/gtjhwqtuis.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yvedp.cn/gtzdhnwxha.html

Java: class Node { int v; Node next; }
来源：http://hz.9152youxi.cn/gtxuidxsng.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xylfe.cn/gthbhfxcsu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ywan-chungtsiang.top/gtisompobf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.sweek.top/gtgijqazyq.html

[N11] 二叉树中序遍历
来源：http://hz.zhixingplan.top/gtywdchvwr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.andypj.xyz/gtuznxbosf.html

PHP:  // 手写递归函数
来源：http://hz.cdnleiting.top/gthrmmqleq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.andypj.xyz/gthulvutuz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenjidiqi.icu/gttjewffsh.html

Java: // 手写递归
来源：http://hz.pengpengdd.cyou/gthhmhsirh.html

Go:   // 手写递归
来源：http://hz.zycfv.cn/gtmbudpvfv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.9152youxi.cn/gtvhochxjg.html

C#:   // 手写递归
来源：http://hz.yangfankeji.com/gtzhuhjpst.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shuidangran.top/gtskucqdtt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhengqikj.top/gtznbuqkvy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.316326.xyz/gtusupizhy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.pengpengdd.cyou/gtonnripwa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sysykeji.top/gtdbvtnlnr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.birdmap.top/gtyitiuwyb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.nanxinkj.top/gtvasxpkgo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.bjfxy.top/gtbxiekerg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gtaqtwmrsk.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtrygaarxu.html

O. 并发与异步
来源：http://hz.gotoacloud.top/gtxozwyyvn.html

================================================================================
来源：http://hz.cheryme.top/gtjkkqmtgh.html

[O01] 启动一个线程
来源：http://hz.zhijiandao.cn/gtjgysiijk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.tian-w.cn/gtwkiobjte.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.aizwys.cn/gtrqpohabw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.c1oappe.top/gtuhmuylgw.html

TS:   // 同 JS
来源：http://hz.jinqigfzy.top/gtrnlwewej.html

Java: new Thread(() -> f()).start()
来源：http://hz.yuanzhike.top/gtdqsewyfe.html

Go:   go f()
来源：http://hz.yonumen.top/gtpscygxhw.html

Ruby: Thread.new { f }
来源：http://hz.zdqjudy.top/gtwveujjuu.html

C#:   Task.Run(() => F());
来源：http://hz.xuetiantiany.cn/gtcknuzrps.html

[O02] 使用线程池
来源：http://hz.vqdsnc.cn/gtbhqkvmbl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xziqi.cn/gthpwnpzqa.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.andypj.xyz/gtpbvbimyw.html

JS:   // worker_threads 线程池
来源：http://hz.xingfuxueyuan.xyz/gtrxdtverg.html

TS:   // worker_threads 线程池
来源：http://hz.jinghuilouyu.cn/gttaomciwr.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hysaishi.cn/gtswhowwro.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gzhubu.top/gtbmtzhayw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yj20258888.top/gturbfgiic.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gogol.net.cn/gthwjkywzb.html

[O03] 加锁保护共享数据
来源：http://hz.tianlin.xyz/gtwjeqbhzl.html

Py:   with lock: shared += 1
来源：http://hz.quarkkingdee.top/gtadtvxnzb.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yj202588.top/gtaxchjizb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.nanxinkj.top/gtvhfefglb.html

TS:   // 同 JS
来源：http://hz.yj20258888.top/gthpqyyofa.html

Java: synchronized (this) { shared++; }
来源：http://hz.fengsongda.top/gtmqgbacdg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hnqzz.top/gtqxztgkvm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jiagoushi.top/gteiiaadjh.html

C#:   lock (gate) { shared++; }
来源：http://hz.smart0.xyz/gtaieingck.html

[O04] 定义异步函数并等待
来源：http://hz.jqgfzy.top/gtlyzjnaly.html

Py:   async def f():⏎    await g()
来源：http://hz.hywenlv.cn/gtnqixnphk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jiagoushi.top/gtoxgmfmpn.html

JS:   async function f() { await g(); }
来源：http://hz.52xcode.cn/gtfknccvha.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cucudq.cn/gtlgxawyqw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.nanxinkj.top/gtmnxcoowx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.316326.xyz/gtzjmnoaje.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jqgufenzy.top/gtmcioftso.html

C#:   async Task F() { await G(); }
来源：http://hz.bjfxy.top/gtbiqutsxs.html

[O05] 并发执行并等待全部完成
来源：http://hz.xylfe.cn/gtnviqjxlv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.andypj.xyz/gtlqozyljv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhiwuduotai.top/gtnqvevcjh.html

JS:   await Promise.all(tasks)
来源：http://hz.xinyue.icu/gtyjafvzvq.html

TS:   await Promise.all(tasks)
来源：http://hz.kuanghao11.cn/gtgbvaigns.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yuxming.cn/gthtgzzyvw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shanyushiyangkeji.top/gtljxcuwbw.html

Ruby: threads.map(&:join)
来源：http://hz.cqqwz.cn/gtblzhmtfx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.gotoacloud.top/gtnfyworoa.html

[O06] 使用进程池
来源：http://hz.pengpengdd.cyou/gtvqaisodw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hywenlv.cn/gtjtenbaay.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yuanzhike.top/gtvpcrvzje.html

JS:   // child_process / cluster 模块
来源：http://hz.tanke756.top/gtjqhzlbdv.html

TS:   // child_process / cluster 模块
来源：http://hz.fzhhl.top/gtgblkhshl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yangfankeji.com/gtfnhvwcxo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nwbrower.top/gtrxvqsard.html

Ruby: // fork 块
来源：http://hz.yanxiufei.cn/gtbktjgcqm.html

C#:   Parallel.For
来源：http://hz.shzxlz.cn/gtbxbdmixk.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtjbsxbgii.html

P. 常用工具函数
来源：http://hz.zdqjudy.top/gtvlcfbylx.html

================================================================================
来源：http://hz.c1oappe.top/gtyxzikdqu.html

[P01] 生成 UUID
来源：http://hz.hywenlv.cn/gtjvxpqtuv.html

Py:   str(uuid.uuid4())
来源：http://hz.dianchejie.cn/gtdteatlvm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.c1oappe.top/gtyamsvtdm.html

JS:   crypto.randomUUID()
来源：http://hz.hysaishi.cn/gttpmeexiz.html

TS:   crypto.randomUUID()
来源：http://hz.pengpengdd.cyou/gtkbeenlqb.html

Java: UUID.randomUUID().toString()
来源：http://hz.svipenyu.cn/gtyhtmwrdy.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xuetiantiany.cn/gteybqirvk.html

Ruby: SecureRandom.uuid
来源：http://hz.xylfe.cn/gtwkkosxwh.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.vqdsnc.cn/gthogasrzj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hywenlv.cn/gtjnwqznhp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gogol.net.cn/gtiqphuemk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.nanxinkj.top/gtoelcynze.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.0kj1m.cn/gtjnocqoan.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.dashuyun.cn/gttnattejv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shzxlz.cn/gttnwlyjng.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gaohongyu789.top/gtfqanyjsi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yj202588.top/gtnwcrbmdx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.quarkkingdee.top/gtuweagbma.html

[P03] 生成短随机字符串
来源：http://hz.mhx1999.top/gtrgnkzyjt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yongpay.top/gtwhcgtbvn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jiagoushi.top/gtfjzopbbm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dashuyun.cn/gtpxbwwwlr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cqqwz.cn/gtjdghqrfz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinqigufen.top/gtksqtxtcs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.snrcjt.cn/gtsarzqyom.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhijiandao.cn/gtpmrnfbfw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gogol.net.cn/gtfumogtmo.html

[P04] 求长度
来源：http://hz.hnqzz.top/gtfmhlpbkz.html


<!-- 参考信息 -->