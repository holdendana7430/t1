代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nanxinkj.top/gtvmhcfott.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.aibaodan.cn/gtahmdebqk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hammf.cn/gtbpfwvdqa.html

[L06] 解析响应为 JSON
来源：http://hz.52xcode.cn/gtnnmojkrq.html

Py:   resp.json()
来源：http://hz.hfpthk.cn/gthllwnnam.html

PHP:  json_decode($body, true);
来源：http://hz.shanyushiyangkeji.top/gtyrtnpdtd.html

JS:   await resp.json()
来源：http://hz.chenzaomai.com/gtkoofmfgk.html

TS:   await resp.json()
来源：http://hz.zhengqikj.top/gtlleukznp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sysykeji.top/gtzmcjybcc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.daxiang520.top/gtusojgysk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenjidiqi.icu/gticuvbiop.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ywan-chungtsiang.top/gtrudzgjde.html

[L07] 处理 HTTP 状态码
来源：http://hz.shzxlz.cn/gtrbluinpp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gzhubu.top/gtrurnzwvr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.tianlin.xyz/gtacqiwifc.html

JS:   resp.ok;  resp.status
来源：http://hz.yj20258.top/gtancqekxl.html

TS:   resp.ok;  resp.status
来源：http://hz.gzhubu.top/gtqkdznqmv.html

Java: resp.statusCode()
来源：http://hz.jinqigufen.top/gtcjwwgjpo.html

Go:   resp.StatusCode
来源：http://hz.pengpengdd.cyou/gtqwlslvtw.html

Ruby: resp.code.to_i
来源：http://hz.shzxlz.cn/gtiiskyddx.html

C#:   (int)resp.StatusCode
来源：http://hz.mhx1999.top/gtsyxgdsre.html

[L08] 并发请求多个地址
来源：http://hz.xuanzx.com/gthvuwwgsb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.guowangkeji.top/gtpjvzjtdb.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj20258888.top/gtdpjxrupz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenlongwang.top/gtrgmsygtl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ivvv.top/gtvunwlhwt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gaohongyu789.top/gtzcnzmwab.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hnxiangtu.top/gtpzrlpviw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.fzhhl.top/gtjuriuzjc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xuanzx.com/gtyhnebgeb.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtcyfgnjku.html

M. 命令行 / 进程 / 环境
来源：http://hz.sweek.top/gtexoxotcn.html

================================================================================
来源：http://hz.bjfxy.top/gtgfqkflfv.html

[M01] 读取命令行参数
来源：http://hz.dianchejie.cn/gtbmtsvlrh.html

Py:   sys.argv[1:]
来源：http://hz.cheryme.top/gtjuvscpys.html

PHP:  $argv;  $argc;
来源：http://hz.yueranfly.top/gtoishyiug.html

JS:   process.argv.slice(2)
来源：http://hz.bjfxy.top/gtmgwtaffr.html

TS:   process.argv.slice(2)
来源：http://hz.ydzc1.top/gtrqpkdxqa.html

Java: args 数组（main 方法参数）
来源：http://hz.zhiwuduotai.top/gtrduhopsg.html

Go:   os.Args[1:]
来源：http://hz.ehwqpu.com/gtxjhkbaoc.html

Ruby: ARGV
来源：http://hz.0kj1m.cn/gtbpuhnvex.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nanxuanxn.top/gtnquwjogg.html

[M02] 读取环境变量
来源：http://hz.jianghu66.top/gtusmqsdqj.html

Py:   os.environ.get("HOME")
来源：http://hz.guannengcc.top/gtoeurzcth.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.pengpengdd.cyou/gteuoyqnvl.html

JS:   process.env.HOME
来源：http://hz.pycfn.com/gtzaxsgjji.html

TS:   process.env.HOME
来源：http://hz.aibaodan.cn/gtaqtcmaaz.html

Java: System.getenv("HOME")
来源：http://hz.jianghu66.top/gtohpdgful.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shuidangran.top/gtusgyqjsn.html

Ruby: ENV["HOME"]
来源：http://hz.c1oappe.top/gtefrzgtvw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhongyouzk.top/gtpjleqjur.html

[M03] 执行外部命令
来源：http://hz.xingfuxueyuan.xyz/gttwmqrjkm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhixingplan.top/gtxumkqywb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cucudq.cn/gtmffkznyv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yongpay.top/gtjcuhxiif.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhaomingkeji.xyz/gtskxkqtjh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhengqikj.top/gtvrgokyeq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cdnleiting.top/gtpntkkjdl.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.guowangkeji.top/gtiqzejbbb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhixingplan.top/gtqwhxvbbq.html

