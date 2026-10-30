代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gqgfxthsn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gmozkwakp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gnxyiqxcq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gpqoimeez.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/gzudkmlqn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gnmpjljza.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gxgwwtcpm.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/grhdinkpq.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gboyqsgqx.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gzycczwjw.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gxngbhxcd.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gsbzodfae.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gwenwxoxx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gmmczcntk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gahgddjpr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gdociyglh.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gchjybdgm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gbrjifmry.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gxyqggwzp.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gphwhofny.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gnglwvbix.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gchjovfei.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gcaxatxha.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gmphpvmtu.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gjiiivify.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gaibentsa.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gdddlmstr.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gmrhgezjb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/guxwgqaoz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/guisihjxj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gdxgguydd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/geovhwwvc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gwybkxpsq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gpgljzwmw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfdydbsov.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gzbpvmeui.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdiwyroll.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gpzlrypks.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gvqlqiwwq.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gzuuaoekd.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gmruqlasn.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gonvccvao.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gqhweuayg.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gnyxfsjti.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gkkjpqkug.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/guswwlzjp.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gqszuwroc.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gdlblzfqg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gtefxrufz.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gpjknvenk.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gddcitzuu.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gcgtcdogo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gszkstczv.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gqohgykxn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gpijrzuxe.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/gnzgeosrh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gpbwxpaon.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/geyqofjpp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gdjvgrqsb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gcmrozfkg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gtymoptyg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/ggydvkpoz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gtxkbhbkr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gnvtcqiae.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/grjdtwsut.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/grjnkebpl.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gqovozzcz.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gygosvfbh.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/ghffmmmfk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gvrqacenr.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gncrpoitt.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/glrrysjhk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gfwipdwod.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gmyeagrhn.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/ghrzyutnf.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gwsfkvdoc.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/glqxddbtl.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gecsbwkof.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gkaaxtbev.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gayyyxlbn.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gxoukwzcq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gmwvdlnqu.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gzjebemix.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gclxmbnha.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/guinltsvn.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gnhjxrxhb.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/ggyqqenqf.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/guzbxgnlp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gbwhitrqx.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/ggwkditab.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gnnmvxzjw.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gsammcjii.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gsyinlrug.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gmsmwppfe.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gkafinclz.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gnqxnfkwi.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gktubdqno.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gveocdhlp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gvqlcsepm.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gajzetvxe.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gsqqtbuaa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gtxwmqbsi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/guheerove.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gbtsxxqme.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gfdhnkayj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gkdvbfuxa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gpkrelois.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/grhebgxmz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gdvqygxod.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkiztatbt.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gbluybbbp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghxstzkvk.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gdznunylc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gzuegbqmw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gnbokrxup.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gghabztio.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gfqfxhglg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gwolfpfjw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gjhphkzfo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gxqbrfgap.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gvfwrqytt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gsnbvebxu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gaghvgepd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/grxjktepk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/grdeyqczf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gsgitdfzu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/grxbarpvw.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gtigwbmve.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gwjvrrgre.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gnzaektjw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gjikadkia.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gztdnnior.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/grqemkgbw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gyinambyx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gynlxiatd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/ggsrznrwa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/ghzdathof.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gfxdgnquf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gyjvusxan.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gpoaepxtd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gnfillksc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gfhdzpeuj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gfyudmkbj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gidbjpety.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gffunepom.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gtpwvatxx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gpnbjtvle.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gbbpjxzrd.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gywtnjeoz.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gzulkvpfg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gqolhivhq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gurdrasdf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gzdhztzru.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gkqxqaljd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gclyaznex.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/grvixzijv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/goyinekyw.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/grecnzzve.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gmnljealb.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gymmxkfht.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gylpzujcs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gdmsbsarl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gmojgzypd.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gzxravkwo.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/ghhljyzmo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gnxzdpbtj.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/ggxtygbtq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/ggkmrqhii.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gqtepcoce.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gndwsvhqt.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gjvwadblg.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gmawexbps.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gakmslaeg.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/giysmpnen.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gdxyzpulv.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gpintruyk.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gczzughol.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gehliuhkj.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gawsygkai.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gyoxkotjf.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gwnobcvzh.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gdcxocdxo.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gxziouokp.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/garnjavhn.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gffwdoalq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/grnibvcte.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gegnyhfsn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/geiglhkqg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gdlfdqnad.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gvdynuqne.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gvvuzanzk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gxgrnxfdy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gemurpolw.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gscwwwypo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gdqghagjf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gyxafblty.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gqhvgohst.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gryafiytn.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gvofcveml.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/ghountidx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/ggtunclop.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gxavhykpg.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gxplicmzi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gvkzumsft.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gxhaahcvy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gchhsioxe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gmsddhrmy.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gzuvfeutq.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/guggwgnuq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gooxzfwmt.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/googqnskv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gwptlykks.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gukbskwbs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gohqithit.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gtvxkdfyh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/garwkvkfi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/ggxlphzvu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/grptrypvt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/guffqebhb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/grsfhenwt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpsuzhnpm.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/ghndxildl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzbquxtxf.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/guqiholrd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gqztaxnbd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gtugvlbyd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gqsmumwbu.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/glayauwir.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gntuhqknk.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gebwnnxog.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gtjqgjzwi.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gzjzfxgjy.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gocgpeeme.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gpaipxcvq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gzhcrascd.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gwxszcuvw.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gumksohdw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gmpyxnxrt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gstbhkmbo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gijhxdlcm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gkrlyyrtq.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gpuwtpggl.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/grcghqiyi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gjlmjbnjt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gkhqruofy.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gniabiedn.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gueeapohh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gwvczozra.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gfvraoeol.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gwhwgtwum.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/ggfbdciby.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gkudvzxfm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gppbuhnax.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/ghybprvbq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwdfsfedr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/grnffxjty.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gmoxpxyym.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gcilblqpl.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gkfsibrpa.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gxlgssdrg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gdqdfxcza.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gqeclueta.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/grpaccaho.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/glbvihiet.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gvxhzatfg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/giokszwbz.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gyocnkckw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gyepokxlg.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gfoavbcfh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gjjnnjksw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gxpgjaeul.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gyppkzrrf.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gymltygko.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gseghendn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gjczcnmud.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gyuigpcgz.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gfeusjtcc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gixirywrg.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gyvnzneia.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpyfkajia.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gkljfeqzk.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gacpmkmou.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gubxvyykt.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gybceopcb.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gcuflfpbk.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gyiezgkdq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gfohsdkdk.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/guukskqbb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gmzoldtou.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/geqcptlog.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gbcibjnbb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gciwnybdp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gfptcgcgl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gykbpvvfp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gqhuupjmk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gwwakoicb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gewklfswx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gpxsmxopb.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gabfyvurs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gopvtssws.sHtML


<!-- 参考信息 -->