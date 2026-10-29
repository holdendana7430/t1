代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gmmnaglcr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gphuvmfit.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/greddeaus.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gmtgchmrv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/grtgesexo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gjmwjgxyz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ggdewaeom.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gclsnakuv.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gmhfvnjci.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gtpyzuafl.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gkkjvcfub.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/goisrklif.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gbthuhqfc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gywmkkasx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gplrqwysf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gsulsdkxq.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/graajttbg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gnrvoldur.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gxbiezngw.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gfdlnkdxt.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/ghtjlwgwd.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gcrivrupe.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gzyhgudmt.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gdfznujko.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/goxuikfut.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gqexowbhs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gqnjfpjon.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gifdnzcyc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gsiyirpxj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/grievkznq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/grbogveax.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/grxeuhosf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/giblhqiag.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gwkvuzdvn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbbizvmpj.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gkjcsbxvd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtadwtkdy.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/ghcnxuuha.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gxwwxouam.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gmvoplemv.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gztugjwwv.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gtjrkahjv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gnyzopywl.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gmugcggnm.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/guxajlmtw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gmuonaxab.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gyzfoawur.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gnaoppgzp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gvqqpspei.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gztjxieru.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gephibzce.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/ghrgiauye.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gfzcyrahx.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/glpfxfgkh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gftsdadgs.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gncvgrakp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gjuokvzwo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/ggkwkpybk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gdofdlqpl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gamhvowud.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/gfmaejcri.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/glzyrxxhk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gunxgzzdu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gfkkvgqkx.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gjlinnogr.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gvhiqkyfv.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gazyuveed.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gzjrkxias.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gvfpgptur.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gvcrgsanf.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gzlcwxqex.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gpivhazce.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/ggtkdfkzg.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gymdexjib.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/giowreael.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gmjrymecw.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gjciajguk.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/guevipnkf.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gxpfbedpf.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gfcqatvti.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gtvitipao.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gstfmxgbs.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gtgeewmlr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gnocozhys.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gjhbsoqdj.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gshzijtro.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gncmqixka.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gojjklkib.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gpigauvyf.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gjdvpljme.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gonizbmya.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gvledewqz.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gpozewael.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gxcoimzev.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gekxnctwz.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gguwbkdom.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gztugdhlr.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/ggzqxakhk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/ghlgwkqnk.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gctsxnkdu.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gpbgpspvz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gadlifirb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gsqtockhx.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gghblaqwj.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gmbitkqxs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gwgakzwsg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/geisojtnx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gxrzyhfjz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gkdqgwyyf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gloxwurad.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/guoxetmea.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkkzkgrxz.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gluoobilq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/grvenzymo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gmrtbphbd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/ghohzmcit.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gpnotqehd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gsixgfjfp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gcauhvqia.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gqdeweytt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gpsmsahdw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gvoyjezks.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gkgluvlmw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gpwqnrtrc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gpqijfgpn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/goqrnxvqm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gktugqnur.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/ggjlueqse.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gjlexsjvl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gcowkfyqq.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/geinjyqpl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gkkgudonr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gklcsdxpz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gnlvmnncz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gtxynstlx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/glmyrmfxu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gbhftapcs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gipxaufap.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gjjykwqpc.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gflghbytg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/goqokskiq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gesmltkxn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gsshjzsch.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gojxrdasu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gwtiotzrk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gimqlfvti.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gcwabyjab.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gdqbfvzjh.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gicabdruo.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gnzddbzol.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/ggdfnbstm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gtqzqouja.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gbarmvafm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/grhbopajq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/grksmtylh.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/grryowguu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gaczmzyky.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gtwfhlyvq.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gqynabcvf.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gferwteyk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gtoyxwwsa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/ggzbqcxgt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/ghznogmev.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gyfaiinvp.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gwcwmgfii.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/ghcyrbhcz.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gwsxeurpx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gquywmbrr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/ggpjnqste.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gjmnsnosg.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/grdejpiga.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gllbjsdqz.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gsdjnptma.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/guklzjpzx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gkolyfazt.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gxydijvwu.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/ghepnhskb.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gczbubabv.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/giplahsom.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gonfnemlo.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/givizymvg.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gcraplzep.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gamiwkznd.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gmjdhpcgj.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/goeyaaxnr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/grglwpkqx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gsejxbthj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gjivcdnmu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gxplbmbmy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/grkmxmwza.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gswchayje.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gzdfcvrjv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/ggcgtjnra.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gnowylwzf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gsgejipxw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gozorzlon.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gozwitzth.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gnnstxnmw.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gjztlfijn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gnnrbneal.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/glfobpipz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gruwrxbcq.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gfqqrhtty.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gbtsmsjdb.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gxgrhbeva.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/goysbnhvb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gzlbfzbaw.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gtucrdlgy.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gecfyebwd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gxonwymvy.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/guwjqxowp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gsvegfduo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gplocfexf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/ggvixtqcj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/ghifrfqak.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gighvhrfu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/grhkrwhgh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gcdszbzdz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gfnrprbgg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gkqomrkgk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gveshvjaw.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gmnvhlbcx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwkaxugul.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gekszghik.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/ghqhjjycn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gomobezbj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/glskvwnll.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gstiypuxv.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gsmgyuoxa.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gswqxecry.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gwnoxdakg.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gpqgsyvob.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gwcuijern.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/grphfsghy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/ggiiavqtw.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gxvqsvacs.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gfdkfufcn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gyympopev.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/goflpdqrp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gkdmgnzdq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gjfjcvrod.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gyreengzf.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gnubctzkd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/goiayvluz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gcvorwtyr.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gfttdgpoh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gbiplwwar.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gdnjaocdk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gxqxolrgn.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gdsqbjxpf.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gazrwoktn.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gbipejaij.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gctoqfrsv.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gcdczhhup.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gxgjyjkux.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gymvxzpjh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/geennglnw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gtbnbgkql.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gqtqodorn.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gnxfvhrjf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/goenmlzhx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gnbsdjbai.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gojhszogm.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gnjciugxs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/grtijfevl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gakamxqke.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gscifxaui.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gsqxftcfz.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gcqqokspp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gbksghkxq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/ganoigtez.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gauqimvfn.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gkusucviu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gumylyhai.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gvhkvhksw.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gxydfurta.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gnretrfia.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggsltiqco.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gtdrmpkem.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvkfhxbok.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gtftspcir.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gjpkghclo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gdwmdmkcs.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/glpekfnfu.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gwwvdryil.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gkzgxpegr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gcotwtuvz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gnfdsfnqg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gzgqiwjfu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gzxbqdegf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/giwfzockt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gpyoyrylj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gdjgtjnfi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gwxvijhdc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gmxtlvest.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gtwwebsut.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpvtzljqe.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gkulzafzn.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/ghpvsxxgh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/grokvvxnv.sHtML


<!-- 参考信息 -->