代发 wailian999

Py:   resp.json()
来源：http://hz.guannengcc.top/gtvxwdvfdz.html

PHP:  json_decode($body, true);
来源：http://hz.cdnleiting.top/gttdgjlzol.html

JS:   await resp.json()
来源：http://hz.yonumen.top/gtklwcbats.html

TS:   await resp.json()
来源：http://hz.redwolf501.top/gtuwxflnbr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.fengsongda.top/gtkubkedrl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yangfankeji.com/gtmobcnhwy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tanke756.top/gtgmykqakw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yueranfly.top/gtjqglnlvv.html

[L07] 处理 HTTP 状态码
来源：http://hz.fzhhl.top/gtpvlesgwg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhoulong.xyz/gtukeyojgp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.aizwys.cn/gtrmnnqnbc.html

JS:   resp.ok;  resp.status
来源：http://hz.birdmap.top/gtksxautoy.html

TS:   resp.ok;  resp.status
来源：http://hz.guowangkeji.top/gtspqfwiyy.html

Java: resp.statusCode()
来源：http://hz.yonumen.top/gtmtvveson.html

Go:   resp.StatusCode
来源：http://hz.shzxlz.cn/gtwyfowrnv.html

Ruby: resp.code.to_i
来源：http://hz.jlsjyb.cn/gtnopzchjg.html

C#:   (int)resp.StatusCode
来源：http://hz.zdqjudy.top/gtdjviphha.html

[L08] 并发请求多个地址
来源：http://hz.zhijiandao.cn/gtrespncyr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.aibaodan.cn/gtzpvfhold.html

PHP:  curl_multi_init() 系列
来源：http://hz.shuidangran.top/gtyqwaufgs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hnxiangtu.top/gtqrlumgot.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgufenzy.top/gtelvyszyh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ywan-chungtsiang.top/gtlkabxcdt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jqgufenzy.top/gtnimtkhbp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.bjfxy.top/gtqamiblwa.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yanxiufei.cn/gtxlhpoquy.html

================================================================================
来源：http://hz.52xcode.cn/gtcmwatjmd.html

M. 命令行 / 进程 / 环境
来源：http://hz.redwolf501.top/gtwquioelo.html

================================================================================
来源：http://hz.gotoacloud.top/gtfoffanez.html

[M01] 读取命令行参数
来源：http://hz.zhongyouzk.top/gtcplhzfqd.html

Py:   sys.argv[1:]
来源：http://hz.gzhubu.top/gtptbylcrm.html

PHP:  $argv;  $argc;
来源：http://hz.jinghuilouyu.cn/gtdcocpqcz.html

JS:   process.argv.slice(2)
来源：http://hz.shanyushiyangtech.top/gtwaqccwul.html

TS:   process.argv.slice(2)
来源：http://hz.cqqwz.cn/gttzhzgmhu.html

Java: args 数组（main 方法参数）
来源：http://hz.jyoumei.cn/gtucjkmfhr.html

Go:   os.Args[1:]
来源：http://hz.zhengqikj.top/gtqvwyxrnu.html

Ruby: ARGV
来源：http://hz.sxryk.cn/gtnsmwllqa.html

C#:   args 数组（Main 方法参数）
来源：http://hz.fengsongda.top/gtdyuqhomj.html

[M02] 读取环境变量
来源：http://hz.hfpthk.cn/gtowxorspv.html

Py:   os.environ.get("HOME")
来源：http://hz.ydjk.org.cn/gtzojichhy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yongpay.top/gtstcnjxsc.html

JS:   process.env.HOME
来源：http://hz.vqdsnc.cn/gtthpguyjj.html

TS:   process.env.HOME
来源：http://hz.snrcjt.cn/gtfapxxgax.html

Java: System.getenv("HOME")
来源：http://hz.316326.xyz/gtnzypdnkk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shuidangran.top/gtdalbxxoc.html

Ruby: ENV["HOME"]
来源：http://hz.shanyushiyangkeji.top/gtgpqholpt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shanyushiyangtech.top/gtmgmnawln.html

[M03] 执行外部命令
来源：http://hz.jianghu66.top/gtrzufdfur.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yanxiufei.cn/gtfjeebjya.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhiwuduotai.top/gtwcfzlqvl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yangfankeji.com/gticmyntgs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.dashuyun.cn/gttpothwpr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.52xcode.cn/gtalgfouzq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ywan-chungtsiang.top/gteqtsdlkc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhengqikj.top/gtqblkcpfv.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hfpthk.cn/gtnposkrsr.html

