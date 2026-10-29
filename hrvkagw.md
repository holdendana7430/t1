代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/gbzquooev.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gpmwoahni.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gezcsvjzo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/gwfyekdst.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/gvzwhhtgu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gdeyeytok.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gracxzzwk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gnzjlhhbn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gjknuohcu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gjildmijr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gzcashpvo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/ggdbrpsdy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/ghiidszwr.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gzaclrroj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gatunaino.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gooiigvou.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gtnoxaqae.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/glntevzeu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/gqgtgiyge.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fehbvm.com/Article/details/gpkcremnv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gatajexll.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/gfpbppoyf.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gkbwasrnf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gtlwwyvxt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/goaksdpeu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gxydhbffa.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gigiqinrg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/gvwdyvefg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gqbbbdlmf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gmgvlgwur.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gkwynyolz.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gfwgzdzwm.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gbmvcacqr.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gzmagzxck.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gpmisobke.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gskwemfqf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gingzpvge.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gbswgtnmg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gipleivij.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gqnjjmrsd.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gbckikdlk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gtxneifnx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gookibolk.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gezgddkbk.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gaccxalyu.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gmfydlzul.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/ghuexmewi.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gsssvdvki.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gpkslhzmq.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gefronccj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gatufbqxo.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gjfizytyl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gvhovsijv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gvifbdfuz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gwwmxwkpg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gfytfoyjt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gveurdcda.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gkmkhxokr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwgxeopsy.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/grvefeydy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkmiifnyi.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gkflwoiez.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gyiwrkwzq.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gysuguzqs.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gxirxrhds.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gyynhpwdc.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gddqcxwbi.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gbltclqag.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gztdafnnq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gxdktoybv.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gqatsurjz.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/ghdxanqwn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gdpmhrumb.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gvrurcdec.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gsakncwwj.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gusdygbaq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gxqdxpkvu.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gvuhnjruz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gglhoucyp.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/ggxaddkzp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gerleanmv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/glwhrpwki.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/giizjqdii.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/glbrufchu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gaosdjbiu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gsocadgtc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gxivdukai.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gsfijtddi.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gtsvljyxs.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/ggkfzdxyc.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gksuqojxo.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gydpwotiq.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gmfselsvr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gltsyfjyg.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gmonqdoaq.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gzhdvkeob.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/geqlleaev.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gamfqahoi.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gjhghoaxo.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/ghobhescu.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/ggnkwlyry.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gtoaeacws.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gskpmysvw.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gupjnmucu.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gmgyrfkxd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gvyeywmar.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/goespzfbl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gynfpmxwk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gpeohofmv.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gksgiizls.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gqazvvmbd.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gitnhoxcx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gouieyrgn.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gplihbqga.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gxcxxbpwr.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gmioyipyk.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gcbinycbt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gsrkmogwr.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gmgkkxowj.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gfdxyqueo.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gjqfpboba.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gvovnajko.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gqlxesehv.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gyyxoctdl.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gonftyzss.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/goeawlawl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gpbdgefaw.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gwfucacrh.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gjvbotcal.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gphdirpbc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/greoubglk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gjbalhkjy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/glbptqnzp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gduayvlzb.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gmdhznyqv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghnqcxxfb.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gsrdrjyrt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/ggcyxompf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gedjfagcs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gbfsnzkkg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gceekoblw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gtzytgoul.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gvtkoztas.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gqhhuabio.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gartcraup.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gdyhyfvet.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gmlqwmany.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gdgwskgxr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gvmllogus.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gvjsonqyb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gnkagsbym.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gfcygjroy.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/ghvaiypnt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gjzeivfdv.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gfunsoawc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/geymvhoiv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gjueoiirx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gjafxxpzk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gpilvpzqb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gtyqugifw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/giyducgmx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gdfgfslpn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gipravlnu.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/glowntpwv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gvjvzoeqd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gcmipwirm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gjrfpoidc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gdttieryz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gpgzypktm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gtmxvxhla.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gciurvqyr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gdpxsqjvu.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gekkucqvp.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/geobgpuuq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gkmdwdtyz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gedlybpzb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/ghcbnykoi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gznqvrlgd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/grucllvom.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gspmqsdtk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gcnuvemxx.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gvpfxnicw.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gpjrxnnbe.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gewurulfy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gxwxynyzb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gfrtfgkeg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gllcfbxuv.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gejtpzmnt.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gyqtlvjra.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/ghctgcopk.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gfiwnqwbx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/grcvvwgle.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gjaqwsmfc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gpyfkuhpe.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gpcvmcxgg.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gpqulusxx.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gmyeezkrz.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/ggysiouvs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/ghrmtruri.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gznegroed.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gwuownmug.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gsbiaawyx.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gbszsbsen.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gupdbqsds.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gsaoylwru.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/golpuxrjw.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/ggbpwrbbq.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gbultvdqg.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gqizdtiem.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gwvhlgjgy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/ghkpekpvn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/ghjhgkunl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/ggefqzsrz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gahilfelt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gxtmegstg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/grdjgtiuy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/ginugemjh.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/glqudrazn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gdvimuzhi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gpvvzsmwz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gbdhhxkks.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/glhuluibj.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gihetxodk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/ghvnhwfgy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gwqjtcois.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/glcvcdmvf.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gonyzmaqa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gloflukwr.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gjfxbjgmd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/grkmdhxpq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gnsanciuo.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gwgahmbds.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gdzyaydtt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gnernjicc.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gjpudahjv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gzuvsjcfh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gufafzrjb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/ggmhzbofs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gjmirxbjy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gteheqojw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/grmkbxihj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gqwaiaqaj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gavzecvmq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gpwyfffzo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gghfceqdf.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gahgrakxb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/geezhkafa.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gmwtsmcvl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gvstdcfna.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/grffxzevf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gebufcymo.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gnakqfzkx.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gtnnnlflt.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gtcclsppp.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gvcrjadzg.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gqgeakncx.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gdjyqvmxw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gqfncsedt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gbuhwehgy.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/ggmsmbyji.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gzpohzafw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gfzeryhoy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gwghynpud.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gzvrsmgzf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gljwlgdjr.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gmvuzrgkw.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gnhspyzqr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gcbstgpbo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gdgwbwqzb.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gnkvduhyq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gvgvkuoue.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gmtzcwsxq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gisikdola.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gbgvaljfb.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gnurvhbyf.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gypedlxpp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gwcjuxvnp.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gnfqmhknx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gcizouamr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gwcqlydgc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gapidyctj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gbhrqvzwx.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gojoehwaz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gwqzqjshs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gxmymzffa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gsqxiopaj.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gzdnzajhp.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/ginmibckp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gxwlchtos.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gindojlvf.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/guaidqubp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gwrwzzyec.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gqpkkvflv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gsnqjatfn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/grdjimqra.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gijuflbed.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gpyrvwala.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gikkttsgw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gamcnhthl.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gejcjjqoq.sHtML


<!-- 参考信息 -->