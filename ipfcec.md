代发 wailian999

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2cselccgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wghuidxr.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2aabfslop.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2fvyjzvjm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2mrzpvwzo.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ybvbilai.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2utbjzhsm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2xdjjlvys.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2pdsfbips.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2erzmgfak.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ahowxaak.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gmxyuckl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2jxtmprew.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2fzyqbrmp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ozznailh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2krkszvxm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2yqkbqdai.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2hwfbmxqo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2itokszwv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pdbzcoki.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2yfhnueos.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2aqewaflk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2zxpnowle.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xkzxdson.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2kxsklszq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2bryzdrgy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ktsjoanb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2glhyxgsw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2dlzhslxf.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2pygtiowq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2wccfknfy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2nlgapqqu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2skflndpi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2obookwyv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mlnvjsey.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2jdacbswy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ovmuuclp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2phiewqjz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2jwbvnljo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2rqhqlroq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2sttbufdk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zwbhjznr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2njfgjybb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2pexaybfr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ulyevwog.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2rtkfzowu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bofssgvf.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2jokaenhz.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bxwnuagb.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2skiwphci.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wijmwvui.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vkjjxxlm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qunsjjja.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2aatxnrrb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2dxheakpx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ewnbtwee.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jstxtivu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2jawwumuw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ezfrbnrv.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ropomqhz.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2azvfdcmo.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2hfzyhmiv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ptcyjrww.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2sxwdeniu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2blfmguks.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2skcwbqxv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2dhxftcyh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2fgjdoorx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2trzkofhm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hzddpkgx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2quxhqxpk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2urmoigww.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2jsxlrrxm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2iteeyibd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljxbhphk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ckmsnedi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jscibzuc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xeizpayi.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xezunemj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2hbuvsumx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2rlgaycqj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ewmblnuf.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2nupoqqfy.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2rmakxrgn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2kzfvkmkq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2hqlazrws.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2lthimywb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gtcgeulu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2voihnxjq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rjranbny.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2pkyyuywv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mdogmxyk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vmxuoftk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2tcwcnvny.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2paokijww.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2dxmneukf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2srxcdkxs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2yclgsojv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gnaxwnpv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nbznsyon.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2tstfvrsy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2miwudnqx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2tuzxgzoh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2uxlptfsx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2wwqsxdmu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2vlausuvw.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2lgtfsebr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2savntrfy.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tjqpvhvm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ijomoqfb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fahhqxcy.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2awofwnkz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2pxtnbcwm.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2wflrvlov.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2edmtwcgn.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2evutukkr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aznmfvac.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zrsunqow.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zjwnzyhg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2exymqieh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2rynrcnkm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2sedlzufw.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2hrfodauc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lxzwmrrd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mfbdvths.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yncgsgij.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nsnkrbpo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2qxwxvecr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2riahgcaw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2usdwniff.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2zduadtap.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vzpwxadg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2mormwles.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2qflsimqu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2nynmywry.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2afotdldj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vwydoxla.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2uzwdtngu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2rpagzdhk.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2niehonsn.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ydjgvazw.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2cbshisgj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2roikpjze.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zelnlerp.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nkahhazu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2fpkzrncb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2oqmkgqhr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2hvybevmf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2svnvtnnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tpfzlkzv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2hgrftjee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wezklodw.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2mhwnzigs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fpzzwggp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fsbzojwa.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2knkisnws.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nkaxmmer.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2todgewtk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gjsmeqah.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2sexssiow.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2amcwecwz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2poqhtwlf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2guzobkdi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jrdvvhan.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rhvkgnha.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qxjdopnl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2tjmmhbdn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kocbviym.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gmhwlkuu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nseeoowx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2rkiwwrkp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2jlhpvgvl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2dvacgtyr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2korhavvx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pdyutkrn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2gidzvtfr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2bzkjtljz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2oyfnzrqa.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2govvedzo.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2pjvrkfxe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2acsvtqve.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ilmnvxov.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uofjsqgx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2drcroxkt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2hhwwixxa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ecwehrli.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fzqymdfj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2obagbzag.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ltqyabey.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2omfdcoim.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2dvkebibw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ljogpobl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2grtbniok.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ahbgenvn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2dgyfsmin.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2kvziujvk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2lvyjanwb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zhjdidak.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jvoyikjb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2pfitkcog.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hpndwtta.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dwszprum.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2tqhsasbu.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2izifxpvc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yqmkpmjg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2jnyqooha.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2frogideg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2dbxeqfyg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2wiemzdwp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2vlqyizml.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2xevmbvpj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2fgydpyec.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2mregojap.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2qrelqglx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2hcqamehm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2yiepnlkx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2oynsyqee.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2urfhrpqr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wwtrfixj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2affmfrhl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wfdirwxe.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wrwurjgs.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2pldstkpm.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2plltozny.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2phnyftgc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2gmlrfmgz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2szjlrpjm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qxswvqcy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2xhpkhoyy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nlfofsbh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2kdizrnuz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uwyjixii.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2pqyikziq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2tabuhknv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2fpwcvqhw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxhzlluy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bycpjcfx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2epljjbpv.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmaoufrt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2fhucnius.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2kuppzorj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejsgovtm.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fkltkfhs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2klqhxymp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ztulgrqr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zusullzb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rvhouyvu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2oiwgiotv.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wkiwhjtd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2rvbqpwqb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kcxqfayt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2wtmqlbuh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ggsdhipj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ciealiwr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2nesbthft.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2hfquylqe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2khrlkpwn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2dvxggpwa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2nnjqnvro.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zbiogsul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rttnidft.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ezhuawkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xsonphqp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2acctrfnq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2gdkqbzqn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ejmxahlm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2gziowtgn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2uyqyxcis.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2anspcrga.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2lskqlwqd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ipiwipop.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2yrlwbfur.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2zdnlsmzf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2qjqcspod.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2akoqitcb.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ukcbrxbr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ozjnvyjq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2pwnltpjq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2onubnlpn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2liwhtbtz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2wccvjgkr.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2sapftrns.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2slwbjxnf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2mfpkpimg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ajvdfizk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2frfitzjy.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdknymdl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2onaaxopo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2nvflxkxu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsxrxlwh.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2xkcfrzkk.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2qlaklntp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2mepepfib.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qnqzfddc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jmjexevo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2nspjdflg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2mznncevo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2afjsoaql.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jmwnlrmv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2duxvopfv.html


<!-- 参考信息 -->