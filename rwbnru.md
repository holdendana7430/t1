代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xziqi.cn/gtebjnayzr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnqzz.top/gthyvdsykk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenzaomai.com/gtxcnrtavk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.dashuyun.cn/gtabstqrqy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shuidangran.top/gtcwppphsx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yanxiufei.cn/gtkswtxxvw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.0kj1m.cn/gtrxluckje.html

[L06] 解析响应为 JSON
来源：http://hz.fengsongda.top/gtqblpboyz.html

Py:   resp.json()
来源：http://hz.shuidangran.top/gtjdmbvpvg.html

PHP:  json_decode($body, true);
来源：http://hz.nanxinkj.top/gtuedvnovp.html

JS:   await resp.json()
来源：http://hz.hywenlv.cn/gtqjseqqec.html

TS:   await resp.json()
来源：http://hz.cashguo.top/gtvnzocilw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.wangdashe.top/gtbxefhkcl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ydzc1.top/gtpqjsxxls.html

Ruby: JSON.parse(resp.body)
来源：http://hz.guannengcc.top/gtpptyeccv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jinqigufen.top/gtlgwfvrnj.html

[L07] 处理 HTTP 状态码
来源：http://hz.meibo888.top/gtifbtluge.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sysykeji.top/gtglieubzq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinyuanbaomall.cn/gttwgymrlj.html

JS:   resp.ok;  resp.status
来源：http://hz.jiagoushi.top/gtvcqpekot.html

TS:   resp.ok;  resp.status
来源：http://hz.guowangkeji.top/gtgdoqvdbv.html

Java: resp.statusCode()
来源：http://hz.ppjwa.cn/gtdhzdrgdo.html

Go:   resp.StatusCode
来源：http://hz.jianghu66.top/gtzabwmlta.html

Ruby: resp.code.to_i
来源：http://hz.jinqigufen.top/gtflokihgh.html

C#:   (int)resp.StatusCode
来源：http://hz.meibo888.top/gtawhngzag.html

[L08] 并发请求多个地址
来源：http://hz.jyoumei.cn/gtlvrajhsf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.nwbrower.top/gtuzqyzokv.html

PHP:  curl_multi_init() 系列
来源：http://hz.gogol.net.cn/gtklpueezb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ivvv.top/gtbzzyyije.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.kuanghao11.cn/gtkpjuzsyo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zycfv.cn/gtrywkivow.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.quarkkingdee.top/gtgkibvzto.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhaomingkeji.xyz/gtfgjdvdmo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.haohaochexian.top/gtmplrrrqi.html

================================================================================
来源：http://hz.cucudq.cn/gtmhxukqyq.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhoulong.xyz/gtdhhikdpr.html

================================================================================
来源：http://hz.ybcxt.top/gtjwwdfwww.html

[M01] 读取命令行参数
来源：http://hz.ydjk.org.cn/gtaiadqgpa.html

Py:   sys.argv[1:]
来源：http://hz.nanxinkj.top/gtukizjdim.html

PHP:  $argv;  $argc;
来源：http://hz.hnxiangtu.top/gtzucmlcri.html

JS:   process.argv.slice(2)
来源：http://hz.xinyue.icu/gtxunwuaki.html

TS:   process.argv.slice(2)
来源：http://hz.hammf.cn/gtljxvrqlk.html

Java: args 数组（main 方法参数）
来源：http://hz.xinyue.icu/gthlrmlbdv.html

Go:   os.Args[1:]
来源：http://hz.cqqwz.cn/gtkohzeqnr.html

Ruby: ARGV
来源：http://hz.cdnleiting.top/gtbtsxcukb.html

C#:   args 数组（Main 方法参数）
来源：http://hz.fengsongda.top/gtkwkwcbmd.html

[M02] 读取环境变量
来源：http://hz.aibaodan.cn/gtaodefywe.html

Py:   os.environ.get("HOME")
来源：http://hz.zhaomingkeji.xyz/gtbqeollfy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hysaishi.cn/gtdvaoavlj.html

JS:   process.env.HOME
来源：http://hz.zhoulong.xyz/gttofkghht.html

TS:   process.env.HOME
来源：http://hz.wangdashe.top/gtzojuaqoq.html

Java: System.getenv("HOME")
来源：http://hz.hammf.cn/gtfhfmtrko.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yueranfly.top/gtwndvcldj.html

Ruby: ENV["HOME"]
来源：http://hz.bjfxy.top/gtqestnosx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.nanxuanxn.top/gtuoiqtqtr.html

