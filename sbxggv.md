代发 wailian999

Py:   resp.json()
来源：http://hz.xziqi.cn/gtbvwykbde.html

PHP:  json_decode($body, true);
来源：http://hz.gaohongyu789.top/gttcunqydx.html

JS:   await resp.json()
来源：http://hz.jyoumei.cn/gtjowliwui.html

TS:   await resp.json()
来源：http://hz.zhengqikj.top/gtbntwfwzr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.wangshuangyany.cn/gtianublco.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cucudq.cn/gtozdnbsjn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yanxiufei.cn/gteblwtnay.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jqgufenzy.top/gtfqqwbuvz.html

[L07] 处理 HTTP 状态码
来源：http://hz.yuanzhike.top/gtfwmhjcpt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cucudq.cn/gtnuhoumnm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cqqwz.cn/gtglvglnhm.html

JS:   resp.ok;  resp.status
来源：http://hz.fzhhl.top/gtcwxmlptf.html

TS:   resp.ok;  resp.status
来源：http://hz.jyoumei.cn/gtskkocshp.html

Java: resp.statusCode()
来源：http://hz.ywan-chungtsiang.top/gtgkcuktvk.html

Go:   resp.StatusCode
来源：http://hz.ybcxt.top/gtdedkhpeg.html

Ruby: resp.code.to_i
来源：http://hz.meibo888.top/gtisgjocpx.html

C#:   (int)resp.StatusCode
来源：http://hz.cdnleiting.top/gtivlhhdnq.html

[L08] 并发请求多个地址
来源：http://hz.zhengqikj.top/gtldismlew.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.quarkkingdee.top/gtmqsrmaag.html

PHP:  curl_multi_init() 系列
来源：http://hz.yongpay.top/gtrdzxxqgp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.52xcode.cn/gtjokavtcr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.bjfxy.top/gtqrsndmyn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ppjwa.cn/gtvncyrtuj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yanxiufei.cn/gtirgtshfb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.dianchejie.cn/gtiedcysis.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shuidangran.top/gtvwmjbdfl.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtpbsduybk.html

M. 命令行 / 进程 / 环境
来源：http://hz.aibaodan.cn/gtbomqenhc.html

================================================================================
来源：http://hz.hammf.cn/gtidwgltzn.html

[M01] 读取命令行参数
来源：http://hz.smart0.xyz/gtcxdxmtlt.html

Py:   sys.argv[1:]
来源：http://hz.hammf.cn/gttmaveghy.html

PHP:  $argv;  $argc;
来源：http://hz.shanyushiyangkeji.top/gtzhdmkdyz.html

JS:   process.argv.slice(2)
来源：http://hz.cheryme.top/gtlnuqhvlg.html

TS:   process.argv.slice(2)
来源：http://hz.redwolf501.top/gtruibnuka.html

Java: args 数组（main 方法参数）
来源：http://hz.iojbl.cn/gtxfwsdnlu.html

Go:   os.Args[1:]
来源：http://hz.52xcode.cn/gtleterdox.html

Ruby: ARGV
来源：http://hz.jyoumei.cn/gtfzjmidgh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hammf.cn/gtayfwkzlb.html

[M02] 读取环境变量
来源：http://hz.dianchejie.cn/gtwvyyylmh.html

Py:   os.environ.get("HOME")
来源：http://hz.jqgufenzy.top/gtgranhhjb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yanxiufei.cn/gtnkzudrdu.html

JS:   process.env.HOME
来源：http://hz.nanxuanxn.top/gtdrfzjypn.html

TS:   process.env.HOME
来源：http://hz.shanyushiyangkeji.top/gtyksijgxi.html

Java: System.getenv("HOME")
来源：http://hz.feifeiyinyue.top/gtoervduiw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.9152youxi.cn/gthrixjfla.html

Ruby: ENV["HOME"]
来源：http://hz.ydzc1.top/gtlmsayoye.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yvedp.cn/gtpwqmozrx.html

[M03] 执行外部命令
来源：http://hz.smart0.xyz/gtsfpoalcg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.vqdsnc.cn/gtueozcdig.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinqigufen.top/gtlkzaabsl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sysykeji.top/gtoopftzhc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangkeji.top/gteoozpvta.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ehwqpu.com/gtukkameem.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhaomingkeji.xyz/gtxxxyrgke.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gotoacloud.top/gtwiwouvjb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shanyushiyangtech.top/gtyrhymjuj.html

