代发 wailian999

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2awgfhyqr.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2foepreqh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2tyfcftrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvbfyhad.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2rfjhvxkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2osxurxfw.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2ykegkvia.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2wnolsojd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2uzjdwzun.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ixsckifc.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jtbkotrk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2wrfkuqgk.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2yurbxcxt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2uqqqaunl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2iqkaqnwb.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2losbbmyi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wgdxjfkm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2guiomcxa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ogjdkfwu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2wyedtker.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ausijvho.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2myhvvakw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2thexwzkz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2kyavrlyv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2edeallnk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2nkvqjvcn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mnwbcbzm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2glcsaxqy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2mjnkxeye.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2fosyqpsq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2elgpneov.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2miodmmyf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2oryefvqi.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2pocvpltx.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2lhyhhiul.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2lvpiuuxs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2lzlqkjxk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2gmuepplg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2myxyyqef.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2dbyhxshy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ygamqmus.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2kamcsjrr.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2cnnaiojw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ciodmpww.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2psdfsytl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2fxkhirzo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2dviezayt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2etyldoju.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2xkajbtts.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2yugissqj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cvjjhnyo.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ltdxnuji.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ozyxjzhi.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tutjrbrv.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2njxuxity.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2timcferl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2hoejlkyj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2rmccvdgb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2lqlrytts.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2wzslfakd.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2boqmyrvj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2jnltlbof.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2fibazihy.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2pdhdmvnd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2gdcoiisd.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2sqrppuzn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2oalzcdtq.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2lnbadhmu.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gmungflp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2dkjfpcna.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2iurpgkxe.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2oirigwiy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tcgdfkaw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dphviyhk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2nzflprva.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2rciwclqj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2svlhjpik.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2wfnhntpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zbnoovnm.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2gmfjnlmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttuwrded.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2yccytzcm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wrcfjbxn.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2fhjwueae.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mzuqaiji.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cisgvpib.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2aajlsjid.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hqfkwzpv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2hwulcuuq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2nsfsalgc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ibellffu.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gdcsxfzw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2yzmpsjjr.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xdczovtf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qjvznzhi.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2btxhwjup.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2aotvlkwg.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ymvphlwm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zdbszxvs.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2mtpfufng.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2binulmnw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2mjawjetr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hhwqguea.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gfktswsk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ztmijbbx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2whmrhmyg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2oimpmssk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2kusyyweo.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2aslazrfi.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2czxtqppr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2rnsfaczc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pbvivtll.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ntdipwyn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2jselcqyt.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2yaujdyqn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2loxogzqd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2iloysncl.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2iplawodd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zpcxqtlq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2cdxolgsz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rykorthi.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tabehjys.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uykjlgjp.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xjhmufxw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2uihwstym.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2tfjhufls.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2wtvmdvxc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2dyyktjum.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2berejond.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mzwtkaoc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zzeqxrhj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fflmbbnz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2hitbcpev.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2yavrkdnn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sccofurq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2xnjjnpjc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2okjrhnia.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2fschrndx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qynqgcfb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2izznkzpx.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2medrexqt.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2kzvqwues.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2scormjid.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2cnivhppw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2twydqxct.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2fjulewzi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2perhsdnr.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2eucfcimm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rlhkukdv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2udwphdxo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2qcubebxp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2epcgaksk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2mgupmeol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gcinjmqk.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ceptvkdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvhdrflu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2gcyfvnsm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bgvlhqlp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bfjoigsj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dolszzvb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ltvkqynh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ygdylhdq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tfwjirmu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2esudrctk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2supvgsvs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2rxhyxzmy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rmzovtxl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2mqdpfgzh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yxjfanqq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2grmimjsu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bpheqlux.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2trpgjgjq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gacqjnxj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cxjefjgd.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2czefihsf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2trjohymg.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2wwwjdesl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gqayzzge.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pisfvcsb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2wraxysef.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ozvzogfj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2jhduatlf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2menbkcfh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2vxmukdcw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2gbodpwbx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2uotzepow.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pndoinen.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2erpsvvkf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zcuadmqf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2gybxnlco.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2lxecluch.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bkxipjtj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2hcolfenl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2grlfwsnr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2acrqxufu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2rtulpayp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2yaflsksw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2blsanezn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2rfhjxaha.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xciwufkd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2wsiiclay.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ilbvgqyl.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2pmccaxsw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kdgpwdej.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wumvffbi.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cetfiyyj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2wkgvewvs.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2cgoufrwe.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ixhoyyqc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2cngafonz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2cdiprnak.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ygweydfz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2berbvcfa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2uegincpx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2pppslmne.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2qtfzrhdv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2rwadvcts.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2gavpkmry.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2yyuujunf.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2rslgwukc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iaagozdy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2uudhxiav.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ubfzibhz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wwzzrkrj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nrrhrkus.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2owuxsqlt.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2tmmlgvxp.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qmbqtfyj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ggpupili.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yxqunugt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ualuevah.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2knhqzfxj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2lvleevdk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2nnnonnpl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2hmmqysvu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zxywojcr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2imvxcbxc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ykrdzlma.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2utdnderx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxbpqcco.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2uzbzzqpi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2eiuplvep.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2wpcrmbqz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2zrydxmop.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ynbypmtz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2bdplbamw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zxnpkjdt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2hcgyrymp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2zlqjuggp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2wfrueski.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kqmhqeoq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gtfmeaim.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jrwyprzx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2btdezbee.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2samyevuw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jnqmryvy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2fyljhnmk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2rdsqqqrs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2aoywaeuu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2munburwa.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2wrethhnk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ervbjuio.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vzdfnnwv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2boyqqtyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tutyksuv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2dxnmkotz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ltythmwc.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2urvwbfwn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zzqtnwpp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2gvmxaavv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2smhurwcx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2tljwfsko.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2sxdsxrpd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2dmibrlod.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2orcrmuxc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2niimizbr.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mcjqbtlt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2zjzplwnn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2usohwaao.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2sagqqmcr.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2eyochhmv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2lqdtihmp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ppjclqww.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2nfktlmjg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2tmewuqmq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2aktvddhu.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2enxjprpk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2jrbaeajf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2gwuvzoms.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2knsijcpj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2nnehubws.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2pxdjtijh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2njuenzcz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ywiyqgfx.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2sbckrymq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2mmgedknr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2tzwpfxsd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lylwtbam.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgigznyv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2kkuwnzmr.html


<!-- 参考信息 -->