[M03] 执行外部命令
来源：http://hz.yueranfly.top/gtikkjkewm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hnxiangtu.top/gtjjzojlyk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yangfankeji.com/gtxfpbvgqr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jiagoushi.top/gthbrgkjec.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cqqwz.cn/gtqcjmwslz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.birdmap.top/gtguduugjc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yongpay.top/gtwcevbnwx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ydjk.org.cn/gtpfvofrhw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.meibo888.top/gttegksqzq.html

[M04] 获取当前工作目录
来源：http://hz.cdnleiting.top/gtktqgssgn.html

Py:   os.getcwd()
来源：http://hz.yanxiufei.cn/gthosjdnfi.html

PHP:  getcwd();
来源：http://hz.hnxiangtu.top/gtsiiltumm.html

JS:   process.cwd()
来源：http://hz.wangshuangyany.cn/gtjopbbjgm.html

TS:   process.cwd()
来源：http://hz.fengsongda.top/gtyswtelrw.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.guannengcc.top/gtrsqtdunh.html

Go:   os.Getwd()
来源：http://hz.redwolf501.top/gtiksynmil.html

Ruby: Dir.pwd
来源：http://hz.bjfxy.top/gtimmhdasm.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.fengsongda.top/gtgkuuvnzs.html

[M05] 设置退出码
来源：http://hz.cucudq.cn/gtalucyfeb.html

Py:   sys.exit(1)
来源：http://hz.hnqzz.top/gtuqayoiml.html

PHP:  exit(1);
来源：http://hz.jinghuilouyu.cn/gtqtcvuyed.html

JS:   process.exit(1)
来源：http://hz.mhx1999.top/gttdtrrzle.html

TS:   process.exit(1)
来源：http://hz.jqgufenzy.top/gtzvrxiqnm.html

Java: System.exit(1)
来源：http://hz.meibo888.top/gtvfwruvek.html

Go:   os.Exit(1)
来源：http://hz.chenjidiqi.icu/gtjwfsysrj.html

Ruby: exit 1
来源：http://hz.yueranfly.top/gtddizygxd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.aizwys.cn/gtjhixowin.html

[M06] 向标准错误输出
来源：http://hz.52xcode.cn/gteiucsxdm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhixingplan.top/gtzzzfeysh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hysaishi.cn/gtnatseobu.html

JS:   console.error("err")
来源：http://hz.ywan-chungtsiang.top/gtbdzprcxr.html

TS:   console.error("err")
来源：http://hz.redwolf501.top/gtrubsubim.html

Java: System.err.println("err")
来源：http://hz.gzhubu.top/gtedpvxric.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.aibaodan.cn/gtocqjelzz.html

Ruby: warn "err"
来源：http://hz.haohaochexian.top/gtaqvoduja.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.sysykeji.top/gtjvzzzhuu.html

[M07] 判断是否为主入口
来源：http://hz.chenlongwang.top/gtgjrlrmiw.html

Py:   if __name__ == "__main__":
来源：http://hz.wangdashe.top/gtxbktmlcc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ppjwa.cn/gtuhemeajz.html

JS:   require.main === module
来源：http://hz.jyoumei.cn/gtsycucoww.html

TS:   require.main === module
来源：http://hz.hongshengwenyu.top/gtlznjoyas.html

Java: public static void main(String[] args)
来源：http://hz.xingfuxueyuan.xyz/gtfoluiyfs.html

Go:   func main()
来源：http://hz.bjfxy.top/gtpongwpiq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.chenlongwang.top/gtubiaqcry.html

C#:   static void Main(string[] args)
来源：http://hz.aizwys.cn/gtrkijpjly.html

[M08] 获取系统与运行时信息
来源：http://hz.jiagoushi.top/gtwkemawom.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shuidangran.top/gtlxeeiels.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jinqigfzy.top/gttqsbomtl.html

JS:   process.platform;  process.version
来源：http://hz.jqgfzy.top/gtzjmnnslj.html

TS:   process.platform;  process.version
来源：http://hz.wangdashe.top/gtwxgnxckp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xylfe.cn/gtswwrhvnq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yonumen.top/gtcoqioqru.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cashguo.top/gtwlcocfrx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.fengsongda.top/gtzncrgggp.html

================================================================================
来源：http://hz.jyoumei.cn/gtjquklmbk.html

N. 数据结构与算法
来源：http://hz.zdqjudy.top/gtgwyzifzs.html

