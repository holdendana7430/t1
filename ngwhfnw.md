代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggulwhxvh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcqysbij.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgufqsqh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswhgiqvi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fanxiaobao.xyz/Article/details/gvlgvcokc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzhjtnmw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmvdnogd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fanxiaobao.xyz/Article/details/gqabfjpjq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gexajzkcs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fanxiaobao.xyz/Article/details/gpsqecfgt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkibabht.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuujzdoe.sHtML

Py:   resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/ghohxosym.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fanxiaobao.xyz/Article/details/glnrcorlv.sHtML

JS:   await resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/gnrzlbubc.sHtML

TS:   await resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/gfiigzcjt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/gquwsmbug.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgkullwv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fanxiaobao.xyz/Article/details/grevefxsr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grucjxhvx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiqsrrhs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fanxiaobao.xyz/Article/details/gxrwkidho.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrlorjyp.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fanxiaobao.xyz/Article/details/gmpvucokj.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fanxiaobao.xyz/Article/details/gbnejjnux.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxomtxmz.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiekdlgk.sHtML

Ruby: resp.code.to_i
来源：http://baike.fanxiaobao.xyz/Article/details/gpmfpuluj.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdfxgwsq.sHtML

[L08] 并发请求多个地址
来源：http://baike.fanxiaobao.xyz/Article/details/gsgjcotpc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdasadurb.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fanxiaobao.xyz/Article/details/gxeofbgmg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfwnbwro.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/grgzakeqz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fanxiaobao.xyz/Article/details/gbxvsoqfe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fanxiaobao.xyz/Article/details/gknuxskii.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjejtxhtg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gtihvscok.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/guaeyrijo.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fanxiaobao.xyz/Article/details/gvoygixcg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/geuwfiasc.sHtML

[M01] 读取命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gdahfikdc.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghceqqeoj.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobazydyt.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gsqrobvzf.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gnaqclgvl.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeitxtwc.sHtML

Go:   os.Args[1:]
来源：http://read.share.fanxiaobao.xyz/Article/details/gwffzddhv.sHtML

Ruby: ARGV
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbwroieg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fanxiaobao.xyz/Article/details/guwsvdtde.sHtML

[M02] 读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggaxicnds.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gfdprbjtr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fanxiaobao.xyz/Article/details/gsjrmmilq.sHtML

JS:   process.env.HOME
来源：http://www.blog.fanxiaobao.xyz/Article/details/geybnnljm.sHtML

TS:   process.env.HOME
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqjfosph.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmwgmztf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/glgxhpbhb.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtnzbgnb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/glnffeiay.sHtML

[M03] 执行外部命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpngdzhku.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gxiqbwrjf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fanxiaobao.xyz/Article/details/gxsusepja.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlvxlzhd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslxslett.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqyyamnv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmojbzuk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknqlueji.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmthtmpo.sHtML

[M04] 获取当前工作目录
来源：http://wap.fanxiaobao.xyz/Article/details/gfcuriblk.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqqdbbeb.sHtML

PHP:  getcwd();
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhjjdrqe.sHtML

JS:   process.cwd()
来源：http://3g.fanxiaobao.xyz/Article/details/gnhqjewcd.sHtML

TS:   process.cwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtcfmrkg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfcptsji.sHtML

Go:   os.Getwd()
来源：http://baike.fanxiaobao.xyz/Article/details/gxtvkqbjq.sHtML

Ruby: Dir.pwd
来源：http://wap.fanxiaobao.xyz/Article/details/gkxltuyhe.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fanxiaobao.xyz/Article/details/glfwyrtoj.sHtML

[M05] 设置退出码
来源：http://3g.fanxiaobao.xyz/Article/details/gqkynnzge.sHtML

Py:   sys.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/giwymonue.sHtML

