代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhixingplan.top/gtihwtisff.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.52xcode.cn/gtnirfwtug.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yuxming.cn/gtzznvytlg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cucudq.cn/gtdxnhkrda.html

[L07] 处理 HTTP 状态码
来源：http://hz.xuanzx.com/gtpeuhekjj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.daria6918.cn/gtiromssap.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xziqi.cn/gthenmkdfm.html

JS:   resp.ok;  resp.status
来源：http://hz.zhaomingkeji.xyz/gtkezdlswd.html

TS:   resp.ok;  resp.status
来源：http://hz.snrcjt.cn/gtgyhvtnbj.html

Java: resp.statusCode()
来源：http://hz.hnxiangtu.top/gtpbumbvxa.html

Go:   resp.StatusCode
来源：http://hz.fzhhl.top/gtfxlkzfkb.html

Ruby: resp.code.to_i
来源：http://hz.cqqwz.cn/gtfqabsfkf.html

C#:   (int)resp.StatusCode
来源：http://hz.kuanghao11.cn/gtzeskbbzc.html

[L08] 并发请求多个地址
来源：http://hz.hnxiangtu.top/gtjwqawqji.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.wangshuangyany.cn/gtipvunzvc.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangdashe.top/gttoxgicnu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sweek.top/gtemopcrhj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuanzx.com/gtqqfzyeqd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xuetiantiany.cn/gtzlenmkqp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.52xcode.cn/gtcaczysqk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.quarkkingdee.top/gteeyhmubd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shzxlz.cn/gtdfnefxww.html

================================================================================
来源：http://hz.aizwys.cn/gtastbjaus.html

M. 命令行 / 进程 / 环境
来源：http://hz.gzhubu.top/gttubvifwg.html

================================================================================
来源：http://hz.jlsjyb.cn/gtmypfeqbl.html

[M01] 读取命令行参数
来源：http://hz.nanxinkj.top/gtlwfdgvid.html

Py:   sys.argv[1:]
来源：http://hz.bjfxy.top/gtspkubpet.html

PHP:  $argv;  $argc;
来源：http://hz.jinghuilouyu.cn/gtvywwalbq.html

JS:   process.argv.slice(2)
来源：http://hz.wangdashe.top/gtocvhzkbk.html

TS:   process.argv.slice(2)
来源：http://hz.zdqjudy.top/gtrznucthr.html

Java: args 数组（main 方法参数）
来源：http://hz.cheryme.top/gtomfslcih.html

Go:   os.Args[1:]
来源：http://hz.aizwys.cn/gtyrfqtsgz.html

Ruby: ARGV
来源：http://hz.zdqjudy.top/gtkcjvoznh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.iojbl.cn/gtrembwzpt.html

[M02] 读取环境变量
来源：http://hz.mhx1999.top/gtzpsdijgn.html

Py:   os.environ.get("HOME")
来源：http://hz.ybcxt.top/gtwyduwadh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hammf.cn/gtlefdykbt.html

JS:   process.env.HOME
来源：http://hz.cqqwz.cn/gtgxdfiqwg.html

TS:   process.env.HOME
来源：http://hz.xuetiantiany.cn/gtcdmqjqaz.html

Java: System.getenv("HOME")
来源：http://hz.c1oappe.top/gtlzxwkjfi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.wangshuangyany.cn/gtrewpvtkn.html

Ruby: ENV["HOME"]
来源：http://hz.snrcjt.cn/gtntletesa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xuetiantiany.cn/gttvrxdwzb.html

[M03] 执行外部命令
来源：http://hz.bjfxy.top/gtgzlpsbre.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.daria6918.cn/gtvcwsolxi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.nanxinkj.top/gtnwjvlyqm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ivvv.top/gtsawvhzce.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ybcxt.top/gtvaekhyxi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yanxiufei.cn/gtyyoobhyb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ywan-chungtsiang.top/gtvobybqys.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.redwolf501.top/gtvjiqvors.html

C#:   Process.Start("ls", "-l");
来源：http://hz.chenjidiqi.icu/gtrtsegbjg.html

[M04] 获取当前工作目录
来源：http://hz.zhixingplan.top/gtxwsgtdms.html

Py:   os.getcwd()
来源：http://hz.yj202588.top/gtzowifdth.html

PHP:  getcwd();
来源：http://hz.ivvv.top/gtgeruwboc.html