[M04] 获取当前工作目录
来源：http://hz.yj202588.top/gtccldtqde.html

Py:   os.getcwd()
来源：http://hz.hammf.cn/gtkmzaqavx.html

PHP:  getcwd();
来源：http://hz.dianchejie.cn/gtjsckovvp.html

JS:   process.cwd()
来源：http://hz.birdmap.top/gtksuucdzp.html

TS:   process.cwd()
来源：http://hz.pycfn.com/gtmnxfskex.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gzhubu.top/gtecsivlzr.html

Go:   os.Getwd()
来源：http://hz.jinqigfzy.top/gtyjvaabsd.html

Ruby: Dir.pwd
来源：http://hz.shzxlz.cn/gterjdnpex.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhixingplan.top/gtjqzbrlzb.html

[M05] 设置退出码
来源：http://hz.snrcjt.cn/gttcfogfid.html

Py:   sys.exit(1)
来源：http://hz.ybcxt.top/gtibpaeaga.html

PHP:  exit(1);
来源：http://hz.cdnleiting.top/gtemiliwbr.html

JS:   process.exit(1)
来源：http://hz.ybcxt.top/gtvafnaaom.html

TS:   process.exit(1)
来源：http://hz.xziqi.cn/gtovpzopwe.html

Java: System.exit(1)
来源：http://hz.haohaochexian.top/gtiyuvvrqa.html

Go:   os.Exit(1)
来源：http://hz.ivvv.top/gtumyjxcre.html

Ruby: exit 1
来源：http://hz.wangdashe.top/gtafwiuxfa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shuidangran.top/gtdsxvzmbi.html

[M06] 向标准错误输出
来源：http://hz.yj202588.top/gtmxkwnuku.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cashguo.top/gtpkuxnucs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.0kj1m.cn/gtrdddgxzn.html

JS:   console.error("err")
来源：http://hz.nanxinkj.top/gtvufkgyeo.html

TS:   console.error("err")
来源：http://hz.yj20258.top/gtkvhfqkzf.html

Java: System.err.println("err")
来源：http://hz.gaohongyu789.top/gtwlclhihz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhiwuduotai.top/gtjggdifle.html

Ruby: warn "err"
来源：http://hz.daria6918.cn/gtznwjiqbm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.9152youxi.cn/gtxntzrkok.html

[M07] 判断是否为主入口
来源：http://hz.smart0.xyz/gtxqyamwdk.html

Py:   if __name__ == "__main__":
来源：http://hz.zdqjudy.top/gtsjlxxcuv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.fzhhl.top/gtglvivfbp.html

JS:   require.main === module
来源：http://hz.yvedp.cn/gtktlfkbrp.html

TS:   require.main === module
来源：http://hz.quarkkingdee.top/gtkqetbpex.html

Java: public static void main(String[] args)
来源：http://hz.zhixingplan.top/gtpxnsloct.html

Go:   func main()
来源：http://hz.jinqigufen.top/gtajpgizqr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.tian-w.cn/gthyqmjvkq.html

C#:   static void Main(string[] args)
来源：http://hz.havefunace.top/gtvhtogevz.html

[M08] 获取系统与运行时信息
来源：http://hz.hnxiangtu.top/gtqrcajhou.html

Py:   platform.system();  platform.python_version()
来源：http://hz.chenjidiqi.icu/gtzjzfzacq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhaomingkeji.xyz/gtalcnjpve.html

JS:   process.platform;  process.version
来源：http://hz.yonumen.top/gtxbrzsbvf.html

TS:   process.platform;  process.version
来源：http://hz.jinqigfzy.top/gtvptuonwb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jyoumei.cn/gtnwjcdcob.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.fzhhl.top/gtgfpqzmwm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yuxming.cn/gtcnkhpbpp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hfpthk.cn/gtfbboxdlq.html

================================================================================
来源：http://hz.hammf.cn/gtjxrazldc.html

N. 数据结构与算法
来源：http://hz.guowangkeji.top/gtzepqegro.html

================================================================================
来源：http://hz.hammf.cn/gtzcpsqgsq.html

