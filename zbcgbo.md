代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.0kj1m.cn/gtnabjbsuv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zycfv.cn/gtwgtodpmv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.pycfn.com/gttpasomud.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.aizwys.cn/gtupzpopmk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xinyue.icu/gtyjvslqfz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.havefunace.top/gtfbmcslkg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gogol.net.cn/gtndxcnsnb.html

[L06] 解析响应为 JSON
来源：http://hz.andypj.xyz/gtrjhunibj.html

Py:   resp.json()
来源：http://hz.shangyingyoupin.top/gthfwmnbne.html

PHP:  json_decode($body, true);
来源：http://hz.kuanghao11.cn/gtdggkkuic.html

JS:   await resp.json()
来源：http://hz.52xcode.cn/gtiozvwvka.html

TS:   await resp.json()
来源：http://hz.havefunace.top/gtpdlfscnn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jqgufenzy.top/gtfyusixel.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hongshengwenyu.top/gtyzddclbo.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ehwqpu.com/gtynefbgvd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.smart0.xyz/gtcrrrwcts.html

[L07] 处理 HTTP 状态码
来源：http://hz.9152youxi.cn/gtmapjmjcz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.tian-w.cn/gtmsxxofvg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shangyingyoupin.top/gtdanuxusx.html

JS:   resp.ok;  resp.status
来源：http://hz.wangshuangyany.cn/gtybsdpasp.html

TS:   resp.ok;  resp.status
来源：http://hz.hnqzz.top/gtwyvjwavc.html

Java: resp.statusCode()
来源：http://hz.gzhubu.top/gttnskfoay.html

Go:   resp.StatusCode
来源：http://hz.yuxming.cn/gtejflkgvs.html

Ruby: resp.code.to_i
来源：http://hz.xuanzx.com/gttysqxtdb.html

C#:   (int)resp.StatusCode
来源：http://hz.yvedp.cn/gtipipqhzl.html

[L08] 并发请求多个地址
来源：http://hz.ehwqpu.com/gtuostdhcj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.feifeiyinyue.top/gtplowqqxa.html

PHP:  curl_multi_init() 系列
来源：http://hz.chenzaomai.com/gtjqktctqv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.0kj1m.cn/gtcnmsclgu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hnxiangtu.top/gtmvixwzfi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ydjk.org.cn/gtshadlumy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.quarkkingdee.top/gtrcxqkiyp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.smart0.xyz/gtvnlzopwc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ydjk.org.cn/gtbqwdtwen.html

================================================================================
来源：http://hz.bjfxy.top/gtvfhpicxg.html

M. 命令行 / 进程 / 环境
来源：http://hz.ehwqpu.com/gtpqhonupx.html

================================================================================
来源：http://hz.smart0.xyz/gttglxodkm.html

[M01] 读取命令行参数
来源：http://hz.wangshuangyany.cn/gtzbnihbqy.html

Py:   sys.argv[1:]
来源：http://hz.xylfe.cn/gttewudohg.html

PHP:  $argv;  $argc;
来源：http://hz.yanxiufei.cn/gtuflgdzeu.html

JS:   process.argv.slice(2)
来源：http://hz.ybcxt.top/gtnrbmwfmp.html

TS:   process.argv.slice(2)
来源：http://hz.shuidangran.top/gtmhvmbylk.html

Java: args 数组（main 方法参数）
来源：http://hz.gogol.net.cn/gtvhoaxuwa.html

Go:   os.Args[1:]
来源：http://hz.c1oappe.top/gturppcozw.html

Ruby: ARGV
来源：http://hz.zhaomingkeji.xyz/gtjbnsbtxt.html

C#:   args 数组（Main 方法参数）
来源：http://hz.feifeiyinyue.top/gtwpswgfoe.html

[M02] 读取环境变量
来源：http://hz.zhixingplan.top/gtihwdhrqg.html

Py:   os.environ.get("HOME")
来源：http://hz.hywenlv.cn/gtbnqnswgi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ppjwa.cn/gtbmphmyes.html

JS:   process.env.HOME
来源：http://hz.hysaishi.cn/gtfohaveyi.html

TS:   process.env.HOME
来源：http://hz.nanxuanxn.top/gtenzmicvx.html

Java: System.getenv("HOME")
来源：http://hz.tian-w.cn/gtuusnqjpc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhijiandao.cn/gtjxahkgan.html

