代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://hz.xylfe.cn/gtuyqyiwne.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jianghu66.top/gtnptuuczd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yueranfly.top/gtpaqadbqx.html

JS:   resp.ok;  resp.status
来源：http://hz.sufxvd.cn/gtnkwzvmpi.html

TS:   resp.ok;  resp.status
来源：http://hz.daxiang520.top/gtrmawkmqs.html

Java: resp.statusCode()
来源：http://hz.ydjk.org.cn/gturqhcbvs.html

Go:   resp.StatusCode
来源：http://hz.hongshengwenyu.top/gtmxznaaoy.html

Ruby: resp.code.to_i
来源：http://hz.yj202588.top/gterfieupb.html

C#:   (int)resp.StatusCode
来源：http://hz.316326.xyz/gtntzilrtf.html

[L08] 并发请求多个地址
来源：http://hz.ehwqpu.com/gtrvzxyipz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.dashuyun.cn/gtfvftuopd.html

PHP:  curl_multi_init() 系列
来源：http://hz.52xcode.cn/gtenjrlaxn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydjk.org.cn/gtlvopogca.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gtinkbczza.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cdnleiting.top/gtejrzukzk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.haohaochexian.top/gtptkogavt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.dianchejie.cn/gtuhhlehhw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yj20258888.top/gtxgxxbjmg.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtvqwdvaow.html

M. 命令行 / 进程 / 环境
来源：http://hz.tian-w.cn/gtgweiuxdi.html

================================================================================
来源：http://hz.bjfxy.top/gtmyjpfkzi.html

[M01] 读取命令行参数
来源：http://hz.nwbrower.top/gtjfxpchvo.html

Py:   sys.argv[1:]
来源：http://hz.zhoulong.xyz/gtdpcmfhxq.html

PHP:  $argv;  $argc;
来源：http://hz.yonumen.top/gtqxhlwvsr.html

JS:   process.argv.slice(2)
来源：http://hz.zhoulong.xyz/gtwjfkjgdt.html

TS:   process.argv.slice(2)
来源：http://hz.shangyingyoupin.top/gtyfpsjamw.html

Java: args 数组（main 方法参数）
来源：http://hz.mhx1999.top/gtaszlasqe.html

Go:   os.Args[1:]
来源：http://hz.c1oappe.top/gtvjatkqpt.html

Ruby: ARGV
来源：http://hz.sufxvd.cn/gtlmgcftfs.html

C#:   args 数组（Main 方法参数）
来源：http://hz.0kj1m.cn/gtpgtvnpqg.html

[M02] 读取环境变量
来源：http://hz.xinyue.icu/gtpmydpdzh.html

Py:   os.environ.get("HOME")
来源：http://hz.yj20258.top/gtazqcjekc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinghuilouyu.cn/gtrsydvoka.html

JS:   process.env.HOME
来源：http://hz.aibaodan.cn/gthpukydcs.html

TS:   process.env.HOME
来源：http://hz.zhixingplan.top/gteoekmfap.html

Java: System.getenv("HOME")
来源：http://hz.hywenlv.cn/gtdrrexroq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jianghu66.top/gteaxwecck.html

Ruby: ENV["HOME"]
来源：http://hz.shanyushiyangtech.top/gtvgxkvjbn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.aibaodan.cn/gtcruwkasg.html

[M03] 执行外部命令
来源：http://hz.aizwys.cn/gtskqjpwda.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jiagoushi.top/gtvpldhnco.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.tian-w.cn/gtyecenxcc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jyoumei.cn/gtigecxveq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xinyue.icu/gtnjetbyfy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ivvv.top/gtddkqklvw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.guannengcc.top/gtwdpytgfo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hfpthk.cn/gtjgahkipa.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gzhubu.top/gtkggecvup.html

[M04] 获取当前工作目录
来源：http://hz.ehwqpu.com/gtgrdyxqok.html

Py:   os.getcwd()
来源：http://hz.smart0.xyz/gttimvjotz.html

PHP:  getcwd();
来源：http://hz.xylfe.cn/gtmtluagjq.html

JS:   process.cwd()
来源：http://hz.jinyuanbaomall.cn/gtuvdpfqbu.html

TS:   process.cwd()
来源：http://hz.feifeiyinyue.top/gtxfwigaou.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.feifeiyinyue.top/gtgmkshklb.html

Go:   os.Getwd()
来源：http://hz.ehwqpu.com/gtsadzvocg.html

