代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2chmctfhp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ncxkbdxc.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2iwbakdby.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2xdjbqrzd.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2upacmjcu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2wehmqdje.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bpxuwhjy.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ccdnaqoz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2sflxfxrq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2jdgrjomb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2hmdmbqdc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2icaserbs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2tappzulw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2rjeyybln.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2laabddaf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2gjllylwd.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2rktlzycu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2havitsxq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jwltrfjk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2pdkraajq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ubodowkd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2rvcdjhkt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2evmcoojd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2uhuasaph.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2zspciiey.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2usfvzqdr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2xshiomxq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lxskgoli.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ffvcyder.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rsgdfjso.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2nncdgqmw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ogunkmnn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ozpvaotq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2zkpcwpjc.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2rnjrtywv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2uetectfh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2merjkrpy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2sanukhez.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2snfygkuz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2rczrdufl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2hdwpwfjr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2lfaqitub.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yfjfjrbp.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2yafprluw.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yqmgijpn.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2xiqosfcf.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fucpfvwb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zvlqmghg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xbhvyvpf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2zsxhukde.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2xutelsjx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2oiejzsgn.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gvhilhov.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2girygmaw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2aorihslr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jbmqbuob.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zwyktljf.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2mphvusgr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2caqxxjlw.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2txekzchn.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2sodrlvun.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2shgyqdxb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2mdtbcoqv.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2pgiygfjk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ftvqanjf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2urfzihkc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2zvmhcmab.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2cneiyxml.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rqyyohow.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ntmtixfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmdsvzdi.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2eggoistc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rfjuzqoi.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wexvjffx.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bnigkmid.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2cmqfceln.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yxbyvism.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gehifnkz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dlsaoede.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2wfndvhdi.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2uiughuhy.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ikgvjimc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2emnkwgbp.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2owuxxxig.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2mlzhwxis.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nmaaqjwq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ojybuvvl.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fvtqahgj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vqajcgen.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ewyevnxn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2solhkecz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2bgpyyqlr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2izecsohh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2azccuxox.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bffvdwiw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jzhrhgif.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2xwpcufxl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2wnsdcwym.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2uzkzdddi.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2vfkotsax.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2udgcvknq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fwsfbwzc.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2yerxwxzf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gofkwoim.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2aqzneegt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ivdtuodn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nfglcutk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2odcaigui.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2cahwhgtr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2zrwsfpxg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vjvpucfr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2nukzxokl.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uideflxq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cyjtkute.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vuqswuog.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ilpjuavs.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2zsfclxgu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2jlmmdiws.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2hbeiydkc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vxsvaepk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2dsoyrksq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rbqpdhnl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tieblygb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rawslsdd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2mcrtbzxw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2mslyflhd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2wpkiptuk.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2crwmnbmz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2tylnbdgk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ffdzozlk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lowpetes.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wwbnnefx.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qbtubjvr.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2kkgqgplc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2vdqlfqdz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2onvqulxf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2vylhmoih.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2xcdhttjf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2zabsjghw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2gcupnubj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2sjtpapnx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kcoikjul.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2rapanvpf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2bqzqyzby.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2xyrqwddv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pfdizkxg.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2tmcjqwrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zgydmtsu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bagrvujv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zjyiibua.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kslmddah.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cevjwcbl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nmmjaydz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rfzfhlvo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kbpqqpmy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2uwavukxz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2glphqedy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2prmqldqp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wsnafwty.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pvadrnnb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2izlkmsem.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zknmmmlu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2icfidtjb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2boykwsfd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2dqzjwubg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qiuhdmmn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2jejltgpj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2bxmpejuz.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ycsjqrnu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2mrvhlhqn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wfqxkyfj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hmhlwone.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2bhtxqfrs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2zqsagbmt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2miwnzrnf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2mrpjlpgj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2tmpfezlg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jonnaytb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2afzvmnpc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ocpeghet.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrqbtmwi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2qzkozutg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dmivkiah.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zqvrcyks.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2dwymkorv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xzslqpap.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lydghlfu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jjupqhfz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqmfcuib.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2orxotafe.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2nxqmrvvs.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uxnrfhui.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2nhtqjgws.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lmrfrabb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zxbkgpnw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vbczraib.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gxklgqzn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yujujokm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2vqzadzyo.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2uettttsc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ugaugcdl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2sgfmxeoe.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2oslwblpd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ogacqkys.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2zengkrjg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ftbbjdix.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2wxpugoks.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2jzogkxrx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2rechnlya.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2qurnwfjx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2kblrozaz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2wnaducix.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2mprelany.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2lskwwhgn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2frscufmn.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2usjtutiu.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xqjzazsb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hdqhlayo.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2fygbtbvn.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pyjsvdwx.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fsxzuwcr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bgquwzok.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sqjwxcly.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2skcqmfeq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2mhcotlxy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wrahdgxn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2wxmlycva.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ajngydiy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bhtsqpwi.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2lslzaxsh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2foabnazd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywzpfwxb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2pucazviq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ckjcddyj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjtvyhcq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2erhwnuxr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ggzrepwb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2durbsynh.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2jeyjnwob.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2bfgnflrp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2yucotjjp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2fjzlitlm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ufrgrdyc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xlsedfmr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ujqfgrnf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2mwddkafq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qacnhipc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2qvbnelvd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2jirffrsq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2yarcrxbp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jfblfjun.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2kigyklzc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gxcnwazx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2iskdvqmp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2otowmpbx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ubalgkpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nnffhywv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2qcyxumgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntsgmrnl.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ndyiblbv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2yeehrney.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ajmmdhhn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2haifpgqr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2yppfmvyz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2hgxasctg.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ivylbglw.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2vxidvmpz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2rgwxbzdg.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2dfdcqkmb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2qfdcjpxf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2gjtzbxmg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2psypieab.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2jjftpbea.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2cthpfeqw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2amumxntc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2zsollgvl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2cagtixji.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2pvomtsvv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ytxojpai.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2gtglljrh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2svxmwdau.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ggwndhch.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2itvjqnuh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2pyrmzxij.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2nvkgdkbq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2icxtafqr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2bwgskioe.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2msqzaxwy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2zowznmbt.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xssfxbci.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dnguhuwl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ejrbvjwo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ehtvzocr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2kjtaivch.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ghznspfd.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ovzdqlcq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2xssngzqv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2rercfkkx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2sbhcuhyn.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2asmcdctd.html


<!-- 参考信息 -->