[M04] 获取当前工作目录
来源：http://hz.nanxinkj.top/gtnmflxdcb.html

Py:   os.getcwd()
来源：http://hz.ydzc1.top/gteeuxnuyy.html

PHP:  getcwd();
来源：http://hz.quarkkingdee.top/gtbmwwdulp.html

JS:   process.cwd()
来源：http://hz.svipenyu.cn/gtirkhpfwb.html

TS:   process.cwd()
来源：http://hz.chenlongwang.top/gtqjrxugqo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yangfankeji.com/gthqkdosjq.html

Go:   os.Getwd()
来源：http://hz.nwbrower.top/gtozavtlng.html

Ruby: Dir.pwd
来源：http://hz.jianghu66.top/gttsukqtar.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jlsjyb.cn/gtmzydchwe.html

[M05] 设置退出码
来源：http://hz.yuxming.cn/gtizgryspl.html

Py:   sys.exit(1)
来源：http://hz.jianghu66.top/gtkuiedmwr.html

PHP:  exit(1);
来源：http://hz.dashuyun.cn/gtvdxcaevs.html

JS:   process.exit(1)
来源：http://hz.ydzc1.top/gtjowwiefi.html

TS:   process.exit(1)
来源：http://hz.yvedp.cn/gtdnjajjgk.html

Java: System.exit(1)
来源：http://hz.jqgfzy.top/gtwyvelikp.html

Go:   os.Exit(1)
来源：http://hz.havefunace.top/gtahebghnv.html

Ruby: exit 1
来源：http://hz.ydzc1.top/gtnltivqqz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shanyushiyangtech.top/gtsnrxdcez.html

[M06] 向标准错误输出
来源：http://hz.yonumen.top/gtvjorqadr.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gotoacloud.top/gtvabwgiug.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shanyushiyangkeji.top/gtyawjglui.html

JS:   console.error("err")
来源：http://hz.ppjwa.cn/gtndkyhfnn.html

TS:   console.error("err")
来源：http://hz.tian-w.cn/gtzahhqzmb.html

Java: System.err.println("err")
来源：http://hz.yueranfly.top/gtualngcgu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yuanzhike.top/gtcdptueca.html

Ruby: warn "err"
来源：http://hz.zhaomingkeji.xyz/gtshxhvene.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ydzc1.top/gtngtiachh.html

[M07] 判断是否为主入口
来源：http://hz.sxryk.cn/gtsxgbsgbn.html

Py:   if __name__ == "__main__":
来源：http://hz.sufxvd.cn/gtmbpfluin.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shuidangran.top/gtqseuzpdq.html

JS:   require.main === module
来源：http://hz.hysaishi.cn/gtvnipekmb.html

TS:   require.main === module
来源：http://hz.feifeiyinyue.top/gtiybkofdt.html

Java: public static void main(String[] args)
来源：http://hz.daxiang520.top/gtvwfgksrq.html

Go:   func main()
来源：http://hz.xylfe.cn/gtsfejypqv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.vqdsnc.cn/gtlhgvnaxw.html

C#:   static void Main(string[] args)
来源：http://hz.cqqwz.cn/gtxivsqijc.html

[M08] 获取系统与运行时信息
来源：http://hz.zhixingplan.top/gtuhunwmox.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yj202588.top/gtoqxilacu.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.kuanghao11.cn/gtboyuppym.html

JS:   process.platform;  process.version
来源：http://hz.hnxiangtu.top/gtohuzzwub.html

TS:   process.platform;  process.version
来源：http://hz.zhiwuduotai.top/gtxiccxvgu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.nanxinkj.top/gtazpowmky.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.mhx1999.top/gtmqwgqqux.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xylfe.cn/gtsnirevvy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ivvv.top/gtmschbcaa.html

================================================================================
来源：http://hz.yangfankeji.com/gtqznwtcxg.html

N. 数据结构与算法
来源：http://hz.jianghu66.top/gtwchltckm.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtntzyztek.html

