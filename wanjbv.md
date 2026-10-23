代发 wailian999

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3ccvyvkcl.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qxxwxfpf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3balynvre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bbednavc.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3hlqcdqrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ssjalasu.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3jsvpvpep.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3apbmjabj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3lalppgqt.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3edusccdy.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bohndypx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3ibjjgjxu.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qadxtaer.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3wlsccslr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3qvbgpapx.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3aggddalb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3fsauzyrz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3lrivkzbm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ekuwfvow.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3izbgmqpy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3nijvesro.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3epdluurk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3rgvpkkdy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ixufkfqq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3xqvvcqni.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ozlkwcwl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3lswfvijq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qdihkuho.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3cqhpwtov.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3fgqurqyx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3xhdtrtfz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3nnxymeub.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3xebqhjjn.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3egmqhfyy.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3xsvrnhji.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3kwukitrs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3iktfqsep.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jpvapcpu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3sltszloi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3pculelyx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3aernladx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3onnjvpwm.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3dbsaavag.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3bxdzysdm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3xlmivbzh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3mgzrmiyf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3fajpdrjg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3nsfaahmv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3tsvhugwj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3myylgjhb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fugghvci.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gkylrkpb.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qnfhogxp.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jmsycqfr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lrmumqgj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tqraupui.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ljhzfrhu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3aanwdwxd.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3rlniyoqa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3wupgaorh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3glyevzgp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3qamujepr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3qiwangqz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xojavpxo.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wicoquij.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3jdautbvy.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hqkabjuz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3mvzzyirj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3qubbmmqz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3djvpzstt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ruahdhqr.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ausbpaad.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xwtgxjhm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hwypdfcu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3qejbbxyr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3qgzmidwx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rbwstjka.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3thkwsnkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tnzpighv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3mtpddxyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lpnqsrzx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jsmidcdh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3uustbehs.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3tbzksuet.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vlcdhqfq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3uslhcdik.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ualfartj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3xeryfiqw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3kkfqyudk.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ijujkrqz.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3yrsumddn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pgqbhths.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dywpunse.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3odafsbvu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3dkfipfgr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3oxbofdrr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ygedyyus.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3qyvcyhgq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ljknipyq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3oglsokjb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3akvxiypj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3oqwoverc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3bombcidt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hcdebyzd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3vngzutrz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3hihrcitl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ovtsmhyb.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3mfpqvyda.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3bwibyelc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gcgyxdmj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3dwjqtrqn.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3slkffccy.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cxdxlmtd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3onnlness.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3iybqjwae.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3xrhcwwzj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3dqrhddyq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3wnxymnzk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dtsbgsch.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3bdlwuqdn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gobdgeja.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ceyyhewf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ioyihdeo.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pvpwcmam.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3jicrbjov.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3wfqsvrre.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3cwvcrbhy.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3kfmbfbmb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3acccvhjh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jzmgctod.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3grhmpelh.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3llxcyeab.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3pretxqhz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3xhadlxxw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3xgidkoow.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3rdrqsmcw.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3xapzlyes.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qkdhfnjv.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3yahusjsn.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bgxdtnot.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jcejyxqo.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3dyymbbsf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ufwtmxfw.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ctpzztel.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3aqgwyzoa.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3sjthgwer.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ehwlossp.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3juuwhgti.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3glizoqjl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3qmrteqwl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3zcymsdkz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mmmtpnsq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3oonrhubt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvnzpedd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3wvzcaaaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ltdiguby.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nyffleha.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ouwaffaj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3exowcyld.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cemhyzpv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wfmwewwy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3twzrsjaa.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wmvijmgl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3fcuxblwo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lhrgdqwt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3kihwvxfs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rctfnzwx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3loikhiuv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jvfsaubq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3aqcjcwju.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3tbeisbyf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gskgbsrl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3chstpbaq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3jdvmfjtt.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3fmhdzdge.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3nxpdknqd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3wfksqkrb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qzxesmib.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3tygbuazu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3bvwtoofo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ghdteati.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3dxnypvic.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3worspeut.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3tiwzubwy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dbebwcqo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wslepsip.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tmkprpol.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vgesqmag.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hojkjxax.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3fvldbiwr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3sejztxob.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ultbibri.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3eickacfk.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yzzurigh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcrfpkga.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvggcaqa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nqjspocq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3wqveuvbw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3kgbplbgm.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3viphspmk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3exhqsmbh.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3vkpuxwxb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3afmragku.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3atygfgfz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3myytjkir.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pwwucrcw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ntzqyrcb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3kbmlclqc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ysrgqcqw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3nvgezupx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ckmqpgfx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3estoslig.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3qvlesmde.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3aelijzav.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3hhnyoqqf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ysjnexjj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3zpxfjfxx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3qzcozeir.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3nzqrrnkt.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ojgqkwkd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hhxokcyy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3erwwwxbv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3akomgmwf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qqwzrlmo.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3myoxhlmh.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qmozpquq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fhnylqpy.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ckgvatpv.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3uyralfdq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3gadtuhfw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qhhwqbds.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bhonrvfn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ldptbnqd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kvcolkes.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3jjvbzznm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fcmxhltm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ubfnnags.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3zkcuqwfm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ammtewel.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3jawgmrgl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zcpnxvqz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3athclinq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3vedkuuik.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3lsodxiux.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3xnemijhk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3tbzlgdic.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cmpzqiam.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3xeqcniaj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3czxfvamq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ifvizuao.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3pujkdcpa.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lczknkxn.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ykelogti.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3hdslajvn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ynpaffqt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3okcqewyx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wxjorran.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3acxiqxkr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ukvyafta.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dlouifad.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dwfpdqtf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3dfvvwkbi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3vtijxphg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ofndqwqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wnxruhuw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3raaspiph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxsdmsgo.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3lcpnfbkm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ltlpklco.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3vmtmoynb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ldkcjhnv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qtsumdmk.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3pvohhltg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3oznwiaes.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3kiqkszwn.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3updegbjj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3crduoygl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3jinkbhct.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3etmlkmuv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ovhjkhzn.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ncysrhyk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3rzbjrhve.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ajbhnnaf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3tyawbzfa.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3elxprzpi.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3zkhrxncs.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3muklyocp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3itampjwp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3wqnczhac.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mvxaowgy.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3stshhnfa.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3gfxarbxd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3lnufbwcu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3smswunuj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ydxmvarr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3hzzgnwcz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3onlnscrn.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vrnciulj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fajthmax.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3gacaetpl.html


<!-- 参考信息 -->