Ruby: Dir.pwd
来源：http://hz.chenzaomai.com/gtaofbkepo.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.316326.xyz/gtguixizru.html

[M05] 设置退出码
来源：http://hz.c1oappe.top/gtlrhkrdwo.html

Py:   sys.exit(1)
来源：http://hz.xylfe.cn/gtfjzuextk.html

PHP:  exit(1);
来源：http://hz.hnxiangtu.top/gtycvzzege.html

JS:   process.exit(1)
来源：http://hz.chenzaomai.com/gtmuhimtex.html

TS:   process.exit(1)
来源：http://hz.zhixingplan.top/gtpgvpohyf.html

Java: System.exit(1)
来源：http://hz.ydjk.org.cn/gtikogxanj.html

Go:   os.Exit(1)
来源：http://hz.ppjwa.cn/gtizvmeawd.html

Ruby: exit 1
来源：http://hz.shanyushiyangkeji.top/gtphxiahez.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hysaishi.cn/gtryolnnjr.html

[M06] 向标准错误输出
来源：http://hz.shanyushiyangkeji.top/gtvxcezqkt.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shanyushiyangtech.top/gtbswfiwyn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.snrcjt.cn/gtcjoltanp.html

JS:   console.error("err")
来源：http://hz.c1oappe.top/gtqdcwyooq.html

TS:   console.error("err")
来源：http://hz.jinqigfzy.top/gtefwtzeov.html

Java: System.err.println("err")
来源：http://hz.zhijiandao.cn/gtxmbcarik.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.daria6918.cn/gtnwbtbyps.html

Ruby: warn "err"
来源：http://hz.xinyue.icu/gtiqtdpzwg.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hammf.cn/gtisiwsrxb.html

[M07] 判断是否为主入口
来源：http://hz.hnxiangtu.top/gtpkzcbvkt.html

Py:   if __name__ == "__main__":
来源：http://hz.iojbl.cn/gtbjymgxfq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yangfankeji.com/gtrjckdgwu.html

JS:   require.main === module
来源：http://hz.hysaishi.cn/gtmaytifei.html

TS:   require.main === module
来源：http://hz.jyoumei.cn/gtxplawgjm.html

Java: public static void main(String[] args)
来源：http://hz.yj20258.top/gthkignavv.html

Go:   func main()
来源：http://hz.hammf.cn/gtrnctgpvt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xziqi.cn/gtygsjlvam.html

C#:   static void Main(string[] args)
来源：http://hz.pengpengdd.cyou/gttadmpkpy.html

[M08] 获取系统与运行时信息
来源：http://hz.yuxming.cn/gtysfgypmj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jianghu66.top/gtlnrpkoyo.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.andypj.xyz/gtvlelaskl.html

JS:   process.platform;  process.version
来源：http://hz.shanyushiyangtech.top/gtkdrhcwdi.html

TS:   process.platform;  process.version
来源：http://hz.sufxvd.cn/gtdupazeqs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.chenzaomai.com/gthbajeezs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jiagoushi.top/gtnhfkjjhy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xuetiantiany.cn/gtqcsdqqdi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ydjk.org.cn/gtutimymop.html

================================================================================
来源：http://hz.birdmap.top/gtsmylltkk.html

N. 数据结构与算法
来源：http://hz.tian-w.cn/gtdcarbzlx.html

================================================================================
来源：http://hz.fengsongda.top/gtzynsvmpj.html

[N01] 二分查找（有序数组）
来源：http://hz.shanyushiyangkeji.top/gtjmwpedof.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.cqqwz.cn/gtlpoexcbj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yueranfly.top/gtxgcxkyap.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jlsjyb.cn/gtiykehdhs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigufen.top/gtyvlblmjz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.guowangkeji.top/gtvdntqzon.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shzxlz.cn/gttqgciowc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.dianchejie.cn/gtjzrnlwot.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yonumen.top/gthinpjhmr.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zdqjudy.top/gtkzjbyfaw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.316326.xyz/gtwnupgdpn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.52xcode.cn/gtjclcjkze.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhaomingkeji.xyz/gtmjjbyumk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.mhx1999.top/gtkfzzsdjo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xziqi.cn/gtssxkrzzd.html

Go:   slices.Sort(arr)
来源：http://hz.zycfv.cn/gtaxgzqajt.html