[M04] 获取当前工作目录
来源：http://hz.jqgufenzy.top/gtyrtthacu.html

Py:   os.getcwd()
来源：http://hz.xingfuxueyuan.xyz/gtnxgctpio.html

PHP:  getcwd();
来源：http://hz.feifeiyinyue.top/gtgasxtnso.html

JS:   process.cwd()
来源：http://hz.ehwqpu.com/gtuxoipwtz.html

TS:   process.cwd()
来源：http://hz.chenlongwang.top/gtkvmomciq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xziqi.cn/gtwjbfhych.html

Go:   os.Getwd()
来源：http://hz.aibaodan.cn/gtdcqdchml.html

Ruby: Dir.pwd
来源：http://hz.tianlin.xyz/gtdavucbou.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yangfankeji.com/gtaqbrtcge.html

[M05] 设置退出码
来源：http://hz.zhixingplan.top/gtodhdjlzv.html

Py:   sys.exit(1)
来源：http://hz.ydzc1.top/gtromdfrjn.html

PHP:  exit(1);
来源：http://hz.vqdsnc.cn/gthpydjkwg.html

JS:   process.exit(1)
来源：http://hz.iojbl.cn/gtgwublbsm.html

TS:   process.exit(1)
来源：http://hz.jiagoushi.top/gtxyyncnij.html

Java: System.exit(1)
来源：http://hz.ppjwa.cn/gtgkdgwfuv.html

Go:   os.Exit(1)
来源：http://hz.jyoumei.cn/gtiddpnfpt.html

Ruby: exit 1
来源：http://hz.dianchejie.cn/gtzbnqfzqb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shanyushiyangkeji.top/gtfwazbqui.html

[M06] 向标准错误输出
来源：http://hz.meibo888.top/gtjzydlluq.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xylfe.cn/gtzgomczgy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhijiandao.cn/gtjvtkgxuk.html

JS:   console.error("err")
来源：http://hz.jqgfzy.top/gtagqyouzh.html

TS:   console.error("err")
来源：http://hz.zhoulong.xyz/gttfnxxxqi.html

Java: System.err.println("err")
来源：http://hz.xziqi.cn/gtrseriflj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jqgfzy.top/gtugflyefx.html

Ruby: warn "err"
来源：http://hz.jiagoushi.top/gtchwyprkz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jqgfzy.top/gtwlklmgxk.html

[M07] 判断是否为主入口
来源：http://hz.shzxlz.cn/gtdccfsoym.html

Py:   if __name__ == "__main__":
来源：http://hz.c1oappe.top/gtzvbxtoqe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.snrcjt.cn/gtiwuxrldp.html

JS:   require.main === module
来源：http://hz.daxiang520.top/gtcnjccxrl.html

TS:   require.main === module
来源：http://hz.jianghu66.top/gtqifnatfd.html

Java: public static void main(String[] args)
来源：http://hz.jyoumei.cn/gtwjimxbmi.html

Go:   func main()
来源：http://hz.xziqi.cn/gtnyoxoxuv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ehwqpu.com/gtaufatffx.html

C#:   static void Main(string[] args)
来源：http://hz.c1oappe.top/gtkwtbielr.html

[M08] 获取系统与运行时信息
来源：http://hz.jlsjyb.cn/gtigifpjko.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yongpay.top/gtkkkdevat.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.redwolf501.top/gteyccymiu.html

JS:   process.platform;  process.version
来源：http://hz.ydjk.org.cn/gtugkuyedl.html

TS:   process.platform;  process.version
来源：http://hz.shzxlz.cn/gtwtqvcyih.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xziqi.cn/gtrqdtcoyv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.guowangkeji.top/gtwuaoztiz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.52xcode.cn/gtysvikhwf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hywenlv.cn/gtkkpfhipe.html

================================================================================
来源：http://hz.jinqigfzy.top/gtktqfgjxq.html

N. 数据结构与算法
来源：http://hz.zhengqikj.top/gtgboflqnn.html

================================================================================
来源：http://hz.jinqigfzy.top/gtjgavydpv.html

