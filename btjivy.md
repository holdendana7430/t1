代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cucudq.cn/gtwqmlwhhw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cqqwz.cn/gtjowiwzbh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.pengpengdd.cyou/gtgyrwwgme.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.mhx1999.top/gthjyxidno.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.andypj.xyz/gtimsdglcm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.nwbrower.top/gtcmkkfqsv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ydjk.org.cn/gtlpyteszy.html

[L06] 解析响应为 JSON
来源：http://hz.aizwys.cn/gtqddkcikq.html

Py:   resp.json()
来源：http://hz.daria6918.cn/gtlthkhfnd.html

PHP:  json_decode($body, true);
来源：http://hz.bjfxy.top/gtszplonsq.html

JS:   await resp.json()
来源：http://hz.xuanzx.com/gtzvtndlvh.html

TS:   await resp.json()
来源：http://hz.yongpay.top/gtehyrhgbc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yonumen.top/gtmghxqtlq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gzhubu.top/gticfhgkkw.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenjidiqi.icu/gtwmowmlej.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.guannengcc.top/gtytvkcyzb.html

[L07] 处理 HTTP 状态码
来源：http://hz.c1oappe.top/gtyxylypub.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gzhubu.top/gtcxchewqn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ywan-chungtsiang.top/gtxotjqpbe.html

JS:   resp.ok;  resp.status
来源：http://hz.pengpengdd.cyou/gtjtasehkm.html

TS:   resp.ok;  resp.status
来源：http://hz.shangyingyoupin.top/gttaczwsni.html

Java: resp.statusCode()
来源：http://hz.ywan-chungtsiang.top/gtqasckapc.html

Go:   resp.StatusCode
来源：http://hz.havefunace.top/gtjxyykiyt.html

Ruby: resp.code.to_i
来源：http://hz.yj20258888.top/gtkpzhhwhz.html

C#:   (int)resp.StatusCode
来源：http://hz.shanyushiyangkeji.top/gtsstjbsbj.html

[L08] 并发请求多个地址
来源：http://hz.birdmap.top/gtlwapjpmt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.snrcjt.cn/gtgbnnmstm.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinqigfzy.top/gtztxsblya.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.smart0.xyz/gtmlfjdlfe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhoulong.xyz/gthxcqqmsc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinghuilouyu.cn/gtukznnjcb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cucudq.cn/gtuucoosak.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ywan-chungtsiang.top/gtfmgrtade.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.nanxuanxn.top/gtdmxwonhc.html

================================================================================
来源：http://hz.daria6918.cn/gtwwawjnzi.html

M. 命令行 / 进程 / 环境
来源：http://hz.yj20258.top/gtfdbmfgqf.html

================================================================================
来源：http://hz.vqdsnc.cn/gtecvsrbir.html

[M01] 读取命令行参数
来源：http://hz.ydzc1.top/gtxxfqgdpb.html

Py:   sys.argv[1:]
来源：http://hz.ybcxt.top/gtqrtkndyo.html

PHP:  $argv;  $argc;
来源：http://hz.dianchejie.cn/gthumvnbey.html

JS:   process.argv.slice(2)
来源：http://hz.sweek.top/gtzukamcpt.html

TS:   process.argv.slice(2)
来源：http://hz.jinghuilouyu.cn/gtngiwkiub.html

Java: args 数组（main 方法参数）
来源：http://hz.aizwys.cn/gtogplyrsv.html

Go:   os.Args[1:]
来源：http://hz.zhongyouzk.top/gtpsbmygib.html

Ruby: ARGV
来源：http://hz.jyoumei.cn/gtoludpeoz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cucudq.cn/gtfskuckzy.html

[M02] 读取环境变量
来源：http://hz.cdnleiting.top/gtjvstcqgl.html

Py:   os.environ.get("HOME")
来源：http://hz.jianghu66.top/gtizpzukcg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.haohaochexian.top/gtgxxgdxsr.html

JS:   process.env.HOME
来源：http://hz.yj202588.top/gttqmoqwto.html

TS:   process.env.HOME
来源：http://hz.zdqjudy.top/gttfinrqam.html

Java: System.getenv("HOME")
来源：http://hz.cdnleiting.top/gtroolwnkv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhijiandao.cn/gtpyuvbzph.html

Ruby: ENV["HOME"]
来源：http://hz.meibo888.top/gtfpcqdlaq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.andypj.xyz/gtunnxxcac.html

