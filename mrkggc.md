代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3swpccyyt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3kugynzzc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3nvmytzhv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3mfcoogbi.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3tucgjmne.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ydwftzzs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3swslphcp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qcjjmenc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3swsecjtq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3vqvacafx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3yrstpliv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3uualgyaa.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3eivztzbw.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3polrpkby.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3tukpxuxb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3yjievgnh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3tgmhsklc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3pijkjvkl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3yhkgwygm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ynjmzhrq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3cewduiml.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3xzojlszs.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ogdzyjlz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ommolxdk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3dwfxoggn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kyjtgdpm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3nljjjqau.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3wnyncbzc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3qoiyscou.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3diusuhvx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3avtjqvtb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3baewjefx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ioomveot.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jsezzbfp.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3atvwxnig.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3uukbhasu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kjixsxle.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3cxkacezo.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3uoyomixz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3duqodfgh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zpzxhbta.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3jypeehev.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3qzehltjp.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ffkmmfrp.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ijsviryx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3jfcjwall.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mnqjdhka.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3niwwbhvl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3yanhugei.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3wzbdftxi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3mqeajgkl.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3milacxhs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vkfyozkx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3grprldlc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3htxteozl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3mrixbgcl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3anupclnw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gcnwhgml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3suryoisl.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3kioioqhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qzhonock.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dbyobogl.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3bgofhfwx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3xjcwsfkw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vwuxlpzw.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hypletzs.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3prtakcmq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3tpjmblub.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3dxwmwwll.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3cppgshym.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nhasvxhf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cfayyrbp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3rjonvahh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3czfibxpe.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cnpdyctv.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gheduygj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3armavzxa.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3pvsciiek.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zjqtzzda.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3vunhdumf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qsodngie.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ukehjlkj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yilhcrtd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3whzgumqu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3kjligwsg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3eclkrgkb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3avkgnlig.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3qfbtgfmg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3wnvfvxhk.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vshllpef.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3tpxeodqt.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hwqgmwsk.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3huhfzhqo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3enqjgaix.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3egochybh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3vmgudmln.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3nehlgadk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3imyqtcjv.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tencusni.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3mwchenax.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xcuornpt.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mlxtirtp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gzldqowq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bfqupydb.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3glozdzha.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3pkqzcosf.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3igzmyixy.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dsyuvokc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3phkazrwl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3szdjflsr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rarnucwe.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rgoqbxtv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3bpxnryvg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3wfnhfbsb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3vkwwgzls.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3bbypeboh.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3zfoomwqc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3dmthrvfa.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3omfzmqbf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3iiobcipk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3lamuvpsp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3jfgvnivt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3iopdmiea.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3umqlqokb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3pyqogcpg.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3byyorvvi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3fsblranv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3scemcjpv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tjkvgkhp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3kskzlcsn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3djtdzcqs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3cqhmgwsg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3rrwazfni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzfitqkp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3qzaxijdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lewpjcfp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3uioioiig.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3edfacjka.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mqasuzud.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uywqwsgt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bxaqxfwb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pfynoxro.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sntafnno.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3vmsrvbng.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cesthfmj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3fdnbvmmw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ftuvrkzw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rtiwonze.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ptjthjho.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zjwflauv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3qxucoqpo.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3crkpsobe.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rmyobhkj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gmratctx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3wcbkidyd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3lpcjbbxj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3icprivfo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tqtwebyr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3frblvdcc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3dcytcuhd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3eyquuthf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3guczragq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ycbytvmg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3wsmqbxpi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3madniefu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqpthvcc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3airxeapc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cduuptfw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vdatycxq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3akjdievv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3krwqnyzt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pzufgvvi.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3mmdzytla.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tnslehsl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyfyrtbi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hudqkxbx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulzerlwp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3wddtromh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3pgrnbmps.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ugtmsewp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3wzmblint.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xtrmtzvm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jzjqlykd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3unsqwmor.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zfpebxpq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vggykvhg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3gmetmmgd.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ixfinerw.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3gbdkvvkb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ubvkhdgz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3amxxvfly.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ihzimebj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3gylgtpdn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ewwqakoo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3olrcroih.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3yjxxaeoa.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3khyrknuk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3thlgovtx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3vzkwylsq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3vzwpzolb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3temgnbrm.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3tnhiprkf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wglqzakd.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kkonpeyw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rffvzjac.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ibelljqw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3xjtiamsz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xdgjmcze.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jufkactd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3izulizwe.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zxsbxzfk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zutolwzj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ptlkkmym.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dpzkhqav.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3yfjindlb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3azrlldlo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3nrpxmgmz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3pfirlflo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3qtrxiakn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3lbzedadw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3xmlkhcrx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ooibyqzk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3iaxzneua.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3fumcchrf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3tnlncmaz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3gsrkbzws.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ywmwjfhn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3cmglfass.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3jldojthm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3aegtlehp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3yvgiaeuw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qxlyuhkj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ivjthjok.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3hzwyuuhu.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kkxejrti.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3zmjvjpgs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3bqaigtqg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3vsbczypl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3hovkfnjp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zthsudtn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ewiiiryl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3uxexpinb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3bztovuov.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gofpmjdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bbwnhkry.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3wbhzqjho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdvqdqem.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3fsngjpki.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3rbhsfrpf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ztuoptvq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3hgfndsqu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jkizkfkx.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3exqcisyo.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3jsmvjetl.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3sohkfevc.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3yckuakbb.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3rlhrsutq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3adwncauo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3xewoxwnh.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3aiecxnxl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tulezrej.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3nuvnhjur.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3gemrjzgh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3lxxlgcuk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3myjxarrv.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3myasjkpi.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3reyetsub.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3xkztovzd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3iflwlsba.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sipytfzq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3spvaiepr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3zarhtcba.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3lkyerdgm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zvhxdezg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3spfrguzz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3mlkvdveq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3mnkauchg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dszkmekm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3sbtnahre.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3zrrjjqer.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3wpsbqibl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3qnexpyww.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwuuudyq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3vphpxgzt.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3dfhdefyz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3xygqyhkx.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3tpcyyeao.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3sjgzaqav.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ircwuppp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3oeaqsftt.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fpbppybr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3vpezijrf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3lhdbdqcr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3aaonodtd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3eyjlmiac.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3eagsruha.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zfrnhkmz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3bnzbxpac.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3qimzswmk.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3evfstaie.html


<!-- 参考信息 -->