[N01] 二分查找（有序数组）
来源：http://hz.gzhubu.top/gtluccyrig.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.quarkkingdee.top/gtxpxnhqtn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.nwbrower.top/gtmeztrbvq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ppjwa.cn/gtgoolsgdp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhongyouzk.top/gthbpysepi.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenlongwang.top/gttslpydcv.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jlsjyb.cn/gttnvnwwra.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.tian-w.cn/gtsxjombgh.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xuetiantiany.cn/gtwscwolef.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhijiandao.cn/gtubgzqzsx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ehwqpu.com/gtgcdsocti.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.wangshuangyany.cn/gtvhrqxhox.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zdqjudy.top/gtutmzvzrq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hnxiangtu.top/gtlivlbasc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yj20258888.top/gtdoqxlmci.html

Go:   slices.Sort(arr)
来源：http://hz.yonumen.top/gtekahergu.html

Ruby: arr.sort
来源：http://hz.quarkkingdee.top/gtvhxvqjlt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhixingplan.top/gtmlwkuxjk.html

[N03] 快速排序（分治示例）
来源：http://hz.aizwys.cn/gtfpmhmyod.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.nanxuanxn.top/gtbbihgngt.html

PHP:  // 递归实现，或用 usort
来源：http://hz.aibaodan.cn/gtbmluziws.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigufen.top/gtltqpwcvi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xziqi.cn/gtwkieiyjj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.iojbl.cn/gtpsmctmqt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.chenlongwang.top/gtxouqulhy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yuxming.cn/gtiyuhomox.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yangfankeji.com/gtkoypfnfd.html

[N04] 斐波那契数列
来源：http://hz.guannengcc.top/gtbysddnkm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangkeji.top/gtkevgijae.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.aibaodan.cn/gtxnwtgmij.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.wangshuangyany.cn/gtxmtehyqi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fzhhl.top/gtrcwkcpqw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jyoumei.cn/gtyltcczoa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.andypj.xyz/gtscxudnfc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.c1oappe.top/gtbsrsujuw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sxryk.cn/gtrevhlimj.html

[N05] 最大公约数
来源：http://hz.jinghuilouyu.cn/gtjaviisic.html

Py:   math.gcd(a, b)
来源：http://hz.snrcjt.cn/gtjseiyxrf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.iojbl.cn/gtmjadmdza.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jianghu66.top/gtzokmmsol.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nwbrower.top/gtbidjosgt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gotoacloud.top/gtyupniqiu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinghuilouyu.cn/gtuxqiviqb.html

Ruby: a.gcd(b)
来源：http://hz.ivvv.top/gtlnijfjaz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jianghu66.top/gtrdtlkvya.html

[N06] 判断回文字符串
来源：http://hz.snrcjt.cn/gtshjbqzun.html

Py:   s == s[::-1]
来源：http://hz.aizwys.cn/gtbzzzwdde.html

PHP:  $s === strrev($s);
来源：http://hz.hnqzz.top/gtyvmujepz.html

JS:   s === [...s].reverse().join("")
来源：http://hz.0kj1m.cn/gtcjpwyfee.html

TS:   s === [...s].reverse().join("")
来源：http://hz.birdmap.top/gtaxqvnpnm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.andypj.xyz/gtlqumhihi.html

Go:   // 双指针从两端比较
来源：http://hz.jinyuanbaomall.cn/gtdxmbfxfw.html

Ruby: s == s.reverse
来源：http://hz.yuanzhike.top/gtelyitaka.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.dianchejie.cn/gtgujtgwnx.html

[N07] 两数之和（返回下标）
来源：http://hz.ydzc1.top/gtorwrclcw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.sufxvd.cn/gtgeblhivc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jlsjyb.cn/gtxhygzvlz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.wangdashe.top/gtmisimnmc.html

TS:   // 手写 Map<string, number>
来源：http://hz.ybcxt.top/gtuvpeeyyj.html

Java: // 手写 HashMap
来源：http://hz.cqqwz.cn/gtsdxgrgmd.html

Go:   // 手写 map[int]int
来源：http://hz.nwbrower.top/gtuuxddcvf.html

Ruby: // 手写 Hash
来源：http://hz.52xcode.cn/gtkvmizuso.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.aizwys.cn/gtktersvlq.html

[N08] 生成全排列
来源：http://hz.zhijiandao.cn/gtrvurorso.html

Py:   itertools.permutations(arr)
来源：http://hz.xinyue.icu/gtfvskmrfm.html

PHP:  // 手写递归交换
来源：http://hz.xylfe.cn/gtuczdocds.html

