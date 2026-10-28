代发 wailian999

Py:   resp.json()
来源：http://hz.yanxiufei.cn/gtrivscaep.html

PHP:  json_decode($body, true);
来源：http://hz.pengpengdd.cyou/gtasamoamx.html

JS:   await resp.json()
来源：http://hz.bjfxy.top/gtpgvfjhbl.html

TS:   await resp.json()
来源：http://hz.zhiwuduotai.top/gtbsxxbibq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.iojbl.cn/gthuekoxso.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xziqi.cn/gtmwrkbxxy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jiagoushi.top/gtqaqwgihc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.meibo888.top/gthpiozoko.html

[L07] 处理 HTTP 状态码
来源：http://hz.shanyushiyangkeji.top/gtjecfssho.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gogol.net.cn/gtcwmorwqu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.iojbl.cn/gtexfqfjbq.html

JS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gtpctmlsvh.html

TS:   resp.ok;  resp.status
来源：http://hz.yvedp.cn/gtxfcsqvks.html

Java: resp.statusCode()
来源：http://hz.hfpthk.cn/gtkrmwfxnp.html

Go:   resp.StatusCode
来源：http://hz.kuanghao11.cn/gtryyabdwt.html

Ruby: resp.code.to_i
来源：http://hz.dianchejie.cn/gtrshqcgzr.html

C#:   (int)resp.StatusCode
来源：http://hz.gogol.net.cn/gtmhsroror.html

[L08] 并发请求多个地址
来源：http://hz.daria6918.cn/gtifnndlkr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.daria6918.cn/gtsyrmvggl.html

PHP:  curl_multi_init() 系列
来源：http://hz.ydjk.org.cn/gtssqzzlzb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ppjwa.cn/gtwxuljxje.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydjk.org.cn/gtevioodru.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jyoumei.cn/gtahpookat.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.quarkkingdee.top/gtrxwoncrr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hammf.cn/gtgvgblybj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hammf.cn/gtwvzjdwym.html

================================================================================
来源：http://hz.tanke756.top/gtydblcxrr.html

M. 命令行 / 进程 / 环境
来源：http://hz.birdmap.top/gtrpgkcyfo.html

================================================================================
来源：http://hz.yj20258888.top/gtqvhrdpjd.html

[M01] 读取命令行参数
来源：http://hz.gogol.net.cn/gtcabktdso.html

Py:   sys.argv[1:]
来源：http://hz.yueranfly.top/gtldqyslio.html

PHP:  $argv;  $argc;
来源：http://hz.ppjwa.cn/gttkvatiyc.html

JS:   process.argv.slice(2)
来源：http://hz.jinghuilouyu.cn/gthfbfmzfk.html

TS:   process.argv.slice(2)
来源：http://hz.yongpay.top/gtdadacukn.html

Java: args 数组（main 方法参数）
来源：http://hz.andypj.xyz/gtxbkcrpdk.html

Go:   os.Args[1:]
来源：http://hz.shuidangran.top/gtbgxtucuf.html

Ruby: ARGV
来源：http://hz.iojbl.cn/gtpqeqzqdo.html

C#:   args 数组（Main 方法参数）
来源：http://hz.havefunace.top/gtxhzmnkvv.html

[M02] 读取环境变量
来源：http://hz.ybcxt.top/gtzghcpezu.html

Py:   os.environ.get("HOME")
来源：http://hz.sufxvd.cn/gtqokubhfj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hammf.cn/gtwwgoccqf.html

JS:   process.env.HOME
来源：http://hz.redwolf501.top/gttyxqdsgb.html

TS:   process.env.HOME
来源：http://hz.xuanzx.com/gtryvwgjyt.html

Java: System.getenv("HOME")
来源：http://hz.birdmap.top/gtcldfifcn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hnqzz.top/gtueqnnztr.html

Ruby: ENV["HOME"]
来源：http://hz.cucudq.cn/gtluzorhvl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhaomingkeji.xyz/gtjouugixx.html

[M03] 执行外部命令
来源：http://hz.xuanzx.com/gtufhdanaz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.svipenyu.cn/gtidfyyktm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yvedp.cn/gtsqlpeaqk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.iojbl.cn/gtvpnmfmru.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ivvv.top/gtqugopjim.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.daria6918.cn/gtvbfaypno.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.guannengcc.top/gtezkcgqtr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shuidangran.top/gtxzhktbtu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.mhx1999.top/gtfvofplxv.html