[M03] 执行外部命令
来源：http://hz.fzhhl.top/gttisqvoni.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.sufxvd.cn/gtyaprxwrm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.tian-w.cn/gtijxjqxsu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhixingplan.top/gtppqswdcj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.redwolf501.top/gtjmlauehi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.shuidangran.top/gtzareptvl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.birdmap.top/gtbghqqvmf.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.feifeiyinyue.top/gtdhgyrnut.html

C#:   Process.Start("ls", "-l");
来源：http://hz.chenlongwang.top/gtwelbmhud.html

[M04] 获取当前工作目录
来源：http://hz.bjfxy.top/gtkdgjxxsu.html

Py:   os.getcwd()
来源：http://hz.ppjwa.cn/gtgeatezvx.html

PHP:  getcwd();
来源：http://hz.jlsjyb.cn/gtjiktsxry.html

JS:   process.cwd()
来源：http://hz.sxryk.cn/gtauyfbeeg.html

TS:   process.cwd()
来源：http://hz.quarkkingdee.top/gtusxcwdqd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sufxvd.cn/gtgvmmwiee.html

Go:   os.Getwd()
来源：http://hz.yangfankeji.com/gtjraqnqlz.html

Ruby: Dir.pwd
来源：http://hz.gaohongyu789.top/gtbkedgybc.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.nanxinkj.top/gtggqzbajs.html

[M05] 设置退出码
来源：http://hz.xziqi.cn/gtsxvcvxwn.html

Py:   sys.exit(1)
来源：http://hz.yuanzhike.top/gtvipvscdn.html

PHP:  exit(1);
来源：http://hz.zycfv.cn/gtanmxcbso.html

JS:   process.exit(1)
来源：http://hz.kuanghao11.cn/gtsqgsaton.html

TS:   process.exit(1)
来源：http://hz.shangyingyoupin.top/gtoqgispik.html

Java: System.exit(1)
来源：http://hz.yj20258.top/gtntxdrdax.html

Go:   os.Exit(1)
来源：http://hz.redwolf501.top/gtpnsayjou.html

Ruby: exit 1
来源：http://hz.xuanzx.com/gtfkjvjutl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.bjfxy.top/gtnmxncikk.html

[M06] 向标准错误输出
来源：http://hz.fzhhl.top/gtixlmbbvg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sweek.top/gthqnbjoni.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cqqwz.cn/gtbkhfkquu.html

JS:   console.error("err")
来源：http://hz.zycfv.cn/gtqmhiolfq.html

TS:   console.error("err")
来源：http://hz.dashuyun.cn/gtnrmkehsh.html

Java: System.err.println("err")
来源：http://hz.yj20258.top/gtauggrnbn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gaohongyu789.top/gtegkenfjr.html

Ruby: warn "err"
来源：http://hz.daria6918.cn/gtsdmmwfpu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cqqwz.cn/gtmvlywsyl.html

[M07] 判断是否为主入口
来源：http://hz.jinyuanbaomall.cn/gtbgqiqbvd.html

Py:   if __name__ == "__main__":
来源：http://hz.svipenyu.cn/gtocmoohjp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.smart0.xyz/gtdamcotfl.html

JS:   require.main === module
来源：http://hz.jinghuilouyu.cn/gtqsvqxfyb.html

TS:   require.main === module
来源：http://hz.guowangkeji.top/gtyspqfixs.html

Java: public static void main(String[] args)
来源：http://hz.tianlin.xyz/gtigmqqcao.html

Go:   func main()
来源：http://hz.316326.xyz/gtqsftperu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.dianchejie.cn/gtxwxhmhbf.html

C#:   static void Main(string[] args)
来源：http://hz.xuanzx.com/gtvepcjbss.html

[M08] 获取系统与运行时信息
来源：http://hz.redwolf501.top/gtuwqgqvok.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ywan-chungtsiang.top/gtggotbdtf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenjidiqi.icu/gtraeyxwmf.html

JS:   process.platform;  process.version
来源：http://hz.yj20258.top/gtdoeiruuf.html

TS:   process.platform;  process.version
来源：http://hz.jinghuilouyu.cn/gtyavceohl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.aizwys.cn/gtfznsttzl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sufxvd.cn/gtxhltjqrt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cucudq.cn/gtgrtukjxj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhengqikj.top/gtjfgantil.html

================================================================================
来源：http://hz.jlsjyb.cn/gtdujqfifh.html

N. 数据结构与算法
来源：http://hz.hysaishi.cn/gtsgclvhhk.html

