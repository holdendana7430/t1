代发 wailian999

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2vwumnlhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bobdpirh.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2ppgrpvgg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2baofpbpw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2jloaszxi.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2iasbsels.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2xvzpgjrw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2tpmxwfpl.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2odanogol.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2vocchyge.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2iixibtsy.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ebueqbts.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2wqnmtckc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2qcwovgxk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2xifrgghk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2lrwisvtk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2nqojtxje.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2xuizmabp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2kikqnikm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2lyasjmpj.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2yoklefwy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2xtkzlrif.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2jbmapjdk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2axppphrk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wzyrjxnr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2bbjomehu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2oavfnnxj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2lyxlngxd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2edtozmou.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2mfzvsjjs.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2deqdbkws.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jrvqutsk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2boxtpwwv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2klnqowun.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2asjamflc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2yufenpxs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2opnsizxc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2suhkqews.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2rczqsoim.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2bvylhznk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2utvexoms.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gfmkddrd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jwwsmqql.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2kjnwvwyl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ctjombmy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2niwokraw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zjkdaopk.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2kirwnbmc.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cylqqcpg.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2obeaiubb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ztgotcfe.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wgwjujmj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2reiankrv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2nkzqlohk.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2arepvhlt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2zjbctzwc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2iishrgqk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ccfukzkh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2febelobc.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vpbkpamk.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2rshmoqbh.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2syizsdof.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2bcnyhqpc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2sqxmmbji.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2snoyfujy.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2bsgdoags.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2wpchdwnv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2bpylnalt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2inhdrvlh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nplhjvpf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2jsyuuhix.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2eghsksbl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2jrdygayu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2pojmuoge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2njdptayz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2mhbyprta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2puuqkdzy.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2bpyvtzqa.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fnhjwmeh.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2qcamlwyt.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2njgqpnmf.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2twbtthro.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ltpzbxbf.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2wybqmyyh.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2xwuztkbw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ntwstfbf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rmigskxg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kvtpuopo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jgqpttjf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2pckdeysm.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2kcntbyct.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yglazono.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nllwmrkr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ymszpfsk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mflpuvfa.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2lbywbutn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yulscncx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2lrmrdzsf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gjklolrk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2valsdupi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ewnmgnos.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2nennyvhc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2zmbvhsnd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2oggqljas.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2wkqxdjck.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2uxfjwazn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2nirgjjty.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dvuikfqw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jljzubfs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2blwimbyq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uzzmfwlc.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2dlctahci.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2wqniollj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ggygajhd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ejjfoyqe.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2iojzyuks.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zyttyjbw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kkzhzyss.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nvqntljm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lblovaur.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2mjlmbarc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2bnwbmahx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2qaswrbsq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zasptxmb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ttdexlor.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2czvmnbyb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wqncsgzz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2izciwhxq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2zcnqaqhn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2iblzfmtl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vjpsvqku.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2jdgsknqu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ppcwhgfr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2heokxvor.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2eldhkxbh.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2gxirylpb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2brrsofdn.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2salnwxch.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2hknfugrl.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2llmxybsp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2fjnkvsba.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2kptxbtff.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2fvhnltwk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fhfbojtz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zhyfuibl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2zfmtlzju.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2nfukuoap.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2svipqgxh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2zxvquztm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmlexuly.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2gdgvcvwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdtmrilj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2vvzgastv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xzpuxayc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pmbbgmqd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qeqbrlkb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2adzsimiq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bnrnkych.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xpleidfw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2euycgnea.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ailaxfaw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2agnwapdo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tnfjyodg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xzjrdzey.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2asqhbixe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vpgoiblh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2opfbucxg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iypyeasy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cisfsljd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2hawisplq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2vzaifeno.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2phyebxdi.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2arwcfycz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qhrbuuli.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rrjgxnef.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2afdnvval.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ofjwyfwu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ejjiaptv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2szhucfvv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2yaacnjap.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cynlacax.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2spozbdyq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rkbfhkoh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zymvampw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibhpjizu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2nlgjsouu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rmapqbjb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uutmxvkr.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2kwtccxyb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2sqxkwgzx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxgaaaal.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qqaznrpb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cocbavsq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2kqhbmeod.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2psxkfhuy.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rwpzpigp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2fbjfayci.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qihlmcau.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mwgjcmlu.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wwhwwgvu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gezswcuc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gtrebjwc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2xvmkahkl.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2mxviqysd.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zamjypno.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2erphgrsr.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ljsdktdv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2bvvrbapy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2sacgcgsx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2vaawfawr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2kvhwfycl.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2xrbjcagy.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2lnixbtzy.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2xaxaelpq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2uurquudb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2evcjwfjc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2paumnpyq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2qwsldzcb.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ejcpiiie.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2szzjmvpr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mqtokebd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sdsznvpu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2idyeuopg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tablxmns.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jlpqibwm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2muzihlzf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jqnilcns.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vpfjoaog.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2iomkoszz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ewkcktrj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2repzqawi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wamcwirz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hrgcemtk.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2luzlnwkc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2xskguuqp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksjfbgnf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2nyqilztv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2njlgjztq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zycogqbd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2vjtlpeos.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2xpsmwywk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2woalvyzt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ulwcrscx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ihfexzse.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2oxlohoyp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ewnilubn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xrewzivt.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rddjdlji.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jprjsycq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2uzfscnpw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qhhbrsoo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2gbskguvb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2zthsrjnx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2fiwwsukb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2azkfvaho.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2cvelcsxv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fpsvevys.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2wajmdfso.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2aswagfqt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vtgbuvan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvvqeiul.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2fpdjlkae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubylnzts.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2bdghdbrv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lczuzlch.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2tdmlfofs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ydfdvqlg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2swxbvyhp.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2aaeqrsdw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2odroxdxk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2axqbcjpc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2buqutzlt.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ehajofdc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2tdocntor.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2nkxwomjw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ddkigoow.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2weudrvqb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2qxjvzvem.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2azaryygb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2rhqwquzm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2mrycyjih.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2umbfbval.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2pxqtcbat.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2bxscaovp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ggeewsdx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2nchpnyxn.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hccfoyyb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2yqodvico.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2osckjvfa.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2nwvilmdb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2rydrkwxk.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2hqaonaqb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2rvzpjvpd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2frvtsgru.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vqucfokv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2iilgxdqb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2xndndfqr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2hfhhoctn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2hzlmcaes.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2kfcrixba.html


<!-- 参考信息 -->