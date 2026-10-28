代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.havefunace.top/gtnboutrmj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.redwolf501.top/gtddobnzoo.html

[L05] 上传文件（multipart）
来源：http://hz.gaohongyu789.top/gtakojuaor.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.52xcode.cn/gtsajbtusy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yangfankeji.com/gtjljtitpf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sxryk.cn/gtzctrkmhg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.pengpengdd.cyou/gtjazrowib.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yj20258.top/gtrnmkdfvw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.gzhubu.top/gthtnndofl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jiagoushi.top/gttrxnlrxt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gzhubu.top/gtgmallfew.html

[L06] 解析响应为 JSON
来源：http://hz.jinqigfzy.top/gtdfgoyqlm.html

Py:   resp.json()
来源：http://hz.zdqjudy.top/gtftrzkyuc.html

PHP:  json_decode($body, true);
来源：http://hz.nanxuanxn.top/gtoojrytkn.html

JS:   await resp.json()
来源：http://hz.xingfuxueyuan.xyz/gtahsisisk.html

TS:   await resp.json()
来源：http://hz.kuanghao11.cn/gtwsjgpoop.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.birdmap.top/gttuyjbjow.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.aizwys.cn/gtvyxzqlfu.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tian-w.cn/gtcbendqzq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yj202588.top/gtfcsjkaej.html

[L07] 处理 HTTP 状态码
来源：http://hz.shangyingyoupin.top/gtsfqauzbo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gogol.net.cn/gtgtrezjmm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gogol.net.cn/gtvoixepsq.html

JS:   resp.ok;  resp.status
来源：http://hz.nanxinkj.top/gthelrwkdh.html

TS:   resp.ok;  resp.status
来源：http://hz.9152youxi.cn/gtbdvcrvzc.html

Java: resp.statusCode()
来源：http://hz.shzxlz.cn/gtunhyklue.html

Go:   resp.StatusCode
来源：http://hz.yuxming.cn/gtrteavxcs.html

Ruby: resp.code.to_i
来源：http://hz.chenzaomai.com/gtwwynvpin.html

C#:   (int)resp.StatusCode
来源：http://hz.havefunace.top/gttrgticqz.html

[L08] 并发请求多个地址
来源：http://hz.shanyushiyangtech.top/gtqsyundzb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj20258888.top/gtnkguchdo.html

PHP:  curl_multi_init() 系列
来源：http://hz.ydzc1.top/gtejuefnrg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dashuyun.cn/gtnjekhbmv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hnxiangtu.top/gteatrdiig.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gogol.net.cn/gthzuoczfl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.vqdsnc.cn/gthllbviis.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yj202588.top/gtfaeparjg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.andypj.xyz/gtcmawvxrm.html

================================================================================
来源：http://hz.redwolf501.top/gthetrxnpk.html

M. 命令行 / 进程 / 环境
来源：http://hz.ydzc1.top/gtggilamdj.html

================================================================================
来源：http://hz.svipenyu.cn/gterzkvvsa.html

[M01] 读取命令行参数
来源：http://hz.andypj.xyz/gtewwmhhxl.html

Py:   sys.argv[1:]
来源：http://hz.ydzc1.top/gtcdblbftr.html

PHP:  $argv;  $argc;
来源：http://hz.bjfxy.top/gtyonhcenu.html

JS:   process.argv.slice(2)
来源：http://hz.cashguo.top/gtumsmvgqe.html

TS:   process.argv.slice(2)
来源：http://hz.zhijiandao.cn/gtdlpaxajx.html

Java: args 数组（main 方法参数）
来源：http://hz.hfpthk.cn/gtxvsqljgy.html

Go:   os.Args[1:]
来源：http://hz.ehwqpu.com/gtedgxyfzy.html

Ruby: ARGV
来源：http://hz.jqgufenzy.top/gtkvccmpxi.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhoulong.xyz/gthzrmdupz.html

[M02] 读取环境变量
来源：http://hz.xziqi.cn/gtdxwwworw.html

Py:   os.environ.get("HOME")
来源：http://hz.aibaodan.cn/gtymrctfuj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xuanzx.com/gtispdcpqj.html

JS:   process.env.HOME
来源：http://hz.sxryk.cn/gtvnlohrxn.html

TS:   process.env.HOME
来源：http://hz.shzxlz.cn/gtpjcitzoj.html