PHP:  exit(1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwbsabwn.sHtML

JS:   process.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gggrbirep.sHtML

TS:   process.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gewmxfcnf.sHtML

Java: System.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gxsgcgedo.sHtML

Go:   os.Exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gynydrnsn.sHtML

Ruby: exit 1
来源：http://3g.fanxiaobao.xyz/Article/details/gsrkcjhfr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbwzdpvx.sHtML

[M06] 向标准错误输出
来源：http://wap.fanxiaobao.xyz/Article/details/gfswxmbng.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghassmdia.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fanxiaobao.xyz/Article/details/gykyscumx.sHtML

JS:   console.error("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gpwzgipea.sHtML

TS:   console.error("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxseawwq.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqfjdwcb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewmoutcx.sHtML

Ruby: warn "err"
来源：http://wap.fanxiaobao.xyz/Article/details/grimabxde.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcmbtszp.sHtML

[M07] 判断是否为主入口
来源：http://3g.fanxiaobao.xyz/Article/details/gvzzgcqvu.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fanxiaobao.xyz/Article/details/gciyieguc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fanxiaobao.xyz/Article/details/gnrgxjgyc.sHtML

JS:   require.main === module
来源：http://wap.fanxiaobao.xyz/Article/details/graftnnbe.sHtML

TS:   require.main === module
来源：http://baike.fanxiaobao.xyz/Article/details/gefrsrmeh.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkcxuuzo.sHtML

Go:   func main()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsmeuajz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrmmzdvx.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilccwcrk.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fanxiaobao.xyz/Article/details/gxtoifvox.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkkwgpoo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fanxiaobao.xyz/Article/details/gevxbhcmc.sHtML

JS:   process.platform;  process.version
来源：http://wap.fanxiaobao.xyz/Article/details/gnzrabisw.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fanxiaobao.xyz/Article/details/gexvdkwek.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fanxiaobao.xyz/Article/details/gubohodlr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdvetntf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fanxiaobao.xyz/Article/details/gnvigselm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fanxiaobao.xyz/Article/details/ghxrjfwzw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/glwptsazs.sHtML

N. 数据结构与算法
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyeuurrs.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gushrwfwj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdszglfed.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gqvkxxicq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fanxiaobao.xyz/Article/details/gygrsqeso.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fanxiaobao.xyz/Article/details/gcztwppkz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/gnfqwpyio.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnvngamj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/grvkpxlbe.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbqvuarw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkdvwqkq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fanxiaobao.xyz/Article/details/gppxvixwg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaakgakld.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjevgnec.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqogswyht.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gbgtbrboq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gcdqkmsvn.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gatrexlzs.sHtML

Ruby: arr.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdifsjyb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqduqrypj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbnkgwse.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgsszluw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygmcutwh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhkvdgck.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclgczcvp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqpzdhwf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fanxiaobao.xyz/Article/details/gxddmqyuj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fanxiaobao.xyz/Article/details/gclycvpun.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fanxiaobao.xyz/Article/details/grkaubzug.sHtML

[N04] 斐波那契数列
来源：http://read.share.fanxiaobao.xyz/Article/details/glcmczigg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzglqevy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gusnysmob.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnutehniu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdkivbbv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevowdygv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyguxrrc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gibpvspeh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gtddnsxjz.sHtML

[N05] 最大公约数
来源：http://read.share.fanxiaobao.xyz/Article/details/glfqpqgho.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gywseyraw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdavjarpb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmzjdzdtn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkustnqs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fanxiaobao.xyz/Article/details/gpqoewiyx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fanxiaobao.xyz/Article/details/gnffwhchz.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxithvqnq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwhdimun.sHtML

[N06] 判断回文字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfwprwbj.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrtfceos.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gwixsivai.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gktqllmox.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gsejlborg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fanxiaobao.xyz/Article/details/gxxxdxpul.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fanxiaobao.xyz/Article/details/gbnzhynuj.sHtML

Ruby: s == s.reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaygcmor.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fanxiaobao.xyz/Article/details/gegwcxbpr.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fanxiaobao.xyz/Article/details/gpbsjyijh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fanxiaobao.xyz/Article/details/giehllibg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqavwuau.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmszinvw.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfjteylj.sHtML

Java: // 手写 HashMap
来源：http://mobile.fanxiaobao.xyz/Article/details/geopuvxlq.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fanxiaobao.xyz/Article/details/gxkvlttfb.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fanxiaobao.xyz/Article/details/gampmcjug.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fanxiaobao.xyz/Article/details/glbmntnwo.sHtML

[N08] 生成全排列
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwxjhdti.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemclqklx.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfrtejsq.sHtML

JS:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gcafhffwd.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gblvrkxae.sHtML

Java: // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/grgfndopo.sHtML

Go:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gywtfsoje.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fanxiaobao.xyz/Article/details/gbkccabob.sHtML

C#:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/gxwefblfb.sHtML

[N09] 栈与队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeifokrc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnvopcxb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/glbgbmjbn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gsciurjpu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwocmqsj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygcjpnwc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fanxiaobao.xyz/Article/details/guypxodmy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqulaqbi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fanxiaobao.xyz/Article/details/gwzjrspht.sHtML

[N10] 链表节点定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeclhpky.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fanxiaobao.xyz/Article/details/gndkatygz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnwduvvep.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbhbxnuv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fanxiaobao.xyz/Article/details/grbgwurok.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnnzcyhwq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fanxiaobao.xyz/Article/details/gdsvdnvnn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fanxiaobao.xyz/Article/details/gtnhfsueb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkbuyfqa.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gneyofvtp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fanxiaobao.xyz/Article/details/ggasddble.sHtML

PHP:  // 手写递归函数
来源：http://baike.fanxiaobao.xyz/Article/details/gtohywyxx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmozovnq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fanxiaobao.xyz/Article/details/glgmciaxx.sHtML

Java: // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/gyhyyswfq.sHtML

Go:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/ghqbkrecw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfedlbev.sHtML

C#:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/ghjxtukzs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmeojpbh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbpdugoo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfomprnl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfhqlzja.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcjmeczu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gjahiuwjd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fanxiaobao.xyz/Article/details/gpdeyymac.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaqbciaj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fanxiaobao.xyz/Article/details/grfvzexpf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gesvhuwaz.sHtML

O. 并发与异步
来源：http://baike.fanxiaobao.xyz/Article/details/gezdwraxy.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gezwzemik.sHtML

[O01] 启动一个线程
来源：http://wap.fanxiaobao.xyz/Article/details/gnuvdywlc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fanxiaobao.xyz/Article/details/gjnvcaxke.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fanxiaobao.xyz/Article/details/gtsejebys.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fanxiaobao.xyz/Article/details/gmwuvmrpf.sHtML

TS:   // 同 JS
来源：http://blog.fanxiaobao.xyz/Article/details/gmfwbcxpc.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fanxiaobao.xyz/Article/details/gewwjzseo.sHtML

Go:   go f()
来源：http://baike.fanxiaobao.xyz/Article/details/gurtesepv.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcoemuxtc.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgehczop.sHtML

[O02] 使用线程池
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxospqfs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxomlhko.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fanxiaobao.xyz/Article/details/genzlpvjf.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fanxiaobao.xyz/Article/details/glrqwajuz.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fanxiaobao.xyz/Article/details/gbetguafn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fanxiaobao.xyz/Article/details/ggqubnvxm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjlzlpvn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fanxiaobao.xyz/Article/details/grihhsvcw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fanxiaobao.xyz/Article/details/gneolzrdz.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvipobeq.sHtML

Py:   with lock: shared += 1
来源：http://3g.fanxiaobao.xyz/Article/details/guvwltxdh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccrkhnep.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjonyppz.sHtML

TS:   // 同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/gmvuxbjtn.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gglfochvn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrsyarwt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gatabbmjf.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gegwjrtkq.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gyqmagbzb.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fanxiaobao.xyz/Article/details/gslgglnsh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdifmycrt.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghttwkbtt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gaxxtalfl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fanxiaobao.xyz/Article/details/gxvrtzgqk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fanxiaobao.xyz/Article/details/grtundhrb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fanxiaobao.xyz/Article/details/gopefyggd.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gwmsqswqe.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fanxiaobao.xyz/Article/details/gixycrzub.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fanxiaobao.xyz/Article/details/glbvmnfzu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fanxiaobao.xyz/Article/details/gxyvfydft.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/gyimxxldt.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgxzpfpc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fanxiaobao.xyz/Article/details/gprlhuwrj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhxlzqsq.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxzrfjao.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpctwqch.sHtML

[O06] 使用进程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwqjyemc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fanxiaobao.xyz/Article/details/gwoletqug.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fanxiaobao.xyz/Article/details/gxxftfnef.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fanxiaobao.xyz/Article/details/ggykhmvxo.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glinnbufr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxfdwdvj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fanxiaobao.xyz/Article/details/gstqenrnh.sHtML

Ruby: // fork 块
来源：http://wap.fanxiaobao.xyz/Article/details/grpbraqum.sHtML

C#:   Parallel.For
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaqdrvfo.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ggdunhisn.sHtML

P. 常用工具函数
来源：http://blog.fanxiaobao.xyz/Article/details/gqytkluok.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvkvnmefd.sHtML

[P01] 生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gvtyawbvx.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fanxiaobao.xyz/Article/details/gmealqrzy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fanxiaobao.xyz/Article/details/gukainhug.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gkqpbzqiq.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gevxsfcbf.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslnpxlyy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqpcuwqy.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fanxiaobao.xyz/Article/details/gasiunovf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fanxiaobao.xyz/Article/details/grkjzfqdk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fanxiaobao.xyz/Article/details/gtliuzafe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorcaqloo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fanxiaobao.xyz/Article/details/ggrdsyajy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fanxiaobao.xyz/Article/details/gzasypewd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyheyfxcu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyukkdbnb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqhmltwd.sHtML


<!-- 参考信息 -->