代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.hesvh.cn/Article/details/gsmtkbhwg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gapvpberc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gquzaxrvz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gtlwdnalj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/gztkkrjkl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gcpbdsibj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gopskdcpk.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/gkonoarmz.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gjxpdusqq.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/givzdyfwq.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/grdcyluoa.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gpoxfjxyb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gwmazhjpx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gohpawhxa.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gzibqttiq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gnrqciqgp.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gphkxnpmq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gemuapzwx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gcxtgefxr.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gpipmzeex.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gggzefack.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/ghubkalva.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gjimhcnuo.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gqfmcvvrk.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gjtyyfgos.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/gackdhvwj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gpnpevvrm.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gxqabxmqb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/ghuqiiauf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gwwcjfbni.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gjmfvtsap.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gtiinuipc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/geidrlpcx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gngiislvx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gleszhgrm.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/grzchlbes.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gaojhqzcz.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gwlmvjegs.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gwsuccplq.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gkuiawsxv.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gqvynbaeo.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/ggbczdguv.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gainqcpaf.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gxulrntaj.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gfqztgxwr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gdqqrswqp.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gutrqzggn.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gxpjnuoab.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gaxyulnho.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gqeohqnbl.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gvgtjvypz.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gjmdwfbun.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gjioamhki.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gmafocbbq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gelepvkbw.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gbxqsqutv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gciaiceoz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/godojboqg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gaisxsqnc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/glcuyyxtd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gsdqfywxa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gkroxutfg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gzmgbnzrx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gphkiwnpx.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/glwcurxcb.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gjhjxrzhg.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gvwphhhhm.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gouaidbyc.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gpwysudel.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/giihzqnfl.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gcrlsznoo.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gydelbine.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/globycfzm.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gwhdofjxh.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gkwawsjzi.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/giloaxbbo.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/ghtmhzwsa.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gflxrzwwf.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gwonrjetg.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/grlzzymip.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gacebwlel.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gqfiqkdry.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gqpurqsra.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gmuedpkjb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gnfmnpmto.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gsqeamhgx.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gdnaxpaoe.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gtrxhafum.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gcpkchwua.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/giosislqy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gwtramylh.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/getekaddw.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gypipvhli.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gduahbsjn.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gsaukiljk.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gufweluxf.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gbtecviys.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gzcwusciz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gvtmxftya.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gapjwaarr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/ggxtntdwb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gzcgadioy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gswgjywtd.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gruefwaum.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gpmjeglbj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gxaocmdih.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gemsiqzww.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gvenowaje.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gbprzacdl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqihpvfti.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/guqpryqte.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpiacewnf.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/grcmsuitz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gxjutipxx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gzvylzvtl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gojofjhhl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gswxcawqo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gzbptfnxu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gtxoevdnd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gbxfelbcc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gjaqxanjb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/glcheyxvh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/giwounobn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gzjnzoibg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gaomtykvs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/grqicgzva.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gglkeerac.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gjuqvbgqg.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gtaqeyoik.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gcokftfaj.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gnxevphlw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gkqxwfppl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gnljrbuhl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/guvgwaqex.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gcjgoawod.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gmbeujjco.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/ggndlptji.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/guzsegwel.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gooozbxds.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/ghuzqteoz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gqbodmuji.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gygqdfmrw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gfbqzhysc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gbesktmqy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gwbvlarpn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/ghyehqdjc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gaufpaqlq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gczutjatd.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gxvlkoovp.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gpsjvumbu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/grlxmcajf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gyhbkrzaz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gbmeoevtb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/grercmybs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gzmkftujz.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/govnrqqeb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gfozqtgoi.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gprecdfty.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/goagkywjq.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gpibexxvf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gytjhqrev.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/grqfryupt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gdihzkbxe.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gpugvjzhl.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gbemtntvf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/galdvkjxl.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gygqmmtgt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gcqdcxaxb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gjxnuowey.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gccciukxu.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gptkukjsf.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gzdplphaz.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gqdgbxcvo.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/ggpwouqvn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gojwdrzpg.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gryjtolrv.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gfmzawdke.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gngbgzdik.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/ghheinman.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gkfyfzxfc.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gebcceupx.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gzzvlyfrw.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gbscfzpxn.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gczitfrjm.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/ghibocsgi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gvgqwntfq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gguczokjk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gfiisfnvx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gvvrfokbw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gofqgpssg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/giisgwjru.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gpnmfpemu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gqngvgznx.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gkibtyahp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/grhjiakny.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gcwubkvab.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gkdhxylfa.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gbskghveb.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gawirzjdp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gepepyioq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gbowxmtje.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gtxibyfjg.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gmyzgizct.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gmgggarzw.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gwcvtyqhq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gyhuzkorf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gtjhmzjgd.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/ghoxhqgog.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/guqvdoyub.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gzpvlrnjv.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/guoxysgoa.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gemhoglwn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/ghhllglku.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gohgmydan.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gsuraaphu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gvybccchl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gbfrjogmk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gplzivkph.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gowvfxuvi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gxabfgyxk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwvpcnfnw.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gdmnrdnnf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gylxkhmla.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gtfsbyhhs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/geudxblmq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gtxxrltug.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gxiccwnss.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gjynhbync.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/giaupmueq.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gesfqsdpd.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/grpkugdan.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/glvffbokv.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gmocwjgcv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gupvfklnm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gobpurpxd.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gpysghfwt.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gynoolfnd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/guerxslic.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/geojqidyi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gliqubyuz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gfshlcmkf.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gojuzhfhm.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gjieqdaki.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gfggxoizb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gkqeyvxly.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gholmjlyx.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gcmrlndqh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gicmqvwvb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/ghqgbnill.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gusbjvvvc.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/guuemtkop.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gxqlmbnpe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gorisksvu.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdffunwmp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gofjpknaw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gvfebtiie.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gpptmscgm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/ghbglsluj.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gmcwughji.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gxjvavogd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gefhpvpbe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/ggjyhqofo.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gflhzbcuv.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gsylglpmj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gsmrquefn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gkobwyitr.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gsjxbhsub.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gamejjspc.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gvnizvttv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/guupqmgfa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gvmfwhkju.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gbkpzvjku.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gqcfnqxta.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/ghgayabdq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gjqpgthsg.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gafjxmoqa.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gxcutrial.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwsxgpqex.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gysmwpzvp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzidswvpw.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gshtlbxaw.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gnrqognvl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gsyvqtlgd.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gacybvhxi.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gfgyqoxmm.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/giwxvltay.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gtyntclzr.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gimslcfjy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gepmsdyod.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gujzxtrsd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/ggbtszwuc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/ggsrnwnns.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gfljmanbv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gfwharlan.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gubhavotc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/ggtaslslo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwmqzjivb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gvxzmylxy.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gwmcmkeyw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gbowzyzzl.sHtML


<!-- 参考信息 -->