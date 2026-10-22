代发 wailian999

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2zfvrtpek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvypcjlo.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2hgvqleem.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2evieexfx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2bqumdoxj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2onoyacin.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yjyadakq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ajeopjwe.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ifwziyzb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2qwbvzhav.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2lhawxulz.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qqtyflkp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2dwuhjoen.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2aoicidom.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2wkxmearr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2grdpqnem.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2uxzzdkdh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2svhlowif.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2tjzvcodb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ysvdaknz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2rttcjszl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2iqreaahc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pazuzkjr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ecfodyrs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2erayduts.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2bhkgholk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ujdjtthi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2dtrbaayn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qkbcuxzl.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2tpwhkabb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2nwgdjtbi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2menrbcyt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2wacqsiqh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xrtjewzn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2plrhtuli.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2qgimtvrx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2paaqaldj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jdwhoywv.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2xfsmwkjy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2yoipzcvx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2slchyess.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2cpwicqnb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2lehbjaoa.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2qgahpayc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2vajvirtj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2rhamjfyu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tmbdmbgd.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2vannkbse.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2reczjdoh.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2indykgan.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gkieuoue.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2pguqfwjn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rmwxyrvv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2qwfmqrxs.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2rmbqemvt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wjkrskci.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2usckgglz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2lhecwkec.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2zdytjlom.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2spyehykz.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zywnbuhl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2cfgigmjk.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ntfjlsms.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2sibnwvee.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2uzdplzrx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2sytclfdv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2fouwzwxr.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2nlbkmusv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2halppscm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tpvmfccm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2isxdxywp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2oqrtxlbi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tanakdnw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2wvztairh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sdjtmixg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ezjzurhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwwndcmm.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wcopnlbr.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ukqtfxoq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2etcamlqd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ykjkqjfc.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2uakjmdqf.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2drfjkupm.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2tubhxjyo.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2pktrzkcz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wlgfzlaj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hmudbrtb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2amfcuxan.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2lfnjuwwp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dkoxorug.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2fiksnipx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ffkwsudr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2svvonzvz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2gmksscuy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xndgwfzi.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2pibpaucl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2szorrkkz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2kichvheh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2avtunsvz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gunlwovf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2mhfjhhwj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2vcsvhjlo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2qzvuagra.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2rgmpnhyu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xhdduyam.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2vyvenrex.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2yeycozuh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2kojaztfw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dcsdbhjm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2myemggdt.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2kjuyfxym.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2jdcqwzfl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2lqwgbhai.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ounetmve.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fstwjwlv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ucsorvvg.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rmpjlvlp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bywlybqr.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ootinyhq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2frmsjqry.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2gcptpgdf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2amzswjwv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2gfcdfgau.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2evspguuf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lkhvuffh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cvxbozky.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bypqbjdj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dmeumegg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2xubricqs.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2bmfxmfgy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pwmmalax.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2rahdbyds.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2sovkzmxn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2qvjminky.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hcnbjpfx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mnhkagos.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2pajfxuyo.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2icmqrfmi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gxujdyjr.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ribycbhh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ubancyjn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2zdueaufm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2wcjvnhvo.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dlgcwgii.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2pyopuajf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2xpulwozk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2dvvckvdk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2htjqnici.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2jhksewie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dwejoofz.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2vospauxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cmhaneim.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2dlzlcgda.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ggcxxqmq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dbhfoant.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nlseilhd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uqpbpdbb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yqgcpcve.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rawxqwis.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2vraeswux.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qdrafuwu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2yadaclfa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ngzzzadq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ikwkboph.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ovoopgst.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2relnjfxr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2fhronjcl.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qrzsbfqz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2uqivuobt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2niqwhvml.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2thdkpnoj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2uwipczeq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2xilfbyml.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zvcmzdtl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2kgpjdqef.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jixcbkhd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2yaziqbyz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2brhwgcrl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2wfzycgsm.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2nphvmmdc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kuptrpek.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fiwfadqb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sqpzelce.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bkuomndo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2izrmrcqa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2eahvyaym.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kjbrvsbi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zecrcdbx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2unonxbol.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2daextihe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yoxqpkzs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nxamkkvp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwslvgiq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2dsaurrgj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2vuiazimt.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wmklmcld.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2sauzrqka.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kddpmvtm.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2nvcbjyrm.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kpotzkdw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gwmxsulh.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lndbpdkp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2tyqkharf.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2cbmhwchd.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2myqpjuiy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gxpynkhv.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2yqjnldyf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2nhmvssuz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2eejdbpqj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2uyzinntx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2fpesfxgo.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2fucrydjs.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2futvifti.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2uapcurdg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2hhrvwhnx.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2sntntubi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kdovzbpu.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2lwjfkzjr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dchcccgx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lnzbvvnu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yqgykbwy.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2juojcmpk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xyjkntjx.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jzboejhy.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wyiazdtq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2pjtrcodj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wqlusqsv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nalguevj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vxivsiam.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2nrnlhiwc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ruftxfkc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ogbpyhki.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2hkearsfm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2xpzaeerh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2fjlegzqd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2migiqisz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zwysxxxq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ymgkfvqc.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqttqkie.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2mhcvjpes.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2usyhnaqf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ecfwpytx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2pwyehmyj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2iokjsprw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2njfhzxtj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tfsfkxyu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zaljevqr.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cgmcjufu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2aubmxumw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2vlrtgxgm.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2uenvghja.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2pewreekh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bfzglshh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ewurlloo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2leebrpjf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2gcrulokq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2rmhpmpya.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2mxpujxyi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2whsyverm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2oigwlcnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bfictdpe.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2cuclcsuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fjksoffu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2hstzawwt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jojoonlc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ywrqzldp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2olxljkuo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2smdjqkgd.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2uaczbult.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2pkzjwuvw.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2mxffqwwt.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2qfszkeoa.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rntbygwf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ysyejenj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2kthlbcak.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ykgjwcee.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rttvtqkv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2hpiuoabp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2oacucssg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2kpiovgte.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ktlqcoym.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2vketqcma.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2vqgdfvjk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2cldxaoci.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2dzfosbjs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ritxudua.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2relymmng.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2cprhgaab.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dqvmyjbk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fourkmdn.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2smgmthyr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2bwlvtcda.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2vgiupapr.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2khbzehvj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2idoibrzq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2zvtttehs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2iidclzfa.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ipwireke.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqstoare.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2qoigkjlp.html


<!-- 参考信息 -->