[N01] 二分查找（有序数组）
来源：http://hz.zhongyouzk.top/gteofvsuas.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.kuanghao11.cn/gtujbtzqit.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.9152youxi.cn/gtvcyyamxn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sxryk.cn/gtajjfsadp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cheryme.top/gtbuggjenu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gtizoxoxlq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yonumen.top/gtvvwtjeta.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shanyushiyangtech.top/gtobfviiso.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.aibaodan.cn/gtmvvaawvc.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yonumen.top/gteiilbgic.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sufxvd.cn/gtcsqvymcp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jqgufenzy.top/gtenjaxwjr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinghuilouyu.cn/gthllibdgz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zycfv.cn/gtwaiapvei.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ydzc1.top/gtumojainy.html

Go:   slices.Sort(arr)
来源：http://hz.ybcxt.top/gtcjxtafkk.html

Ruby: arr.sort
来源：http://hz.shanyushiyangtech.top/gtbgjecshh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.pycfn.com/gtbalwcbdm.html

[N03] 快速排序（分治示例）
来源：http://hz.cheryme.top/gtiwqeclip.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinqigfzy.top/gtiycddkdu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhongyouzk.top/gtembedcfh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yongpay.top/gtrcpkcfmz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ywan-chungtsiang.top/gtnsxnrrbj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yongpay.top/gteebsetct.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yj202588.top/gtwaovasfe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hnxiangtu.top/gtiiijsguj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhaomingkeji.xyz/gtzkqjlrwe.html

[N04] 斐波那契数列
来源：http://hz.cashguo.top/gtguftvysm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.pycfn.com/gtgwsktdir.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ehwqpu.com/gtcxwptdgx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yueranfly.top/gtcuzkyqwt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gthdwsvfau.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.svipenyu.cn/gtpfrfnozc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.havefunace.top/gtwvutiuen.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.tianlin.xyz/gtxcdugwrz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenjidiqi.icu/gtvnklaczy.html

[N05] 最大公约数
来源：http://hz.hnqzz.top/gtofprsiyj.html

Py:   math.gcd(a, b)
来源：http://hz.jlsjyb.cn/gtgmnmkgsr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xingfuxueyuan.xyz/gtjrigfuix.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhixingplan.top/gtkwohabiw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nanxuanxn.top/gtetlwzmve.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.tian-w.cn/gtsmvkwzrn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinghuilouyu.cn/gtbsxmlxuh.html

Ruby: a.gcd(b)
来源：http://hz.yanxiufei.cn/gtzgzzlrgd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cqqwz.cn/gthqzkdjro.html

[N06] 判断回文字符串
来源：http://hz.yueranfly.top/gtsouafwsl.html

Py:   s == s[::-1]
来源：http://hz.jinqigfzy.top/gtskbnvsyz.html

PHP:  $s === strrev($s);
来源：http://hz.aibaodan.cn/gtqlrzukse.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ivvv.top/gtzehozbbi.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ydzc1.top/gtbzsgmzsc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ydjk.org.cn/gtyzdxvllp.html

Go:   // 双指针从两端比较
来源：http://hz.jyoumei.cn/gtnaiojirl.html

Ruby: s == s.reverse
来源：http://hz.sysykeji.top/gtzcnislov.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jyoumei.cn/gtwmbenshc.html

[N07] 两数之和（返回下标）
来源：http://hz.ppjwa.cn/gtrbdwjxde.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhixingplan.top/gtpadfzfav.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shanyushiyangtech.top/gtadhitkal.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.birdmap.top/gtvlvkngwn.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinqigufen.top/gtmvsfkeva.html

Java: // 手写 HashMap
来源：http://hz.ybcxt.top/gtyizdvoxl.html

Go:   // 手写 map[int]int
来源：http://hz.shanyushiyangkeji.top/gtvjledsxe.html

Ruby: // 手写 Hash
来源：http://hz.nanxinkj.top/gtnoyifbpu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ydzc1.top/gthazmychs.html

[N08] 生成全排列
来源：http://hz.cashguo.top/gtymiefrie.html

Py:   itertools.permutations(arr)
来源：http://hz.aizwys.cn/gtisoehnmg.html

PHP:  // 手写递归交换
来源：http://hz.ydjk.org.cn/gtqnrovnpg.html

JS:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gthxuaxmos.html

TS:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtcnzrjjic.html

Java: // 手写回溯递归
来源：http://hz.aibaodan.cn/gtqqhrbttc.html

Go:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtboxgpqiw.html

Ruby: arr.permutation.to_a
来源：http://hz.ybcxt.top/gtizmvdyxz.html

