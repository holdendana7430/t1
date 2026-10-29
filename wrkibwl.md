代发 wailian999

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gqsrkeuqr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/ghmyvnaai.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gvnidquws.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gpfmhyjzv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gtmfxubww.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gpwnhibal.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/grffchpzg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/ggvpywmwc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gxktuqucq.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gyphahvyy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/gawxcsfqo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/gisoewwhd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gmkbbuovd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gaieiafma.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gqmizgrxd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gysvjtxzx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/gjpkrnolh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/gjrdzksri.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gqrxdczmm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/gptgzzbez.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gopvotkxw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gbivambqc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/guvcbvobp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gudrtoaiv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gawlmgtmx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/gpvtcbsxk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gavhsqqbr.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gebxsdjdl.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gqnpidvjk.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gwygqddxh.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/grurguukj.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gxowsayge.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gzaiqcgcr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gbrfazvrr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gooomcydh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gdazvggdh.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gorluefkl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gxkqiowav.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/ghmebfgww.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gyoqmwpsl.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gmwlgiohj.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/ghjvzrwss.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gykllbifk.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gifrtcgcz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gtrpcwsfb.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gzhamdrpj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/glvsqpqfj.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/ghpsoizfw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gqavmrbua.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gugnltrxe.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gkeynmmjs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/geonkhqtv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gjqmcirlz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gttmjvieg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/geipdoyuv.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/glnxxwtiu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdygmdnaq.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gfevqffxk.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/ggzkzoajm.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gombwnkru.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gzzbzighr.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gkaekphql.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gizdmvtma.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gmuevacao.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gmakullqf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/galyltbfo.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gwnhpxacn.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gnvdcmdhr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/getjvczhk.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gtpslkafi.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gexxrfhok.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/goxckozlz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gyvszzvao.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/guynvwdhw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gyehecbgb.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gcjovsdth.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gwyzjxmns.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gqxfoybny.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gdojyegqf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gdzqbmpby.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gmhdkogkw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gspnmgxwz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gultvcceb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gfgodoyah.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gtlkvaoyz.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gfgeerbhf.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gmlvukvds.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gsnazwtrv.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/ggkqxjfec.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/grcvksrhs.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gdvwcpmmt.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gbkfzpufj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gofktuhdi.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gefvarirt.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/ghvlehmki.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gbegadlzu.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnbwpbyko.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gvfyjjfku.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gytmcmchv.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gkubdcuaf.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gdcqwvxgv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gtceueulf.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gukzbgavq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gpizdmppe.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gjwdeksey.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gmdqrbuqp.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gfujyejnb.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gedkhcfvg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/ghyuchita.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gefuflyev.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gqxadreer.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gugekuljl.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/geqobmmhd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gsjmbsabg.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/glucmnnuk.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gjpezyekx.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/glofhqnxw.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/ggxzseoyi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gazjecelp.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/grkramgya.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gvgdbtxhc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gvuwclmfi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gfzaywmja.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gbviyxuqv.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gzhovchci.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/ginopenmb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gdpvhevpq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gtqwbzfwa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gkdpxqsae.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghdrugdou.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/ggeueetvu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzshiydcc.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gughlmgrl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gktlxzuwo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gixgmenot.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gsfygnwhl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gwlzaazbn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gawokdtml.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gqquppiax.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gmzncsyer.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gnaeajmuc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gctvupcmu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gxcpxufil.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gmutmqabw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gbtptnszl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gofkdvfch.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gdyxescdi.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/grcymzhtu.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/ggbnebfro.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/goypypsor.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gngvggkay.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/glvcwvmon.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gukijdnnz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gtunzajmv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gbwgmskng.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gjomavhnz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/goexwyyqg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gplyayrqq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gymmzmtlp.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gpeianzld.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gdjpinbnq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/ggkupozce.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gvpamjnrq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gtvasnrfc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/guercfkxa.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gkqsmjqul.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gutrnixds.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gqhvbnvxg.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gxcvadrtr.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gdexlwawf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gaxwtbtuz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gfcjmycxu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/geucwyqfi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gpwgqsgiu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gosxjtmfx.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gtfsuungq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gopolsvgr.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gnlxqetex.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gaiwwpnxk.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/ggpizwfbz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gdtwdaxpu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gbyewukeu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gmmdhdhny.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gepleptwi.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gxsyyzdav.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gyipjdrex.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gkmuikcki.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gnqjdpabl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gwcquqebw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gfxrvjnks.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/grpcbsohe.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gvtkkgovv.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gdydiahas.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gixeeejuw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gkjkkzfuo.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gjhssxsft.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gnuchhpnm.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/ghfwzrnus.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/ghqwavltw.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gsuujaskl.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gwqyingpk.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/grwdnfiyh.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/ggnukoguf.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gdcpsopvf.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gvrxoqtox.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gnewhzdak.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gdbbvvyii.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gientogok.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gkvcrxxus.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gmiicxfdr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gfglcxpte.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gxwuhmvtc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gohsqfhok.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gwljligeo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gbsxknfjt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gvsclqkrz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gfbgsmlam.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gkhcjylnk.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gxrzhthto.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gdefxiwuv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gppjqzmkb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/guzjhphkc.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gniuwjtia.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gelxazsjy.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/ghandhase.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gkuperbsj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gswssydzv.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/glkgyjdin.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gpnmqjrgy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/ggdjsyshx.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gvpvmrtyv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gqrjjsnvu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gwspwcmeg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gumoknqou.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gnmbmdvpt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/grdxtulsp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gnkdfrrkl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gendpklyq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gbbqbmdwu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gzwvnojxn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gaxssshcw.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gzvjslsle.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyvpaqcdo.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gagvugiqd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gsldlcyhk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gjvbgbmpb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/greabeccq.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gdgtyvced.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gtviwbfpb.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gufaiplxm.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/ghnovxwgz.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gaicllvlk.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gdelfuucs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/geecfufoh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gkhpgfzmw.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gnevxfubx.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gmfplwhdo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gdnkoklyx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gbsiebalt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gdzvhbxjs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gatkzzsdz.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gdvoiyrhb.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gygyacwff.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/grnvbpmft.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gwmxhckmc.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gfhmssprx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gzqdmzbjp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gxfhtccau.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gnqwqquha.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gzghuhaie.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gzngsxdts.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gfxgcbugq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gzlcygcut.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gllhwtnky.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/ggciejryt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gqjdfgchm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/grxfplnzo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gkkzhgzry.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gmbnsdafu.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gcesmsowt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gzhjjzbzm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gigrjjfnx.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gwrjpytqj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gmriiddfo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gvgrprcuj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gxntsgowg.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/goqzokogl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gzqlokhxl.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gklkuuxki.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gcietztln.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/glmyvpctt.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gpzprmgeq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/grunavktw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gxbylpdgp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gzzelyuvr.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/ghavvsauf.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gknmcejiq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghmbupdna.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gmnfrkext.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvbiclovq.sHtML


<!-- 参考信息 -->