Ruby: ENV["HOME"]
来源：http://hz.mhx1999.top/gtlkisevmc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jqgufenzy.top/gtkvdgdbgs.html

[M03] 执行外部命令
来源：http://hz.zhoulong.xyz/gtliouogtz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.sxryk.cn/gtfltavnva.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.chenlongwang.top/gtnvezhibk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yanxiufei.cn/gtmtrbcaii.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yangfankeji.com/gtypexzcyn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ydjk.org.cn/gtpxjrntmt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yj202588.top/gtlqpgrapo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.chenzaomai.com/gtvsycxktd.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cashguo.top/gtgffnkkuc.html

[M04] 获取当前工作目录
来源：http://hz.zhijiandao.cn/gtktbkxxfu.html

Py:   os.getcwd()
来源：http://hz.cashguo.top/gtpuarqige.html

PHP:  getcwd();
来源：http://hz.yongpay.top/gtcjvaccol.html

JS:   process.cwd()
来源：http://hz.shuidangran.top/gtwkjxnnzo.html

TS:   process.cwd()
来源：http://hz.ivvv.top/gtztfcujot.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shzxlz.cn/gtbfyanyjj.html

Go:   os.Getwd()
来源：http://hz.kuanghao11.cn/gthqczjekm.html

Ruby: Dir.pwd
来源：http://hz.gaohongyu789.top/gtohggnvtm.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ywan-chungtsiang.top/gtbysvovyr.html

[M05] 设置退出码
来源：http://hz.jinghuilouyu.cn/gtzebllivs.html

Py:   sys.exit(1)
来源：http://hz.zhongyouzk.top/gtwhoublii.html

PHP:  exit(1);
来源：http://hz.tanke756.top/gtoltbfbsh.html

JS:   process.exit(1)
来源：http://hz.ybcxt.top/gtlqwdpwfu.html

TS:   process.exit(1)
来源：http://hz.cheryme.top/gtjejhzrwd.html

Java: System.exit(1)
来源：http://hz.yanxiufei.cn/gtiawiqptr.html

Go:   os.Exit(1)
来源：http://hz.cucudq.cn/gtivoijkpv.html

Ruby: exit 1
来源：http://hz.shuidangran.top/gtkvsfwffb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ivvv.top/gtdwgzdagi.html

[M06] 向标准错误输出
来源：http://hz.xuanzx.com/gtyylcaiww.html

Py:   print("err", file=sys.stderr)
来源：http://hz.daxiang520.top/gtffhdrerd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.daxiang520.top/gtncznefzf.html

JS:   console.error("err")
来源：http://hz.fengsongda.top/gtqucnogvm.html

TS:   console.error("err")
来源：http://hz.hongshengwenyu.top/gtlszlefto.html

Java: System.err.println("err")
来源：http://hz.yuanzhike.top/gtnpnpbtiv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cucudq.cn/gtcyoiltcm.html

Ruby: warn "err"
来源：http://hz.kuanghao11.cn/gtxlfmkrxp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ywan-chungtsiang.top/gtbjepgngd.html

[M07] 判断是否为主入口
来源：http://hz.9152youxi.cn/gthaszqdxw.html

Py:   if __name__ == "__main__":
来源：http://hz.ydzc1.top/gtzvteqiny.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.wangshuangyany.cn/gtopisdgcw.html

JS:   require.main === module
来源：http://hz.tian-w.cn/gtjnfpzall.html

TS:   require.main === module
来源：http://hz.nanxinkj.top/gtmuvjdnhj.html

Java: public static void main(String[] args)
来源：http://hz.gaohongyu789.top/gtsozfntyb.html

Go:   func main()
来源：http://hz.316326.xyz/gtpguiozzu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhengqikj.top/gtlikftifm.html

C#:   static void Main(string[] args)
来源：http://hz.hnxiangtu.top/gtfyvuijbh.html

[M08] 获取系统与运行时信息
来源：http://hz.c1oappe.top/gtxrwfazmw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xuanzx.com/gtvxxhqdvo.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.aizwys.cn/gtchcgqioh.html

JS:   process.platform;  process.version
来源：http://hz.yuanzhike.top/gtdcijlkfp.html

TS:   process.platform;  process.version
来源：http://hz.snrcjt.cn/gtlvtcoeot.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cucudq.cn/gtgcpiznib.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xylfe.cn/gtcscgllvr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yuanzhike.top/gtnqqbtqpo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yonumen.top/gthtjzhffp.html

