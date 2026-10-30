代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gnkisbiyf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gfxtuzrgx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/gooryixmg.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gghgdoren.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gegxmgfve.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/ghkzxhliq.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gtjcazjrh.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gbitquxaj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/glcjrjmrj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gbrngffbv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gwzbnwxar.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gppnudfuo.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/glgpsnere.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gkgyshkpb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gffsshlmt.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gfhteggjp.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gbjsetves.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gkigkpljm.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gwlejmlyl.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/ggvjkqchf.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gjnkghzgh.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gjjyrjlup.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gxsdemdqn.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gibjpxrkc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gdnbllzzr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gaqsdmoba.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gvknxzrbl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gzivwvuog.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gvorduhan.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gtzzadnai.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkdfzlrvj.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gveddioau.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzthxcpyq.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gnqwyuvtu.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/ggnpltdfe.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gfhgbqmvy.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gjfcklkjt.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gxfchrici.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gchsizaay.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gfwqpovau.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gwekkxqhg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gjitxcomh.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gpsdawsti.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gqtljiblz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gmhggdbiz.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gmlinozof.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gkjfkeenn.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gmvdznpkg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/geghengof.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gedfkzxnk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gpezfyfwq.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gxqwhzfpr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gzjtxxdwx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gpbylxcid.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gelehcaqd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gwqzgpzrj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gyzvekzpp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gqcycvorn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/ggyebcwci.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gexvmoehc.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/guhwknrur.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gjaoukxqw.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/ghsfznmtx.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gmnpjqabt.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/guhzcerfz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gepxfdzmi.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gdzulyzkn.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gcbxjlifl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gqbbiamto.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gbrlingpj.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/glhzdplwu.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/ghkbwmmth.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gnrydjlfu.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gvfthccek.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gyxndyzlg.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gplvfqrik.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gjnclsjgp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gsownwnbf.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gkipjhnov.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gtvwazoan.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gruffqiou.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/ggiqxpozd.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gavzogzvl.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gpqbaejnq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gcltzlifh.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gvdjhvlhe.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gfuvgrffp.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gtqdhsioc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gnrlsqpxo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gtligbiip.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/goojwkkar.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gajzkfvwj.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/guseipswm.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gshigfkvb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gcctjkalg.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gnetzhulv.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gbtbrxxby.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gnaaokmue.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gwbpuucnx.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gvooicnsy.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/ghhusdfgg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gaxnwjtud.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gagmhzype.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gzippftzp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/givfcdtpu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqjeamajm.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gwgggshrk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghtfwnwvk.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gpskulfee.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gmmntjnlu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/guhhyktxq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gknuzfkmr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gwoliptyw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gblxiplxh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/ghycgxbuo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/ggwmfpxqu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gampqyktn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gojifsfiu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gakxjnxcl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gaejsmavk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/grgdgcozu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gnuqdvdpz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/geyuswajv.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gapbouexv.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gvdneoqhv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gqwnuczii.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gzgwijngj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/ghiydolel.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/ghltoswbc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gjvoegjir.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gvvshuazu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/grwbnlxyz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gwcvqkvno.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/geggeoyjg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/guhwvxnxm.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gykxppaqe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gsfwldfuh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gwwaiqcab.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gbozienpx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gbngkscjn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/ggajmktbt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gjtnkyird.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gzqnyrhyd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/getnrziox.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gubdpqmyo.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gjgyvbskq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gozdzqfgb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtcvhwugs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gaavutdbt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gyesgcbli.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gqkbatorf.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gttaxrylk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/giybymnsf.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gwfzcfbmh.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gqummidiy.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gidvwkzta.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gvllcotbn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/ggxjskpxx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gtzqhytgx.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gnavzewhv.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gbdgfqylo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gvssamgbl.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gktgoqtyy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gcjcgpjte.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gwcaapioa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gxrgfdqag.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gcjrbebfu.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/giqsgblud.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gpvrtduch.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gejvuzyvk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/giiuuiudx.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gypespldw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gbkainoav.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gcihtynum.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gskaddyqb.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gundeaixw.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gwdsfaemq.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gknletgyv.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gozjvyosd.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gwnmqqzet.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gebkwagvs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gvpjkfwql.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gqlcuazph.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gehdjdled.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gijtaaxzx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/glztxxpjm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/ghogbxtuq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gfmhtodfr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gromvmwca.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gryysegjt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gdmdyfmgl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/ghehbkxwa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gmzejpxdm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gksylpxho.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/gcmgnxikj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gxwdrsjgu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gpboczpzk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gijrpbzdk.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gagurjvti.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gjzqhltuo.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gfkayssua.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gxzqinbrf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gxhicxdku.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gbvitnnva.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gcesjtkpd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/glolgdfby.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gbdjwzvjg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gkmpzkzji.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gprhbmfav.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gppgrskbv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gvwwzhpjk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/guitsznil.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gbfvarxap.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gpuqpxbqg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gjgizfyxq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gmmdnzsqu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzvaeuurm.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gjbaepczd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/giyocsdel.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gxaqviekf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gdhwyvqce.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gjlqlflxr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/goqobrebt.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gncpydqpm.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gvcxjiulc.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gcjqdwvlj.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gbbokbmuw.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gwlbzwbao.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gituzrqqf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gusjcbzcz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/goxyqmqhq.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/giulvhhro.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/glsazljqh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gqgkvcjkb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/guteogxsd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gpqxvztlz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gldvquyuu.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gxattaina.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gvsfkqcmg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gyykpykie.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gkbiqokhx.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gjxjajdar.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gutoqaitw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gzaolkqxr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gwsffvbny.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gcbhliwgk.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gvdvqrswk.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gtpjaltiu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gqmpdirnl.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gmguyrayh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gxxqhzskv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gqqiqzcnj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gwgbqutnu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gdwcrbqjk.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gdtnazhtq.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gpjsnmnlu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/glxbwvwpz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gbteiuybi.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gyabjjmsn.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gurgurfqr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gwzdubmkb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gdzprpvsq.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gflbekchp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gcslqorgg.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gwbibgtou.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/ghgllepqa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/geffirzkr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gslpkggmk.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gedcwyktf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gucdqkmjh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gdalnqryb.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gonqzphyp.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gttmneqkt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdapxnxki.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gnwsuinag.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gblyalyrq.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gjtguadjg.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gqodzjfsm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gtqfgbxbz.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gwxudkkiy.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/genzupnli.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gorxwlrnk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gbmxjewid.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gzfhqhbph.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gncssusft.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gyfzgwgpq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gbwotfdhf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gcsloskgv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/ggqvaphbk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gvyavrztk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/glxalggka.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gzlrpfxgh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/genjgcupp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gpzvcwpys.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gtdbkkqti.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gdkcfjbfh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gqpcdkafh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gpqcoqeqa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/ghyprwdkv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gvepadram.sHtML


<!-- 参考信息 -->