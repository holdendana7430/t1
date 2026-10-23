代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3kocmuupu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3uxxnugiu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3vzslbamd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tcnkwonw.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3qypgzgsl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ubgtptjk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3rmjqrwyy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ltxtwnoj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ahxhvrlm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3bqcqyujj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3uyinqyvb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3axypgqmr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3bkiedpev.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3kwccaeob.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3bepuhsub.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3dniyyglk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3pynkuruz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3gmcpzwxg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3dnmakbph.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3tywnavrw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3tyrxhlrx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3kpxvpizy.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ejeaudwe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3nsqynpwb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3qrqojwqu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3jugkjtlp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hrxoexvc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3eotzwmzd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3kxjlvlyw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3zbvmwvwa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pptvhpxt.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nxijcvcj.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qbxmoesc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3cwuzwpga.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ijdinijt.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vrnbtvid.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3yybbntzn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3uygzgsuz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3fmwphcag.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ibyfalir.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gqyhqbfx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3gmjgffvo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3xsdhywkc.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3bztuxuhk.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3anjcjzbw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3iyabwcav.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ibxpvsay.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3jmegmcgz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3gljfexgh.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3helfynil.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3gyluahbn.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3xwjxplgv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qakcajpx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3srbsrcmt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3shwfcmjn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3bfbhojbp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gjbbbthe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ilavctkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqnockwk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3acrafwxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nydqhvvz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3znzylcno.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3wrvymjkn.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3xdiswpms.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sunzmmst.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hqoefvju.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3uwancgag.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zinobrgc.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3qnvutgtn.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3zrvdrxpb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lnkicfbj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nqlqcfio.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3bkjftgza.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tqxslzir.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3kfxfjlbl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qnotypdr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xmjmawck.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3qofndhxs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hqkefzww.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3pjnzlbpy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3zhqbcgab.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3swcnyhvh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jilhrbmg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bnvdzmal.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3qjyewkee.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3negsjdfn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3basmivir.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3dwholppm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3veevsgcj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3mxrczwvr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3biqxlzbz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jkttaxmn.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rxvtlout.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3dshtqqwe.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3xwunaqxw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3esarftcv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3uffsmpre.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3fkbpndbk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3locjdbth.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gwxklgwi.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3redtxjds.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hotxbejz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hubpmjmn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lfyewzrb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3cmczokhu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3cjpochku.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3gipkodfj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3sdblwmqr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3xpmphqdt.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3userqbta.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rounyrww.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3papflkqc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3gselafjv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ezktactx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3egnugfxx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3uyzfvqid.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3wwofzfsb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3bwlewnvi.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dqcpujrd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tujsxeoy.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gfhvjfwx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3pfjipmlm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3teiqewmk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wgygnxhc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3xxekepnv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3huxdgpvb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ircgxryb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nwqzljbi.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3actcevuj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3auogqebr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3uifxpldt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3yrvqkvgz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3xvpfaxzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vwapljti.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3fvjrvajx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gssucabg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zuvwmekw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lsmijzhg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ycnrmhpx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dsvheevu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nkywrxda.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hswkbwci.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rjoerphf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3tqmrqefi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gwpsakok.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ivumvpuy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pajbrmfr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3lonzquhs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xuabvabn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ahcnoibv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ghoaaujp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bufwlsag.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ueejolwk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3yngfeljg.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3gtvznphe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3hbvexmbl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3knicyflb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3flbycyqj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zngylaht.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3cqtxnhjo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3wevjqtsw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3mtxiaswd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3wnpxmkia.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3cqbjxbje.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pbzrshmx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qxwcivco.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ppwlwqep.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fguateos.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pktnrtav.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xmicdjkk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eqiwucyn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wzmpnsqy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3holyihav.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tlehfjwu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3moccyvqr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxndovad.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjenbics.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3zhtwjmlf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3akxztzbl.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3eeevbpae.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3qwiuvgdv.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3aglrajzu.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3irlnepsk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fvmnzebo.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ewizkorx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pgvmovfq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3jrbcjkqy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ngxgglbi.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3iewwmdkw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hgvmgdzp.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3kjedfsls.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3qzxmeftb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3dgulqnwm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3kgxbijck.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3amnlqncy.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3wmlqzwbo.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3sdkmbjwb.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3qunvfwft.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3dweddeug.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3qlkaqdog.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3isepinls.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3otepedgy.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yssprdvs.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mepfxzfu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jndhkobg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rbucicyp.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3hrxbuind.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xeztnxbe.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3blpanwfy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3pontiarn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cfbsvrtt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3crvgttoc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3gwjrlpnp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3cjfwcdqd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3bzwkrqma.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cwzlnleg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qmapmuib.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3rhytcnwf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3yiqmvjle.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ijqhxxui.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3dxcpbpvz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3blymosya.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzzayggv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3fjeemqff.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3wvpfnhqw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3btuigwtf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gbnfkvox.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3utffacnx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3avppjhtv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ehwzhxct.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3tbrnmqbk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ackclpmo.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cvengdmv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3wrokzhkh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wcnmprko.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3rwctfhbe.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3nllgwbqc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3xeanhbxu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tzweldkj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3buefnxjn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lmztqzqh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3mrefnshq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3evhcdbax.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fqkwness.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3igldnqys.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3werpzqqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vgflipmr.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3vejghotj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zmtvozkn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3qmyusvba.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3zaxtmmzq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ubjovfze.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3orvsxlac.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3krcseinm.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3xnpsocxk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3adgyqykt.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tarunstm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3xczjshal.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3wlkriscq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3desdxkoo.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3hslzhxts.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3jowazpeb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3arhougvd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3hsrxhpgy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3lrqtctdw.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3hvoyxdvh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3yluuwkrc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3vqmdaais.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3nrywtbcx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3udhpsens.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3oxejwhoc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3nhsuirkj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3rbkeguii.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnffbosw.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3fahgrwcq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3wwsohnkr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3csgvqiql.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbqzrssd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ngzivpnk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3qklqfhlj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3pdrypavs.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3fyfvjvzh.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jvdglaex.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ipsbvser.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3qhgrnhad.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3juyebhir.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qcjhrula.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jqgahdop.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3yyngptpi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ygmilidt.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gwmkjjmx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3scxjnjqd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3bdsxpzrl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3asbwdqus.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3liyadlda.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vwpkbrxq.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cjshkoyw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3xdbtpmzy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3dewjsuxu.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3plxvmyyj.html


<!-- 参考信息 -->