Ruby: arr.sort
来源：http://hz.svipenyu.cn/gtgszproeo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yongpay.top/gtswunrcpi.html

[N03] 快速排序（分治示例）
来源：http://hz.ydjk.org.cn/gtrreexknd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hnqzz.top/gtzxdxqrfy.html

PHP:  // 递归实现，或用 usort
来源：http://hz.havefunace.top/gtraldtspy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.c1oappe.top/gtulziflol.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgfzy.top/gtnbmjngzt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhijiandao.cn/gtdeysdjgd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.haohaochexian.top/gtucrsoilh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shanyushiyangkeji.top/gtnzjjpdhi.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hongshengwenyu.top/gtpewjblml.html

[N04] 斐波那契数列
来源：http://hz.aibaodan.cn/gteazagfri.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ybcxt.top/gtwhbdxnwi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hywenlv.cn/gtxbxxgpjz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fzhhl.top/gtnnqbmwne.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuxming.cn/gtsrqrubeg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.havefunace.top/gtuabttpjf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinqigufen.top/gtwgbusotg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hywenlv.cn/gtziacizvg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hnxiangtu.top/gtkzmgvvne.html

[N05] 最大公约数
来源：http://hz.c1oappe.top/gtrlgykrcp.html

Py:   math.gcd(a, b)
来源：http://hz.shanyushiyangkeji.top/gtylptpnwm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yangfankeji.com/gtgcpxxfjq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zdqjudy.top/gtufcbrizp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daria6918.cn/gtmzcqjdsl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.tianlin.xyz/gtshvspedh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhoulong.xyz/gtvmbwdroc.html

Ruby: a.gcd(b)
来源：http://hz.dashuyun.cn/gtryluelbn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.birdmap.top/gtpyvniuex.html

[N06] 判断回文字符串
来源：http://hz.fzhhl.top/gtmsxvvbni.html

Py:   s == s[::-1]
来源：http://hz.havefunace.top/gtuvbkxitw.html

PHP:  $s === strrev($s);
来源：http://hz.gaohongyu789.top/gtcuwpmvfb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cashguo.top/gtidvzckan.html

TS:   s === [...s].reverse().join("")
来源：http://hz.quarkkingdee.top/gtvgahrsza.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.tanke756.top/gtyuqmrswk.html

Go:   // 双指针从两端比较
来源：http://hz.fengsongda.top/gtkwvtxwhr.html

Ruby: s == s.reverse
来源：http://hz.iojbl.cn/gteukqkfgt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hfpthk.cn/gtgkiskkfb.html

[N07] 两数之和（返回下标）
来源：http://hz.xuetiantiany.cn/gtyzkkkdlg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yuanzhike.top/gtwldpwzac.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhixingplan.top/gtudkvezoc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sysykeji.top/gtdtvnwqkr.html

TS:   // 手写 Map<string, number>
来源：http://hz.hammf.cn/gtrjhkvtid.html

Java: // 手写 HashMap
来源：http://hz.0kj1m.cn/gtzvrvhhne.html

Go:   // 手写 map[int]int
来源：http://hz.gotoacloud.top/gtulczgxfp.html

Ruby: // 手写 Hash
来源：http://hz.zhongyouzk.top/gtaqekvcwg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinyuanbaomall.cn/gtavivmknx.html

[N08] 生成全排列
来源：http://hz.zhoulong.xyz/gtcydtpbez.html

Py:   itertools.permutations(arr)
来源：http://hz.jinyuanbaomall.cn/gtypsfgmsz.html

PHP:  // 手写递归交换
来源：http://hz.ydzc1.top/gtzvwtkfyv.html

JS:   // 手写回溯递归
来源：http://hz.xziqi.cn/gtqdxesbtu.html

TS:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtpzuckgcb.html

Java: // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gttsffgpza.html

Go:   // 手写回溯递归
来源：http://hz.chenlongwang.top/gtrfslursn.html

Ruby: arr.permutation.to_a
来源：http://hz.snrcjt.cn/gtffxamiri.html

C#:   // 手写回溯递归
来源：http://hz.yongpay.top/gtpkitwbxo.html

[N09] 栈与队列
来源：http://hz.jinqigufen.top/gtinjtwamh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.cheryme.top/gtjavqeizq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.mhx1999.top/gtqafzfmav.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.wangdashe.top/gtpdyyfaus.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.gaohongyu789.top/gtpilvvhkz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ywan-chungtsiang.top/gtsnhokcce.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinqigfzy.top/gtqzygxvlu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yangfankeji.com/gtcoowrunj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.daxiang520.top/gtynooxuay.html

