代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xyybbbcd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2oqhujieq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jlfzyelc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2ddhwdxjv.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2dkbnsepr.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jxhsucuu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gkujxzgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckpcdppl.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2flftcghz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ynzzocoj.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2hfnraqum.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2oxozvgpb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2bcrihqco.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ymcmowkl.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bkevdyds.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2clxxdlna.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xhpcwiip.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ishkugxm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qixinuom.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2hbezdzju.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2vazgynjk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2kvtlwhlm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wfzprvkb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2vypkhayx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2dfwuvtda.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2xwqwtntk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2cfzszlmb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2fahujnlr.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2qbwpxluz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ragotnqh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pthqazns.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vsujdxdg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jmscvqjc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2emffsxxf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2nildfbhh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2oqcpihnw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wfyrwkya.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2fbunfpvi.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2gkvnxflr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rwrdnzlx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2twprhild.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2qtjjjtms.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2nhlzuwok.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2bkzvonsm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2yznnquif.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zwicwtci.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2uiteuywb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2iycohbme.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2duwbsgqi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rkcahxbk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ywvzzzef.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2nvedhiye.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2rqxqnkiq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2lpovgerw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pfjuibkg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2elicxfey.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2kocuovdq.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2morkofjj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gamkoraj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2thyuldex.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xghewgdh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2mrystetb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2gaplqhur.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2nhajmloa.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uwuolmur.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2sznbiccg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2dslhywjg.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wydekzxm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ayxiqdbo.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2owbrqnis.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xzxwxfks.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2chyhkgxx.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2flgzjxcl.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2uvujhtmt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2wpnpqexn.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2uxcrkyaz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mkxbfbij.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lrimqplk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2gohiduyr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2cdtrfftg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2nxrqyrim.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2sltrcxvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbdtolnf.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2iwxjmrqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxifeyxo.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2eqspnjlx.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2wzftsvru.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2avesodqb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2undmdtee.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mjlrwopo.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2raqkjgqt.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ubvopwtv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2tdrnxmnq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2nodgvhuk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vcbgabat.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2viwtkdis.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2pttdhipt.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xrvcxqrf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gtcwbssw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wxorhyce.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dqvfvobn.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2zolmszme.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2unaocpxa.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2hyqmsudp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2pmgkiadc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ajbazlse.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2yaugdags.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ljpprcqk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ywkdtztr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2fdteuuqw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2rnjlnhki.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2rqennolk.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ywdjftue.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2xmalytqi.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2blpbyhmv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2krfgwyom.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vjcopwyk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2jtokyztu.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2sayctytr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2tdcnizdc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2wwhjqnte.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2uwwqlrmn.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yuujretx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ildfzxjx.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2chmvatpr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2owgouqeb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nqioyphq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gzjaqyzb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2dqbtbewc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ykgmwbjt.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2txdbwjgq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bpcbvqsg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2szszeofj.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2klmemzib.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sccszuga.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2xrhdrkpx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2huioggdl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2zripuuro.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2fjbaeksi.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vgwjglyi.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2cdtslkkq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ydiwtmag.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dagkuzyt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cejlpmbd.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ylqrxesc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2idwxtqrc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2tqdtdaln.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2tpytwuym.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2kmmrirnx.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2whrufvwh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2dezdecrb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cehbnrrk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mopgicfj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2rjowedmu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2czcbunmz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2fscnpgns.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2paxxmdme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fttlvyog.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2qwotktch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gzjxtaee.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2pogjsemm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fdgfgtin.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rtpmyfne.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2sckjlvxn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2eqndfcte.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yxyhxsle.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zfsekflb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2xkzhtkpt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jwrpglkk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2guxqhtas.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2yoldttpw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2tckdpurt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zoahncvt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mjydhqoj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2lwlqctnw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2miijnlft.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kowpkryv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2uucyxgcs.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2bvpsrvgz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2inbiegrc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2egoajvfa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2uopmasda.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2mphhzovb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wotgpskv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2wdhjcyxc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2pssqzkdw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2lfgcjefq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2kamlhmxf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xfxiexyt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wvwrovgu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xzhkzifr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pzsrlkfi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2udhoobrl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2nbkgsrbq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2iyamdjwu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dobqkgvk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2uhsqgfhg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2uehpmldd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2absrwpap.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovwzmtne.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ugtldsor.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ehnfninl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2podylnoe.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2glupccfg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2myzghjhx.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jywdpshg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2paasqxdm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pgpgmtav.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vdrpckge.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nqgaemhd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2nkcouvzi.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2tavjwcmu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2miquhask.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tcotyngt.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2fothnfeg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2yaxbgqlc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2xgkksbha.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2fcvnitpi.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ijcszrtv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2jrsvgtep.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2gxlojkdh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2yoxpsbtk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2veiopkfo.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2jzygwgtj.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qdtvlmwe.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2hxcytbwl.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pywyjuva.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lnocxcnx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lsqdvtle.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2aiiczpjc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2lcwpulzu.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vxijksvw.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2shyjmgiu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hjnfckpk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vaxdlume.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fllgbbce.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2udklibpw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2uorlyfzj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2gofwjenp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lgcbpxjm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2odhlvrcd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2vjlcwhij.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2rxymmqkw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2udczefxc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zjydjvqa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rlebgqfi.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcjildim.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2pgeqyrgm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2dyeugbib.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqczlfnn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tcgschhd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2qgoyppck.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2gjctszfn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kyhumdcc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rspmmoqt.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2iwysdugm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kibqoqqs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2hejenkkp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nuyyubnc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2qcatbrvl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2dpdrzndu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2updoiiam.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2msigphxa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2dxfguaas.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xttoslmq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2udgyecsl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2fpfugkbm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2axsqizbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqzuaztb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2kobjiwur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwxenels.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ztxpeioj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2wtfkghks.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2igefahnj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2hxbtsbsk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gfpeoogu.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2nnecaaip.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2gkrjtqvz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2qcgtygwt.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2gidzkute.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2takpckum.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2jxcmxmoj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2uqlxoaej.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2epyyrrmb.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2unrbwlah.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2gjxehppk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2nwuwckta.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2gdxznqog.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2byytyqbc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2biprmsfn.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ojpymffa.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2bmjqtuny.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2fruyvsdd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dsgakozz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2agyykpfe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2cjvuzxbo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2inyaukhn.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ffeolmoi.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2totecwux.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2aawaspsm.html


<!-- 参考信息 -->