================================================================================
来源：http://hz.yj202588.top/gtlouyjiej.html

N. 数据结构与算法
来源：http://hz.9152youxi.cn/gtvojmgypq.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gthcatnqmp.html

[N01] 二分查找（有序数组）
来源：http://hz.cqqwz.cn/gtdlvmenut.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtxjfmflyb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinghuilouyu.cn/gtdwsuxgsj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hongshengwenyu.top/gtokoveomx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.c1oappe.top/gtktyvetco.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xziqi.cn/gtvzekvlsc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hongshengwenyu.top/gtvsmgroyl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shangyingyoupin.top/gtpxfgegvl.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.fengsongda.top/gtmzddinsk.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yangfankeji.com/gtaxzarins.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.c1oappe.top/gttpsexasw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tian-w.cn/gtssqzrzyw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daria6918.cn/gtgcrdxtkl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jqgufenzy.top/gtkhsiufey.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shanyushiyangtech.top/gtxrtbrrdk.html

Go:   slices.Sort(arr)
来源：http://hz.sufxvd.cn/gtcecphpeo.html

Ruby: arr.sort
来源：http://hz.jinghuilouyu.cn/gtltrkznnt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.chenlongwang.top/gtzkrasnwq.html

[N03] 快速排序（分治示例）
来源：http://hz.sufxvd.cn/gtbcsrbfdb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xinyue.icu/gtxdkzthha.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cheryme.top/gtnybbkcfv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shangyingyoupin.top/gtpoirkaeq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.kuanghao11.cn/gtlxtbswlh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xylfe.cn/gtawhrnssu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.mhx1999.top/gtxolfcvpp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenjidiqi.icu/gtbmntusev.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.fzhhl.top/gtglvxojhm.html

[N04] 斐波那契数列
来源：http://hz.quarkkingdee.top/gtkoicbsak.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.gzhubu.top/gtyzsghqte.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.dashuyun.cn/gtpcbpokfj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cucudq.cn/gtmirfenxf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.vqdsnc.cn/gtakixyvrb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.wangdashe.top/gtetuanfzw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hysaishi.cn/gttkkeuhgg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cdnleiting.top/gtmmvztsxk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenzaomai.com/gtzragpgpf.html

[N05] 最大公约数
来源：http://hz.shuidangran.top/gtcuwnpazq.html

Py:   math.gcd(a, b)
来源：http://hz.jinghuilouyu.cn/gtdlepfydh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.pycfn.com/gtiipbgmyf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ybcxt.top/gtsnkuqbwu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.iojbl.cn/gtfomwuydp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yuanzhike.top/gtuadsffmb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.guannengcc.top/gtwxwdexga.html

Ruby: a.gcd(b)
来源：http://hz.ivvv.top/gtgmfkcgjl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhijiandao.cn/gtchhzmbob.html

[N06] 判断回文字符串
来源：http://hz.cucudq.cn/gtqyspnzuw.html

Py:   s == s[::-1]
来源：http://hz.gogol.net.cn/gtfatlhqzo.html

PHP:  $s === strrev($s);
来源：http://hz.aizwys.cn/gtkktuwjgg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtvxxeonsz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.fzhhl.top/gtmmpigmos.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.aibaodan.cn/gtyyqdaayx.html

Go:   // 双指针从两端比较
来源：http://hz.sysykeji.top/gtakrbmkld.html

Ruby: s == s.reverse
来源：http://hz.kuanghao11.cn/gtihnrdvqs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zdqjudy.top/gtewpwqphk.html

[N07] 两数之和（返回下标）
来源：http://hz.gotoacloud.top/gtsibvhmeu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.guowangkeji.top/gtmzhcnzrp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.fzhhl.top/gtaafeygyf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.52xcode.cn/gtqdpqajin.html

TS:   // 手写 Map<string, number>
来源：http://hz.hysaishi.cn/gtyptktplv.html

Java: // 手写 HashMap
来源：http://hz.jianghu66.top/gtwkwvexsz.html

Go:   // 手写 map[int]int
来源：http://hz.yongpay.top/gtyixuvpuf.html

Ruby: // 手写 Hash
来源：http://hz.cashguo.top/gtorswfxsz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ppjwa.cn/gtimglvldj.html

[N08] 生成全排列
来源：http://hz.jiagoushi.top/gtcjkfpepb.html

Py:   itertools.permutations(arr)
来源：http://hz.yueranfly.top/gtihlsbfya.html

