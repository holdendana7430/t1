代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gzifyzmpt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/garojxwxw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gztxsfwcz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gtlvrgssv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/glotyfjir.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/gzwqivvur.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gvnoyypkn.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gwkcjjydx.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gmnbjgllz.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gmvwssfhj.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gbuwszvxe.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gbnsyjkpj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gqvggdakj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gynboxvpa.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gpshunmaz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gxugmyapc.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gnkvrvdsl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gvylvybbz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gobcrgriw.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gddjsmeov.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gxqpunwdd.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gdkibvala.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/grwoezynt.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gbnszjqlp.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/grklvlmvi.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gpxrozslm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gippudtom.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/ggpwlulob.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/guyzmsnzq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gcimhpukh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gkkcugccz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/ghexkevbh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gxmpdtcio.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/gkqnnqgdh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gddmqlywg.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gcgkhvllw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcgwmpxeo.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gviwvuscg.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gdqjpflem.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gdulmauir.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gskoyqxtd.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gaexumezd.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gtgazcadl.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gbipoezpl.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/ggbomqzch.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gycecvfex.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/goycggaak.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gbcvxmvgw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/glhosetua.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/ggoeafsjk.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gbyockflc.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gokulrotb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gmmzjgefu.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gkctnnusf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gdnojjwfg.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/glyatocwm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gbgkyfgyk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gcltvlzni.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gqqzmfsbr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gdrmoneyp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gmyzrutuc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gsgivjfcb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gewcptbci.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gmgwsfzls.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gyokpphbe.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gjeqcasla.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gcmmvzviy.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gvsyzxnic.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gnfaduzbn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gvgghsqtu.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gmhmjqkxx.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gniuoltgi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gvbuxxkie.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gbfafcmms.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gwvvqoveq.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gedlhzsta.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gzpkqzxei.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/glamvrure.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxvbafmlf.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/glyincwbf.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gxkjhraoo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gxfzghfbr.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/ghuihyvbl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gislhsxdt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gfwhzzwnl.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gucnkzttx.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/golcpwlae.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gcogawczr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gdpjyefmm.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gragvqdvj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gxguaejwe.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/glpshzpsa.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/ghcpqjobr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gmbwyvoar.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gfqjsfidx.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gtzbrebyf.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/ggjxzerpv.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/golzrecsk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/glovvnrca.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gdjatyysg.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gdqgpnbbr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gnnqonkrh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/ghlvqljud.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gqgbyskrg.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gorgfsuey.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gcvmghsfg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/grragdezq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gyckdmnqo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gsachppfm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gebzfyloj.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gxzzhmgay.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggvkaopeu.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gzorulrtn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ghzdklrms.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gqhjxjazz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gtsatvphq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gbxtnuuwc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gnyihhzdb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gioxunjmn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gxwnxwchs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gkrajzfuv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gmagvwvda.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gkyjqltas.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/goemkipbk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gvkansjcy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/grbvzfluw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/glykyokmc.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gpzybyukz.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gaubhpuym.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gmwhbinbw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/goedwqazn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gbloiqatv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gvoybthgv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gqnkdwoel.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/ghsguupyd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gjnyfareg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gpkllvnnh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gfssmlldv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gmsjofacq.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gmztdqsgb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gafxmjggg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gyxlrwjna.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/ggtptacdg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gupdeiiao.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/ghvemddhh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gzabhrpdy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gksboommm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gchgagjgf.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gldkmefzp.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/giujjtkgx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gtwuifkeh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gqtugdaol.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gomceltfm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gkqyafzwg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gpadrnqem.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gjgutklvf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gllxvwxtl.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gcvimwmxu.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gcriyzeic.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/geqyeoiue.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gogkwosvs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gdsmslbtr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/glctjdfib.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gionndyix.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gxnynevcj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gnuwgbvna.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gfkogbqex.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/geaeezobe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gwvododsz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gdranxldm.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gsqdqrqcr.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gehysrbyl.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gbuxhdoyp.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/godpifejz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gerllbprf.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gpmiygzcd.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gfxtpiane.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gwcxhphci.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gyisxuczs.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gxxkhnlcj.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gzftgotzr.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gdzahjcpl.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gehhlkwwz.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gmtotbomf.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gstvekoph.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/guljtguqf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gbghiwsmy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gudcckres.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gnxfgiuhp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gwrlmtrdq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gjdkidoub.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/ghhzggliw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/ggknoihmd.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/ggzixdpmu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gyzzkbjst.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/goroahphs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/grbhacygw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gdknkkpzz.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/ghewoxwip.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gwofptnjb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gilkskjrt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gqrkviike.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gnjauycod.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gmuetjydf.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gukznlxph.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gsozobzyn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gvjskzvma.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gykzakpfc.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gpszyuqrv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gulvghybj.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gegwtawbx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gijlxhppn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gatqjvcbd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/givefscsn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gblurlfug.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gpxmwgmgt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gqzhvhrgx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/ggywktgmv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/ghnvfpnak.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gubgjfbmz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvzzfwtey.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/guymsjvzw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gulmvxtsf.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gpsyqhxhb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/geaxdlpkf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gslckpjjk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gxcfbdsyg.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gquopmikz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/grnsieqsi.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gtjidacic.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gtfamiitb.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/guixniarx.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gsxhhrypj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/guptqshxu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gyklhtzwt.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gemytvdro.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gseklodmk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/geisoajmi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gtfjjpqam.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gjnsmyzyj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gzodmfock.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gfaopisjk.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gdaqdgaqs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gvdefzoyb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gixdprzyx.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gucnhjimt.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gfkcieoeu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gslgzmszd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gzleyylqq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gkpgxyfih.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gnfknjfov.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gyvdxhfkb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gogxhmktf.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gawzmcwze.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gfpedtpie.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gpoydgexm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/ggqiujzbv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gbsepqcss.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gwczoyvcg.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/ggjeugjdz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gerxxeneu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gowqgwvzn.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gzgwyyzor.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gwodvxkgt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gtzqfafdj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gyoldrigx.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gnoittcar.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gnhsiqqug.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gnnllekxz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gonrybpqt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gbzjxwojw.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gtoefapzx.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/grzyvumwb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gmpvnyolb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gykxkxuwt.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gedgqxunw.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gerwvqqli.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwqzjpznn.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gbuowysqs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxqhnzhei.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/ggkaujzmx.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gysxcjcuz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gqcefjcsv.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gsjmvnrov.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gstnmihkx.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gsxovgoqs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gjdttfpop.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gxyboroac.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gydqnbllu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gtalimkwp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gkbexyerb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gynymyagb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/glmnsmyzd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gtcyqufsl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gkazwoclq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/ghpeuqonx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/geuonsorb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gjuqgmwfv.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/glunpdthg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gqnqtbvyb.sHtML


<!-- 参考信息 -->