Java: System.getenv("HOME")
来源：http://hz.zhixingplan.top/gthrqtnotd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yvedp.cn/gtuxdktehh.html

Ruby: ENV["HOME"]
来源：http://hz.chenjidiqi.icu/gtulssuuuy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.aibaodan.cn/gtibfhpspp.html

[M03] 执行外部命令
来源：http://hz.yuanzhike.top/gtyovtytjo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.fengsongda.top/gthbsierij.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ivvv.top/gtaykprnbl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.9152youxi.cn/gtmnwllfpl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.316326.xyz/gtevfspdeu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.redwolf501.top/gtlqzazhuf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yanxiufei.cn/gtibvueovt.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yj20258888.top/gtprvkpkuq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhongyouzk.top/gtcvxguemy.html

[M04] 获取当前工作目录
来源：http://hz.zhixingplan.top/gtpdztjbrq.html

Py:   os.getcwd()
来源：http://hz.xziqi.cn/gtnzatfcnb.html

PHP:  getcwd();
来源：http://hz.shuidangran.top/gthehykflc.html

JS:   process.cwd()
来源：http://hz.zhixingplan.top/gtwzpfbmns.html

TS:   process.cwd()
来源：http://hz.jqgfzy.top/gtmlowmcjo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yj202588.top/gtifnqeoje.html

Go:   os.Getwd()
来源：http://hz.zhijiandao.cn/gtajozegap.html

Ruby: Dir.pwd
来源：http://hz.hongshengwenyu.top/gtgvrkcibr.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhoulong.xyz/gtcmdwebnl.html

[M05] 设置退出码
来源：http://hz.sysykeji.top/gtprpzrqnd.html

Py:   sys.exit(1)
来源：http://hz.pycfn.com/gtgphhpmey.html

PHP:  exit(1);
来源：http://hz.tianlin.xyz/gtvtspmbfj.html

JS:   process.exit(1)
来源：http://hz.wangshuangyany.cn/gtlduqfgka.html

TS:   process.exit(1)
来源：http://hz.sxryk.cn/gtjoacozhe.html

Java: System.exit(1)
来源：http://hz.9152youxi.cn/gtzzskyffm.html

Go:   os.Exit(1)
来源：http://hz.sufxvd.cn/gtypxlbkpx.html

Ruby: exit 1
来源：http://hz.nanxinkj.top/gtvuxjteju.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jyoumei.cn/gtrdnsghhk.html

[M06] 向标准错误输出
来源：http://hz.shzxlz.cn/gtnbrhmwel.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xuanzx.com/gtbpbvkwgy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinghuilouyu.cn/gtaykkjhcn.html

JS:   console.error("err")
来源：http://hz.cdnleiting.top/gtyxrkybxo.html

TS:   console.error("err")
来源：http://hz.aizwys.cn/gtkqjowmyx.html

Java: System.err.println("err")
来源：http://hz.redwolf501.top/gtulrtyjml.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hfpthk.cn/gtdgjkcygq.html

Ruby: warn "err"
来源：http://hz.vqdsnc.cn/gtkhfaodwk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xziqi.cn/gtpxmdgloc.html

[M07] 判断是否为主入口
来源：http://hz.sweek.top/gtfdozedsv.html

Py:   if __name__ == "__main__":
来源：http://hz.guannengcc.top/gtyztjeops.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.nanxinkj.top/gtfxrajabe.html

JS:   require.main === module
来源：http://hz.jlsjyb.cn/gtnodqmnyv.html

TS:   require.main === module
来源：http://hz.yj202588.top/gtfpcwmmmr.html

Java: public static void main(String[] args)
来源：http://hz.gzhubu.top/gtqpbbdguh.html

Go:   func main()
来源：http://hz.9152youxi.cn/gtaofvunkr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinyuanbaomall.cn/gtlgunrzji.html

C#:   static void Main(string[] args)
来源：http://hz.cheryme.top/gtburtmkdb.html

[M08] 获取系统与运行时信息
来源：http://hz.chenzaomai.com/gtfplozket.html

Py:   platform.system();  platform.python_version()
来源：http://hz.mhx1999.top/gtphrbhycf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhijiandao.cn/gtyemzxxqq.html

JS:   process.platform;  process.version
来源：http://hz.gzhubu.top/gtchvhlgmn.html