================================================================================
来源：http://hz.cucudq.cn/gtkvhuyohg.html

[N01] 二分查找（有序数组）
来源：http://hz.52xcode.cn/gtiicjkqyu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gotoacloud.top/gtnoxbjpud.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gotoacloud.top/gtzvqqwpxg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydzc1.top/gtdzeccjve.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gogol.net.cn/gtwmchjgsd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.c1oappe.top/gtsrmwapld.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shuidangran.top/gtsxorzeev.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.cdnleiting.top/gtajjsgqio.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.quarkkingdee.top/gtegyegtgp.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhijiandao.cn/gtnpwtyewe.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhixingplan.top/gtoyvchbfm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yvedp.cn/gthkweqafk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fengsongda.top/gtdyuzjjpz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yonumen.top/gtgejamcnv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhixingplan.top/gtyqkvreqj.html

Go:   slices.Sort(arr)
来源：http://hz.gzhubu.top/gtdufhrgza.html

Ruby: arr.sort
来源：http://hz.meibo888.top/gtvlehtkcu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jqgufenzy.top/gtkynvwvex.html

[N03] 快速排序（分治示例）
来源：http://hz.yuanzhike.top/gtyquippix.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jianghu66.top/gtjyoxijue.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cdnleiting.top/gtaukkaqpi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shuidangran.top/gtoxthsoot.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhaomingkeji.xyz/gtulivabiq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.vqdsnc.cn/gtehuychof.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cheryme.top/gtveglnqxc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jinqigufen.top/gtxxlypbla.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ehwqpu.com/gtalpiqukn.html

[N04] 斐波那契数列
来源：http://hz.ydzc1.top/gtczdirwvr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.daria6918.cn/gtvqivetxo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shuidangran.top/gtoynxkmpd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xuanzx.com/gtshsnjppx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xylfe.cn/gtdjrehwcr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yangfankeji.com/gtjyvmsmfq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.wangshuangyany.cn/gticjjsxww.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.dianchejie.cn/gtrikzjtwc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jqgfzy.top/gtwnyjqxai.html

[N05] 最大公约数
来源：http://hz.hnxiangtu.top/gttocoqtpy.html

Py:   math.gcd(a, b)
来源：http://hz.nanxinkj.top/gtfhqqwgav.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.wangshuangyany.cn/gtdfitaidf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xylfe.cn/gtlraadamj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangdashe.top/gtpaynwmpj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.feifeiyinyue.top/gtlfajczce.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.daxiang520.top/gtqybxlvte.html

Ruby: a.gcd(b)
来源：http://hz.cashguo.top/gtqvjmfeum.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jqgfzy.top/gtflusjhkx.html

[N06] 判断回文字符串
来源：http://hz.jinqigufen.top/gtamkvtwzj.html

Py:   s == s[::-1]
来源：http://hz.fengsongda.top/gtyvmcpjqi.html

PHP:  $s === strrev($s);
来源：http://hz.dianchejie.cn/gtcgvxtmxj.html

JS:   s === [...s].reverse().join("")
来源：http://hz.pycfn.com/gtneldcpyl.html

