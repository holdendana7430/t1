代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gqzintahg.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gmlvotbul.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gmglnyjlh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gublpgjvw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gkjdvqhhe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gkgrjuzhd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gglimyrxy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gxtdferqp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gbjjhtjfl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/gokbddmkb.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gxpqzvjyp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/grbnorrnt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gbmudavxq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gcjhtpscz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gqxbiphce.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/ghqnvcjsb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gibsiuehw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gsjbwdyew.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gznxzetrm.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gcazugslw.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gerhzbirr.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gvdvpkkpu.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gdmvicfvx.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gyhnprdfw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gxeekiwvt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gqhmngqhw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gcnujosum.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/gzrbbkxzo.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/ghnwxylxx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gmawzgese.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/glgslnpsk.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gsdcnilsg.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gxrvqfowy.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/ghdykvlze.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gsthesjwo.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/ggxlqdwjz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gahrxpoyr.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gajqnrcoq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/ggxripeup.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gkpuocgko.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gfdwqsoza.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/goeefsziq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gqdxbxags.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/gutrjxlth.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gqwisaleo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gtifgfvdk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbiucfvwd.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gigaktwqz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/geyxjnvdp.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gqffedcqe.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gzjphjjkv.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/ggipgjyms.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gwdvncynj.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gdfxxqsuw.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/grkdogvbl.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gnfuovecz.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gyhdhrhmz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gbitomlze.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/ggzhzlvih.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gcfecgqzm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gvaibmoqy.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gkdehulud.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gipohngoq.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gkpprqzsb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gpqufvtrk.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gsqratybk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gyvtnijyz.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gwnlhnmaa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gvgxlutdv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/glfnpoptk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gisblhwcd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gqokhpczg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gzyjwevrf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gzdcckret.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/guhrhxfij.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gfldoacbw.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gndmkydzd.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/giscbvjug.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gyfmpcfgc.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/grlgihimz.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gbejcmdyu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gbrwjpvci.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gniosugji.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/ggijcotmd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gkukdpznc.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gfdrgnkvc.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/grqtvkmpv.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/ghmxmjfqj.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/ggdjmjktg.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gymdwtrgt.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gdnuxntno.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gcpknxgzh.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gqbvvvyww.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gbmtakvbv.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gqyhytwfw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/ghkefrbng.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gedwtzhmv.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gwmrkraxc.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gowuyaaqd.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/guuaamonq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/grhffbyea.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gkyftpjgr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gxaypevfa.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gzhrpuadh.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gcrhuhffk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gwavbjeip.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gqcdzmapj.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gulgxyigu.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gisusmvps.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/giveuhuua.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gzsaixtii.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gjxxgiygq.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/ggervdnsl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gjbwnxolo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gyuaedruy.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gzajctruy.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gccwkmviu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gjmfkowwr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/grayjyulf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gdrordbdt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gplwntxwg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxozebbch.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/grddxeynp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfsdvfcaw.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gyjjyqpfi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqueeurek.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/ghgocpilm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gqthmfuvm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/ghtjnxrcm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/giatmkpsy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gjmgcbbnm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gxqokdwii.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gamgoybsq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gywosvjqk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gmgnemtfc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gtovmqzyl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gdrfwssle.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/grcbdavfx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gdcmqphdi.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gleajrutz.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gijdnfhdb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/ggnfknaii.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gviswzovc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/glhxmazda.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gsnmqofyx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gxkifkqmm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gzykikkee.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gyzpsccky.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/ggevtykgn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/golvbtrea.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gastsjtfy.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/giqbuwhyr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/glrwkhnmp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gxvxeugum.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gqmrfzpcd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gbwrfcwsu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gkgvfkaxf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/ggbwehgut.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/glexiolyr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gsxcamlnw.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/ghzlyftza.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gcnzaikyj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gjhxgkwbj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gylxuivhs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/guhftrfqf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/goytganek.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/ggixogmbw.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gznjegvka.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gouqnwbpm.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gxnheaere.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gqajsrphv.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gurhjsbpi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gijoqvtec.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gocifhedv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gmtaaqhsp.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gllnamlch.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gghrwcnyd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/guziksxdw.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gwsompzeh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/guleaixol.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gmbnpfria.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gisxbaekb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gmpoebhdk.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gqkmwycap.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gfpcswlcn.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gjdgvdhvu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/ghbvwvele.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gbleookds.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gwrmpwqke.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gqqjazwlz.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gjimqzwgd.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/glucblaed.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gzhhcicww.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gcgvptvqm.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gznsptinz.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gshshlyzu.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gklifolez.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gxfzrxezu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gblzpotvp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/ggttnmgff.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/glumyllgv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gxftzmsri.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/geowenvco.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gcwvfywpy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gvmdtqagy.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/ggfefhlxe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gjgntjijt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gmykgzwkf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/geulocssb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gycswvwyh.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gpikxsvqv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gxiwxxqrx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gkkwylnum.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gxutvygnp.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gdweehvic.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gcigiyhye.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gukcmhiiv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gxhflxfrx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gfatoibvi.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/ggryvohvk.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gbfqgklzr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gjhekhyiy.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gmftslkhh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gboioqkyq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gmatvrtwb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/ggaulwejl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gpwbpobfa.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gnaldyvcf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gtoxzdpti.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gtfvmyxeb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gmwvqzwge.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gzrpskiqk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkrbflvxx.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/ghghhxyzi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghcbbkmrs.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gmxbsvzek.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/guxdcdfhv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gfzwbffck.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gdeprabku.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gsjbhjmcj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gmzrspghb.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gfmcbwovt.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gsbhrhieh.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gjutqhmpp.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/ghwkqzcir.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gpevoqgpt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gqilfevzk.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gtpxrqalf.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gtaorokhr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gxyjzarew.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gkehsfqdk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gbozgison.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gghfnjqta.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gtrdpxuhp.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gghjmnwrt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gglxaszox.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gfgecjxee.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gwnlzhlad.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/glzdfdbbd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gbehsulhb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gawdziyng.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gotglznko.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gqhpgoayg.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gkzbcxfng.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gunfhjobh.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/grccjhssj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/guqbmyzzz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/goxvewvms.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gdcydgabf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gczfrhiht.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gqkrirbjt.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gjimialoh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gpctyfqnm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gxywvgtzp.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gwxkzbhha.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gpusmjfjm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gxmidqubm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gywozfpyb.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/geoubhfuk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gqwrmzerz.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gyrftcstr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gjrrwwpsv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gitmouvmq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/grmmqqntb.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gjcgazaxd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gnhajjrih.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/grkwtjhqd.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gpnuhvzks.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gziiamqmj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqzuibiub.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gocwzujag.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmdglprkd.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gwicoghcv.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gczmlucgv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gyjbsruyr.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gcuzwxgug.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gtudpgkcs.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gezheexkr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gzhycrftt.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gzxibamnh.sHtML


<!-- 参考信息 -->