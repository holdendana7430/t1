代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jjyazlyb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2srqtfbfe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xmcvigvj.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cukaqdvb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2fyvgbwaz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2uuoxgxcz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2acdhtqra.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2nyhljocn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2gbxxvcvt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2kulpeuqg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2vfutcxhy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2indywgal.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2fkrmxxyl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2sonhbqfi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2eyzkxsui.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2edcsusod.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2kajpiohs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2xoymkyyc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qqnyzoen.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2icmmprzr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mrddgpur.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2bdxobged.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2bxdlgune.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2vevzcqtf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ksgfzyjw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2cwjkxtyk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mnivxrzl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2hhkczmgt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2typpiitx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2pjpkjjky.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2lywbtudd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2dpiwsmsz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2vewruidg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jcnnxetm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2lssvuidh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2cmgdztsg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2wdsqvajn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ukaqiizx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ogdayvdr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2qcabsgye.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wyvrgapy.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rhdkfygv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2votmfnqe.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2eptprhdh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2cqrkkkkh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2fktiigxn.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2oasuztkz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qbtblswy.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hswniewv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2crahenmj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2qsegmdcx.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ekqyqthh.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2sqvnbrkv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2noiymnyn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jffmoswj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2xzgbgjhy.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2kwydqezx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2khhquhls.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ecixzzrt.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2tzotrdgn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ukyvljsd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2sqhuawae.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2udjuefsf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2jozzeqyw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2meaacouy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yhmwunln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2akhoknui.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2jlmunxgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2miqvmidb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rdzimjxy.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2klqqredg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2mexgsjsk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mrzxdkxn.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2cwbndozg.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fmkwljjq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2cwaquyii.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2uuguwuto.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2zyluzlks.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xqacdbyc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fbmpxxei.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2qchzkwvc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2sbdncmoj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vtknbixg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2umjkwrhd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2oeyfitwg.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2npgekwjw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wrvprauj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2pwnkwxwz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fciylmch.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2iuusjzbu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jxgffaih.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2whyaxnaz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2tbqeeygc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2jwikgwis.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2joopypaf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2oymrzclu.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2wuwygtci.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cdgxgfcu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2bismxjbj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2yahoocgy.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2apttxvtz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2gnjvjnyg.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2icywtqxw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2vowqvqpq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2rmnyixcb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2rzsakizs.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2sqkdncwy.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2mpygecye.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dcpzosqn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ovnfzypv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jyofqpau.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2unfzfnde.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2rsnanand.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2qpghoqdt.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2zzavtmsl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jlsinpil.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ocebgptj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wqfxfdjv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tjvmmbmn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lfrxmrag.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2mdtlggle.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ikqqwwsm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jphfbzdx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2uwbxniiu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2omhtphhi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2whmaiamv.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bxldzbux.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dpozojji.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2oxnkjfsd.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2gavgtmer.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ooigwcwu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ixmmpqks.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2objgavth.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2gptfgvoa.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ptyuxhfw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2bxryonvw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lntpskhw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2efkbqetb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2oyintlsv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2hdutagcp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2nbfxwpxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtigtxmv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2etjklmgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2posnzfmg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rnabmzgy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zbumaesf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2haylxjte.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bmgyefby.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wyhnvszk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2koqittfl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zoyfihhz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2wahnhbmi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zjkydfup.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ejwvnecr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2osbsiynl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2iaaztdhf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2cixwckri.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2arimpagn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jwyzwywy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2waapijvb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2whgdujad.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2dqbxjcoe.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2zewzmbjt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2qxujhqvm.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2pudxjxkb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ayzxqgjv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2fforctor.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ycbznllm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2pcnmgojr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2fionbxps.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2peepczju.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2pyoflqqf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2izxoqnpg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2arfsviho.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tcuuyisz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2puokksly.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xlypuyvg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2epwgrwvp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ywyeojxl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2btlklmta.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2bqotqdwe.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hygiidxo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2bmmtfdmy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kaczyhaf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2prwuljfi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2nugeizup.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2wtsyvgiy.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2dltzmrdi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ulbgebrx.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hyfqmzay.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2omjqmjqz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2pdjcyuuj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2aemfdsmv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oahbppyy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2zvmozphn.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2erlrrovv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2nqafgyox.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2cbzwkkgq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2sqzexkjc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2uhnlljwc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2rxjrepub.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2tdsvjkwb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2spqaqwbr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2phwlihfd.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2whfbszwz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2dyuthkpt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2nrviimjc.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2bstyztzk.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2pipedbay.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2pspexkkl.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ztffjoyp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ldileppb.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dtktjvki.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2loceqxqx.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ijvjgeck.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ajmadfol.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qnypipsq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wmkeokfg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2edfgiarn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rjtpdfxu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2khzsupcj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wrrlgczh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2yohsmovc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2elsvopjp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2smrcviqw.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2yyzcujxu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2kmjlxebd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbboodkl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2oluyzxvg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2kewmuplt.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2gjbqhhzm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2cttzlbzg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2fmodbsej.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gljameht.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rtlbbpro.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2btjgovwu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2lilefrih.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ogmmyzvg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ifxczsnf.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gpywwfwd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cjrqceeg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2qvsfripd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tsbtwydm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2tvpgjgol.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2mtvzollv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2bsceydjp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2tmcxlbsq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2nqfpjvbx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2oevarqba.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2zowmhdcx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ungehawe.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rqnqezjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhzpzkpf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2mtfupbqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ekyguvho.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2bdibebpi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2sjpvdwlm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2eqsotqlh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2nxmngmpo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bdjssbdi.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2snaujtfu.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2zvpmadjd.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2rhosjljb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2hagpefma.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nazuunwp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2rscqflbn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2jlaigxxy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2scllbxrv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2repmwovt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jvasndmk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2qzygzayt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2hnibinbf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2qzehsokb.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2kovawxrd.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qmxuoytm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2texitjyp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2hjlruulw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2dqdkouia.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vnvzgntc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2tqoeizuj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2vtkfktiu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2yjihdhmn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2brmvdjxj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2grtqexbb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2fnlsjqio.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2amygvmsj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2baiffbsn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2igqsyazr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2pgzgdxkz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2uwejxxns.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2rrmlxnge.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2vpdffjaj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wfdiuqow.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2linfsbkp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pyzitqcm.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2yymgucoh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2wiropkby.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2odllppdv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2flhdmrxb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ajnsuelw.html


<!-- 参考信息 -->