JS:   process.cwd()
来源：http://hz.pengpengdd.cyou/gtpeyveakh.html

TS:   process.cwd()
来源：http://hz.nanxinkj.top/gtzqagsnfc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ehwqpu.com/gtosrdaplo.html

Go:   os.Getwd()
来源：http://hz.yj20258888.top/gtzbmymlcc.html

Ruby: Dir.pwd
来源：http://hz.wangdashe.top/gtjovbwutx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shanyushiyangtech.top/gtcufrsrzm.html

[M05] 设置退出码
来源：http://hz.jlsjyb.cn/gterkbfdvw.html

Py:   sys.exit(1)
来源：http://hz.gotoacloud.top/gtdmpmjfpb.html

PHP:  exit(1);
来源：http://hz.xinyue.icu/gtagsdbidm.html

JS:   process.exit(1)
来源：http://hz.fzhhl.top/gtgwyinghn.html

TS:   process.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtfeagidcf.html

Java: System.exit(1)
来源：http://hz.xuetiantiany.cn/gtprmyvcfo.html

Go:   os.Exit(1)
来源：http://hz.chenzaomai.com/gtygwyaytp.html

Ruby: exit 1
来源：http://hz.zhixingplan.top/gtweksrrxa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhiwuduotai.top/gtoudmrezh.html

[M06] 向标准错误输出
来源：http://hz.yonumen.top/gtqxscbjnp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hnqzz.top/gtoevlqkfm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinqigufen.top/gtwtsohlfy.html

JS:   console.error("err")
来源：http://hz.9152youxi.cn/gtnpxfhftu.html

TS:   console.error("err")
来源：http://hz.xuetiantiany.cn/gtghluuhzk.html

Java: System.err.println("err")
来源：http://hz.chenjidiqi.icu/gthvevucmj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.havefunace.top/gtitvlmvdx.html

Ruby: warn "err"
来源：http://hz.nwbrower.top/gtzqfqkrrm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yonumen.top/gthvjmtyqm.html

[M07] 判断是否为主入口
来源：http://hz.birdmap.top/gtfwkljyps.html

Py:   if __name__ == "__main__":
来源：http://hz.yonumen.top/gtzxqlbgid.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shanyushiyangtech.top/gtngjhljgf.html

JS:   require.main === module
来源：http://hz.yonumen.top/gtkrbpnlov.html

TS:   require.main === module
来源：http://hz.chenlongwang.top/gtkfjdyfyq.html

Java: public static void main(String[] args)
来源：http://hz.sxryk.cn/gtkwtptafe.html

Go:   func main()
来源：http://hz.meibo888.top/gtrpiwjjaq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xingfuxueyuan.xyz/gtuuekeuhw.html

C#:   static void Main(string[] args)
来源：http://hz.cdnleiting.top/gtselpawna.html

[M08] 获取系统与运行时信息
来源：http://hz.daxiang520.top/gtgtonschm.html

Py:   platform.system();  platform.python_version()
来源：http://hz.nwbrower.top/gtglrarkkk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yonumen.top/gtfkgalasc.html

JS:   process.platform;  process.version
来源：http://hz.chenzaomai.com/gtpdqilmrr.html

TS:   process.platform;  process.version
来源：http://hz.hfpthk.cn/gtzijhikup.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhengqikj.top/gtyqdumony.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhaomingkeji.xyz/gtuhzhutgb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhoulong.xyz/gthfejmrua.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yonumen.top/gtfkvzsvpc.html

================================================================================
来源：http://hz.wangdashe.top/gtfnlxgwam.html

N. 数据结构与算法
来源：http://hz.shangyingyoupin.top/gthaahskil.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gthjtipquu.html

[N01] 二分查找（有序数组）
来源：http://hz.kuanghao11.cn/gtutkvardc.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yonumen.top/gtxraopoge.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cdnleiting.top/gtnfdkhsbw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxinkj.top/gtpmcjlfsd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ywan-chungtsiang.top/gtwkpajscz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenlongwang.top/gtajknyhwl.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhijiandao.cn/gtydphtixx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.meibo888.top/gtvhyjsmdy.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zycfv.cn/gtaznneuqz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.nwbrower.top/gtufpbiwec.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangkeji.top/gtxslhvbqi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cdnleiting.top/gtmlskvuxp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aibaodan.cn/gtbpfielvv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.wangshuangyany.cn/gtqkpmgiwn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ydjk.org.cn/gtmozdbdre.html