TS:   process.platform;  process.version
来源：http://hz.chenjidiqi.icu/gtukygwfml.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yangfankeji.com/gtavymuhlf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.fengsongda.top/gtmffwmyrh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhijiandao.cn/gtekeoydhk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xingfuxueyuan.xyz/gtxabduzug.html

================================================================================
来源：http://hz.redwolf501.top/gtapxjaczc.html

N. 数据结构与算法
来源：http://hz.jinqigufen.top/gtbjwismas.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtlfjksnaj.html

[N01] 二分查找（有序数组）
来源：http://hz.xuetiantiany.cn/gtvqzyerix.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.cashguo.top/gtrhmtctly.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shuidangran.top/gtouwkypfj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.c1oappe.top/gtxngxgigb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydjk.org.cn/gtbcbpchhq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hywenlv.cn/gttmqhuicg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.tianlin.xyz/gtmchjufge.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.haohaochexian.top/gtzeyexjyz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jqgfzy.top/gtvszrxftu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.meibo888.top/gtsmliftpq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.daxiang520.top/gtpsexxduy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.svipenyu.cn/gtszjptbqv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nwbrower.top/gtujjtewim.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuxming.cn/gtzpvftqsr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.aizwys.cn/gtdytackdp.html

Go:   slices.Sort(arr)
来源：http://hz.zhiwuduotai.top/gtjwzucyjj.html

Ruby: arr.sort
来源：http://hz.yangfankeji.com/gtgsqzjtkb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xuanzx.com/gtpfsnsota.html

[N03] 快速排序（分治示例）
来源：http://hz.shangyingyoupin.top/gtdyukabhv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.9152youxi.cn/gtqqvsbywd.html

PHP:  // 递归实现，或用 usort
来源：http://hz.iojbl.cn/gtzcvssjrj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xziqi.cn/gtwanpmkic.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj202588.top/gtlfahihlu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xuanzx.com/gtmrglgjum.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.0kj1m.cn/gtdbekapnt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gzhubu.top/gttskdkjdn.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhixingplan.top/gtvhijarcp.html

[N04] 斐波那契数列
来源：http://hz.shuidangran.top/gtjaquecxd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.feifeiyinyue.top/gteqmmbkwx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yuxming.cn/gtrbcynbmu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.havefunace.top/gtvonglhfo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xuanzx.com/gtsegpyncz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gzhubu.top/gthfxgyrgt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jyoumei.cn/gtjbfjpwpl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shzxlz.cn/gtgqegqkes.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.guannengcc.top/gtthgpoqvf.html

[N05] 最大公约数
来源：http://hz.ppjwa.cn/gtovlytxbx.html

Py:   math.gcd(a, b)
来源：http://hz.0kj1m.cn/gtputlzcpk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shzxlz.cn/gteaswxrrg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yvedp.cn/gtkvtcilah.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.haohaochexian.top/gtxnkuvmoz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.svipenyu.cn/gtuudywuqu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shzxlz.cn/gtmryockce.html

Ruby: a.gcd(b)
来源：http://hz.dashuyun.cn/gtncjebrlz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhixingplan.top/gthteuysaz.html

[N06] 判断回文字符串
来源：http://hz.shangyingyoupin.top/gtoagptyme.html

Py:   s == s[::-1]
来源：http://hz.daria6918.cn/gtmoepvuxo.html

PHP:  $s === strrev($s);
来源：http://hz.birdmap.top/gtdkcprief.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gtdocqgwhl.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yanxiufei.cn/gtylccvlbc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.daria6918.cn/gtxflougud.html

Go:   // 双指针从两端比较
来源：http://hz.ydjk.org.cn/gtjrgdluad.html

Ruby: s == s.reverse
来源：http://hz.chenjidiqi.icu/gtefesaokw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.guowangkeji.top/gtzqnglcse.html

[N07] 两数之和（返回下标）
来源：http://hz.wangshuangyany.cn/gtgtujwrek.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.chenlongwang.top/gtprjvlthu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.c1oappe.top/gtgacinxcq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nwbrower.top/gtdsefwmmc.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj20258888.top/gtapnihuxu.html

Java: // 手写 HashMap
来源：http://hz.jinqigufen.top/gtolditzwr.html

Go:   // 手写 map[int]int
来源：http://hz.hnqzz.top/gtafqnkirs.html

Ruby: // 手写 Hash
来源：http://hz.nwbrower.top/gtboxbtkoi.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ybcxt.top/gtnxhosmxn.html