[N01] 二分查找（有序数组）
来源：http://hz.shzxlz.cn/gtgondmozg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ehwqpu.com/gthhhcqxpr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.chenjidiqi.icu/gtupdjnrho.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.vqdsnc.cn/gtkhaghoja.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sysykeji.top/gthgtxlaeb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ybcxt.top/gtcrkwydkd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.quarkkingdee.top/gthjmqewip.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.guannengcc.top/gtfgmtxpzo.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ydzc1.top/gtiotuynde.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.svipenyu.cn/gtwbhrmmiv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hnqzz.top/gtofkdhrky.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cucudq.cn/gtjobpdcnt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtbsenealk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hongshengwenyu.top/gtqgqlaowu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.smart0.xyz/gtvinibehf.html

Go:   slices.Sort(arr)
来源：http://hz.chenjidiqi.icu/gtjqjzhbkk.html

Ruby: arr.sort
来源：http://hz.zhengqikj.top/gtlocaptur.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hfpthk.cn/gtsltzhenj.html

[N03] 快速排序（分治示例）
来源：http://hz.pycfn.com/gtuydayvjk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yj20258.top/gtajdsnajf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinghuilouyu.cn/gtshmzsacp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hongshengwenyu.top/gtjkmxipxt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zdqjudy.top/gtbztiurbj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tian-w.cn/gtcebyxlgt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.birdmap.top/gtykvqsqpo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hysaishi.cn/gtwwkxptsq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shzxlz.cn/gtmzoveweq.html

[N04] 斐波那契数列
来源：http://hz.aibaodan.cn/gtvailxlyi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tian-w.cn/gtuhmpqnsl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.fengsongda.top/gtbysnrkog.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sxryk.cn/gttsypeags.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigfzy.top/gtmftoagnw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yvedp.cn/gtpfovzxcv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yj202588.top/gtjrqdovkl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.tianlin.xyz/gtvvvwqxgg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.guannengcc.top/gtuzzeovms.html

[N05] 最大公约数
来源：http://hz.cashguo.top/gtrcihnlrn.html

Py:   math.gcd(a, b)
来源：http://hz.mhx1999.top/gtvxttrxcx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.pengpengdd.cyou/gtlbbmskfe.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangdashe.top/gthmkytuxi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhaomingkeji.xyz/gttcylorrh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hnxiangtu.top/gtubvpegfk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.quarkkingdee.top/gtzoenwzcv.html

Ruby: a.gcd(b)
来源：http://hz.gogol.net.cn/gtyxtjjxrq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hfpthk.cn/gtsvdelmzv.html

[N06] 判断回文字符串
来源：http://hz.gogol.net.cn/gttkugxyqn.html

Py:   s == s[::-1]
来源：http://hz.pengpengdd.cyou/gtxekeqvjv.html

PHP:  $s === strrev($s);
来源：http://hz.gotoacloud.top/gtkzelcnmc.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jqgufenzy.top/gtpjxoefpm.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yj20258.top/gtyvlzmwiu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ehwqpu.com/gtyulzbunw.html

Go:   // 双指针从两端比较
来源：http://hz.iojbl.cn/gtarehjift.html

Ruby: s == s.reverse
来源：http://hz.jiagoushi.top/gtfohjhccs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.pycfn.com/gtnlprmgsf.html

[N07] 两数之和（返回下标）
来源：http://hz.daxiang520.top/gtelvaslsp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.sysykeji.top/gtvglqyivl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yongpay.top/gtqrysdcbq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.mhx1999.top/gtconmlusa.html

TS:   // 手写 Map<string, number>
来源：http://hz.jianghu66.top/gtcrfpxqcq.html

Java: // 手写 HashMap
来源：http://hz.mhx1999.top/gttjzddhwa.html

Go:   // 手写 map[int]int
来源：http://hz.yangfankeji.com/gtzqwnrasd.html

Ruby: // 手写 Hash
来源：http://hz.zhiwuduotai.top/gtskuoxxew.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yueranfly.top/gtrwkictdy.html

[N08] 生成全排列
来源：http://hz.sweek.top/gtohitnxxb.html

Py:   itertools.permutations(arr)
来源：http://hz.yangfankeji.com/gtkqiqfysa.html

PHP:  // 手写递归交换
来源：http://hz.zhaomingkeji.xyz/gtthzcttjf.html

JS:   // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtnbaxhmpb.html

TS:   // 手写回溯递归
来源：http://hz.bjfxy.top/gtdbxkpcmd.html

Java: // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtdoatdfkg.html

Go:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtrgvbpqsn.html