JS:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtueorxerg.html

TS:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtktrlohdj.html

Java: // 手写回溯递归
来源：http://hz.jianghu66.top/gtitqntfqg.html

Go:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtlfctvoxb.html

Ruby: arr.permutation.to_a
来源：http://hz.vqdsnc.cn/gtnblvcjct.html

C#:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtgxewrjim.html

[N09] 栈与队列
来源：http://hz.daxiang520.top/gtyevvdpti.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.chenzaomai.com/gtddcibvir.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xylfe.cn/gtrvawedxb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinqigufen.top/gtluwzalrc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.fengsongda.top/gtwjrxpzqv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hnxiangtu.top/gtqwkkxakh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.andypj.xyz/gtuwbqxiog.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.haohaochexian.top/gtnwowydtd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jyoumei.cn/gtzblwmbyi.html

[N10] 链表节点定义
来源：http://hz.zhoulong.xyz/gtceflulxp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.pengpengdd.cyou/gturbtlwum.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.dashuyun.cn/gtocskbgkx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ydzc1.top/gtoihirimu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shangyingyoupin.top/gtoksmbsoj.html

Java: class Node { int v; Node next; }
来源：http://hz.xingfuxueyuan.xyz/gtnlmjckph.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jqgfzy.top/gtcnolwjgo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.daria6918.cn/gtfoobmyia.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shangyingyoupin.top/gtwtzrkbqa.html

[N11] 二叉树中序遍历
来源：http://hz.jinqigufen.top/gtikgqjnnc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.gzhubu.top/gtuyxmvobk.html

PHP:  // 手写递归函数
来源：http://hz.daria6918.cn/gtfuizzabo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhongyouzk.top/gtzibdnmop.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cashguo.top/gtrpemohrg.html

Java: // 手写递归
来源：http://hz.316326.xyz/gtiwbzsydc.html

Go:   // 手写递归
来源：http://hz.dianchejie.cn/gtvdxkshjp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yonumen.top/gtvtbmemdr.html

C#:   // 手写递归
来源：http://hz.yongpay.top/gtypdguwfr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shuidangran.top/gtcmiqakgl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.sweek.top/gtkbliudjx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hammf.cn/gtdkrtaoxy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangdashe.top/gtxxffosww.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhongyouzk.top/gtmeouuonq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangkeji.top/gtbkvqefwv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zdqjudy.top/gtpwxsrakt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.smart0.xyz/gtvjukimab.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guannengcc.top/gtbpvjyima.html

================================================================================
来源：http://hz.shzxlz.cn/gtguanihuz.html

O. 并发与异步
来源：http://hz.ehwqpu.com/gtboeqhdex.html

================================================================================
来源：http://hz.mhx1999.top/gtndwcozic.html

[O01] 启动一个线程
来源：http://hz.gaohongyu789.top/gtcnmexiwp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hammf.cn/gtyisojuhx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shangyingyoupin.top/gtjipxyaop.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.vqdsnc.cn/gtlmwjgmoz.html

TS:   // 同 JS
来源：http://hz.zhijiandao.cn/gtdqmxjjcq.html

Java: new Thread(() -> f()).start()
来源：http://hz.jlsjyb.cn/gtgabapzwi.html

Go:   go f()
来源：http://hz.yj20258888.top/gtvqbmaszs.html

Ruby: Thread.new { f }
来源：http://hz.redwolf501.top/gtkgtlhaoa.html

C#:   Task.Run(() => F());
来源：http://hz.gaohongyu789.top/gtzqhvqbcd.html

[O02] 使用线程池
来源：http://hz.svipenyu.cn/gtfeeygwpt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.daxiang520.top/gtcjxjoktx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ybcxt.top/gtlmvvfljf.html

JS:   // worker_threads 线程池
来源：http://hz.tian-w.cn/gtcxjesdpg.html

TS:   // worker_threads 线程池
来源：http://hz.yj20258.top/gtniqnkhbf.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.daxiang520.top/gtdvdjalqj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.fzhhl.top/gtqcdmidsn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.316326.xyz/gttualtxsm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ydjk.org.cn/gtaavvkwnt.html

[O03] 加锁保护共享数据
来源：http://hz.jqgufenzy.top/gtqivuytrr.html

Py:   with lock: shared += 1
来源：http://hz.havefunace.top/gtcnkorjcu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.guannengcc.top/gtijvjkajt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhiwuduotai.top/gtooaqghbf.html