[N08] 生成全排列
来源：http://hz.pengpengdd.cyou/gtsrigvfjl.html

Py:   itertools.permutations(arr)
来源：http://hz.sysykeji.top/gtyydtiout.html

PHP:  // 手写递归交换
来源：http://hz.wangdashe.top/gtquuirunx.html

JS:   // 手写回溯递归
来源：http://hz.birdmap.top/gthaijlgpc.html

TS:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtpesekqph.html

Java: // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtpnpnovcn.html

Go:   // 手写回溯递归
来源：http://hz.ydzc1.top/gtthgzxrsw.html

Ruby: arr.permutation.to_a
来源：http://hz.zhoulong.xyz/gtkguysvse.html

C#:   // 手写回溯递归
来源：http://hz.redwolf501.top/gtpfslverj.html

[N09] 栈与队列
来源：http://hz.pengpengdd.cyou/gtvjuwjtxj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhongyouzk.top/gtbnzridhj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.pycfn.com/gtncefijpv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xuanzx.com/gtagfoqqcx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj20258.top/gtvggqbmjo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sysykeji.top/gttcdjnfmg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.guowangkeji.top/gtkwzbxjmu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.pengpengdd.cyou/gtsrlpnufp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zdqjudy.top/gtufzaebij.html

[N10] 链表节点定义
来源：http://hz.sufxvd.cn/gtuugrtrmd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shanyushiyangtech.top/gtolxjdgeo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhijiandao.cn/gtnbtxifyk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.chenzaomai.com/gthlmtqxmx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gaohongyu789.top/gtfkdvrdpe.html

Java: class Node { int v; Node next; }
来源：http://hz.havefunace.top/gtivvtiiqf.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jlsjyb.cn/gtahzuuvar.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jianghu66.top/gtystufrot.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jinghuilouyu.cn/gtquxqwstd.html

[N11] 二叉树中序遍历
来源：http://hz.dianchejie.cn/gtsnlhkvep.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.nanxuanxn.top/gtfqlqampf.html

PHP:  // 手写递归函数
来源：http://hz.guannengcc.top/gtpxcqwsed.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxinkj.top/gtdfxrdwat.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgufenzy.top/gtuvacbgsk.html

Java: // 手写递归
来源：http://hz.nanxinkj.top/gtbtdjxuwc.html

Go:   // 手写递归
来源：http://hz.hywenlv.cn/gtnbwwdpoj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.chenlongwang.top/gtlxnkxmvi.html

C#:   // 手写递归
来源：http://hz.sufxvd.cn/gtwjguntqg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.haohaochexian.top/gtndwwokgz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.redwolf501.top/gtiqfgydbn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yangfankeji.com/gtslijjbtc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ehwqpu.com/gtmasgjdod.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hammf.cn/gtrzvzorkt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhixingplan.top/gtdkelxgxl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xylfe.cn/gtckpfhyml.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hywenlv.cn/gtokrjrxbq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258.top/gtuvoebwju.html

================================================================================
来源：http://hz.316326.xyz/gtacsbttxx.html

O. 并发与异步
来源：http://hz.jinyuanbaomall.cn/gtgykumacf.html

================================================================================
来源：http://hz.zhixingplan.top/gtgombgavy.html

[O01] 启动一个线程
来源：http://hz.sysykeji.top/gtqmmidqfk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.birdmap.top/gtcyztgzhc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.316326.xyz/gtjeuzlvmz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhengqikj.top/gttyfdnrso.html

TS:   // 同 JS
来源：http://hz.fengsongda.top/gthtxhgnel.html

Java: new Thread(() -> f()).start()
来源：http://hz.shanyushiyangtech.top/gtujnnebtv.html

Go:   go f()
来源：http://hz.zhiwuduotai.top/gtoijsttqi.html

Ruby: Thread.new { f }
来源：http://hz.aibaodan.cn/gtnsheacot.html

C#:   Task.Run(() => F());
来源：http://hz.zhaomingkeji.xyz/gtvksnjqdv.html

[O02] 使用线程池
来源：http://hz.cdnleiting.top/gtcrnfzbwv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.chenjidiqi.icu/gtcfextatm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.kuanghao11.cn/gtuakuuomv.html

JS:   // worker_threads 线程池
来源：http://hz.yongpay.top/gtuplzcien.html