================================================================================
来源：http://hz.dianchejie.cn/gtbkxrdwus.html

[N01] 二分查找（有序数组）
来源：http://hz.jinghuilouyu.cn/gtegrxzmiw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shangyingyoupin.top/gtmowddwhq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zdqjudy.top/gtjsvqzxph.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shuidangran.top/gtmqwusksr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yueranfly.top/gtzbknftkw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yongpay.top/gtfvxkoeot.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xylfe.cn/gtcgsncapo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sufxvd.cn/gtgefcflzn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yuxming.cn/gtuiivtlrs.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.nanxinkj.top/gteglhflzq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.guowangkeji.top/gtscotjitv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yuxming.cn/gtfiaciuwu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenlongwang.top/gtfomdkxiz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinghuilouyu.cn/gthjtxqnsg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.guowangkeji.top/gtaocrwvbg.html

Go:   slices.Sort(arr)
来源：http://hz.jlsjyb.cn/gtewivlsva.html

Ruby: arr.sort
来源：http://hz.yuxming.cn/gtxonazyjt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.chenjidiqi.icu/gtrdiuwmbw.html

[N03] 快速排序（分治示例）
来源：http://hz.meibo888.top/gtwnqzfyhr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.dianchejie.cn/gtvzbbznxi.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sufxvd.cn/gtifhxlxkx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zdqjudy.top/gtqxertrwk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.mhx1999.top/gtxsmdrjvt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinghuilouyu.cn/gtbquagzib.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.aizwys.cn/gtexnfbawx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cdnleiting.top/gthuoxyzxq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yangfankeji.com/gtwmhclxgp.html

[N04] 斐波那契数列
来源：http://hz.jianghu66.top/gtrnqmcvex.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.mhx1999.top/gtbpvkwqit.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yangfankeji.com/gtcuywhobw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aizwys.cn/gtmijjmiur.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cheryme.top/gtmjiqbaoy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.quarkkingdee.top/gtskahnlhr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sweek.top/gtjhcycosu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.pycfn.com/gtoypeuvea.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ywan-chungtsiang.top/gtaiocxazq.html

[N05] 最大公约数
来源：http://hz.yangfankeji.com/gtsnkygxvy.html

Py:   math.gcd(a, b)
来源：http://hz.iojbl.cn/gtfyfhofqv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yangfankeji.com/gtejlhbybv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigfzy.top/gtywewlurm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daxiang520.top/gtjfifrfhl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenlongwang.top/gtnivakjxg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.vqdsnc.cn/gtervuvbsb.html

Ruby: a.gcd(b)
来源：http://hz.hysaishi.cn/gtffvhzsyq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shanyushiyangtech.top/gtbfgeusrm.html

[N06] 判断回文字符串
来源：http://hz.yanxiufei.cn/gttaowusta.html

Py:   s == s[::-1]
来源：http://hz.316326.xyz/gtnqqiotnf.html

PHP:  $s === strrev($s);
来源：http://hz.tanke756.top/gtfstdnsbx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yueranfly.top/gtrtckcaku.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tanke756.top/gtiixbgkde.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yueranfly.top/gtjjdbejys.html

Go:   // 双指针从两端比较
来源：http://hz.chenjidiqi.icu/gtfcprydby.html

Ruby: s == s.reverse
来源：http://hz.jiagoushi.top/gtwxfjxkys.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ydzc1.top/gtpmnmetsr.html

[N07] 两数之和（返回下标）
来源：http://hz.sufxvd.cn/gtodcnpzga.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.52xcode.cn/gtrffagvvx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.daria6918.cn/gtbywyzond.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.pycfn.com/gtodanoaou.html

TS:   // 手写 Map<string, number>
来源：http://hz.ywan-chungtsiang.top/gtgcfuhwmc.html

Java: // 手写 HashMap
来源：http://hz.haohaochexian.top/gtjpqdyngw.html

Go:   // 手写 map[int]int
来源：http://hz.nanxuanxn.top/gtqusprytn.html

Ruby: // 手写 Hash
来源：http://hz.feifeiyinyue.top/gtezptfrje.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jqgfzy.top/gtfbxltoul.html

[N08] 生成全排列
来源：http://hz.cdnleiting.top/gtmndmfcoa.html

Py:   itertools.permutations(arr)
来源：http://hz.jqgufenzy.top/gtderdnpnz.html

PHP:  // 手写递归交换
来源：http://hz.yj20258888.top/gtvsgcuwnh.html