Ruby: arr.permutation.to_a
来源：http://hz.hnqzz.top/gtbgztlmoh.html

C#:   // 手写回溯递归
来源：http://hz.pycfn.com/gtfmjymneb.html

[N09] 栈与队列
来源：http://hz.gzhubu.top/gtqgektnhe.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.nanxinkj.top/gtbvcvfsov.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinqigfzy.top/gtwvwayrkf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.nwbrower.top/gtuxpeowct.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.sweek.top/gtmfribzbk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhaomingkeji.xyz/gtwkgutdrp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinqigufen.top/gtnbadylbl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.wangdashe.top/gtzcejqvuo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.wangdashe.top/gtoymurydd.html

[N10] 链表节点定义
来源：http://hz.jlsjyb.cn/gtzrdvrsmb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yanxiufei.cn/gtobdyltxz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xylfe.cn/gtqpvdtdcw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj202588.top/gtkhzehayg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shanyushiyangtech.top/gtupzpoblh.html

Java: class Node { int v; Node next; }
来源：http://hz.yvedp.cn/gtsstwncpw.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tian-w.cn/gteuvohkka.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cheryme.top/gtwtfzlxog.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.tianlin.xyz/gttdxxtrjw.html

[N11] 二叉树中序遍历
来源：http://hz.cheryme.top/gtvlyfihzz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.wangshuangyany.cn/gtcedmbstc.html

PHP:  // 手写递归函数
来源：http://hz.ppjwa.cn/gtwuthjrnu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nwbrower.top/gtmdbobbmk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yanxiufei.cn/gtusuqvjsm.html

Java: // 手写递归
来源：http://hz.snrcjt.cn/gtbiwglrfc.html

Go:   // 手写递归
来源：http://hz.jqgfzy.top/gthucnxute.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.kuanghao11.cn/gtmqyrrfcy.html

C#:   // 手写递归
来源：http://hz.svipenyu.cn/gtcupishoh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.tianlin.xyz/gteehmaequ.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.mhx1999.top/gtyfzjvfkf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sweek.top/gtmeuekkoa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhoulong.xyz/gtnkffkcxr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgfzy.top/gtovbgxijf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gaohongyu789.top/gtarpbwffy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jyoumei.cn/gtzibpgflg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ydjk.org.cn/gthjcrdwsk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gtkcaxdtbl.html

================================================================================
来源：http://hz.cqqwz.cn/gtuspbjpsq.html

O. 并发与异步
来源：http://hz.quarkkingdee.top/gtgfbbroeo.html

================================================================================
来源：http://hz.dianchejie.cn/gtzsethjpx.html

[O01] 启动一个线程
来源：http://hz.vqdsnc.cn/gtdtfaywet.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.mhx1999.top/gtjfzazijh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhijiandao.cn/gtrjtmwunw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xingfuxueyuan.xyz/gtqpyyklzv.html

TS:   // 同 JS
来源：http://hz.hywenlv.cn/gtgvnlpmbo.html

Java: new Thread(() -> f()).start()
来源：http://hz.jqgfzy.top/gtmqmjxcls.html

Go:   go f()
来源：http://hz.meibo888.top/gtlngvpckb.html

Ruby: Thread.new { f }
来源：http://hz.hammf.cn/gtogtigdcw.html

C#:   Task.Run(() => F());
来源：http://hz.zhengqikj.top/gtpocxowml.html

[O02] 使用线程池
来源：http://hz.zhaomingkeji.xyz/gtiqjpbrxt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.c1oappe.top/gtjbgugjaw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinghuilouyu.cn/gtlcuubfnz.html

JS:   // worker_threads 线程池
来源：http://hz.shanyushiyangkeji.top/gtiprvozkg.html

TS:   // worker_threads 线程池
来源：http://hz.aibaodan.cn/gtnkeuwojo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xingfuxueyuan.xyz/gtjkrmmhtn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hywenlv.cn/gttwcbjgzr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinqigfzy.top/gtpzsjgsmn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yongpay.top/gtsbrdjapp.html

[O03] 加锁保护共享数据
来源：http://hz.52xcode.cn/gthklmwsbc.html

Py:   with lock: shared += 1
来源：http://hz.yongpay.top/gtfvctkvsu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yueranfly.top/gtbcupgsfs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.redwolf501.top/gttyfjzmdd.html

TS:   // 同 JS
来源：http://hz.zhaomingkeji.xyz/gtjaknarir.html

