代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/ghxgbkcss.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gkhshzaem.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gxjtirjap.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gquwosdtb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gzvlcocgx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gzccfzfjo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gnlygjktl.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gynqyzbyd.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/ggpdzajfc.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gppynbnkx.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/glnoxvqzu.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gvnhwyqsv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gekfhdgqh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gpcumvdsw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gkcqfvlxl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/grxmwflyf.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gorzcpves.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/goeffbloj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gjynvewnx.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/ggxwoxrui.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gywsvlfin.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gfrfcadqm.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gzzhdukkz.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gsjlazunj.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gzacrjiol.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gegqbicip.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gdquuxvyn.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gzgogyecg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gerhenmro.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gavnmmpzn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gwaejqqhr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gergjtprr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gwcpuyqnl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gayeincnx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gozdngyqm.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/glkbybftw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmxnyeiao.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gzmlddbrl.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gzlyatpdu.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gkdcuqcbe.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gdbopjldv.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gwejetrep.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gefcpnqvu.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gdrgpsbym.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gjctwkcxl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gsuyxqjkx.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gzfvkappq.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gvxxuykfv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gbowkgoil.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gutqsdegt.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gmiqalodn.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/ghmvubmwb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gagauvxbt.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gchcamsut.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gkpcwyfhg.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gatjcbjbv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gjmkmpmzc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gjwqfnupp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gnukrdlqe.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gauuigkre.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gshkdamtm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gacovuosp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/giflexsoy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gcoexzmyb.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/ggfenfabu.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gkrtxajoi.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gkckmkbsp.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gdjxfspqx.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gbbhzfyrv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/grghmuqsm.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gatyizulh.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gunjosiaj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gxinirvnz.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gqkhvouzf.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gjlsojcaa.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gdntzjcab.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gyumouydc.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gkppzyosb.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gkgdumzsl.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gzmuwetho.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gfndtqeza.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gwadxawln.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gjhozpdkg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gqbhntcyo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/ghirdglyf.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/genoclgan.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gunghlvxj.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gbsxudlzi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gruzdhfqc.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gaxstwtec.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gvudnonsd.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gewqdaaew.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gjpjqqqrk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/goxvvfpcu.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/ghaxwxdhm.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gtxfrvltt.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gonawcshs.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/glqreqmej.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gamoosxsl.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gqptwxaak.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gbljcrpij.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gazekcyqb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/ghibewjkv.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/ghrbqqnyj.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gnqresuks.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gijxzvohx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gfsytzxjz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/glcejrljm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/godedgdti.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grqweeyms.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gitpmiazv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggcvesacs.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/glcspicjb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gmvdhgkke.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gqxmdbhrf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gwpdauzur.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gjuutxnyx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gppuwtlzi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gxmdtojdi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gklronesz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/grstktyws.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gonbbizbf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gcfhkhned.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gsfiffyih.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gdmnveqoj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gvdpvbqzc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gqrjjpewy.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gfdqqonjw.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gbcpluezy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gxbdagmon.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gnqqfwwew.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/ggdaklcij.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gzchpsufe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/goxvnjcvo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/ggdvrwihy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gkgpupsog.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gjwqcbzpy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gfyteyzaq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/grllgxtro.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/glyzgqnkk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtxkueafy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/glkfluuaf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gmiwstdqw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gutlcdbha.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gvxyvieap.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/godbtcvso.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gawpmvwlf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gbpbzzhfk.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gikkzlzhv.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gyvjmfmne.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/ghdqqxvwh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gtsrmaccq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gecaxmnvn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gpxhpfwuy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/ggmjuqppn.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gniocjpan.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/ggojjxjpt.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gvxeohocq.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gpxxyhwzy.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gftjicufe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gzaaocdjb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gzmvjokna.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gigjdfjwz.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/ggpduketd.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gdswowegi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gmbccfsid.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gqysivizq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gpsjrnclw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/ghoqwaqmk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gjnygfzjz.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/guwbisbmd.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/giyfmawzp.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gqmaecgsg.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gunnnjvis.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/ganvfqswh.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gahmzzcxk.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/ggdirwxke.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gkhhdfwyc.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gqppsncly.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gweshlueh.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gjudncgxk.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gxknslyav.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gmijoudvm.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gwfuhffeg.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gmvkbrmbb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gexrrypcs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gmgxdiqmp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/glmecurcp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/ggfwcexyu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gkecwguhf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gcvnjofwx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/ghrzznidr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gxxodmtdj.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/godieaxdn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gtjkgoibh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/glmsqeouj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gmxdcthpx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gmwiwofsu.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gwnnqnwoy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gfbkjfgsd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gvfniccvc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gzjjovisc.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gthqsozrz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/ggydygayx.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gfgebgkzm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gundohuvc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gsfynmdso.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gquqijyss.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gaibobcqv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gkfilqgkp.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gbhnglyfx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gzkykihyn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gfvjbhrcy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gxtlnllgw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/geokfffri.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gzglnkuhy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gpjjstymf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gvrczfldw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/glkoptqub.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/ggvtuxwdx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvjoqwxcl.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gmzjcpert.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdckeegiz.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gmbanqkqc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gyktikhpc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gxsttzpmt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gvtwmpisr.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/guvhouwya.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gcelhyztt.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gxnerqpck.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gzrhywozy.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/goutrmcbc.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/grfxrekjp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gvrcnmeuh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gfgmprkmm.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gspzlbzun.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gbcykgfmq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gxyfunust.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gkqfwruob.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gdkjvrjtn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gnuardnin.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gkxuualiv.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/glethtkdq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gtmvibqcb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gobtdxolj.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gbnskdgnq.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/glkrzzvyt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gokiconsx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gxmtmuunh.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/ggdtflerv.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gpkgzaylt.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gzpmghvab.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gswnrkpld.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gmmzllofc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/goespgyfa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gbrnxgudj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gntlakwts.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gexnwhnxb.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gfauotntz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gksedbwjz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gjztfxrao.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gmormvrpr.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gflukpmla.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gqxneetuk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gnjdgzhyr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gsrwkddxs.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gzuwuhwsb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gwgwhhrpk.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gcwizpruj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gacowkwrs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gxepxmqsx.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gnjwqqbdh.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/ghtumebxj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gvwiqwcry.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gmpglqawo.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gunulycas.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gctccddjh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcardfvmd.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gqahdtdov.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gntpufhcp.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/ghiwrkrnp.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/getmyjvgy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gxqllwoka.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gauuywwhb.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gypoybrtv.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/genxtwvhe.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gdkitnwvf.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/giorceynp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gvgmvuhpl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gxardwulo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gjaxdcuxx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gvyafbivh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gerepyfjm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gigtreham.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/goahuafdz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gedmeeaxq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gfywdbkda.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gnoygvhdk.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gqkwvqjmb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gaohnagor.sHtML


<!-- 参考信息 -->