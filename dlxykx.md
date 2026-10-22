代发 wailian999

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2cldsqaly.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fmowpodh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2kalmazpu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ghzhwcur.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2hremwhes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jccryfsv.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2tiswfftt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ovlittmh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2znihnwgh.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ckwwysuh.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2tsixgwwm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2vllzviud.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2lnhbiegh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2lwyadyuc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2evmbeboj.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qqumspqn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2emaciqvo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2lguipawo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2lotyodjr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2yhojlfqp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ouektbor.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2mdficxfb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2kslkrlpc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2bqxmmasv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ootdlrme.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2klxoalqz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kqncbaqt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jfycfscs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2yyrcadse.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2kwizmcdh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2bggzrmls.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2maksopui.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2bdkzjhje.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2obotbebf.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2kvxtpnnh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2yfsofmxt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rukbrtvk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2btcknnor.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2fnofjfjf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2blhetbks.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2bvtqjcho.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2oilzhxbd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2wydoqcxj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2qeruzjkm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2vdhzlnbh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2duxeznyo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2qfmezcfj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2iujafhnn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2spshrmye.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2qcoecrbn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jajistrg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kyrttzgi.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dupjqryw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2osnbexij.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cdtmpodq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2udelazin.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pskvzwnw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2dxrprmry.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2edkjycvc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2qujhqund.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2umycffop.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2uxpaeodz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2taxbwyjd.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2cxnjiifq.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2pcmrndre.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2yeswywiw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2izutonvt.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2xmjrywkr.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jvpuqasu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2asbjpetu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2xtkpihck.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2tjzvkkux.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2soysageq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bveiooju.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2zkjbfxew.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2gogpugbn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hanpszfs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rzeshlkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2llcfghdw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2wriqyjoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhvoiilo.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2oxgibigv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2cxtedjfq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2tbsjaqqs.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2evpimxni.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ngrlzhuc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qordbnwy.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2mfvytygo.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ofenlptj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mnjczyrt.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hcoaqpzq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ganexpuq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ckdslxit.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hcnjapno.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ytkjyfur.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cpnugplv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gnkfwpvw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2wkycgfhf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cntnhjyq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ixofjibv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2oemtsntj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2bgfgrgts.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2eekcnwwb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ucrqxkmh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2cbpcjsem.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2fvzqsdxp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2eqkziyky.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2wvxmsggx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2pzotbbgk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xamvyygx.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2syngjnnw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pyqeyqxu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fzilvfmu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2hjhzonlv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2nahdlrvc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2rfsodmru.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2fkczbnnq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2pctgruop.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jjspvlla.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vgkdwqaq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rxlgxhfy.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xsljjxvt.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rzeazfji.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dwozqcwe.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2vizjblio.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ngnaafmv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2mtwrdlav.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2pjgvadyt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2htkijfml.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wzhfddnh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ateckhxb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2wikkhaaf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2opjidhbx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2yagpynbm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zfjvdtke.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2peigpbyj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2tdebltpv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2dojjzswg.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vfitchll.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2debfkjtk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2gpgzdwfp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2zterdaps.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2loscyezw.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gcmrtoxv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2neliozgd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2rzhvnhhi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mkswcxbd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cahezxkw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zgepkppi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2pbfrgdsk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2gqqwgame.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2hfbvadlo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2yysfqsjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rdneyubu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2isixwzmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ijntimmn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2qnuqxbfg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nllguhfr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bldqhxbw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ynglccof.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zavxlsdm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zwtdrpqn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hagxgilp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2fcsfmyxd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2malpaipn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2vtjiqekb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2eesyqzbs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2boprbiuj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mpbsfkiy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tomgditz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ppksftri.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2hlhhkkti.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gpfgmeao.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2xamqtkef.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2kdelnhsg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2uwnvdeba.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2isyouwji.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ghkmalkm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vwxgoqel.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gzmdeant.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2zmphowai.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2vdyvfiza.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2icfmknxn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2mdwheiio.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wvvlbtmj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xxwvnnfz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rhzzzwcu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ltaqgdru.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2eaxmfqdt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2vmppwuug.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lfrxlbqn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kbwskjsf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2sbootqjh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2iyaotdqo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdyfcmcd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jzkzttxl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bccriamt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2cswsywcy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2voiddtuz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2vpdvnkxb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2qemzqsbj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oubshnnk.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2iyzqfusd.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lnnojwxk.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xkxsprci.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2btqerwbk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2abusbgop.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ksvlpbob.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ijxcfmef.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2yzjgudyw.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2sqlwrrpu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2kmiolnmn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2fidrhwxa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2wwqncxpe.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ohuqkwkm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2nhuqmnuq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2qfjkeors.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2pxqvqsko.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2twnrfnmy.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ikyvllfz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hgrjyxxn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2vuniiqak.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dzgyhfni.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iryqybpn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2inqthuji.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zysvmjym.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2yrbpewql.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dnjuklyh.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vdgboiur.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gqtdkniy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pmenkmtu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2phklnzvp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2fbxfpfsh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wpnnllug.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ftxnzdcq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yieiafpk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2gmejqnjo.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2fgnkipaa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2nowqxigc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2iyhscjdl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2btkxqzeq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2dbgcrelz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2sukeazjr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2qrhcdbyg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2nywscgxa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qoqriizc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2zmnwhrps.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2tbcglopz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2vesbwphw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2afwlimsx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vlitpdms.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mxhfacpt.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tavuaebo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2fcihjdca.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ecnekfta.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2hmdjvwof.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2bdndkvkr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2qsczawhb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kmixzrbr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2linqhdqy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2nqbkwdll.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2wiuaczjv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zmwdsjga.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wztlqyla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2amsxbsis.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2xfnitwhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svqzxogx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2madwabfm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ayvdgkzy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2lpzigkds.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2dpaypzhc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yfmlllgf.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2qlmvjnku.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2sxzregam.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2dwidreef.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2nptktmbb.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2txdfgsqw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2rxnypsve.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2qhwxpheh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rzjqkdsm.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rjlkwtrx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ygrokqqq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2kfcxnasa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2wclhjoau.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2qngaoeca.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2poffzjqf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ufvggbgv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ajoljitq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2oygmonsy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ntmutziv.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kxkthtuf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2dmvfdgqr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tarfryjl.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2makkmlya.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2rajuzlai.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2acxlatfu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2drukjpvo.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vndxxyhe.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2alcljgmf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2pdrwbxin.html


<!-- 参考信息 -->