[N10] 链表节点定义
来源：http://hz.xziqi.cn/gtcligshrd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yonumen.top/gtvjqaaeup.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cucudq.cn/gtqhslzxfl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jianghu66.top/gtbiqortxw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hywenlv.cn/gtuadrlwqn.html

Java: class Node { int v; Node next; }
来源：http://hz.guannengcc.top/gtqmpjtciv.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zdqjudy.top/gtwoeeufyj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.316326.xyz/gtxghjzdpz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jianghu66.top/gtrnzjfdwf.html

[N11] 二叉树中序遍历
来源：http://hz.birdmap.top/gtgoyeptzd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.pengpengdd.cyou/gtjoykikpa.html

PHP:  // 手写递归函数
来源：http://hz.iojbl.cn/gtuwyshdzc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydjk.org.cn/gtvuhqlznd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hfpthk.cn/gtwknxbpte.html

Java: // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtynjwjgad.html

Go:   // 手写递归
来源：http://hz.ppjwa.cn/gtfzmolzng.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhijiandao.cn/gtjnqekjek.html

C#:   // 手写递归
来源：http://hz.hongshengwenyu.top/gtueneqhfo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hongshengwenyu.top/gtnbygednw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.sweek.top/gtupavxjon.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.dashuyun.cn/gtfvqgwmms.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nwbrower.top/gtcbwmzdur.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgufenzy.top/gtiyadryxw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guowangkeji.top/gtqsshevfs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sufxvd.cn/gtjzcnjahv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.fzhhl.top/gtotrpmldt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydjk.org.cn/gtudeurzme.html

================================================================================
来源：http://hz.redwolf501.top/gtnbdiqunq.html

O. 并发与异步
来源：http://hz.aizwys.cn/gtcxqdchuu.html

================================================================================
来源：http://hz.hfpthk.cn/gthnowgfaa.html

[O01] 启动一个线程
来源：http://hz.jinghuilouyu.cn/gtnpsfbdgs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yangfankeji.com/gtsfqphbpl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jianghu66.top/gtdkcmxxup.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xingfuxueyuan.xyz/gtrytpurjn.html

TS:   // 同 JS
来源：http://hz.gogol.net.cn/gtdhjmvvnj.html

Java: new Thread(() -> f()).start()
来源：http://hz.chenzaomai.com/gtvymnpegl.html

Go:   go f()
来源：http://hz.daria6918.cn/gtrdtuizdx.html

Ruby: Thread.new { f }
来源：http://hz.meibo888.top/gtzdaljakn.html

C#:   Task.Run(() => F());
来源：http://hz.guowangkeji.top/gtpwsazrsw.html

[O02] 使用线程池
来源：http://hz.chenlongwang.top/gtjnhzoslf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.pycfn.com/gtcydcxznb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xuanzx.com/gtnerobpod.html

JS:   // worker_threads 线程池
来源：http://hz.yuanzhike.top/gtalzevimu.html

TS:   // worker_threads 线程池
来源：http://hz.shuidangran.top/gtrwwwanvm.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.svipenyu.cn/gtmoruhocw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.meibo888.top/gtczditfys.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hywenlv.cn/gthiammpju.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.sufxvd.cn/gtctzxwftu.html

[O03] 加锁保护共享数据
来源：http://hz.jiagoushi.top/gtojiknfig.html

Py:   with lock: shared += 1
来源：http://hz.xingfuxueyuan.xyz/gtmggurwsx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ybcxt.top/gtqpwuzzhi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.nanxuanxn.top/gtfddilxjo.html

TS:   // 同 JS
来源：http://hz.yueranfly.top/gtpknlnfzw.html

Java: synchronized (this) { shared++; }
来源：http://hz.c1oappe.top/gtdvitaiar.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhongyouzk.top/gthkgknxrp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ppjwa.cn/gtlcpsjyet.html

C#:   lock (gate) { shared++; }
来源：http://hz.smart0.xyz/gtzbhxihrk.html

[O04] 定义异步函数并等待
来源：http://hz.yuxming.cn/gtrcowzerk.html

Py:   async def f():⏎    await g()
来源：http://hz.shzxlz.cn/gtjhvoakfj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.andypj.xyz/gttnxtrwyj.html