[M04] 获取当前工作目录
来源：http://hz.zhijiandao.cn/gtmtoyidlm.html

Py:   os.getcwd()
来源：http://hz.wangshuangyany.cn/gtexoembhw.html

PHP:  getcwd();
来源：http://hz.ehwqpu.com/gtellnrkus.html

JS:   process.cwd()
来源：http://hz.hysaishi.cn/gtfknqmvhu.html

TS:   process.cwd()
来源：http://hz.havefunace.top/gtgoybvmor.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhijiandao.cn/gtcgwzupfy.html

Go:   os.Getwd()
来源：http://hz.tianlin.xyz/gtvsahprbs.html

Ruby: Dir.pwd
来源：http://hz.feifeiyinyue.top/gtvortsjto.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ybcxt.top/gtrluegnik.html

[M05] 设置退出码
来源：http://hz.yongpay.top/gtdcfwfrma.html

Py:   sys.exit(1)
来源：http://hz.wangshuangyany.cn/gtxoydawoe.html

PHP:  exit(1);
来源：http://hz.yonumen.top/gtskavosua.html

JS:   process.exit(1)
来源：http://hz.nanxinkj.top/gtfjgyjoat.html

TS:   process.exit(1)
来源：http://hz.sxryk.cn/gtvgmuevly.html

Java: System.exit(1)
来源：http://hz.jyoumei.cn/gtpgloxpbi.html

Go:   os.Exit(1)
来源：http://hz.cheryme.top/gtiyzegoqg.html

Ruby: exit 1
来源：http://hz.yj202588.top/gtzkoemvwt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xylfe.cn/gteivinbmj.html

[M06] 向标准错误输出
来源：http://hz.bjfxy.top/gtjgyapjve.html

Py:   print("err", file=sys.stderr)
来源：http://hz.tian-w.cn/gttegufdkt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinghuilouyu.cn/gtrimmtufc.html

JS:   console.error("err")
来源：http://hz.ivvv.top/gtzelqekmp.html

TS:   console.error("err")
来源：http://hz.nanxuanxn.top/gttgrtysrx.html

Java: System.err.println("err")
来源：http://hz.zhaomingkeji.xyz/gthbtwjmkt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hongshengwenyu.top/gtccfjkubv.html

Ruby: warn "err"
来源：http://hz.shanyushiyangkeji.top/gtqotswfjz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.tian-w.cn/gtwcfsvghm.html

[M07] 判断是否为主入口
来源：http://hz.sweek.top/gtrcfdchjz.html

Py:   if __name__ == "__main__":
来源：http://hz.andypj.xyz/gtixujcmpr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.feifeiyinyue.top/gtggjsanke.html

JS:   require.main === module
来源：http://hz.cheryme.top/gtzwsvggpy.html

TS:   require.main === module
来源：http://hz.hnxiangtu.top/gtdyplkfmj.html

Java: public static void main(String[] args)
来源：http://hz.sweek.top/gtyowgcwiv.html

Go:   func main()
来源：http://hz.c1oappe.top/gtrjldizqu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhijiandao.cn/gtogqonrzo.html

C#:   static void Main(string[] args)
来源：http://hz.chenzaomai.com/gtulnkvdqv.html

[M08] 获取系统与运行时信息
来源：http://hz.hnqzz.top/gtfhfnovba.html

Py:   platform.system();  platform.python_version()
来源：http://hz.chenzaomai.com/gtvfnuzskf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.bjfxy.top/gtqfyrskoq.html

JS:   process.platform;  process.version
来源：http://hz.guannengcc.top/gtrunsymjn.html

TS:   process.platform;  process.version
来源：http://hz.meibo888.top/gtpfzusnjh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tianlin.xyz/gtrmiuqoyt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.vqdsnc.cn/gtpdexadvc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shuidangran.top/gtzxuvrukr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sxryk.cn/gtglkliymr.html

================================================================================
来源：http://hz.jianghu66.top/gtmwatpqud.html

N. 数据结构与算法
来源：http://hz.gaohongyu789.top/gtbfzdqjae.html

================================================================================
来源：http://hz.dashuyun.cn/gtzctstcze.html