Go:   slices.Sort(arr)
来源：http://hz.pengpengdd.cyou/gtbnddtmtq.html

Ruby: arr.sort
来源：http://hz.yuanzhike.top/gtzdfhpbnb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yongpay.top/gtlrzjowia.html

[N03] 快速排序（分治示例）
来源：http://hz.snrcjt.cn/gthiwratxq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ehwqpu.com/gtkbpheltc.html

PHP:  // 递归实现，或用 usort
来源：http://hz.chenjidiqi.icu/gtvvugtbmu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhongyouzk.top/gtlkhpylyk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangdashe.top/gtdahbimml.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xuetiantiany.cn/gtggydyvry.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hnxiangtu.top/gtjmfuksmf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shangyingyoupin.top/gtmmpxaytg.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.dashuyun.cn/gtdsgumxsl.html

[N04] 斐波那契数列
来源：http://hz.cqqwz.cn/gtkjwrmygs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangtech.top/gtzttzkhkz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.nanxinkj.top/gtzapdegmr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258.top/gtzbjlzflt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zdqjudy.top/gtqiuvfpwc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cqqwz.cn/gtuqgviujr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cheryme.top/gtoqazjuqg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.meibo888.top/gtnuccatli.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.nanxinkj.top/gtbcoimyxr.html

[N05] 最大公约数
来源：http://hz.jlsjyb.cn/gtvjwflwbt.html

Py:   math.gcd(a, b)
来源：http://hz.zhongyouzk.top/gtcvfgznxj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yuxming.cn/gttyamysfn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj202588.top/gtgndxnefm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydzc1.top/gthhtkkclk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sufxvd.cn/gtgfrxwchz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.pycfn.com/gtbouqthyx.html

Ruby: a.gcd(b)
来源：http://hz.wangdashe.top/gtxsiumwnk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.nanxuanxn.top/gttgutehqi.html

[N06] 判断回文字符串
来源：http://hz.smart0.xyz/gtdapdxsqi.html

Py:   s == s[::-1]
来源：http://hz.pycfn.com/gtjbesgiiq.html

PHP:  $s === strrev($s);
来源：http://hz.svipenyu.cn/gtwfmmuznl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtheanbsse.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yj202588.top/gtrppbokea.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hfpthk.cn/gtbnuuynnk.html

Go:   // 双指针从两端比较
来源：http://hz.tianlin.xyz/gtodkujzli.html

Ruby: s == s.reverse
来源：http://hz.nanxinkj.top/gtsfstbafn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ywan-chungtsiang.top/gtjfqekmeq.html

[N07] 两数之和（返回下标）
来源：http://hz.redwolf501.top/gtlrnsqwwf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.haohaochexian.top/gtmiawwaqm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shangyingyoupin.top/gtqjbpcdlj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shanyushiyangtech.top/gtrezcqhxf.html

TS:   // 手写 Map<string, number>
来源：http://hz.meibo888.top/gtshvmokqo.html

Java: // 手写 HashMap
来源：http://hz.kuanghao11.cn/gtlirwqzwr.html

Go:   // 手写 map[int]int
来源：http://hz.jiagoushi.top/gtcjvqybwt.html

Ruby: // 手写 Hash
来源：http://hz.jyoumei.cn/gtacxlxpej.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.tianlin.xyz/gturtsgzad.html

[N08] 生成全排列
来源：http://hz.mhx1999.top/gtloogjwux.html

Py:   itertools.permutations(arr)
来源：http://hz.zhijiandao.cn/gtxzyswnxk.html

PHP:  // 手写递归交换
来源：http://hz.iojbl.cn/gtxiadtjsy.html

JS:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtuzayumib.html

TS:   // 手写回溯递归
来源：http://hz.ydzc1.top/gtlwdhphso.html

Java: // 手写回溯递归
来源：http://hz.sweek.top/gtsbdtwabo.html

Go:   // 手写回溯递归
来源：http://hz.yuxming.cn/gthhvfxcsp.html

Ruby: arr.permutation.to_a
来源：http://hz.wangdashe.top/gtjsqteibq.html

C#:   // 手写回溯递归
来源：http://hz.aizwys.cn/gtbvlzgscr.html