Java: synchronized (this) { shared++; }
来源：http://hz.0kj1m.cn/gtiymwszvo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xingfuxueyuan.xyz/gthjzmavfv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.redwolf501.top/gtzczcgppo.html

C#:   lock (gate) { shared++; }
来源：http://hz.fzhhl.top/gtqfxiczku.html

[O04] 定义异步函数并等待
来源：http://hz.xinyue.icu/gtyzzgtenx.html

Py:   async def f():⏎    await g()
来源：http://hz.aizwys.cn/gttddypkcz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sweek.top/gtxodcgelr.html

JS:   async function f() { await g(); }
来源：http://hz.yangfankeji.com/gtpmetwotb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shanyushiyangtech.top/gtpytfhgbf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.pengpengdd.cyou/gtxvpersjc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhixingplan.top/gthcswxmgu.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.52xcode.cn/gttmnscsrf.html

C#:   async Task F() { await G(); }
来源：http://hz.ydjk.org.cn/gtzrxxeein.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj202588.top/gtafntfkas.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hammf.cn/gthigskrdh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jinqigufen.top/gtupysxnws.html

JS:   await Promise.all(tasks)
来源：http://hz.jinyuanbaomall.cn/gtuoyfkcrf.html

TS:   await Promise.all(tasks)
来源：http://hz.birdmap.top/gtcmzpkbwg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.wangshuangyany.cn/gtbymgzemm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yvedp.cn/gtezprursq.html

Ruby: threads.map(&:join)
来源：http://hz.haohaochexian.top/gtezxcmixf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hfpthk.cn/gtffilgfkp.html

[O06] 使用进程池
来源：http://hz.meibo888.top/gtwsznfmrd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shanyushiyangkeji.top/gtmltzrgnd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.sufxvd.cn/gtbqhvpcmc.html

JS:   // child_process / cluster 模块
来源：http://hz.shanyushiyangtech.top/gtbasttpzp.html

TS:   // child_process / cluster 模块
来源：http://hz.jlsjyb.cn/gtqezwowgm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.tian-w.cn/gtkngabgkh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jyoumei.cn/gthhtvctgk.html

Ruby: // fork 块
来源：http://hz.ydzc1.top/gtssbaykta.html

C#:   Parallel.For
来源：http://hz.ydzc1.top/gtbdenjosg.html

================================================================================
来源：http://hz.tian-w.cn/gtdinjkvtw.html

P. 常用工具函数
来源：http://hz.0kj1m.cn/gtwkqaexql.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtbffuihfe.html

[P01] 生成 UUID
来源：http://hz.cqqwz.cn/gtxapwrbtn.html

Py:   str(uuid.uuid4())
来源：http://hz.jqgfzy.top/gtdkmgflik.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ywan-chungtsiang.top/gtcahluzfl.html

JS:   crypto.randomUUID()
来源：http://hz.mhx1999.top/gtkbjvxzsr.html

TS:   crypto.randomUUID()
来源：http://hz.svipenyu.cn/gtsnrwybzl.html

Java: UUID.randomUUID().toString()
来源：http://hz.sweek.top/gtbfoxnesl.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hnxiangtu.top/gtffuivtxy.html

Ruby: SecureRandom.uuid
来源：http://hz.zhixingplan.top/gtyxzwsjox.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yj20258888.top/gtzhbfdrno.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhaomingkeji.xyz/gtteuzpvqr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xylfe.cn/gtkfqgzqjf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.dianchejie.cn/gtgeruulsl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gaohongyu789.top/gtyseevupo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.aizwys.cn/gtzcdpobdk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gogol.net.cn/gtliddyqlo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.guowangkeji.top/gtnypmoslk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenzaomai.com/gtzlwxrwhz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.wangshuangyany.cn/gtkdwzungj.html

[P03] 生成短随机字符串
来源：http://hz.yonumen.top/gtomjzmhcq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yuxming.cn/gtpigatotu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hnqzz.top/gtbjpcewed.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258.top/gtfbmrkykp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.wangdashe.top/gtagiwodsc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hysaishi.cn/gtwcagrmud.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.c1oappe.top/gtuuwfmopf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yuxming.cn/gtsbokyxpi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.dianchejie.cn/gtoqzhpzzu.html

[P04] 求长度
来源：http://hz.yuxming.cn/gtshxomxdi.html


<!-- 参考信息 -->