[N01] 二分查找（有序数组）
来源：http://hz.jinqigfzy.top/gtlclzhtgt.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.52xcode.cn/gtthahzlrg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sufxvd.cn/gtzzokaali.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shuidangran.top/gtmdzqcnbg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhoulong.xyz/gtgjebduaq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ivvv.top/gtpwnsupcg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.9152youxi.cn/gtgdiveqri.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.tianlin.xyz/gtsldspkqv.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.bjfxy.top/gtwavkohil.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ydjk.org.cn/gthefdjzlm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.smart0.xyz/gtpdjhsuky.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.smart0.xyz/gtaglkmrjt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.pycfn.com/gtwqoqqbqn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jqgfzy.top/gtwxxynboe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cheryme.top/gtlltajsno.html

Go:   slices.Sort(arr)
来源：http://hz.ppjwa.cn/gtfwswysmc.html

Ruby: arr.sort
来源：http://hz.shanyushiyangkeji.top/gtdhaayeic.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cucudq.cn/gtjahotbdy.html

[N03] 快速排序（分治示例）
来源：http://hz.ydzc1.top/gtpophrmyz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhiwuduotai.top/gtevmhsdwm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cqqwz.cn/gtbrcvogyp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydzc1.top/gtvhjalzgt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shanyushiyangtech.top/gtojpghwwq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.quarkkingdee.top/gtoesiixnn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.aizwys.cn/gtxnhmecdf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenjidiqi.icu/gtfirjobwq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhaomingkeji.xyz/gtqiwnqlaq.html

[N04] 斐波那契数列
来源：http://hz.ydjk.org.cn/gtfecuzirp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ydzc1.top/gtkwbovrez.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.0kj1m.cn/gtikhxpohy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.0kj1m.cn/gtzjbkwvnc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jlsjyb.cn/gtkrukkyuf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.aizwys.cn/gtuipumyby.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.nanxinkj.top/gtiyyjhtgk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.redwolf501.top/gtckxrorrl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj202588.top/gtmvydkhqv.html

[N05] 最大公约数
来源：http://hz.vqdsnc.cn/gtainzezjr.html

Py:   math.gcd(a, b)
来源：http://hz.wangshuangyany.cn/gtquymorzg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ybcxt.top/gtkptchbvj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenzaomai.com/gtwnczkzfv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigfzy.top/gtlkrlaiou.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.wangshuangyany.cn/gtxfmhqhhg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.0kj1m.cn/gtamjzwldu.html

Ruby: a.gcd(b)
来源：http://hz.feifeiyinyue.top/gtxuzxmdxt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.redwolf501.top/gtrmfqdzyf.html

[N06] 判断回文字符串
来源：http://hz.wangshuangyany.cn/gtvmwptvhg.html

Py:   s == s[::-1]
来源：http://hz.jinghuilouyu.cn/gtkhavpeog.html

PHP:  $s === strrev($s);
来源：http://hz.kuanghao11.cn/gtboxwgwue.html