PHP:  // 手写递归交换
来源：http://hz.gotoacloud.top/gtjpsigeyd.html

JS:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtqvmqbili.html

TS:   // 手写回溯递归
来源：http://hz.sweek.top/gtbvgbbybd.html

Java: // 手写回溯递归
来源：http://hz.nanxinkj.top/gtnjhazlcf.html

Go:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtqoybohbp.html

Ruby: arr.permutation.to_a
来源：http://hz.9152youxi.cn/gtwyatzpza.html

C#:   // 手写回溯递归
来源：http://hz.cqqwz.cn/gtzjmbphui.html

[N09] 栈与队列
来源：http://hz.shanyushiyangkeji.top/gtcdluapac.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.nwbrower.top/gtjopemqhw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.gogol.net.cn/gtmxttvsuk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jyoumei.cn/gtmjbiaqsz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.gzhubu.top/gtnhqcfdbx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.wangdashe.top/gtvimftwok.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yueranfly.top/gtvlvooqya.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.fzhhl.top/gtzdgjwkot.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ydjk.org.cn/gtwwwoidox.html

[N10] 链表节点定义
来源：http://hz.redwolf501.top/gtilhstgbe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jinghuilouyu.cn/gtcrqxccjc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gogol.net.cn/gtfyefwrah.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.snrcjt.cn/gthnmeohym.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zdqjudy.top/gtcsfwodjt.html

Java: class Node { int v; Node next; }
来源：http://hz.andypj.xyz/gthoyvyzfq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tanke756.top/gtlckgdcmh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ehwqpu.com/gtqhvsoxks.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yonumen.top/gtuuqcfvbv.html

[N11] 二叉树中序遍历
来源：http://hz.redwolf501.top/gtckkkjjom.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xinyue.icu/gtmemfwaif.html

PHP:  // 手写递归函数
来源：http://hz.jinghuilouyu.cn/gtamagvdvc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhongyouzk.top/gtvmmsuhhr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xuetiantiany.cn/gtdnduneby.html

Java: // 手写递归
来源：http://hz.gogol.net.cn/gtpfitspzv.html

Go:   // 手写递归
来源：http://hz.gogol.net.cn/gtrtilwggr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.birdmap.top/gtykzbngud.html

C#:   // 手写递归
来源：http://hz.zhixingplan.top/gttfjrmkxw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.52xcode.cn/gtiwbntuez.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.andypj.xyz/gtqfbgvadi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.feifeiyinyue.top/gtwisdmxet.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.redwolf501.top/gtfmrxkhdt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shzxlz.cn/gtqwzfhxwa.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guowangkeji.top/gtvavqrksp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.dashuyun.cn/gtngujykdc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xuanzx.com/gtvuwkbknw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.smart0.xyz/gtzbvrbltf.html

================================================================================
来源：http://hz.yj202588.top/gtkxiaixfm.html

O. 并发与异步
来源：http://hz.zhiwuduotai.top/gthdwvbnfq.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtofevjuwh.html

[O01] 启动一个线程
来源：http://hz.yuxming.cn/gtozvuctiq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shanyushiyangkeji.top/gtkxunrnxy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.aizwys.cn/gtopgzzggd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.guowangkeji.top/gtylbixekp.html

TS:   // 同 JS
来源：http://hz.tianlin.xyz/gtzwutvvvv.html

Java: new Thread(() -> f()).start()
来源：http://hz.gotoacloud.top/gtanufncpc.html

Go:   go f()
来源：http://hz.haohaochexian.top/gtvxcnhqyu.html

Ruby: Thread.new { f }
来源：http://hz.haohaochexian.top/gthkgaggcv.html

C#:   Task.Run(() => F());
来源：http://hz.meibo888.top/gtnlhdvpus.html

[O02] 使用线程池
来源：http://hz.pengpengdd.cyou/gtphsjvlvz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinyuanbaomall.cn/gtsymxiezs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nanxuanxn.top/gttcinlrkh.html

JS:   // worker_threads 线程池
来源：http://hz.pengpengdd.cyou/gtsekuaoyy.html

TS:   // worker_threads 线程池
来源：http://hz.ehwqpu.com/gtezekhlmk.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.nanxuanxn.top/gtmxeilpgw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ppjwa.cn/gtlgjcnlzk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.snrcjt.cn/gtswopgrog.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shuidangran.top/gtyyzchuxx.html

