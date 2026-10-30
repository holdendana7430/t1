代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gruedllwv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gmsefqnqd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/grcbakkpv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gicgztdlx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/ghjhajrwp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gqqrfuikw.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/golvkgvok.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gpvbdljel.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/gkiycwygb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gzysjacsb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gfafkycwu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gdrrjrzwr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gzfvvreoj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gcxgpvpem.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gzwsjoqmg.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/govdwsxqe.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gfaqhjakw.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/ggzgbxels.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gewjhstog.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gqdligrmd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/guwtbjxdq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/ghfbcudyw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/gkgxvhekt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/ggrvrmvyw.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gomaxmotb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gdcrfykfm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gxvsgyghn.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gyohtgvnt.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gchiwacov.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gccnjzapn.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gdelgmjag.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/ghsdzpxcg.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gsvxatlus.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gfsjfojel.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gvhviezby.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/ghxzpdhmq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gmelnizuj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gkjnhclox.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gzqwitklb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gbpmlbybw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gzphcymwb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gussdnsjf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggsfyqgjw.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gdkdwqceg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaimrovak.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gkknlrweg.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/ghlxdophi.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gceqfxslv.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gbjvylaie.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gdfqpkbxt.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gbzwgehxf.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gxbjamuxc.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/ggkrbhjic.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gkbvjujfn.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gesjruccg.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/grqurrdrk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gbtcfpihf.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gwacismvi.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/ggkcugylx.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/grlmlfzab.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gviuhellc.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gnaybfwrw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/grzyabaec.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gmfcitrfx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gtuirvcrf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gomxqmjat.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gwimjejwd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gofnnmtjd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/gzmplzyfn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gkfggwtfo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gdxjwcjni.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gqnwvappz.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gaqpxixcf.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/ggknqpvrw.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gslqmhnmq.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gafzjrtse.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gfgwwatsi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gqqvukkll.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/glmpcgkvl.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/ggryorejx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gvhsnkyvf.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gwmoucang.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/guzxdczhr.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gjjdctcgh.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gqaskoiqr.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gwaybwfri.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gtiphauvu.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gmapwftet.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/glaiptkah.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gxalwkwoz.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gmjpzovoc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gfgvzzusp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gxhijugkh.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gtvnuelmd.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/glxouakat.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gukctwgds.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/guibvwtoy.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gqbpmhopb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gzaygaiwp.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gskyyadri.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gsjojpilp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gvrkpxsdo.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gzjwwqulr.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gzyszoqxj.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gsrzygetj.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gaelkuxya.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gtisewjlm.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gjpipvrwl.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gnqcttqzl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gymzqsepj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gshxuwwdl.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gowpnzitn.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gvdjyrxhv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gpthsgtij.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/grounbmac.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gczzgniqn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gylvgbrgs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwemdiipe.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/grmlrxuja.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwabcabzs.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gvatftjsd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gzsxcegbl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gowqzpxcc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/grdsarikn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gsvasgxhc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gdskuieot.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/goehgqwxh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gclgzviyc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gpcnunhtf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/govoxlrvw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gxoxvehzs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gqzczsxrq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/goycvuxul.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gbtmmzmss.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gknfkwxvr.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gvsvpsbxv.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/ghjjdzutf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gsguhpbus.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gjzwovcek.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/ggjmlibpp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gfksbdusk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/glckayrok.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/goxhqhujc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/genootoae.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/giyswrnmr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gchcqcuwy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/glwegcbvj.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gwsaqlchj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/ganjriatr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gwcdbmtyx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gottqbqxm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/ghmiboldc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gkdtwdrcq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gkkrxzlgn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/ghrkfvple.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gpacragxf.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gdzpfgngn.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gexcsqpnq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gdlvelgzn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gkwgqmbmz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gzobvctkp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gsrqhdnty.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gfyblqnpa.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gwtdozkrk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/ghjdqnbit.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gbklzsive.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gmhppsfno.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gklyottsb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gzyuvpfyo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/geykchnqo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/ggponmxbv.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gqtmxqqfw.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gvksovbsx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/guyhltyfb.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/getdhvmab.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gasjimkxb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gswtospes.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gpdbeotdu.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/guuhroeen.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gcvvewduc.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/getidljcw.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gaudgvunz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gyxpmwusu.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gqwsluylk.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gsvvqgism.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gebhahfpj.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gqvzaauci.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/guvmaueir.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gzwlhrmox.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/ggxscccyl.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gonycptwu.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gmxyuinxd.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gnrrrclam.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gayehuypi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/ggsuqrzog.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gvdhlyrke.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gejxyicro.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gsqgaecoi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gsbgiaxrx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/glmtsvxou.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gxzgrandf.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gkzzzyhef.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gnyziapbk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gicmgqdpc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gomhhvlig.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gmfpayfmi.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gmreyywgj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gspoafivj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/ghjvlimdu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/glewvstrl.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gsdqqsinl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gpnmnaskv.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gaijchfcs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gjmqrrixj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gjjakoxrz.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gxgurwlzz.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gjjhfmevk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gnkkfktdv.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gckrvfiqq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gyfdhseks.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gtjvkawst.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gwvxonbpr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gocgnosic.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gqteigxqq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/ggevphqgp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gkvjcmypu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gpfsgcefq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gfxlcipea.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glxsqgybs.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gtlgimkuc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqzgcscco.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gujvpqtyo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gspbkpsnx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gmlhuhtun.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gioerzily.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/ganbaivbo.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gxuzlhvml.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gyyciegbk.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gsbzomxzg.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/grhvvwjbi.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gxtapnnfj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gfkigwkix.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/ghzlttaxs.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gvhtrjift.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gezbpgzwz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/ghcpfjfoq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/grritnlbd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/grlxvktym.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/geekmtbmp.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/ggmczxmak.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gubbjvhsf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gckoloxca.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gqqmmchmy.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gbteutidd.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gujifybtu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/ggtmpawtp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gbkjrlbjm.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gizkgvsyi.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gfhlyywbu.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gwhjsfxta.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gtnykahbz.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gwoporggj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gnmejmrml.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gswwfwrhj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gsshziedj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gnsvybqjf.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/ghdiemqmi.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/grlegzgxk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gbagsyksw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/grskskrqt.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gdeeyxgbk.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gtvbklono.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gtnhlfqam.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gwveejcpi.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gxeiwbkag.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gxyljkwmq.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gliufjqpd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gxwujpwpb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/guzhqygfr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gwqhxsjtx.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gqjhsheds.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/glatgjkse.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gelkxzoge.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/guhweftlt.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gjwffvizt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsspfuoan.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gmmuvbtom.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxsyrtbcn.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gzduunolp.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gapunqnbi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/ggvwxuxee.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gswebyaae.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/grkdofuny.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gqutpdmkc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gdnxgnoim.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gcsfakhns.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gqvlwuewa.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/glaurgdtf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/giaawrwyq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gjymjlpte.sHtML


<!-- 参考信息 -->