TS:   s === [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtvtuxmobe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xingfuxueyuan.xyz/gtyiikaihg.html

Go:   // 双指针从两端比较
来源：http://hz.0kj1m.cn/gtwgecnoyr.html

Ruby: s == s.reverse
来源：http://hz.zhaomingkeji.xyz/gtgmvamdla.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xziqi.cn/gthkexohau.html

[N07] 两数之和（返回下标）
来源：http://hz.9152youxi.cn/gtftohijtp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hysaishi.cn/gtvimjqhjr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gogol.net.cn/gtlsjgeyur.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hywenlv.cn/gtsussqjxo.html

TS:   // 手写 Map<string, number>
来源：http://hz.jqgufenzy.top/gthesoibcg.html

Java: // 手写 HashMap
来源：http://hz.cashguo.top/gthhtjtrth.html

Go:   // 手写 map[int]int
来源：http://hz.sxryk.cn/gteenmqbfc.html

Ruby: // 手写 Hash
来源：http://hz.ivvv.top/gttdpbaszz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shzxlz.cn/gtoodouddp.html

[N08] 生成全排列
来源：http://hz.xylfe.cn/gtdejudrvr.html

Py:   itertools.permutations(arr)
来源：http://hz.sysykeji.top/gtxndneaiu.html

PHP:  // 手写递归交换
来源：http://hz.cucudq.cn/gtswejkysz.html

JS:   // 手写回溯递归
来源：http://hz.havefunace.top/gtkldbvbdb.html

TS:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtmhbqjwnd.html

Java: // 手写回溯递归
来源：http://hz.gotoacloud.top/gttbccywai.html

Go:   // 手写回溯递归
来源：http://hz.ehwqpu.com/gtbqmehfsa.html

Ruby: arr.permutation.to_a
来源：http://hz.yj202588.top/gtpbawwhfi.html

C#:   // 手写回溯递归
来源：http://hz.cqqwz.cn/gtvcrgotau.html

[N09] 栈与队列
来源：http://hz.iojbl.cn/gtdksjbsyv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.chenlongwang.top/gtkhkikrta.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.sxryk.cn/gtavxxczau.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhixingplan.top/gtoooromnj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shanyushiyangkeji.top/gtpyggrsen.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ydjk.org.cn/gtmcfzfnpi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.wangshuangyany.cn/gtyrefypfu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sufxvd.cn/gtemfjiwfb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yj20258888.top/gtxxeiznge.html

[N10] 链表节点定义
来源：http://hz.jlsjyb.cn/gtxgklqcuu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yuxming.cn/gtsckdrhoc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gaohongyu789.top/gtkbheiygq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yuanzhike.top/gtqkrppprh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhoulong.xyz/gtgrxajbwx.html

Java: class Node { int v; Node next; }
来源：http://hz.yuxming.cn/gtyswveuwc.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xuanzx.com/gtevyumemw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhongyouzk.top/gtpqzsucmz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.bjfxy.top/gtebfnywtw.html

[N11] 二叉树中序遍历
来源：http://hz.nanxinkj.top/gtqqspwppl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xinyue.icu/gtwhalpmbx.html

PHP:  // 手写递归函数
来源：http://hz.ppjwa.cn/gtjkalyipn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gogol.net.cn/gtnmopzhcw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgfzy.top/gtjdbfiyrj.html

Java: // 手写递归
来源：http://hz.zdqjudy.top/gtcygvzevb.html

Go:   // 手写递归
来源：http://hz.ivvv.top/gtkjpyccpd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.sufxvd.cn/gtvnawqvlm.html

C#:   // 手写递归
来源：http://hz.fengsongda.top/gterhrowre.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.redwolf501.top/gtpnyktukq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hammf.cn/gtcjmaeewa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.mhx1999.top/gtfudjxeqg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtfvzcxcei.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.birdmap.top/gtjjlnudjm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigufen.top/gtthgififm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shanyushiyangkeji.top/gtebvttrwc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ybcxt.top/gttrumtxij.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.smart0.xyz/gtsisagmus.html

================================================================================
来源：http://hz.ybcxt.top/gtdvkksrjv.html

O. 并发与异步
来源：http://hz.snrcjt.cn/gtjmygzvkp.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtkryecymu.html

[O01] 启动一个线程
来源：http://hz.52xcode.cn/gtpokxozta.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhengqikj.top/gteqtsbmro.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jqgufenzy.top/gtsslbxzui.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.52xcode.cn/gtgbvfouhl.html

TS:   // 同 JS
来源：http://hz.shanyushiyangkeji.top/gtijkixkhe.html

Java: new Thread(() -> f()).start()
来源：http://hz.wangshuangyany.cn/gtcfrxrupg.html

Go:   go f()
来源：http://hz.c1oappe.top/gtcltbyjmx.html

Ruby: Thread.new { f }
来源：http://hz.gaohongyu789.top/gtoyazbjqi.html

C#:   Task.Run(() => F());
来源：http://hz.fengsongda.top/gtbnoaqhsv.html

[O02] 使用线程池
来源：http://hz.zycfv.cn/gtnmfzpfee.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinqigfzy.top/gtwyjbfbqd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nwbrower.top/gtsmtwjchg.html

JS:   // worker_threads 线程池
来源：http://hz.hywenlv.cn/gtuwkffyzj.html

TS:   // worker_threads 线程池
来源：http://hz.yj202588.top/gtihyuxbmb.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinqigufen.top/gtzklaedgv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.tianlin.xyz/gtuycyobux.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.wangshuangyany.cn/gtcylvqxxd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yuxming.cn/gtpizsrenl.html

[O03] 加锁保护共享数据
来源：http://hz.nanxinkj.top/gtffxnnrfc.html

Py:   with lock: shared += 1
来源：http://hz.yueranfly.top/gtcnzwjkyv.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xuetiantiany.cn/gtkyrowtev.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.wangdashe.top/gthcioytjj.html

TS:   // 同 JS
来源：http://hz.xingfuxueyuan.xyz/gtcslkaduv.html

Java: synchronized (this) { shared++; }
来源：http://hz.sysykeji.top/gtcqtyehjd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zycfv.cn/gtqajtekdk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.nwbrower.top/gtcswehais.html

C#:   lock (gate) { shared++; }
来源：http://hz.jinqigufen.top/gtceaikegc.html

[O04] 定义异步函数并等待
来源：http://hz.dianchejie.cn/gtkgvibcad.html

Py:   async def f():⏎    await g()
来源：http://hz.zhijiandao.cn/gtmvvpgfdr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.chenjidiqi.icu/gtnazapaio.html

JS:   async function f() { await g(); }
来源：http://hz.hfpthk.cn/gtkxnrzeyq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xuanzx.com/gtnlsqfmco.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yongpay.top/gtlvxdlnqk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhixingplan.top/gtozsqlnpk.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hfpthk.cn/gttshdpios.html

C#:   async Task F() { await G(); }
来源：http://hz.shanyushiyangkeji.top/gtxfhndcmu.html

[O05] 并发执行并等待全部完成
来源：http://hz.gogol.net.cn/gtysexykgr.html

Py:   asyncio.gather(*tasks)
来源：http://hz.snrcjt.cn/gtjwxoxjfr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhaomingkeji.xyz/gtvaqrubqh.html

JS:   await Promise.all(tasks)
来源：http://hz.ybcxt.top/gtoysyjznk.html

TS:   await Promise.all(tasks)
来源：http://hz.smart0.xyz/gtyekhlcai.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ehwqpu.com/gtusdoiloh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.haohaochexian.top/gtcluymxcc.html

Ruby: threads.map(&:join)
来源：http://hz.gzhubu.top/gtngpdmsgl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinyuanbaomall.cn/gtfuvwlxeg.html

[O06] 使用进程池
来源：http://hz.wangdashe.top/gtsrulaihb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhixingplan.top/gtqpvbzhrn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.gzhubu.top/gtxghmjsuv.html

JS:   // child_process / cluster 模块
来源：http://hz.aizwys.cn/gtceqoxawi.html

TS:   // child_process / cluster 模块
来源：http://hz.yvedp.cn/gtyhecdrha.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yuanzhike.top/gtchldbuny.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.kuanghao11.cn/gtagkgtwqa.html

Ruby: // fork 块
来源：http://hz.shuidangran.top/gtavbppuci.html

C#:   Parallel.For
来源：http://hz.nanxinkj.top/gtyadhedrn.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtwuowlpjl.html

P. 常用工具函数
来源：http://hz.9152youxi.cn/gtcwhlbmqq.html

================================================================================
来源：http://hz.yvedp.cn/gtrdhqxrbx.html

[P01] 生成 UUID
来源：http://hz.svipenyu.cn/gteczqylyi.html

Py:   str(uuid.uuid4())
来源：http://hz.cucudq.cn/gtczwdhumh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.tanke756.top/gtnfttguuu.html

JS:   crypto.randomUUID()
来源：http://hz.ybcxt.top/gtwxxezdvl.html

TS:   crypto.randomUUID()
来源：http://hz.chenzaomai.com/gtlypnhgpj.html

Java: UUID.randomUUID().toString()
来源：http://hz.ybcxt.top/gtytsotvpz.html

Go:   // 用 github.com/google/uuid
来源：http://hz.meibo888.top/gtzpnqsdfq.html

Ruby: SecureRandom.uuid
来源：http://hz.jinqigfzy.top/gthzthhqyq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.9152youxi.cn/gtndeezbko.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yangfankeji.com/gtlcyniocr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xuanzx.com/gtsfkjzfpb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.9152youxi.cn/gtoerwupbe.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ybcxt.top/gtikcwdrzv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shuidangran.top/gtslvdpjtl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.bjfxy.top/gtchiozhtn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hongshengwenyu.top/gtlsfeexav.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.shangyingyoupin.top/gtjmtbkwul.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.gotoacloud.top/gtlautkuqy.html

[P03] 生成短随机字符串
来源：http://hz.jianghu66.top/gtlcmjyeoh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jiagoushi.top/gtwrokthav.html


<!-- 参考信息 -->