JS:   // 手写回溯递归
来源：http://hz.yonumen.top/gtxjjhkhwb.html

TS:   // 手写回溯递归
来源：http://hz.yonumen.top/gthiaptsft.html

Java: // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtsafosueo.html

Go:   // 手写回溯递归
来源：http://hz.cucudq.cn/gtrjafrzrq.html

Ruby: arr.permutation.to_a
来源：http://hz.quarkkingdee.top/gtegqbfvcs.html

C#:   // 手写回溯递归
来源：http://hz.dianchejie.cn/gtnbgovewj.html

[N09] 栈与队列
来源：http://hz.havefunace.top/gtslcoscpa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yvedp.cn/gtqkquzdzb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yj20258.top/gtvprxahwh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hnxiangtu.top/gtytvdcpih.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.sweek.top/gtgyrclidp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.pycfn.com/gtauqrytpa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.aibaodan.cn/gtpegyowpe.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sxryk.cn/gttvvhwrmn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cheryme.top/gtybzcnpen.html

[N10] 链表节点定义
来源：http://hz.jinghuilouyu.cn/gtvlpejxyu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.sufxvd.cn/gtxlqqpqwa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yangfankeji.com/gteiynzecl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jqgfzy.top/gtbvkutjuw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.birdmap.top/gtrhahxmkw.html

Java: class Node { int v; Node next; }
来源：http://hz.c1oappe.top/gtvsmrfhap.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xylfe.cn/gtokjqsqjn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sysykeji.top/gtknrkrgfu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhongyouzk.top/gtzebpxdds.html

[N11] 二叉树中序遍历
来源：http://hz.yangfankeji.com/gtlkjmkybr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.smart0.xyz/gttjghsxzd.html

PHP:  // 手写递归函数
来源：http://hz.bjfxy.top/gtakahawvb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ppjwa.cn/gtlohpyjdg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hywenlv.cn/gtfuotclwl.html

Java: // 手写递归
来源：http://hz.gzhubu.top/gtokrzpfef.html

Go:   // 手写递归
来源：http://hz.chenzaomai.com/gttgxoxilk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.0kj1m.cn/gtnwmixxat.html

C#:   // 手写递归
来源：http://hz.ydzc1.top/gtvbrdhxen.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.guowangkeji.top/gtonovmazm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yvedp.cn/gttreqtsge.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yonumen.top/gtwcaavcjh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jlsjyb.cn/gtlmmwcdwf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xziqi.cn/gtomvpjfgk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fzhhl.top/gtvydbzpdz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.nanxuanxn.top/gtcmpvydfc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cqqwz.cn/gtdppzldpy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guowangkeji.top/gtukzkvjsr.html

================================================================================
来源：http://hz.zycfv.cn/gtvkigkxdh.html

O. 并发与异步
来源：http://hz.gaohongyu789.top/gtmkgqjwbg.html

================================================================================
来源：http://hz.52xcode.cn/gtlfswlkyj.html

[O01] 启动一个线程
来源：http://hz.havefunace.top/gttcjvxmht.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhaomingkeji.xyz/gtudmbwjof.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yvedp.cn/gtjfzlxyul.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hnqzz.top/gtkqcglkdd.html

TS:   // 同 JS
来源：http://hz.nanxuanxn.top/gtrafleckb.html

Java: new Thread(() -> f()).start()
来源：http://hz.zdqjudy.top/gtqdvtjgkr.html

Go:   go f()
来源：http://hz.cucudq.cn/gtbfpuisgf.html

Ruby: Thread.new { f }
来源：http://hz.svipenyu.cn/gtywrjozop.html

C#:   Task.Run(() => F());
来源：http://hz.nanxuanxn.top/gtqifiqucy.html

[O02] 使用线程池
来源：http://hz.zhongyouzk.top/gtmuboqjxf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shuidangran.top/gtqvzspbyo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xinyue.icu/gtbqfpypmb.html

JS:   // worker_threads 线程池
来源：http://hz.daria6918.cn/gtblowgvha.html

TS:   // worker_threads 线程池
来源：http://hz.wangshuangyany.cn/gtloyvjpzo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xuanzx.com/gtwjgdrwbf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.quarkkingdee.top/gtsldteshs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ydzc1.top/gttkujwqir.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.iojbl.cn/gtielacrur.html

[O03] 加锁保护共享数据
来源：http://hz.hywenlv.cn/gtrwwqript.html

