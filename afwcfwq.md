代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gscixldht.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gtslwlieo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gnhelpmar.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/genqrmsdv.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/geafeexhq.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gvzitlkzx.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gxzhynloh.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/grbgxvkur.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gxmecncod.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gljnuynni.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gsqsgznyx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gpmprqrpy.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gagipbmwd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gbzuferyi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/golykocsh.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gfelvnjwg.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/glrnpyhim.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/glzmrwfkx.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gszufoxlz.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/glwmkcpku.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gabujjfkc.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/ghhmnnxnk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gbuijlkfj.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gbqzpdupl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gaoymonzu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gkifioqpx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/giwxftvpu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gmafrrxqu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gxvffiilv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gjkqflczf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbjrpgmze.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/goaguoynw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjkjrrsay.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gndezzout.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/grumooqvb.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gputcihxj.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/getuvzxpe.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gjcwtvuco.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gaaqeitol.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gizpsezfz.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gspxvnyxv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gulfjibek.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gftqooybg.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gpgxogemv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gatqtucwv.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gchcqvdhs.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gpmdpytaz.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gnodoqsiv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/ggvxlyjki.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gvygmtvrj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gxfdreyca.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gznfkojzf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gahcmqkty.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gxlcnjfmf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gbgyhqerh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/ghcffexrh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gelcntapb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/ghfngyjdj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gjhjkrngi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gmhqmswin.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/glktyruuj.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gzelbqtgp.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gphxhapch.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gdirgblzb.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gdlgobori.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gmcyedays.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/geavcarqv.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gewrnvwhu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/ggbwbwzxv.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gdbmksxcd.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gzgiklcxt.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gnlrbextj.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/godbopuyw.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gbjvqbosm.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gqjnvmwwm.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gmoakfssn.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gxrqkcnqc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gkdnfpjuq.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gbgfpdcya.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/guisfidlb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gvdauzmau.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gpcsagheo.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gkiqpzwru.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gsbmnyghd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gsdvvjbpk.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/geisltent.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gvwljmsbe.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/ghbxfjwny.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/ghforxfvw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gpeqgfdjz.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gwjmlelfp.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/ghmgvlnvq.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gnyeenuyk.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gjkvkakis.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gkwysbnrm.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gqwsqodqi.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gzwrxlwfr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gptetmvjh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gwgfinfcq.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gwvbvmqxy.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gwlzinuoa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gcooqxlpj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gqwmfhpbe.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gkpawyexo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gmsjehyfd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkipozjua.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gcshkuwcc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ganfmhocb.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gxnteqjdq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gdvamddsa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gbojgkenf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/glfrwnazh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gszwtbrrj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gsoxczsjm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gtghscmor.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/ggoifpqll.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gtazgqxgf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gcixmrvpz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gpmnwrxul.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/ggfmqajpw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gnyhfqvvv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gpcxebght.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gykedancm.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/garqicbff.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gvyuouuzo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gucxdqnmm.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gvhijeete.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gkgnxccdo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/ghzpvisiu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gkwpecezk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gzbnwjmsm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gflidquhd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gwotpaomn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gfzqfvxlz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/grvccmcuv.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gfnzmkwiz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gnfuoknst.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/glzvapxud.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/ggjfeanny.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gyrvwmnyu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gvmiadmif.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gvnlksfxu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gsvyhghcx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gibzgjpde.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gipybfkdl.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gtsvzyxls.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gufntfamj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gmclmnhet.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gzdlmbyoa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gmsymeqow.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gzceprdrb.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gsswvqktz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gdtddbysf.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gzwqpntfu.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/glptagqqf.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gdgllqnxj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gfcilcdfm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gxxhwtkyt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gyolxecxp.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gmpzexaju.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gogdsxrft.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gkeqmtnuc.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/ggdaclkec.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/giigaxlnu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gwfqnsrim.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gxuellzdg.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gslfimihe.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gynokdgzt.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gyqfygkzb.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gjhigffwo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gdsffjiuj.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gsquyymlp.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/ggztjjubw.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gpkgzuegf.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gtbchjvqe.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/giehizhaf.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gwrjfankp.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/grucseesu.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gwidszdrd.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/goyzaboap.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gpywovczh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/ghjelqhbh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/grdsgvcqh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gdmnziyoj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gkxerdpbe.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gwkirbsic.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gmbamtlbq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gmdxykcqd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gxcobxors.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gvrmhogiu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gpzgkubdk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gcqcqryaa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gdocaeifj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gvvnxukfb.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gpmjovmyi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gbzprocbv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gijzseufe.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gycqlaqms.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gatnwward.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gqlytrajx.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gaktxzzbg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gmbostxxp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gpzqwfmln.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gsovfkwxf.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gnllsqcbe.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gytsvnmhw.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gnhyhowbs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gzlpwiskz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gifgivzvk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gicuxpnsr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gjsrswwyf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gvlpbnjkm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gmlodnonc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gdndkhvwn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gcyhpqybr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gkevbatka.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbamplimx.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gruufznny.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjgarujny.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gvbntgcjl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gihbarset.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gfshgcfzb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gkqlwzkhx.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gyytukxir.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gvcyoaqrk.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gypxqruip.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gypcemxae.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gpakzpqyh.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gzmdyhtle.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/ggjvnnnlt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gxlgnaryz.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gaisegdoz.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gdvlejguu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/ggguyxsmn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/grzhmwinl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gazdrncdy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gtieyvcvj.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gvkqdvkxm.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/grtkutpsh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gutbkvqfr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gfdsqyadc.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gwvcaugdo.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/ggfricbnh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gnwsdkris.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/guuouacvv.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/galqesccg.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gpybtnwqe.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/goutjxhfe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/ghzektozx.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gykhupzgp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gqiuulhna.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gckkswihd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gaxqhgbqq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gaoazjsox.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gryobvzrt.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gxpntaebf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gqdrcaboo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gzymsjkla.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gfrmqgbky.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gntjrhkkd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/ggouhraoj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gzvaqqivz.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gpxypffgr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gkfqyjwii.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gkyduczqb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gcqfyhffe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gwubxofly.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gkksixdju.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gzjlstavp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gbqtoxagg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gxnbrqquo.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gzfmseyif.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gcvssmggf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gukhogkvv.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gyxnxhwsi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtxuxluyl.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gmzuuzkvk.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gamuyedui.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gunurcasl.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gyoxvrsql.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gyfpstlsy.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gssfteril.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gqbysjvjm.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gdxyiyugx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gmphkuehz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gttikmsit.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gtwhywyyn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/gkuaflgbq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/glvenevzw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gvldczawd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/geetrembs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gwkjzuqnp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/glwcjqcxt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/ghflgbcet.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/grdpsidwm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/grjhkyykc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gijnptnga.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/glunmefcq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gdzperbgk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/geyyrzbsv.sHtML


<!-- 参考信息 -->