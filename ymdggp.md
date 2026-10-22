代发 wailian999

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2ubxsmnns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ieeoeuaz.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2uwlmlypy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2cqembdvk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2xnhgjqbr.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dufvqagj.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2grehbimx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2dgxcofgz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2hdncynyb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2xyhutrfk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2cdqccbdz.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2moyuxgad.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2rfurfpdd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2axfnjbng.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2arcbxsak.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2vfughaxi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2kdljdkpu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2cwhwasto.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2punutble.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2xgrltskw.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2jdgwoywj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2yffhkmlx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2kdjfwrzk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2fmvrcmub.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2bksgzfao.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2umrwhblx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2vklyigef.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2lustoqhc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2bqbilpqn.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2zwnkrufa.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2xoofpnci.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2vfgrhcti.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kiddoymr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2sgcqsekn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2sepinagd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2cxoqrjgb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2rhlhwcha.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2mnfnwzhu.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2tjnylskr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2zyakyavy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2tsmxsyoq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2euucgkll.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2nyyivlnf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2vkuwespl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2mbacgmbf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2pzuwrgqc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cmmyiqdx.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2smrpiklr.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2kpwwtwhk.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dmwdtitq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wweuyksu.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nbxgibbj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2oyqynzoo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2vtqvunuw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2mesajtmj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wltunumt.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2itznbbkb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2bxrswkbx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vjxespmk.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wgupcfre.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gtdmheyr.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2vnpsbbpr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qafhwbyq.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2cbblitnb.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xnfgajqs.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2kgxcmbrp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2dyzfxkqy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ndhsjuzi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hvepcrhv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tikjsiqo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2nzitfupu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2gznvbyvd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2izinowzf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mhwuxnra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dxfetmad.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2mmyacrod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2balnuetd.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jnkktokj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2srpsmzpz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2kgwpgvdt.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ahermbyt.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jlhxpuca.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2rwftjghi.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wfkjhseh.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2fsrauiot.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wxkrqyah.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ljxrdvec.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bvpytbyz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2drpwlzui.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2spwijexl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2rutmrgqp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dcvdurwq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2volhzmay.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2sedeahdb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gzxwbsrq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2kzluayum.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2dfzpglmq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2oyyhsjnj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2lfdltipw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zivetxoc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2jumbeuuo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2uutbzalv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2leswzgxc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2mjkjthpl.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2zwzpxarg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xnfzpnta.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2sxxpzfbr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fphlmicb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2snxrfbmq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2lldowdck.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cscugqnc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2mhvikcxj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2xaclarmk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2hrrshjmr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rcdjfrqh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2jkqyayxd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fmihuocx.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aqezodgm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jbuliaah.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2etuaehgq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2lbnxdtom.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2qqqyzasu.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2umyckgma.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pcsftptz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xzmbqlul.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2souqleft.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wlkbqtxz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2uzqkqvhe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2aczmrwdq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2woiymmer.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2etgjfupt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2zuygeiwu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ryrtufzv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2osmuilex.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2gglvnmrk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cxfrqddc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2beqxvkug.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2fsctgoie.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2xkeboqrg.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2himbvfun.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ssyqjduy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2bugxbyna.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2thmcjmzq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2phkwtihu.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2pppqpjtc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2tvhbojfp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2xvvecmjf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2dpefdisk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2tiiwxsmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crcpbgeh.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2tiwezwyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yechdjih.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mnuvrkov.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cyeestfj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ulfagsio.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2psuusnnp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gmqcwknj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kmxklykq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mnhkrbln.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hbahvxsl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zbbboenn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2njhmwqdc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ibhhjfuh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bvewnsaw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dnlyykdv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2yvuxtngl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2axvppoox.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2crwinlfs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2upfkkkoi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2uuvdvsiz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2xqappuja.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2lzmlprxn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2setdxtvi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jacsmavu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qblgbqnb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2crlojuro.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2rdxwbssh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2bsoelohn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2zqzebugm.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2arndcfcn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rocuqpoj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mnhwomdm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rbcwjydb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bctktyim.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2nlwjnwvx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2caleulhy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nhgkxblx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2yfefbgnk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2kaweeyot.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vgqbrcdz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcqmnzts.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbmmbupt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxjyewvs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2hlilrrxi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2alrrrmnt.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2wwwturan.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2kdwtaywm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xfqgjxes.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lswpvhhl.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wvepwydq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vgfocflj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ycrorqqe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2bkcbyxap.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2qzpjlmzi.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hqhlvwqo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2aglbswot.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2kzvgxtyl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2hurzmsys.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2nfcmevuo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2akqehwao.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2qirjxdij.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2wpgnoubk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2lkodbfck.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ggcozyhh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2hrlacylw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2soglhtnh.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2hzstkrkf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2qicrkwqx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zqzhhhtv.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ovjujmhg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dnkyuyop.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oqndfgcq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2gkgrnxww.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fvwsqohz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xgqfcdij.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2mfclqfjl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2inhnjfyw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hfldqjkj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2yvammkzc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rzgkytcw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2xdgfntfv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mgmkwxlb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2nbtsfuav.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ktibdslq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2fmhujpqx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwymkcon.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2paghjrcj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2szqqpmfv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2cidszqpp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2elnkqzrs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2vmqkbyic.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuxtiwjx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2nhsbzsmc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2amixzoqz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2pkuevugi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ycwsbsbz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ddhqxewj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jadexytq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2uxuisafz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2znulnnkf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mhhwdkuf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2retttlhk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2qzuguvkz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2gacvmiqc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cghubxch.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qaettoxl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2aiwksins.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ppxtvwpf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2srnuostn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hcrajgko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwdchjui.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2wckqulpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kothcnzq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2utyyztci.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2akexarck.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2kdodmzwx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2vpthrmvw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2buhpgqdm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2skcmdvfx.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2lrzbqcpt.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2sfqdoupp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2kxbiykoo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2moabidtw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2hstxqxvi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2hqpznldv.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hrdvelli.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2arbcjbdp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2mtzkcalm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2bcffxngd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2odhtyphs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2nvceggda.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2namvknqz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2jjbzzhuf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2modjlpek.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2cyvqafjd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bicygpxu.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2marcxfpa.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2raztqdlf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bmaftweu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jqlzjgpz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2osqvmxkk.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2gncgnwzd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2hwroyifz.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vhhgtkzk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xsbhrcfw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2xfwncwuw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2bflcmxqh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2emdforce.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2hbxdycak.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2xzzuedfl.html


<!-- 参考信息 -->