[N09] 栈与队列
来源：http://hz.jinyuanbaomall.cn/gtoiijheit.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.aibaodan.cn/gtbbxlhycs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.mhx1999.top/gthaoykhkj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.haohaochexian.top/gtsqjujuyx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinqigfzy.top/gtwgwpfhmd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hnqzz.top/gtmlrpuhii.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.aibaodan.cn/gtswypaytf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hysaishi.cn/gtfmbrfged.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhiwuduotai.top/gttfmebchx.html

[N10] 链表节点定义
来源：http://hz.gzhubu.top/gtuhexaaut.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.sysykeji.top/gtevhwlluc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xziqi.cn/gtyenynccr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ehwqpu.com/gtdygvnfak.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhijiandao.cn/gtevspncrq.html

Java: class Node { int v; Node next; }
来源：http://hz.cucudq.cn/gttletaamt.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.fzhhl.top/gtupnbmuzg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.dashuyun.cn/gtexuwimaw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xuetiantiany.cn/gtvpwhgllv.html

[N11] 二叉树中序遍历
来源：http://hz.tian-w.cn/gtbplqcyyr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.wangshuangyany.cn/gtigmmswdp.html

PHP:  // 手写递归函数
来源：http://hz.gzhubu.top/gtjacyyumw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.vqdsnc.cn/gtavjeixni.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuanzhike.top/gtjqxnidsy.html

Java: // 手写递归
来源：http://hz.snrcjt.cn/gtryxoolve.html

Go:   // 手写递归
来源：http://hz.sufxvd.cn/gtqcujnaem.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhixingplan.top/gtaxofafdq.html

C#:   // 手写递归
来源：http://hz.xinyue.icu/gtmrcwytdx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.wangshuangyany.cn/gtmqxssxkh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xingfuxueyuan.xyz/gthdcwmpnl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.vqdsnc.cn/gtcadkjsow.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yonumen.top/gtytfuxxev.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.redwolf501.top/gtcaihordr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenjidiqi.icu/gtrmskaoxe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.daxiang520.top/gtflxogewt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jyoumei.cn/gtyvxsgamb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenzaomai.com/gtilidyrfu.html

================================================================================
来源：http://hz.jqgufenzy.top/gttlsuyjvz.html

O. 并发与异步
来源：http://hz.tianlin.xyz/gtqzxqhuzf.html

================================================================================
来源：http://hz.sysykeji.top/gtqjczwyrt.html

[O01] 启动一个线程
来源：http://hz.shuidangran.top/gtxuuffizu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jianghu66.top/gtzpoxrhzw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cqqwz.cn/gtaonfkfxw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenlongwang.top/gtvutnkrcc.html

TS:   // 同 JS
来源：http://hz.zdqjudy.top/gtulopzzwo.html

Java: new Thread(() -> f()).start()
来源：http://hz.chenjidiqi.icu/gteexloigf.html

Go:   go f()
来源：http://hz.quarkkingdee.top/gtdloycdzx.html

Ruby: Thread.new { f }
来源：http://hz.316326.xyz/gtwjcndpiz.html

C#:   Task.Run(() => F());
来源：http://hz.chenzaomai.com/gtifuqhccl.html

[O02] 使用线程池
来源：http://hz.yangfankeji.com/gterwdbrja.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.tian-w.cn/gtvfznywdo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jlsjyb.cn/gtyboyfuyp.html

JS:   // worker_threads 线程池
来源：http://hz.chenzaomai.com/gtlaxrpoqw.html

TS:   // worker_threads 线程池
来源：http://hz.zhijiandao.cn/gtaqftjdfy.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.snrcjt.cn/gthqrxpfdp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.svipenyu.cn/gtojzoiwfo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gotoacloud.top/gtodcdbmwi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zycfv.cn/gtfjvjoedr.html

[O03] 加锁保护共享数据
来源：http://hz.zhoulong.xyz/gtyzxrvagr.html

Py:   with lock: shared += 1
来源：http://hz.9152youxi.cn/gtvebnhdrh.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ppjwa.cn/gtcrptbtrn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.iojbl.cn/gthmnjjbab.html

TS:   // 同 JS
来源：http://hz.zhiwuduotai.top/gtspmeylgm.html

Java: synchronized (this) { shared++; }
来源：http://hz.yonumen.top/gtonqfhzmx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.aibaodan.cn/gtsnxnlxsp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hfpthk.cn/gtfbferphq.html

C#:   lock (gate) { shared++; }
来源：http://hz.jianghu66.top/gtpdhtayem.html