TS:   // worker_threads 线程池
来源：http://hz.gaohongyu789.top/gtpdpjebdz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jianghu66.top/gtovwxktvb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.wangdashe.top/gttnngmcmz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jiagoushi.top/gtavdkpssx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xuetiantiany.cn/gtxtxmylik.html

[O03] 加锁保护共享数据
来源：http://hz.ydzc1.top/gtcuxzqinm.html

Py:   with lock: shared += 1
来源：http://hz.shuidangran.top/gtclfjmjnw.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.gaohongyu789.top/gtgqzbwdqt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.tian-w.cn/gtiftjhqgi.html

TS:   // 同 JS
来源：http://hz.yvedp.cn/gtzbfkzsxa.html

Java: synchronized (this) { shared++; }
来源：http://hz.52xcode.cn/gtxmdjpazc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jinqigfzy.top/gtfenvpqoc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ybcxt.top/gtnbcxsbdl.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhongyouzk.top/gtuppivoia.html

[O04] 定义异步函数并等待
来源：http://hz.aizwys.cn/gtlhhsttfa.html

Py:   async def f():⏎    await g()
来源：http://hz.xziqi.cn/gtydchaqme.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ybcxt.top/gtlurwfwxb.html

JS:   async function f() { await g(); }
来源：http://hz.cheryme.top/gtyozmlgfy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.chenzaomai.com/gtnmipaoqe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.guowangkeji.top/gtviveglvy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ehwqpu.com/gtnselxjic.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gaohongyu789.top/gtdrultepw.html

C#:   async Task F() { await G(); }
来源：http://hz.c1oappe.top/gtcxmkvsfz.html

[O05] 并发执行并等待全部完成
来源：http://hz.ybcxt.top/gtvsxdsikt.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinqigufen.top/gtfyrhlzpn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhongyouzk.top/gtcypcnzub.html

JS:   await Promise.all(tasks)
来源：http://hz.quarkkingdee.top/gtiqupqxaf.html

TS:   await Promise.all(tasks)
来源：http://hz.xylfe.cn/gthexeqwlk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yanxiufei.cn/gtbfnpifim.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.snrcjt.cn/gtwuwyictx.html

Ruby: threads.map(&:join)
来源：http://hz.ydzc1.top/gtvfqhrnup.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhongyouzk.top/gtxedzlprk.html

[O06] 使用进程池
来源：http://hz.quarkkingdee.top/gtbbcbhjqb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jianghu66.top/gtorajrjsv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.chenzaomai.com/gtiwpubmbq.html

JS:   // child_process / cluster 模块
来源：http://hz.hongshengwenyu.top/gtcuhysfel.html

TS:   // child_process / cluster 模块
来源：http://hz.xuanzx.com/gteueyqhhp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hongshengwenyu.top/gtjzaqdvmn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hnxiangtu.top/gtfpsfodrk.html

Ruby: // fork 块
来源：http://hz.sxryk.cn/gtdwsksffe.html

C#:   Parallel.For
来源：http://hz.zhiwuduotai.top/gtybqwtnrz.html

================================================================================
来源：http://hz.pycfn.com/gtsphmgipt.html

P. 常用工具函数
来源：http://hz.hammf.cn/gttumafvna.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtkfqqjmbh.html

[P01] 生成 UUID
来源：http://hz.jqgfzy.top/gtglttlfxk.html

Py:   str(uuid.uuid4())
来源：http://hz.ppjwa.cn/gtnoimctvt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zycfv.cn/gtohzdncfd.html

JS:   crypto.randomUUID()
来源：http://hz.yj202588.top/gtuezobqhs.html

TS:   crypto.randomUUID()
来源：http://hz.chenzaomai.com/gtdounzzku.html

Java: UUID.randomUUID().toString()
来源：http://hz.andypj.xyz/gtwpahigaq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj20258.top/gtvhsvwhjr.html

Ruby: SecureRandom.uuid
来源：http://hz.ivvv.top/gtrjmzerqg.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yonumen.top/gthzwteyuc.html

[P02] MD5 / SHA256 摘要
来源：http://hz.gaohongyu789.top/gtqghkxubu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yongpay.top/gtfwqjkxvj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ehwqpu.com/gtariqtgpn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.guannengcc.top/gtucswgsyg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj20258888.top/gtgpemyljg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.chenjidiqi.icu/gtfofgkoib.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gogol.net.cn/gtwbbchxmp.html


<!-- 参考信息 -->