TS:   // 同 JS
来源：http://hz.zhixingplan.top/gtyllofsty.html

Java: synchronized (this) { shared++; }
来源：http://hz.yj20258.top/gtwxeogplh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.daria6918.cn/gtcdiffjlu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yj202588.top/gtclelhjkg.html

C#:   lock (gate) { shared++; }
来源：http://hz.cashguo.top/gtcfoaljfq.html

[O04] 定义异步函数并等待
来源：http://hz.0kj1m.cn/gtkwcyvvzo.html

Py:   async def f():⏎    await g()
来源：http://hz.nanxinkj.top/gtgwiiheci.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.daria6918.cn/gtxsbnklkf.html

JS:   async function f() { await g(); }
来源：http://hz.sysykeji.top/gthzvfulfp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hfpthk.cn/gtwbkostue.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jinqigufen.top/gtrnomrqyt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yuxming.cn/gtnmgeviya.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zycfv.cn/gtzaiylzib.html

C#:   async Task F() { await G(); }
来源：http://hz.52xcode.cn/gtkanycgiw.html

[O05] 并发执行并等待全部完成
来源：http://hz.meibo888.top/gtxculqccm.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ybcxt.top/gtqzaayonn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.316326.xyz/gtneoqbxpq.html

JS:   await Promise.all(tasks)
来源：http://hz.tian-w.cn/gtkanpmrra.html

TS:   await Promise.all(tasks)
来源：http://hz.cheryme.top/gtglkpqamn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.guowangkeji.top/gtspnxipww.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xingfuxueyuan.xyz/gtgsxpsfqm.html

Ruby: threads.map(&:join)
来源：http://hz.sysykeji.top/gtzmhhwibr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shangyingyoupin.top/gtlhyhiomx.html

[O06] 使用进程池
来源：http://hz.fengsongda.top/gtircdrkyw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.daxiang520.top/gtpitliitq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.c1oappe.top/gtgrqhidbl.html

JS:   // child_process / cluster 模块
来源：http://hz.xuetiantiany.cn/gtrofagsbg.html

TS:   // child_process / cluster 模块
来源：http://hz.yanxiufei.cn/gtiopperbl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.mhx1999.top/gtdngzmldb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.quarkkingdee.top/gtcgwrvjeo.html

Ruby: // fork 块
来源：http://hz.haohaochexian.top/gtzcpjgfsa.html

C#:   Parallel.For
来源：http://hz.shanyushiyangkeji.top/gtdnllkouy.html

================================================================================
来源：http://hz.dashuyun.cn/gtjerqbwxw.html

P. 常用工具函数
来源：http://hz.c1oappe.top/gtlbjwivof.html

================================================================================
来源：http://hz.zhixingplan.top/gtarqlyruv.html

[P01] 生成 UUID
来源：http://hz.tian-w.cn/gtgjwydlqe.html

Py:   str(uuid.uuid4())
来源：http://hz.hywenlv.cn/gteifacanq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.nanxinkj.top/gthfuzbgvv.html

JS:   crypto.randomUUID()
来源：http://hz.yangfankeji.com/gtmvovkijq.html

TS:   crypto.randomUUID()
来源：http://hz.jinghuilouyu.cn/gtwcpcyzma.html

Java: UUID.randomUUID().toString()
来源：http://hz.yangfankeji.com/gtmqyzbmxg.html

Go:   // 用 github.com/google/uuid
来源：http://hz.aibaodan.cn/gtnkhdnfkd.html

Ruby: SecureRandom.uuid
来源：http://hz.hnxiangtu.top/gtnzmwbmbq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.dashuyun.cn/gteeaubkbi.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yangfankeji.com/gtyjtwzpyi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cdnleiting.top/gtnxzqtbnk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.guannengcc.top/gtrkoggwoj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ydzc1.top/gtkumdlvnn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.chenzaomai.com/gtxnaxasxt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yongpay.top/gtsaefebvs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.guannengcc.top/gtocpyajig.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jyoumei.cn/gtrbvmnghs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jianghu66.top/gtphegzdvv.html

[P03] 生成短随机字符串
来源：http://hz.zhengqikj.top/gtqkitybxt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xinyue.icu/gtngnvmhyc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hongshengwenyu.top/gtoykjvdhg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.haohaochexian.top/gtcjhguabf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.guowangkeji.top/gtbyuibugs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.0kj1m.cn/gtelzdtcwt.html


<!-- 参考信息 -->