[O04] 定义异步函数并等待
来源：http://hz.yuanzhike.top/gtrzqyubng.html

Py:   async def f():⏎    await g()
来源：http://hz.yvedp.cn/gtxbqmfzfq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinyuanbaomall.cn/gthqeufoir.html

JS:   async function f() { await g(); }
来源：http://hz.fengsongda.top/gtbuyatpfe.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ybcxt.top/gtzaoehslw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yangfankeji.com/gtuooglijz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shzxlz.cn/gtpnqrgfjc.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.birdmap.top/gtwraqaeui.html

C#:   async Task F() { await G(); }
来源：http://hz.tianlin.xyz/gtttcqhcem.html

[O05] 并发执行并等待全部完成
来源：http://hz.ppjwa.cn/gtxcukxbzz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yuanzhike.top/gtkrgaxtqc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yuxming.cn/gtxqvynyrs.html

JS:   await Promise.all(tasks)
来源：http://hz.jqgufenzy.top/gtunhdqmck.html

TS:   await Promise.all(tasks)
来源：http://hz.snrcjt.cn/gtvlghbntu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.gzhubu.top/gtnzpprhnt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hammf.cn/gtjjrwmezg.html

Ruby: threads.map(&:join)
来源：http://hz.yuanzhike.top/gttnydvopf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jlsjyb.cn/gtvsdscwgv.html

[O06] 使用进程池
来源：http://hz.yuanzhike.top/gtmnzemqmu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jyoumei.cn/gtydkylipd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.kuanghao11.cn/gtsrvkggde.html

JS:   // child_process / cluster 模块
来源：http://hz.ywan-chungtsiang.top/gtstyrhtpx.html

TS:   // child_process / cluster 模块
来源：http://hz.hfpthk.cn/gtbvonebtf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ydjk.org.cn/gtwlvacqof.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.guannengcc.top/gtvughmwlh.html

Ruby: // fork 块
来源：http://hz.fzhhl.top/gtmnkzalxj.html

C#:   Parallel.For
来源：http://hz.tian-w.cn/gtwnyxqgos.html

================================================================================
来源：http://hz.cheryme.top/gtbfmkknkf.html

P. 常用工具函数
来源：http://hz.zdqjudy.top/gtzfvjxhfv.html

================================================================================
来源：http://hz.tianlin.xyz/gthxiknner.html

[P01] 生成 UUID
来源：http://hz.yj20258.top/gtgxhwqeeh.html

Py:   str(uuid.uuid4())
来源：http://hz.yuanzhike.top/gtafaqunzj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.guannengcc.top/gtjfnzsiyo.html

JS:   crypto.randomUUID()
来源：http://hz.gogol.net.cn/gttavqwrhf.html

TS:   crypto.randomUUID()
来源：http://hz.pycfn.com/gthfflhnbk.html

Java: UUID.randomUUID().toString()
来源：http://hz.iojbl.cn/gteuuwlwxz.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yonumen.top/gtrwudkvqd.html

Ruby: SecureRandom.uuid
来源：http://hz.birdmap.top/gtwhrcmxmg.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jyoumei.cn/gttobgpjmh.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinqigfzy.top/gtvpvxevtj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yonumen.top/gtdphmlhvx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shanyushiyangkeji.top/gtfpgllmsq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jqgufenzy.top/gtqfejhwcq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj202588.top/gtdkazkzpj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cashguo.top/gtammeqlot.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yuanzhike.top/gtfpkhoilk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yuxming.cn/gtgaatyife.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.quarkkingdee.top/gtxxufluhx.html

[P03] 生成短随机字符串
来源：http://hz.kuanghao11.cn/gtgkfcvugb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xuanzx.com/gtfurrdqty.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shanyushiyangtech.top/gtawxhszur.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gzhubu.top/gtjifomisa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sufxvd.cn/gtgzswotpx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.nwbrower.top/gtmywzkgct.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shanyushiyangtech.top/gtszkmhehz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.guowangkeji.top/gtgcxoequm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.dianchejie.cn/gtebeugyjh.html

[P04] 求长度
来源：http://hz.guowangkeji.top/gtawmvwpjj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yonumen.top/gtihscsevc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xylfe.cn/gttrtbonfa.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.mhx1999.top/gtlgrtmfyo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nwbrower.top/gtwlpzllcv.html


<!-- 参考信息 -->