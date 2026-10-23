代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3uilirfma.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3nchurqki.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vpumnydu.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ymzccivu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3hnitcfqq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3hnzssivw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3yzabtcfj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3cuzbmaxc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3jpagjqet.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ixqhxmio.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3sviouram.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3altckhul.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ccfevqjo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3kcyocrmp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3iyvxpcwz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3olkzioxb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xamgxkfd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3yodcjhla.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ezhvpnyy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3mgdaxgdt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3yaxzisxd.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3iplzstzd.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3modsyvlg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3vdtjbgns.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3gwuponbg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3yebaapei.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3bjsgcbos.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3uxibfomn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3hkasqnuy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ujqizrwl.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3fdkkdcwu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3thqyjzee.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3qdmzrgls.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3oeshmifz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3bumosfsy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3lzkaqpeg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3eplppcvr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3xunkoigj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cntrxsbv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kttimivd.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3blpndmtx.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3oxbjagjv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3iubycajc.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3srxlwhwd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3yujpayqv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3kzjzytkk.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3etmztuxy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3xyuatczz.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3iahedpbx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ibwvcwft.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3grwbzqbz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zdpdcyum.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3mrhnvhkx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3kihlffkv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3iujguuig.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3gmtysykt.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ssqyawji.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3unpfazhe.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3icrzfqpj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ustgoiks.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rnvebaot.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ihgjkzph.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3gyheesav.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3haorokmp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3stfftobw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ufembcoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3svxumpxy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3tgsbnrhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tyywstlj.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ewqwluih.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3umixvpfu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3nqoyqvtt.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3izzjrfzk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lqzzdigp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3izplunuo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ibemfozq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3mnwgwkfh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3snjvdblt.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rhmivnzc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nqskocmv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3mjqvfncy.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3qgmkftas.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3btownwuv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3igjgpqua.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ohmxwxvm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3oxocryfv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kesmjdka.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3gsninsqi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3iblrgchm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ppmqvcjb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3yqnxiyic.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3gfmnfhsl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3vjuufslt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ftgntzfq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3xipwnhpg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3jvohleko.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3knnrzkwv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gkdilhxo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3czebnany.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nidlumij.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pvyvsctd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3fasovmpy.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3kftbciwt.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3jiyucson.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3clvxttjq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3abpcydto.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cdjwmtjv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3tqmpqxht.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lmtipgle.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3angttkrb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zasnrmbq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ghsaqzud.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3enwvzhkc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3tdawzvjt.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3hkcmdgta.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3uhspvhje.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cztcyddq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fwzqvfok.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3uznmjnxx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3osydsxtp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3hsgolqhm.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3vealiwbe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wdrxzgoo.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ykcnfpzg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3otxhrojw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ajhuxyyf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jnddfhlg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qrdqactx.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3jcltldku.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3kqirgnty.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3fanoxhck.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3bbnpukeq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3svhflsuk.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3jsgypcfp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3wbkvqcgv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mbrhhanv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cpbckjfk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3qbcrjhge.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3eqsfighn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3qhgllfpk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3vuicqgus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rguzkssp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ghgxbfyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ppyreszg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3vmxnrjhg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wnriblxj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zcbcvikl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vejcgxsd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3amccjpyg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zevuzjra.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fclzytrv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3sitemhnd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wqnkkbtl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3flhgqboe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wvjpimky.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3sdherwof.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jhvctplw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fyoxfafb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3wytxivgs.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3sazjgdlb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fafbkdjd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kjybvsuu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3buyzesup.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3pjkcjwsp.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3zlbbdyyj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3trrnuyng.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3tzofbhzi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3uvsynkks.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3usgypxsw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ucwuxzyt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3fkknnugi.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ammhglqr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vtmrycfk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxxclcry.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3eltlcwsc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wcdlmmgo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3twlvvuaa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3tqvjgxbe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3arsigkij.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uelbqasb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3irrwumss.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xzojmysd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqjvcunh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ieavuhtz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dryqhlop.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3wucwchqy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3kpoypgtz.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xtibwpiv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3dfomwtog.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3dpymiioc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3oxrjcuxu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3blxnvjck.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hbfvtytm.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3druwspaq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3utkielsc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3couxveef.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3etxsgkjj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3uhujophg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3bgsgqcvk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3dkeqqrhh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3bizqkuql.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3vgpdzbxx.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3tthiuxjb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3uoavyuib.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3zcjjxdgz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3uupgvtbg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ibzezktc.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3cedmiaje.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3bjomlbwg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ipzxmuwu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vdaitavf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vrzphjrh.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3peobyxee.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lgzdpapb.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xtixmqsd.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3khmnwowx.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3yrgpecig.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gmsmjqei.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3reapvxbn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3covwbgzd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3uwqcumjz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3cgoragmk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3zkcmtbua.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cglcfrsh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3qahmoegj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3keqipccd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3onlpcgnk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3otmnxsaf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3rknxpege.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3repoqiju.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3bforqltx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3hmheutfv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3wsvpudpt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3weqiyrfw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ohagtzmj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3artsacxz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3loxqrpes.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3nzkmdtlm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ymbdcbgo.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3izoicgew.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vvsjqoiz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3fvutergg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bmygxqpl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3avwugufv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wplzjbpr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3jblnkwtc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3cwokmzod.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3evuouytu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vbpfvfgx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3vrgyfcdl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3livvtvop.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3vqopbclr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bdpsnskq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3veihdnru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mexxujwx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3pzblxyvs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3qgqbejrl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ihvyhyno.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ielwtgqe.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pqynvygo.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3czxytsgw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3osvhbkoo.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3bcgymshm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3inrusyja.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xnwsueit.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3equynunc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3zyvbqpgw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ocjtkgns.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nsllpnon.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3chbbcqzx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3wsxudsvm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3gjrlzwsp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3qmzkvwtp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3eyynlpmf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3qvzzgiek.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3jtrcolwd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3kikkiqgg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sgcwavhe.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvjmbpmk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3nlzqqzrg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3mnuaxeiu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fotmeoge.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3eosrqvrw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3qsdyjlsm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3yalsqhbh.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibwbddtf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfgncahb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3kldykfrx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3dmicadwp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3eentnavg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3vaxyybaf.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3hnusaryj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3sixyoryl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3qrrldeop.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3tscmxuxa.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3onjcqfii.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ohofxiif.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3bgtzwfmm.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vkozxapy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3wnwsnbmk.html


<!-- 参考信息 -->