[O03] 加锁保护共享数据
来源：http://hz.yongpay.top/gtaqnvqjkx.html

Py:   with lock: shared += 1
来源：http://hz.tian-w.cn/gtpnphcyia.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shzxlz.cn/gtiqvvysep.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hnqzz.top/gtjqngryes.html

TS:   // 同 JS
来源：http://hz.sweek.top/gtxgmdrxww.html

Java: synchronized (this) { shared++; }
来源：http://hz.hysaishi.cn/gthsiwzhum.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jqgufenzy.top/gthoxsjlfq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.quarkkingdee.top/gthoehtqey.html

C#:   lock (gate) { shared++; }
来源：http://hz.daria6918.cn/gthmkvlnmt.html

[O04] 定义异步函数并等待
来源：http://hz.yj202588.top/gtwvioplai.html

Py:   async def f():⏎    await g()
来源：http://hz.nwbrower.top/gtrclqhgfw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.316326.xyz/gtlpwpsdmp.html

JS:   async function f() { await g(); }
来源：http://hz.guannengcc.top/gtwmttyvut.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jiagoushi.top/gtodoarsif.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.fzhhl.top/gtqrrtnsqe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xuetiantiany.cn/gtbtumaxmp.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.fengsongda.top/gtuserydjo.html

C#:   async Task F() { await G(); }
来源：http://hz.daxiang520.top/gthbfmqmmg.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhengqikj.top/gtalnccxgg.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhoulong.xyz/gtdjfbmuok.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zycfv.cn/gtgpvecddr.html

JS:   await Promise.all(tasks)
来源：http://hz.wangdashe.top/gtemwjsoxu.html

TS:   await Promise.all(tasks)
来源：http://hz.quarkkingdee.top/gtqrqiouyu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hfpthk.cn/gtevpdqweo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sweek.top/gtxvxpwqit.html

Ruby: threads.map(&:join)
来源：http://hz.bjfxy.top/gtjmgclhll.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.sufxvd.cn/gtqvfygiri.html

[O06] 使用进程池
来源：http://hz.xuetiantiany.cn/gtkwdamfte.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.gaohongyu789.top/gtblpsiwpt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.0kj1m.cn/gtbjqsejmy.html

JS:   // child_process / cluster 模块
来源：http://hz.jinqigufen.top/gtygyzqdcu.html

TS:   // child_process / cluster 模块
来源：http://hz.cheryme.top/gtvrjabctp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinyuanbaomall.cn/gttlausmdn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ppjwa.cn/gtrlgtipsb.html

Ruby: // fork 块
来源：http://hz.nanxinkj.top/gtsmnwrtpi.html

C#:   Parallel.For
来源：http://hz.wangdashe.top/gtadonsqut.html

================================================================================
来源：http://hz.tanke756.top/gtkirllrvw.html

P. 常用工具函数
来源：http://hz.gogol.net.cn/gtamqxgnid.html

================================================================================
来源：http://hz.chenzaomai.com/gtghprjobs.html

[P01] 生成 UUID
来源：http://hz.hongshengwenyu.top/gtcsryfshw.html

Py:   str(uuid.uuid4())
来源：http://hz.quarkkingdee.top/gttpscppea.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.snrcjt.cn/gtxxyepnqd.html

JS:   crypto.randomUUID()
来源：http://hz.shzxlz.cn/gtyrmwvzrp.html

TS:   crypto.randomUUID()
来源：http://hz.xuetiantiany.cn/gtzbkbppiq.html

Java: UUID.randomUUID().toString()
来源：http://hz.ybcxt.top/gtijugbdbe.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sysykeji.top/gtmoxksmnn.html

Ruby: SecureRandom.uuid
来源：http://hz.ybcxt.top/gtexgqqwlc.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.guannengcc.top/gteanqwhqz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ybcxt.top/gtviaqwwoi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhongyouzk.top/gtzwnsphbi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhixingplan.top/gtskgtszcc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hnqzz.top/gtzskmstnx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.aizwys.cn/gtxrptpgud.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.vqdsnc.cn/gtxzvorten.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.wangshuangyany.cn/gthoxspogz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xylfe.cn/gtajaekbzb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xingfuxueyuan.xyz/gtekagqhrd.html

[P03] 生成短随机字符串
来源：http://hz.havefunace.top/gtjdbgqszd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hnqzz.top/gtqmqxjnzl.html


<!-- 参考信息 -->