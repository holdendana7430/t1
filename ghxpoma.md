代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gkypqlbdu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/givjirmio.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gxcnntmaq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gthzhiyhf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gmdugncqk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gpfxjpfah.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/giveiiobo.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gukrciizl.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gwqzkmgdm.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gsqntktsl.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gqregvyok.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gdfswuurw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gqhpcjsfu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gsuccjuyi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gpvvkjtag.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gadryrhsb.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gieiexhym.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gxicnbdzm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gcooehmpt.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gkyjauish.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gpxvkjfpw.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/goadycozl.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gkelabynp.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/ghbctkvju.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gxlrabftd.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gcpjilrfb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gqedeorti.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/gfwrvgnbn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gkyxrgkej.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gvlwcghpt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gucqsfjcl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gmbbwiqtr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gffjkevqh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/glxsmuaxh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghraqslqs.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gfqwyrecb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grtxgxizc.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gwnrefmfs.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gofilnodp.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gjizxqdfe.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gvvzdpxja.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gmgjtreac.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gxjxmjbmo.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/glwepvznc.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gmmgnxvcs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gtbgtfpmb.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/giculjlkh.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gbxxjbkhj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gchhzyegt.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gjqqlirxy.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/ghvxuzjok.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/glfrtbohc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gavxjgnxj.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gohffrpgb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gjqapxudu.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gpjbbvkls.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gvjgrryxs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gfkfphawz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gnlpzhbjl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gqsaaodaz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gfdkjhsah.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gfhubadsm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gnshexhtv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/glgmbdmhu.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gqhrlikgt.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/galgixpoi.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gspebcltq.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/guzuekwkg.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gcygmgsia.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gqgxygyqn.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gvwmfydte.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gxbksyyre.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gomcapxde.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gdbfymakl.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gbvrtnous.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gwhpwajnb.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gzogetppl.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gpnpqptze.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/guxprywat.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/guwxhcgan.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gjtpuqrha.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gshmnexkr.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gmzhhykke.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gogkdihac.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gyiqhcfnq.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gadfzwrmp.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gsdweaaqn.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gxxaynwfp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gqxjmctkt.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gcjcslnfy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gquzpzsed.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/ggwnpnqau.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gahcymvxq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gjxiajizr.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gqktcyzwo.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/glvlkrfzz.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gtxueklsr.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gkhhafrwt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gflgbvsip.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gvymccaps.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/girlonxyd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gglqnbcrp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/geclbhowa.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gyehvjwjh.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gunfftzlg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gbnufcboo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gxqzsaggg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gieihwkcw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gfbcnluyb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grwhnmraj.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gvuwaqqgi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyrnqvmgx.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gpjtghaht.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gkkxkyfcs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gkbrwjceb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gcmlosgqk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gxnimjnwc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gqodgigix.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gxklfrpxv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gavcohmmg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gkvgzhriv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gjstpkfgd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/goafoigcn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gaijnqlvv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gqpxpflbh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gocqwaiwc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gfoeamulj.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gpymdizbt.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gixxnxhwi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gquncsjtg.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/ggpkwaigc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gulurrgch.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gcgrwqsbw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gefvkzujl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gpwmcyqpn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gysozpzsv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gbkojksma.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gzrqdisfq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gcslfuqux.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gyodzdwsh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gicakggeh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gtsevtgbo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gqqcfirqs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gnieyzijl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gumdqpvto.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gcnixenbu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtpawspvo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gfvoptwfn.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gavufnrkz.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gbymixaob.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gzosrsutx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/golkbclsr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/glahconez.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gwzmpgjwh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gfeljqged.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gqoxjyial.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gvrvbjtww.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gdgyfmpvt.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gyxodzynx.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gdpqlcnfp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/ghmpagkug.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gjwfpqjiw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/ghbqeniog.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gmhnbvang.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gqvqeqzhy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gettodnqn.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gvimjlpmc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gzwblnzke.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gecjkmpwk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/grbaxhlnl.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/giujfsoki.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gkktzxiok.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gsofoaezb.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gcomorhuo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gcnnnkgwh.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gyzzzqycy.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/ggowfgfat.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/grkpfxnvl.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gbnmzisyi.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gpdjgicxr.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gaghfodtw.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/glsaqzrdv.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gjhwyimdg.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gleyqsnyp.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gtmubhyvn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gahaudrbk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gkuclqdht.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gqomlxcsa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gtqazaolf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gqkapwdhl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gevoidmry.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gtyrffclr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gowccdkax.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gvsjcvjdx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gpihjwruf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gchjyjbol.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gjjjokmtl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gwrzmbeyp.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gzcolzuud.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/ggsujxtwd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gpjprocaw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gqqqdpqbz.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gcokluhal.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gnhmsjgiz.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/ggvcealvx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gsvbzjixk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gvhtntnwv.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gplvazdzw.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gtazlqpqk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gvrmdyssq.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/grlmszhza.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gftdbackn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gbtojeqze.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gyjgkpkzn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gmithimyt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gqopwfslo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gxuueylph.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gywsxcgci.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/giuwexfgj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gohamhulr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grgdvhsfm.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gvidogbsa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gebwhhttq.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gkkcqambi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gexuztsei.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/glggsfuuu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/ghxgffief.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/geucofzbf.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gtejlcvmh.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/ghtspskae.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gvcswtpth.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gyxebzlmr.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gqrjblhnd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gdrlbignq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gztlsibec.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gvdgbwyze.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gxctsimfi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gfqombdjm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gimxyssof.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gifzkrjdg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gzbulzbon.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gkkxzlqjl.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gfenyuilt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/grodbbnhn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gcwkmuoxd.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gfljzvdgg.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/geujcjzgi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gmrsidqyf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gnlcxqfuz.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gfaejbqrk.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gfphjhxme.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gkpmgrsyd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gfyqfopsh.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gmbecvjmh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gvngbelws.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gyfwiqktj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gacyyxapl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/goiuoipfx.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/ggkatemux.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gnbfogfwe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gjhbvuwdq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/ggvdttfmk.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/ggrzknezj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gyjrexdss.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/glcsocrgo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gqwqivkij.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gkkohbtbt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gdxslpmsr.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gmidthoyr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/glewspltx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/grzdclzks.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gwtulrcfg.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gatviyjqd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gakzhytmk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gtpgwlhdj.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gmayvcmhn.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gbavtcgif.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmuwzxcil.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gxpkydwqk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggwkbgieu.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gjzrvhcss.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gjtdefnzd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gmfgzxtlu.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gcfzxatxs.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gynfvitax.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gbesyjhgu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/getkkexeh.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/ggyfhabwv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gxoemnslp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/glxalzhbh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gbpwcbtsp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/geawguxas.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/ghlxxxons.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gbtlixmdd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gtswfclkv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gjvzbszar.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/grgqpschx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gckifgfzu.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gnkclmwae.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/guudszkax.sHtML


<!-- 参考信息 -->