C#:   // 手写回溯递归
来源：http://hz.jiagoushi.top/gtwdlxtvur.html

[N09] 栈与队列
来源：http://hz.sxryk.cn/gtdzpzjktc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hongshengwenyu.top/gtctuboooy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.andypj.xyz/gtjvnfxrzb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.tanke756.top/gtrveyiapq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.meibo888.top/gtozwzlypl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.nanxinkj.top/gtvbkbptpx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zdqjudy.top/gtcoointeb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhijiandao.cn/gtvouyrpbr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ppjwa.cn/gtszeqozmm.html

[N10] 链表节点定义
来源：http://hz.jiagoushi.top/gtsunqmbbf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jyoumei.cn/gtfiipewsh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.andypj.xyz/gtbkxnhhnf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.bjfxy.top/gtrqkvirmk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.quarkkingdee.top/gtkgivjxlt.html

Java: class Node { int v; Node next; }
来源：http://hz.hongshengwenyu.top/gttypowtst.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.52xcode.cn/gtwkxremmm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hammf.cn/gtdipdqqtk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yj20258.top/gttglqusci.html

[N11] 二叉树中序遍历
来源：http://hz.kuanghao11.cn/gteeydktyl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hywenlv.cn/gtcstddksb.html

PHP:  // 手写递归函数
来源：http://hz.gzhubu.top/gtyjjpuzkg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.kuanghao11.cn/gttzmbstvs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenzaomai.com/gtyejppuit.html

Java: // 手写递归
来源：http://hz.shangyingyoupin.top/gtwwsttuxa.html

Go:   // 手写递归
来源：http://hz.tian-w.cn/gtbbugriqw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.gogol.net.cn/gtcvppaecx.html

C#:   // 手写递归
来源：http://hz.pengpengdd.cyou/gthctccjvl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.sxryk.cn/gtpehrecye.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.gotoacloud.top/gtvsafiglv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinghuilouyu.cn/gtkapuhela.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.pycfn.com/gtreaddzyu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.fengsongda.top/gtodtougds.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shangyingyoupin.top/gtkesduomu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.9152youxi.cn/gtgiisllay.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.gaohongyu789.top/gtphldzisz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nanxinkj.top/gtuscqsacq.html

================================================================================
来源：http://hz.hfpthk.cn/gtwqcgxuyx.html

O. 并发与异步
来源：http://hz.pycfn.com/gtmxruqwbp.html

================================================================================
来源：http://hz.nanxuanxn.top/gtwpzxbfht.html

[O01] 启动一个线程
来源：http://hz.xziqi.cn/gtvjlrkgdy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.daxiang520.top/gtjijwrlre.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hfpthk.cn/gtkyydbtun.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.wangdashe.top/gtxpgjkafp.html

TS:   // 同 JS
来源：http://hz.birdmap.top/gtmcqilkep.html

Java: new Thread(() -> f()).start()
来源：http://hz.jqgfzy.top/gteivyqkfx.html

Go:   go f()
来源：http://hz.andypj.xyz/gtomlsawtf.html

Ruby: Thread.new { f }
来源：http://hz.jinyuanbaomall.cn/gtiyotfcuu.html

C#:   Task.Run(() => F());
来源：http://hz.xuanzx.com/gtwbqbztdz.html

[O02] 使用线程池
来源：http://hz.ehwqpu.com/gtqenwizho.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yj20258888.top/gtkpqbrhqf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.aibaodan.cn/gthekskxjr.html

JS:   // worker_threads 线程池
来源：http://hz.andypj.xyz/gtksjhzfhz.html

TS:   // worker_threads 线程池
来源：http://hz.hongshengwenyu.top/gtwtlnzmjf.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.chenzaomai.com/gtapbujgzr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.sufxvd.cn/gtmhjhrzuv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ydzc1.top/gtndiiieew.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yueranfly.top/gtuwqbesut.html

[O03] 加锁保护共享数据
来源：http://hz.ydzc1.top/gthwzuulte.html

Py:   with lock: shared += 1
来源：http://hz.jinqigfzy.top/gtvgujswfz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.redwolf501.top/gtugydjtua.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenlongwang.top/gtgwotgzsp.html

TS:   // 同 JS
来源：http://hz.gzhubu.top/gtbxrpqwds.html