Py:   with lock: shared += 1
来源：http://hz.0kj1m.cn/gtvhnljvnu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xingfuxueyuan.xyz/gtibkeebjk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yuanzhike.top/gttizsxnzl.html

TS:   // 同 JS
来源：http://hz.zhijiandao.cn/gtdoseqygw.html

Java: synchronized (this) { shared++; }
来源：http://hz.feifeiyinyue.top/gtjytfcstw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zdqjudy.top/gtswyyttjg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.tian-w.cn/gtzruujyut.html

C#:   lock (gate) { shared++; }
来源：http://hz.shuidangran.top/gtaaqvbvnn.html

[O04] 定义异步函数并等待
来源：http://hz.pycfn.com/gtrglvdksg.html

Py:   async def f():⏎    await g()
来源：http://hz.vqdsnc.cn/gttwqcfecz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ydzc1.top/gtgipexisp.html

JS:   async function f() { await g(); }
来源：http://hz.iojbl.cn/gtzkyzlprp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.gotoacloud.top/gtnrrgzpnr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zycfv.cn/gtvjptmkpc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.mhx1999.top/gtpfuezphx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shangyingyoupin.top/gtoqsmffeq.html

C#:   async Task F() { await G(); }
来源：http://hz.yongpay.top/gtgcefdsai.html

[O05] 并发执行并等待全部完成
来源：http://hz.jlsjyb.cn/gtubecwkju.html

Py:   asyncio.gather(*tasks)
来源：http://hz.tian-w.cn/gthekpigyb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhoulong.xyz/gtwjbneixk.html

JS:   await Promise.all(tasks)
来源：http://hz.316326.xyz/gtfoauszwo.html

TS:   await Promise.all(tasks)
来源：http://hz.yj20258.top/gtkecdpyzx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.kuanghao11.cn/gtgepolziv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.dianchejie.cn/gtebjyuswy.html

Ruby: threads.map(&:join)
来源：http://hz.yuxming.cn/gtbwirdfac.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.quarkkingdee.top/gtfiwqztfb.html

[O06] 使用进程池
来源：http://hz.52xcode.cn/gtatcnvxus.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.0kj1m.cn/gtokvmrftv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.birdmap.top/gtueplnzau.html

JS:   // child_process / cluster 模块
来源：http://hz.ivvv.top/gtvlpkhoco.html

TS:   // child_process / cluster 模块
来源：http://hz.jlsjyb.cn/gtwjbmnpdn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.gzhubu.top/gtskvkvkfv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jiagoushi.top/gtxjzolovl.html

Ruby: // fork 块
来源：http://hz.dianchejie.cn/gthsoiutvx.html

C#:   Parallel.For
来源：http://hz.jianghu66.top/gtpzavgxkt.html

================================================================================
来源：http://hz.birdmap.top/gtcnknnnme.html

P. 常用工具函数
来源：http://hz.yj202588.top/gtarmwbxro.html

================================================================================
来源：http://hz.nwbrower.top/gtnrtyhdir.html

[P01] 生成 UUID
来源：http://hz.jinqigfzy.top/gtoulniybj.html

Py:   str(uuid.uuid4())
来源：http://hz.hnxiangtu.top/gtxwttzngo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.daxiang520.top/gtofkwxvun.html

JS:   crypto.randomUUID()
来源：http://hz.hysaishi.cn/gtdtgtmnsv.html

TS:   crypto.randomUUID()
来源：http://hz.zycfv.cn/gtextitzht.html

Java: UUID.randomUUID().toString()
来源：http://hz.zycfv.cn/gttxyaykbo.html

Go:   // 用 github.com/google/uuid
来源：http://hz.pycfn.com/gtilopzctj.html

Ruby: SecureRandom.uuid
来源：http://hz.cdnleiting.top/gtddyfcetg.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shuidangran.top/gtzbfdgnps.html

[P02] MD5 / SHA256 摘要
来源：http://hz.gzhubu.top/gtttwdzyrg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zycfv.cn/gtvtgvzfwh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.dashuyun.cn/gtwuvepxes.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.meibo888.top/gttiznziid.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hnqzz.top/gtksjbpgcz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhiwuduotai.top/gtacqbxlsb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.iojbl.cn/gtwxkchiiw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yj202588.top/gtlvmphawk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.nanxuanxn.top/gtlgkfqsbl.html

[P03] 生成短随机字符串
来源：http://hz.yvedp.cn/gtmsogblvl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.bjfxy.top/gtznccajsq.html


<!-- 参考信息 -->