JS:   async function f() { await g(); }
来源：http://hz.birdmap.top/gtticgoruc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.gaohongyu789.top/gtddibbbvp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jiagoushi.top/gtznkeuemw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ydzc1.top/gtqujqzfet.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xingfuxueyuan.xyz/gtdfwemvnc.html

C#:   async Task F() { await G(); }
来源：http://hz.cashguo.top/gtbvisggvy.html

[O05] 并发执行并等待全部完成
来源：http://hz.0kj1m.cn/gtufeglcvx.html

Py:   asyncio.gather(*tasks)
来源：http://hz.feifeiyinyue.top/gtavjujkej.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.sysykeji.top/gtqmyggdrl.html

JS:   await Promise.all(tasks)
来源：http://hz.xuanzx.com/gtmjjehyom.html

TS:   await Promise.all(tasks)
来源：http://hz.jqgfzy.top/gtctbshchj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinqigufen.top/gtfwuuojtw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhiwuduotai.top/gtlluldmnz.html

Ruby: threads.map(&:join)
来源：http://hz.daxiang520.top/gtshespcng.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yueranfly.top/gtjgocgpet.html

[O06] 使用进程池
来源：http://hz.bjfxy.top/gtmalnqyrx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yueranfly.top/gtubgwqdjs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cdnleiting.top/gtzsvitjpr.html

JS:   // child_process / cluster 模块
来源：http://hz.hammf.cn/gtmznasktd.html

TS:   // child_process / cluster 模块
来源：http://hz.redwolf501.top/gtkxgonfbd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yonumen.top/gtwzrzbhjw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gaohongyu789.top/gtayxhiiif.html

Ruby: // fork 块
来源：http://hz.xinyue.icu/gtxopnotvy.html

C#:   Parallel.For
来源：http://hz.mhx1999.top/gtoltdkgxa.html

================================================================================
来源：http://hz.haohaochexian.top/gtszycwvfy.html

P. 常用工具函数
来源：http://hz.xinyue.icu/gtwbpgictb.html

================================================================================
来源：http://hz.mhx1999.top/gtjhrwkrrx.html

[P01] 生成 UUID
来源：http://hz.hywenlv.cn/gtavadpdfu.html

Py:   str(uuid.uuid4())
来源：http://hz.guowangkeji.top/gtiiiuircd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhaomingkeji.xyz/gtingvehzb.html

JS:   crypto.randomUUID()
来源：http://hz.ivvv.top/gtmazapawl.html

TS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtssohrwpo.html

Java: UUID.randomUUID().toString()
来源：http://hz.iojbl.cn/gtlokduyhc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.nanxinkj.top/gtbdqeefss.html

Ruby: SecureRandom.uuid
来源：http://hz.nanxuanxn.top/gtfzltthpf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.fzhhl.top/gtumtzjakr.html

[P02] MD5 / SHA256 摘要
来源：http://hz.316326.xyz/gtyecnycvk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hammf.cn/gtywbpdsui.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.fengsongda.top/gthkmfapfp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cucudq.cn/gtmfkxaoer.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cdnleiting.top/gtmlkohnxt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.wangdashe.top/gtadwoudyb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cqqwz.cn/gtzstvjzdy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cucudq.cn/gtsugkrehm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xuetiantiany.cn/gtgenprmbj.html

[P03] 生成短随机字符串
来源：http://hz.haohaochexian.top/gtuwsnulhi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.c1oappe.top/gtzxklpeot.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hfpthk.cn/gtsjuvlnfw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zdqjudy.top/gtdqhmobfm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuanzhike.top/gttxkrwlfp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yangfankeji.com/gtickjdnsu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yj20258888.top/gtwmskkmaz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jlsjyb.cn/gtlnbvzmbf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ydzc1.top/gtukmphzvx.html

[P04] 求长度
来源：http://hz.iojbl.cn/gtuvwlstas.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shanyushiyangtech.top/gtgvnazbea.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhiwuduotai.top/gtjzdlomkp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sysykeji.top/gtjvscziuz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gotoacloud.top/gteiofzfjr.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yuxming.cn/gtpqplkpnm.html

Go:   len(arr);  len(m)
来源：http://hz.cqqwz.cn/gtsuefnvfj.html

Ruby: x.length;  x.size
来源：http://hz.chenzaomai.com/gtrogodwok.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cucudq.cn/gtomiuckew.html


<!-- 参考信息 -->