Java: synchronized (this) { shared++; }
来源：http://hz.shzxlz.cn/gtcvpnebbj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.mhx1999.top/gtnusrtsrv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.aizwys.cn/gtzzgumkxn.html

C#:   lock (gate) { shared++; }
来源：http://hz.xziqi.cn/gtpesdpfhi.html

[O04] 定义异步函数并等待
来源：http://hz.yangfankeji.com/gtjjavmfwx.html

Py:   async def f():⏎    await g()
来源：http://hz.cdnleiting.top/gthokherrs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gzhubu.top/gtxaiawvgt.html

JS:   async function f() { await g(); }
来源：http://hz.havefunace.top/gttlaobwck.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jqgfzy.top/gtouuvrvcb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yueranfly.top/gtxdxinrwf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jinqigfzy.top/gtyjubrzzt.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.9152youxi.cn/gtizqjmsfa.html

C#:   async Task F() { await G(); }
来源：http://hz.shanyushiyangkeji.top/gtxpmsroio.html

[O05] 并发执行并等待全部完成
来源：http://hz.smart0.xyz/gthgiequtm.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xingfuxueyuan.xyz/gtploobutz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.guannengcc.top/gtomssrdfh.html

JS:   await Promise.all(tasks)
来源：http://hz.ivvv.top/gtbbwwccnj.html

TS:   await Promise.all(tasks)
来源：http://hz.hongshengwenyu.top/gtazuapxpe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ybcxt.top/gtyuqwqgfb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cucudq.cn/gtkvwajlhl.html

Ruby: threads.map(&:join)
来源：http://hz.ydjk.org.cn/gtyobjfcly.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.aibaodan.cn/gttdyxakno.html

[O06] 使用进程池
来源：http://hz.xuetiantiany.cn/gtuhgpppjo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ydzc1.top/gtwwfkrhuw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shuidangran.top/gtimewbahj.html

JS:   // child_process / cluster 模块
来源：http://hz.yangfankeji.com/gtismnicqb.html

TS:   // child_process / cluster 模块
来源：http://hz.zhongyouzk.top/gtihuuscgg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yuanzhike.top/gtnsgtcsec.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.tianlin.xyz/gtondwwqdi.html

Ruby: // fork 块
来源：http://hz.jlsjyb.cn/gtquwpjfpd.html

C#:   Parallel.For
来源：http://hz.zhijiandao.cn/gtgryrdmvb.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtsushshas.html

P. 常用工具函数
来源：http://hz.yongpay.top/gtdyzcansz.html

================================================================================
来源：http://hz.jqgfzy.top/gtnninxhyk.html

[P01] 生成 UUID
来源：http://hz.chenjidiqi.icu/gtlrjrmzyi.html

Py:   str(uuid.uuid4())
来源：http://hz.jyoumei.cn/gtwbgxzdpg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gogol.net.cn/gtpwxihutz.html

JS:   crypto.randomUUID()
来源：http://hz.meibo888.top/gtdpvzourz.html

TS:   crypto.randomUUID()
来源：http://hz.shanyushiyangkeji.top/gtyvihfwnx.html

Java: UUID.randomUUID().toString()
来源：http://hz.jianghu66.top/gthflgaquq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.bjfxy.top/gtgpaiwkhb.html

Ruby: SecureRandom.uuid
来源：http://hz.zhengqikj.top/gtmunxxsvp.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.havefunace.top/gtnlnvzizk.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zdqjudy.top/gtdgjetcbd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.kuanghao11.cn/gtsperibdb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.nanxuanxn.top/gtdrcrhphz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xziqi.cn/gtzkwuhqzc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hfpthk.cn/gtvawywlas.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hfpthk.cn/gthmrdusuz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.nanxinkj.top/gtzbgovdox.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cucudq.cn/gtxdznprll.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.pycfn.com/gtkfuvamda.html

[P03] 生成短随机字符串
来源：http://hz.shanyushiyangtech.top/gtxupxtuzu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.9152youxi.cn/gtiivjucvy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yvedp.cn/gtslhogpiv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cashguo.top/gtdjsmhwbd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.snrcjt.cn/gtfucvvouk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cashguo.top/gtvcisawpy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jqgfzy.top/gtmgkutgal.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.iojbl.cn/gtnjvjchxw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.havefunace.top/gtwfpvpkqd.html

[P04] 求长度
来源：http://hz.aibaodan.cn/gtolztwski.html


<!-- 参考信息 -->