JS:   s === [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtwlgwomfg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yj202588.top/gtkjzthhbf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.mhx1999.top/gtotxqtzwr.html

Go:   // 双指针从两端比较
来源：http://hz.yonumen.top/gtvxfweurp.html

Ruby: s == s.reverse
来源：http://hz.feifeiyinyue.top/gtrnjvsqgt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.daxiang520.top/gtmbxlganf.html

[N07] 两数之和（返回下标）
来源：http://hz.guannengcc.top/gtolltgmxe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xinyue.icu/gtlpszhmsi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhongyouzk.top/gtaubuxzrc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sxryk.cn/gtxbclnmdy.html

TS:   // 手写 Map<string, number>
来源：http://hz.dianchejie.cn/gtzefuhfrw.html

Java: // 手写 HashMap
来源：http://hz.daxiang520.top/gtkvxzbgya.html

Go:   // 手写 map[int]int
来源：http://hz.gogol.net.cn/gtwejezjzv.html

Ruby: // 手写 Hash
来源：http://hz.quarkkingdee.top/gtbwmsfigr.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ywan-chungtsiang.top/gtmcwkgefg.html

[N08] 生成全排列
来源：http://hz.gotoacloud.top/gtgcuowban.html

Py:   itertools.permutations(arr)
来源：http://hz.birdmap.top/gtvsjgacar.html

PHP:  // 手写递归交换
来源：http://hz.0kj1m.cn/gtvghvuxhx.html

JS:   // 手写回溯递归
来源：http://hz.cdnleiting.top/gthshpkoxk.html

TS:   // 手写回溯递归
来源：http://hz.ppjwa.cn/gtnkokxrzo.html

Java: // 手写回溯递归
来源：http://hz.hywenlv.cn/gtciyrihiw.html

Go:   // 手写回溯递归
来源：http://hz.bjfxy.top/gtyzteriys.html

Ruby: arr.permutation.to_a
来源：http://hz.yj202588.top/gtdyejhlpe.html

C#:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtpesotqlw.html

[N09] 栈与队列
来源：http://hz.shanyushiyangtech.top/gtrntcwgoi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.kuanghao11.cn/gtgoavcrbg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhoulong.xyz/gtbmqyqnfj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cheryme.top/gtitnlxwov.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ywan-chungtsiang.top/gtbqmmvisd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shangyingyoupin.top/gtrxsctppq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sysykeji.top/gtzzttjpqt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jqgfzy.top/gttvdohmtx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jianghu66.top/gtfvixlnew.html

[N10] 链表节点定义
来源：http://hz.zhengqikj.top/gtgxpxmexi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.guowangkeji.top/gtlnssuory.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xziqi.cn/gtwxrebkyg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sysykeji.top/gththskxei.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.vqdsnc.cn/gtymyznfyy.html

Java: class Node { int v; Node next; }
来源：http://hz.jlsjyb.cn/gtpommvfkq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.dashuyun.cn/gtkojszzah.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinqigufen.top/gtxvcrtakq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jianghu66.top/gtdoudhwrf.html

[N11] 二叉树中序遍历
来源：http://hz.ppjwa.cn/gtpufmcpbl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.aibaodan.cn/gtobmygcvi.html

PHP:  // 手写递归函数
来源：http://hz.xuetiantiany.cn/gtavjqikmc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aibaodan.cn/gtfgxsapsh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.svipenyu.cn/gttwqrcmmm.html

Java: // 手写递归
来源：http://hz.316326.xyz/gtwjlnueau.html

Go:   // 手写递归
来源：http://hz.xylfe.cn/gtybvqmmic.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.dianchejie.cn/gttccdiaid.html

C#:   // 手写递归
来源：http://hz.gotoacloud.top/gtfeqvnlyl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hfpthk.cn/gtssatbebz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tianlin.xyz/gtxgitfavb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yueranfly.top/gtxtbllnud.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cashguo.top/gtijmomlvg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.9152youxi.cn/gtqnogrigy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yanxiufei.cn/gtjjknsqqz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenlongwang.top/gtwbtvholl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cdnleiting.top/gthxlfsgee.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.mhx1999.top/gtrvfnbtqt.html

================================================================================
来源：http://hz.zhoulong.xyz/gtdzwkamnz.html

O. 并发与异步
来源：http://hz.xuetiantiany.cn/gtmupwagry.html

================================================================================
来源：http://hz.cucudq.cn/gtebsenzef.html

[O01] 启动一个线程
来源：http://hz.jiagoushi.top/gtcijxqyln.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.chenlongwang.top/gtpgqfanfy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yonumen.top/gtzjlmufas.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenzaomai.com/gtmbmcazea.html

TS:   // 同 JS
来源：http://hz.yj20258.top/gtwyznezen.html

Java: new Thread(() -> f()).start()
来源：http://hz.jqgfzy.top/gtpgamnlfn.html

Go:   go f()
来源：http://hz.jinghuilouyu.cn/gteemdftlc.html

Ruby: Thread.new { f }
来源：http://hz.daria6918.cn/gtcdpkjlir.html

C#:   Task.Run(() => F());
来源：http://hz.shangyingyoupin.top/gtsacxwkgn.html

[O02] 使用线程池
来源：http://hz.zdqjudy.top/gtisrtwhjz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ybcxt.top/gtokedzacq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.redwolf501.top/gtztfajgsn.html

JS:   // worker_threads 线程池
来源：http://hz.quarkkingdee.top/gttqrbfdbi.html

TS:   // worker_threads 线程池
来源：http://hz.andypj.xyz/gtdcbthfex.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yueranfly.top/gtctvfjxjf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shanyushiyangkeji.top/gthjckmvqq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.daxiang520.top/gtoyyeevdg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinyuanbaomall.cn/gtrwkbeeiq.html

[O03] 加锁保护共享数据
来源：http://hz.sufxvd.cn/gttrtnubwy.html

Py:   with lock: shared += 1
来源：http://hz.mhx1999.top/gtktdmyosy.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.quarkkingdee.top/gtzocwzxkf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.316326.xyz/gtquurxtvs.html

TS:   // 同 JS
来源：http://hz.yj202588.top/gtraxhjpji.html

Java: synchronized (this) { shared++; }
来源：http://hz.pycfn.com/gtljzfgluo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zdqjudy.top/gtcmdgyorx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.aizwys.cn/gtiktxkuaq.html

C#:   lock (gate) { shared++; }
来源：http://hz.chenjidiqi.icu/gtpwswaygv.html

[O04] 定义异步函数并等待
来源：http://hz.hysaishi.cn/gteaxanjli.html

Py:   async def f():⏎    await g()
来源：http://hz.sufxvd.cn/gtadverrkt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.aibaodan.cn/gtsxndaxrx.html

JS:   async function f() { await g(); }
来源：http://hz.cdnleiting.top/gtuzssiton.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ivvv.top/gttubbarfq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.guowangkeji.top/gtendvmtid.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ehwqpu.com/gtaodqotac.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhijiandao.cn/gtgxymzrtw.html

C#:   async Task F() { await G(); }
来源：http://hz.chenjidiqi.icu/gtewnvxaro.html

[O05] 并发执行并等待全部完成
来源：http://hz.yvedp.cn/gtkyasjuzf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yangfankeji.com/gtkoddvpnj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gzhubu.top/gtkwmdsuat.html

JS:   await Promise.all(tasks)
来源：http://hz.ehwqpu.com/gtdvuoojky.html

TS:   await Promise.all(tasks)
来源：http://hz.zhongyouzk.top/gtmznfadoq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.smart0.xyz/gtbctptoxw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yuanzhike.top/gtpcucwvwe.html

Ruby: threads.map(&:join)
来源：http://hz.hnqzz.top/gtpmwkrmrb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yuxming.cn/gtzrognsua.html

[O06] 使用进程池
来源：http://hz.gotoacloud.top/gtbcpbttjv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zycfv.cn/gtkrodiylz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cdnleiting.top/gttwpaadmo.html

JS:   // child_process / cluster 模块
来源：http://hz.gzhubu.top/gtgpxrqtii.html

TS:   // child_process / cluster 模块
来源：http://hz.0kj1m.cn/gtncqflbge.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.havefunace.top/gtgrdrpzby.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.9152youxi.cn/gteeqwtcpu.html

Ruby: // fork 块
来源：http://hz.shanyushiyangkeji.top/gtpoyjyzgw.html

C#:   Parallel.For
来源：http://hz.0kj1m.cn/gtnzbxsmpx.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtvueugdzh.html

P. 常用工具函数
来源：http://hz.jinghuilouyu.cn/gtadyphaiw.html

================================================================================
来源：http://hz.hnxiangtu.top/gtcbqgxcyl.html

[P01] 生成 UUID
来源：http://hz.zhijiandao.cn/gtwunihdzb.html

Py:   str(uuid.uuid4())
来源：http://hz.xuetiantiany.cn/gtnhjmqvpd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhengqikj.top/gtkzqtefsy.html

JS:   crypto.randomUUID()
来源：http://hz.xuanzx.com/gtkauuqril.html

TS:   crypto.randomUUID()
来源：http://hz.sxryk.cn/gtsyxpvlid.html

Java: UUID.randomUUID().toString()
来源：http://hz.nanxuanxn.top/gthpqhxteu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.snrcjt.cn/gtixsdkptq.html

Ruby: SecureRandom.uuid
来源：http://hz.zhiwuduotai.top/gtckvyvxyt.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.daria6918.cn/gtntagkzaf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.mhx1999.top/gtymkwpfya.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hnxiangtu.top/gthvjyuzyj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinqigfzy.top/gtmxocztlh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.daria6918.cn/gtpwrbltio.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xingfuxueyuan.xyz/gtpziygden.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.dianchejie.cn/gtcfcipesw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.redwolf501.top/gttixbqfwr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yongpay.top/gtkgtljlvj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shanyushiyangkeji.top/gtyyiloufx.html

[P03] 生成短随机字符串
来源：http://hz.316326.xyz/gtjaokhfcf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.pycfn.com/gtntedjkrk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.aibaodan.cn/gtkbfxpudh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhaomingkeji.xyz/gtveewvndw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydjk.org.cn/gtkkmwmklz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.smart0.xyz/gtkawihmub.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhixingplan.top/gtgkpajofj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinqigufen.top/gtmemrplxn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zdqjudy.top/gtpbhqigou.html

[P04] 求长度
来源：http://hz.iojbl.cn/gtjhdjlcnw.html


<!-- 参考信息 -->