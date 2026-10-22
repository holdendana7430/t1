代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2spfvzkwi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2dqkapyig.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2yjiclckc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2zckeibvw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2lygqildb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2epdbufps.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2hvqdnuos.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2xaavvutm.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ynwqozdf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ptcowihu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2xijxbnee.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jalqubcl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2xbhvklqm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2xucfosta.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ztnsxnvd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2elqpvdln.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2kstooxys.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2byekfesf.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2llemldjl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2fefzgobn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2vmteclbt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2odapdeus.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ciidhiio.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2zjersxeq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2hnbrbprd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hiidbvbx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2odyrdoog.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2zfavmxnd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2xfxwpjop.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2eqiuvuxr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2nheonywc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2mpmwoacn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2udunpvmn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2vqmvhhyv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vfxlflip.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qppomvtu.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2pgilzirg.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jvjaoedm.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ebmkpgnd.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2evfcgvtv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wzomojba.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2rgauyvyy.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2icqvxbxq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2joqqudrj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tsagoeer.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ynfzspzl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kesfcpfz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2esndnpla.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ftifxeop.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2iuesyhku.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rmkldzxm.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2wzvxgokx.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mizaxjwu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ssltsmjb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2kysvdrhm.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2mmeggaas.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kwcpuoqm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rjaxlczi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ywmmswks.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2xyfppsic.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2omperytq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jcsrkolu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dotpogdb.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2fpphxoun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eeylnlda.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2rnzkkccg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2obkslljs.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2fegqkfce.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kwwonpgd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lzfeqjwj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qntggdys.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kvgzmxgi.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2rzbpnhuc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ibzwbbix.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wcwdmlez.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nphghfmw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dxdremzt.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lusmuzkj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lacdotdt.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fgvvssme.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2shjnlubv.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2bgzsrzzi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2izruqyvj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2bowvcyaq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tmqklmps.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2zntytjbr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vnjqklrz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nlaoxfks.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2gcwjquzw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2jfggprke.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2iatrvlya.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2seozfxyf.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xvtuymly.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mpaonxie.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2afjiekgh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ckpgmvwg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zwenlouo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ujtsxkjo.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2mwfhspcx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2bckhagjc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ejgzswop.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2mzqvqygr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yevvvizf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vcmdmbwn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hwsclufx.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xlqhnzxn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iwjxsjnc.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dphgvoql.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2lkekwadf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2aebznekx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2knyzsecd.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zbvnwwvz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2libykfzl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bipseddz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wxhakgkc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nkmusmud.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2wlltzqga.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2kmdvtxrg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zvjiykgw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2kweojugk.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2cpmauhwa.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2kaffwayt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wmzfttdz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vjvscorx.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ijlarspe.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2fhfzmwur.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2nlnctojg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2duphryvf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ecrtpyze.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2anxmmbgf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2prmhzwmu.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hwjangxg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2brpvxnme.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2boekdcyv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2hktosfoh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2bmhfupsb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2qflkpmkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jdhsbmcc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2dsbjbedk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2msinmhed.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rubrthge.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kwuhnswo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2trasoxzo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kfjbumpi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fhmyshos.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qzfwsygm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gscnstnb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2roesufrm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gpddyaon.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2gztviywu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2evdmyfyl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2uepeqhal.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mmwagdwp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2asvzcdff.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2smhzrngt.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zdyxawpk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2khkidhhw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2nakqzmbs.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2zlzkbvry.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2wzuguaps.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2idkllwmq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2agoidwxk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nayrxwrw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zsbnywjw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2hncoyjjg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ehmzblfl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2zsqhahfy.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2tscamhlh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gyuwygns.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mzfgnyqv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ijznqjvc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2abwyyqfe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zitoqqio.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2rqsmfyyh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fihcmhkx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wvqmjexo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2fecueays.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ihpbomnh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxzicrlg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xhhsxctb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bqazgwke.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2rjqasgjj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2oizwtxzg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2tdqlbonl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2aixmwgtb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2wncqsgvx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2cknsrarn.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2pxojqdhp.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2aguolvdn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jejjskfu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2procurku.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2acueruhx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2rnwrmwna.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2fgowjstp.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2tdyynghj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2qwvwydwp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2oeneibzb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2yexfaxwx.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2fxlueirh.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2cydmjtmp.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2gidljqxz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2doqnhuju.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2xikutpkg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2rilfetlz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ncemowkh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2uiirvfcu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2irjnyngu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cxcjdyax.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jbavbjcu.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pldtuugz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2svcdoczc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ryzmdspt.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nfjsjzth.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2uawtuvsk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zzvajhyq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cwindiyn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2tdryszzg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2msyvcekm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2gsmxghbl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tltesbkr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2yqemxefx.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2mogoqfet.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2nurqpvkk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqlqxjdx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2qwxvrqkr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2sokneayd.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2mfsywzdr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2sojeawhu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2shuzwmhi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2curoytpx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2tvchjekl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2nmgwoqiu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2muobcpeg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2obexxrmo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2zirsrjod.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xtwrjglc.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xtbqwwww.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2grjqiceo.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fxjjvhvz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2dctbhagx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2sfbyouuk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ligpcxer.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xzqmvsjd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zpbxzfuq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hdezvppt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2hewhxory.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2quviphsu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2nnshtseo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cpfhfwfd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2huedsojk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nxlpaiao.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2bwxussnh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wurrlumj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2locffgbk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2zhbklriw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2stzsodsv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2kjenktdy.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2zzrgttsd.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2nvworqtb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2wnijixzf.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2axlwbfpa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2qcwqhpqa.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2esptgqkz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rxtkscmx.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2azckwaft.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2bnduecit.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2fzvlmkms.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2gbdeepwj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2zzayhlyg.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ojuhpkmm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2cqormrdc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2wzlhpjdf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2iczmbbqs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2uaxgixhv.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qawgvyvq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2dhdjuwvb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2kmazzhtl.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2khbuhmwg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2kkddwxhw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2wkuguast.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2btrlrvyd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykxxlftw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2okjlhbep.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2rzlaprjv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2gbuvrrja.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2luushtgx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2bskrxyma.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2phrokfsw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2aerpavvf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2aivspwvn.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xwdkanao.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ecdiwxdc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2pxptombf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2egchbghi.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pvztdfij.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ewjkglvi.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2cwfgwrut.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2hjfumsbu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2avgmgcck.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wibnwily.html


<!-- 参考信息 -->