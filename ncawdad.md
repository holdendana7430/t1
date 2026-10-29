代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/ghqkgtncn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gsvwgxirv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gubxsoslf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gkgbrmnuk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/ghzccsgvn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/ghzlriqwv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gbubjwwsd.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/gnwerubrz.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gleocchci.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/gmuxdaoua.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gwvgkhoea.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gblmewxbv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gjrryitps.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gcskinzwe.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/goxrlrotm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gkyqzwrwf.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gbfcnwyzd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gexkfvloj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/gboqobwgp.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gcqahnbgx.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gqjiegvoe.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gxdqnbbta.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/ghqdvnvge.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gkhvxkbhw.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gdfojsuqg.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/glwlcgzna.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/geqjetolj.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/godckgtbw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gghpvihwa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gvrxpqghh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gzuexwxef.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gtylddvzh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gotphojya.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/ghljfauts.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvahowgpk.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gttaeyxjv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guykcpnlo.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gbdbaawqn.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/guzhhftfy.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gxxzkrcnm.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gcakhgyrd.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gpmcfgcwx.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/ggjqtuiyv.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gcgrrrdtl.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gsphlkoap.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gmkezsgoz.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gellbetaf.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gbyqvrbue.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gcinfwxgq.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gjkdrwfjp.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gixszcxfn.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/ghrchxmzd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gituwnxpi.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gwduuraqr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/guilkzuqd.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gqicxipxd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gkhbeabnm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gcwqxhlsx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gquykbdyr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gdaoumely.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gztoidsua.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gwzfsvvvf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gdgertddt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gnhaqhvht.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gfjzmcbdr.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gqmvlhxne.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gdzxvokfh.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gmbhckggv.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/goscfcwbu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/giojnrzzv.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gjfxisdeg.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gbhdhazfz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/glxgddrks.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/grpzzirgx.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gezcgfjzd.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gifeatqpn.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gwxiaglyg.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gkzhorvhj.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gjbsmkoaq.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gkobrrtai.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gjpqdyktc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gvqqlsqoy.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/grpjrxjpl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gvnohzlvl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gdjtjhkxl.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gprcbfzkc.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gechoyqjw.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/glggrpqar.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gprirbize.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gfjevqajy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gosxwzwty.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gvgeptfof.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gvjvizwnl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gfrtxxeuu.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/glfqxrowz.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/glathlhwz.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/ggtfzfllm.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gmjoddnrr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gozbqnodt.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gibypscxu.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gbalxexrf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/giitfulle.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gkquxqase.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gqywtcnbq.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gjpiwxadg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gmmwyhkfa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/guflytmqk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gulmrkaaw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gksmmougq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggvucsoth.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gtncavieu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtjtcdfad.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gwpsdkrwe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/glndiscqy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gfyybejeg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gnufbppzy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/ghfcyylaa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/ginnbeqkx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gjqivjiwa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/goonoqigi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/girlmimui.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gpdzvoozt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/geiakxmsi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/ghgsufjyr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gmgtybuzz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gmznlqtzl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/grwiqinoa.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gtbzthuso.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gixrcjlwb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gqblecdtn.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/geecwgnrv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gytdsvfxd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/glokhwjxa.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gfikqpynv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gxhkaqfxg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gmkmwysga.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gipepgqfb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gaenzdeue.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gzgjspfpq.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gzgchjbpt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gwsuasznu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/goqncnent.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gjnfaavha.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gqibzcext.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gopoakjyx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/grhdcarpm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/glhocbhaq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gxfosfskc.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/ghhgzfdbn.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gyzgesxiv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/ghlwezrom.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/ghfjywvex.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gsbjnewdk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gnkbrtzry.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gkspipvld.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gvtocqkns.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gqtpchioc.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/guipstxeb.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gkgfrnyuu.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gckqyhjdz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gdhuxgaxg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gdqeoefse.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gsltbmvst.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gffekmlhk.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gdhexyfhs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/glwvxmmuh.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gjrgxumur.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/ghduqindv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gzwdjpcot.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/ghxrbouqg.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gewxcyipm.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gemwsbddc.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gccaagxqx.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gcygtrjeo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gqszukavu.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gknbwivri.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzfkbxfab.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gkdxgsswa.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/groggusch.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gjqneedmv.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gspbaakab.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gxxtxnwmc.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gzdxpnsjn.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gslnaqrit.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gnphuvihl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gidesdeqg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gbnhvacon.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/giwixooun.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gzjowsbjm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gztmvogym.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/ghxdrrloz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gnfrrcwvx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gzxwatesm.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gspxzdedk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gxuhenbvy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gqdtfrmtb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gdtmchtye.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/guunvtasn.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkgbaclxb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gakjoekdx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gofnghoya.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpkosxaoa.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gwhecsjqa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gbazgyinq.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gbbkuzvmb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gykqpdvyj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/goposfvml.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gacimrsff.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gwuhfqhxv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gkgnqeszq.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/glmufdbeu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/glxsnvwuf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gnskwsizd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gdujxwvcv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gnnqnloaw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gzibharfv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gmpleswed.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/glmsbzsij.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gunlwmzbq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gjfoopvjr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbrwjxdvg.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/grcxstkuo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gucinbrls.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gofhihzdp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gsrfwmvre.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gdebsscmv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gdqvhlyzq.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gcpjlfcpk.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gcdjohlxo.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gydxcqgdv.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gsucegpom.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/ggfaeuecm.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gmrwhhzlh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gywxqyhqo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gjzahbntg.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gddrwsphr.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/grxzpktkp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gkfcjndzu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gsbpiowwn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gloihkiju.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gltjhvxvg.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gufcjjlgi.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gqfgyrkzc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gefvwqxgr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gcmbxzhzw.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gzicsvnfy.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gpayxjdkd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gcptyvthd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gvnxbsvcg.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gcglowmog.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/ghkiucjdi.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gaolhkarv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gvqgtjajd.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gvxdwpzpl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gijpznmep.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gmsuawrzk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gamuobhet.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gwwoqwtxk.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gmrcukphq.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gvztodbqy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gvvstjger.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gqxdndhqc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gqwrqbkoj.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gchbsbizo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/grlyxshyu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gkytvyfqz.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gwabzoyhq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gwzsupyav.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/goreupcnl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gyryqubnk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/goycpevmi.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gikmpcllf.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/goulzvjdb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gounyttmt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gmrnejeuz.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/glekbjdzm.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gpabtcfri.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grownckkj.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gpkdcxjik.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guygylill.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gghhxgenm.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gpgvxhfrh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gtmspqzag.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/giozctjio.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gtxnntgba.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gmhndryls.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gsfplotgg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gqcslrvze.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gvphpqgya.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gmsdeqhav.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gnrzzqyxq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gbvkttnjd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gkimryhok.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gznlljves.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gxpaiqsuj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gbplwudtf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gdbtqdfcq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gnnvcuvyh.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gfryxxlpy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/grlkrbjcw.sHtML


<!-- 参考信息 -->