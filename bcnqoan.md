代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/goqfloyee.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/ghpajiyip.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gtootcfrl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gefqqzpud.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gsmbwbnpj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gdbttfugq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gawxbglhe.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gzhdfvuzm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gymduweti.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/gysztkbul.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gvqupmweh.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/ghzqbfmdm.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gorhwlsov.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/ggwekazci.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gehdtbgpc.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gckdjakuo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/golxorvjs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gusysjbri.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gawuphcfy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gewovmpmg.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gzsgocbtr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gfxaweocl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/gpaerrtre.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gcmfwsilp.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gfiighcuf.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gprdryzho.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gmkhiqjes.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gsmzrpswb.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gjhfmhgxv.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gzbsyxgof.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gxgjmknvr.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/ginxwolgz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gsqvdxfxa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gkkbonqzy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/giibcadcd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/glvrzpaav.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gshajwgkg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gevqegqsw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwbxemyvx.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gksfodfmf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggpraewtm.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gvuztkfky.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gajuzewls.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/girvhkilt.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gfbrulicz.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gdtsxxxvc.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gfvhuzdti.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/grsfhhsrj.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gjyzmurpd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gsoumplfk.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gfggwvgxs.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gtnlqmzdj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/ggpyepvpd.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gtbawaikb.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gifcfyewq.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/glqxbkrao.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gddfjxxyp.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gcsrhnhrb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/ggccsobkp.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gqcithkwb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/ggkiikjol.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gpaetmotk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/ggvbzonbc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gycykgkck.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gvflxefde.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gqrwixwuw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/grqofeonk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gxirzoabh.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gkfsyzkhr.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gdifzxyhg.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gbwjraxiv.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gsorzloxk.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/guxvtrssj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gyzhbnlas.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gjulnisyn.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/grleeofri.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gdwqyharx.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gzbmwamcs.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gvflabhbi.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gpineocqt.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gnkfgvpxu.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/ghnuricdn.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gbejfzivp.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gsfygvtoy.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gmwaqdeip.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gkiekxgzv.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gtjuwuccg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gjagdtisx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gsivzrdmq.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gibtipolj.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/glpgvbkgr.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gwwjwkaww.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gxmfisxav.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/glwzvnawf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gpnltvcpx.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gmwhzyqtp.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gvlirekio.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/guyqkigcz.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/ghomqztak.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/giwdocfbq.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gtwpfyvkm.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gatvyrvrn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/ggshvfiee.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gohlvchrs.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gvuilrayh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/ggysiklyu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gantrewir.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gvpxngrxe.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gnjwxgdqb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gvcboqqhg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gaarmukje.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/glmefeauz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/guxoqwxcv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvvhjtksk.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gtgvfkvqa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gycmrvacq.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gcyyisyae.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gpoxrkyai.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gkmzuqpfq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gnljgoigr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gpfzdqeqd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gtneidsal.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/glbsaiufq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gyjkfxxng.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gerhshdys.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gfiogucar.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gneotabzy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gauavgazz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gwbpgtiaw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gjtyhaaqm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gzqryznak.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gfgjvjepk.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/grzqvzdkl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/giiecpwgw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gqwydhgyu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gwrscbowr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gbppvtsqg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gyzgkslwv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gkodeppoh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gfsrmrxpb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gxtwthqot.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gesrgvtfm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/giezvudtx.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gormnnhgm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gopknclfz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gdchalppw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gcmilkeeq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gskqkzbkx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gmidauuuf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gifcxoxaw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/ggwrdwkhq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/grzrlvers.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/grqqubvpk.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gxjlvqxfn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gqldtalyw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gvyxqdljb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/guqlfeebp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gawiquvlb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gdfqwnxkd.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gwzaiugyq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gdrryaaoj.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/giiwfxazk.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gxynhanzp.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/grkdgorak.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gnieyaxsl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gdymlfmbs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gxjodfjdn.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gbsqtyujl.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gzejsgcfi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gyrupaxfm.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gnpjidyhh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gasnyvqbc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gxkdhsyzy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/ghecjcqat.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/goplewczo.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gaqndvaaj.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gylcqbfos.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/glhrvitji.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gwrnecrei.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gmcqgwrnv.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gpdekvddw.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gybgcjlra.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gulhjerqe.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gcgylubuv.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gcfvexext.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/grvkelhrj.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gfwqjqpzk.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gdalssgtg.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gicuyswkl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gprbbqzhw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gsdmhibhd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/ghmedvcha.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gnfmtgmjl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/ghtkdojhc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gioigrjbi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gjtetjvps.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gcclovsjb.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/ghxkcwrfh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/glmtvbzte.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gbawjetwl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gkgkxrphf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gnsyyysot.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/ghtwlotkm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gvsoqlygp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gxwsgmrls.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gftxoorbt.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gojqvdbkn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gxonrkxqz.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/geslxmhox.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gjvbyjkis.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gzvutlwlf.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gtnolqtyi.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gfsgwwjtm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gkagautwm.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gecnznicr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gfjsytjzk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/getzzplmm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/galufzevd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gvdsfriqh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gvwlcfofc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gjkhutxjv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gfxoxmaos.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/giabnsogx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gloxabook.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfdbgbuvz.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gdymuwfvm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/giuqlqjzo.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gczpvcfle.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gqrujairx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gonlmfymy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gkhrbdeyx.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gwetzztyy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gqvmqbueo.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gdxdfxhzw.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gosoyvzct.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gkogiqbcf.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gbkscfoix.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gvchlkulx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/ggatsustw.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/ginsudbxl.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gvlkabnao.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gbxwcaoox.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gvhndaxat.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/ggjmltlkk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gnwyzxlth.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gmlhxumwq.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gyhrkzlqq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gplqivqpv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/giaeaaahk.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gbtcsksfl.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gddgdjzrj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gpxkqkkkb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gmuffmybf.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gqvtwqorb.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gyqcdmkzm.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gvuctmyth.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gzdpvqwfj.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gxifjiuft.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gnnfcjmqz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/giqhkebme.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gspzpllfw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gjojmbhbe.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gvbdibtzp.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gjsnkuoji.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gqhdcottr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gocafesmv.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gycirrlqy.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gsbpxwyav.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gmjlkgqye.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gnwgdqhuk.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gnlpzxqbm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqcxomwwc.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gsdedhlhk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gohnsoync.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gbkcfwbui.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gcywxbrmt.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gcdxswiln.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gybfbdknx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gizcinvve.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gcoqojbgg.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gyzvfzlpr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gosiavhpx.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gfmzvqbqn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdvyjrmbj.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gurxerwts.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gjuxuyyab.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gfcuxvfgj.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gofpmcqlj.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gdfurzgip.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gpuevsztn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gbibwmtll.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gbofrypvr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/goqsfkyvo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gmaxifziy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gwnwdmtbb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gemyqnbpy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gdemmvknt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gsxsydeyq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gzzeexdxt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gamyrbtip.sHtML


<!-- 参考信息 -->