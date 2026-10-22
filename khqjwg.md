代发 wailian999

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2naoufpln.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2vttdyogh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2syuehpiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wiiibaoh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2pgfgiiqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xnijgxot.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2mduhtqbm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ifwaqpov.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2wbcoltle.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2xxnyxyqx.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vcphcgiy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ldpfsqpr.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2kuhoqkeq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2fbftxtgs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cctxlset.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ybdnxibb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2mombhuns.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2cdqupmuh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2rnoodmeb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2fhqupjpi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2aahrsrpt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ejqcmmiz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2plzgclce.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kvvtanxc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ebhupasj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2czsyztld.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2cpudveul.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2epwqzfax.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ieioquwp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2giloujhg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2tygovdhw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2rjjfowwk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2jsovdfsq.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2bovzdrfi.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2xscimlda.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2vvtzwbtg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2fmrpazdh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2nwcjdrxg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2zgrzjhdw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2gyfaqeyz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2cxecdycz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2xwiwspmb.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2syqucewy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2lpahxhxp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2axoorjba.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2cyixvpsj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2qswxysuk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2cbokzpoq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2qgxnirid.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2wsaflqtl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dixubolg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yckpyiqn.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rvdplids.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aufrxlsz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pukerbbr.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xwcjcdtr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fyqtjpga.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2krmincsv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2rpjazxul.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vpiwytid.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2emdgolge.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2fuzcbpnw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ebrwikuz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2detmcqpv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ifhqxfpm.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2rjazpptu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2cjrshnpt.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2enmkzbft.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2pqkliuqn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2mllwkici.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2zvfxvjnt.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2oetrpyeu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xqahxryt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ztinttzj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2dyzeyzjq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2yfteynhx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2kcdctvxc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2wiacvcma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eajlyqdj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xrshyjly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxdldpjg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2nbaoajvf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2okydrssa.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2wklodnpg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bvqcxfig.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qetabrxh.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bhejziik.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2guygmawx.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2nwselith.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2rqyjwiud.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hvepfcfq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wtljbnkr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2trkolilv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wryxtpsv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xinbhcie.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hvdwhtac.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gcnmjphp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2fkljjyde.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dorczvdf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2dpmjufrw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zwabqlyl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2wzjilgoy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2falmseod.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ylfpqixi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ykorlkec.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ebwainyj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2atspispm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2byrqtuoa.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2jtmvrhhm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wqbvslks.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2yvwdsrqr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2aiedxtxb.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2lupuyxos.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2yszbejlz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2meauhafd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2dycdktbe.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ymjrokeu.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2axtcojmn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fowbzrfj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2rmxlfwir.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jxmbvpxe.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ltrrzxia.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bjbangcg.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2maihstkq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2baxexkma.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2cirdfsji.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2tabwnfvb.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jksboejc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2iustuihg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fqydasgx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2iglxppsj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2qyrttggn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2rejwbiie.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2opsjfhnc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2gnltojjh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2dmzxznbs.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2njcphhtk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2vbloxpdf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2obgliebo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wpcsxxar.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2afksluks.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2azzdwght.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2zovapxds.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2zaoeiwig.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ihlcmarc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2nzcmwhoz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2mocfjhve.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lkgidtna.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xvudeful.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2omotjylx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2qagwjbka.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2efiuxjnc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2xdoqbjcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nvoiqxkb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2cpdnnbts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqcjcbdn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2kdsyhdaa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yquplyrr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xsvdvryz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2liznucuz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jtyjclpr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2byjmefrb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qdzgsaez.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2fvzdiukg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2loranbsd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2rvpwafhi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qvxefezr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2moxymfhm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ajcaytvc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jwmtvsbr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2shlntxpo.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2txpnfdnx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fueuymjx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2eljnpyup.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2sopirhmn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2vkhyqter.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2rcwmodrp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2vbybcvve.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gntgziob.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wvggcdln.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ulqjzubp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2thptcpqd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2eqpmfelx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ktdqtpaw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2skczhcqk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2olfyqkqt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fkvhzlcv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rmxyypbn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xeibrkmc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2hhkjhmml.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2gbssfouz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2iekxwwzx.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2mniyptiy.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2scmucpga.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2dplqjxho.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2zyezqvbu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2uzqnsuzr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2dowetesw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2uagbevsn.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2osaytfhz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2zcduxzbc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2wypioyeq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rssdpfya.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2qadvrynh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mxddzwhn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mnkgfuly.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2wltqpppi.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2aormnjlv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2nspibwui.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ysqplfxo.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2mhnumtjq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2cuglhyyv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ewplvrgl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2haoflzkk.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2cxokbufa.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2oyrouyfi.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2djrbanty.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2hxatgfuw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2xyeyyrrg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2slfeovxn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2bfesmbms.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2tcvvcnce.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aanbmmge.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2euwsejju.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lvbaoygp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jynbjogx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rytndxgr.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lrubwvwe.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jhkllodm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ledehofz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2trnbmcdr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jlwzihtk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2klastgej.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wsjjmwfi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2oikybslk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jcltqfst.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2yxkjfzfz.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2aingsdpe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2jogzymbq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2obreqdyi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2htbrvaiw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2nagrfrbj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ydyrxrgw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2xtajeqkt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2mfacxlci.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2juzvpzpl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hxzzqrie.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2nhglwete.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2lfgeirvm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kjnmrbjy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ougushmh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yalshjcr.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jkzzuhgv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2nmwdkqzl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cpvysgkm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2vaqpunsx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2yahgcivp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2lfsdpaaj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2hltwhgxi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2puaqoakb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dtmtnkkf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2fknepboz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cqehtdkl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pcrltejy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afmwtxej.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ibjwhnzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2npsxdsxj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2bgodpjaf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xutgbdwj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2nslsgjab.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2nivieoxw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ynupjqdy.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zblvjexn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2vvfxhder.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2jbdmrcor.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2bvqqgoly.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2xccqmght.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ixqbsoym.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2kxbtcmfy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2effeqosl.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2basylgad.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wchmmwgr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2lcxsbylv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2xxgmlfig.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2csyfzbfl.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2bsxnqrvq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wwbeplby.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2syhinumr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2mxxarurt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2wfaopwpa.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xoovfhod.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2psxlaqbs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2qugwskdv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xekuidqn.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2kkaslsbh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2sujrsyqt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2jjblocig.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckrcjeew.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uyctheht.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2qyqvblia.html


<!-- 参考信息 -->