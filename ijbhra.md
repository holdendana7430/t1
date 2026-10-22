代发 wailian999

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2tfjkttae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpvliiag.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2aqugnvxz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2nzzpwnvr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2qnmacyzl.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yiakefjr.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qdjovnes.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2hhjdahkx.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2ensqxjjs.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2krnwbjba.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2xmxwmxmm.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2kstvvzvk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2heyktgkm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2rmcmxuur.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2nxgyegiy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2tntclvtx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2jqkbvvpt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2qkxugtpu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2zuvumnch.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2cldvsqba.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2vsrmojxu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2halgtudv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2kuvfewbs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2eysdmvyy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2pofypznd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2lcirvlfu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2anxeozph.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2qitzziub.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ynrvgmqi.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2kuihkony.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2dnodkglv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2wnvfosms.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2egzdofcc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ggnbweje.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2jzekipku.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2suffxiet.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2epdecoob.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2nxcuwrmo.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2irgcznsc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2sucfurch.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2yzavnuyi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kpxewsrq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dditkcfq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2jhrjmmyt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2uxegdynv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2hvqiszwk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cuebdtdx.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2tobhdcxi.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bwiuflre.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2wlsahbzq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ylrfufkn.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2awdcgpry.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pmmiinvo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2xwankrza.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2pgtatokv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2chgxurfe.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fcbjrezw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2nxedwqbd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2vxbozcqq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zzopcejz.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ivpqbdsv.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2edynnhbe.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ypjhwglk.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2rsjeirhu.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2sinpkdgp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2lnmjrbvq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2reeoieqz.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2bbkmtkfu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vaklzzvm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2azneqlvo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2qucaxhph.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2khzgymxp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2scwhbiej.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2bvotjrdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kzjxtspe.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2rimaedpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rbghbydn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vtuvpdsq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vzrhufab.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2rsjndsek.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fhuatgyb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rzhhsnzg.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2nmoasjcs.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2wvsklkif.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2qyeincxb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2klrsixqu.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rsmgdbsx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kjosqfrr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2aruvsima.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ijkowvee.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2cgmqllvr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zhnhzqst.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hifnliub.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2jdmitvmx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mbnyeegs.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2llsdiccq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bsakmjvf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2petlzinn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wpzjfknp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vekmobur.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2xuagwzru.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2pzqbehai.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2flvlzziy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2voormxbe.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2dudnrsxt.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2lenpzksi.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2zrszjvls.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2iseeivdi.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lkppexhk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2fetmqqfh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2yxkbvewc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2bnujnddw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2vzehuxbb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2phbqxpzi.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hqlupukj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xaffgnoh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2crljcwcs.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jgzsmssf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sefmozlu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fbiowwbr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2qbpnakbh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2kbqymvfo.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2wrmhefey.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ytgrkuzi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2dljqjqrs.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vwjxleii.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rppxvana.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wmxtvqkx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2hctkxzhk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ohlgptfz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pjkgfhki.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ohkrtkqx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2xprzlqjq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2vdtfvghk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ayodsnvg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jqwhfrac.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2yfrkirxn.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2gfmfrbtj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2pvozefvh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zjujqvsq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2valhjlir.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2proeevnm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2saxgkxiw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xbnsisie.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2parsdpmp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2dddkadbw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2rkmzdxwj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2gfklgruo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ojpujwxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dprsocwa.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2evpnrxuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2conpbbsb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bsjtxvlb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vyjsxzkp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xmqggiyl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lorolkqj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wampzdsx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cxvnygcj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ugiqlpky.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2wwlsggon.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2erbkumkz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2yipyckfn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2txihwbud.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2byffboxx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2niylphit.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pxfaohrl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2daqhxfpl.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yfkvgkxg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2bkybnytc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mqpxekmv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2gulukwrq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2lwrvvvdq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2hewivtpe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2johjsqrq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rpybfvyc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ozltksuu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ljhassfi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2hxqqgctl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ezxgnlmn.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2cqnqpjrk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pjvrdqnh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofmmksof.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2usykfavo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tmxrdiff.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yjlelhfy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2bnruuwja.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wpkhciht.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zhxnppxp.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2vgtmfroj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rmxrjixa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2stlqfpyo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2dciqdbvz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnwiyqla.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2lfyaxgev.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2mqtdmitu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cjvdhesz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2jcybajbw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rredvzhb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2nlefhcar.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fobhzpyk.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uaasafds.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hucvvgye.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2iaqyavzk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2qakgukfa.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kwojuyzi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wunqnxzm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2tmuauonb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ekaqonof.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2gfzomscq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2usuytwfy.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2bfmeolya.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2tmieqyqe.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2akxvdvox.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2mhozbirm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2pnfpxfpl.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2fgifruki.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eumdmvwo.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2riabttxk.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yrbomawt.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xasndlfv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ewuqixfx.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qhrapwhh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2njomfsrx.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qhhftzzk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fxgurmmj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bhaulvws.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2aqqcvrqq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rocnqxrf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2omxnqotm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2efrbkvxv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2yozsaicb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2snugdpig.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2haxnwzjd.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2jlabdqhd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ovzmjqai.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2pwhptvlx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2pzhsxdac.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2yafsraui.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2pgupqwda.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2sbyxmcsk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2zfvsgisd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqqueurm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2vkumpuem.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ghwxwzba.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2sdnufqzw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rlbxropr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2iqmklzja.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bimgrtid.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vtksafze.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2cgobohxz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gjtkahuj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2vtultgsj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2tzodbstt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2wxzsidix.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ujqvdoev.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qwjrqqpz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ejkasmdw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2oowbjhwh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dfjstktt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2abujzcoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cywgiydn.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2iqqaxyir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ocbtfavc.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2tctovkuz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2xsyryowl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2qeobkztn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2gjnwsffl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qhvhyzcl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ipgpthnq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ekxeywty.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2vbcyemvc.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2hsicsltj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iochopub.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ikijehlm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2doteuyjd.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dzpfqbuo.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2necuvqzn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2liwtztvj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2lslscrzh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2sxtmgnxt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2xnjukndg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2dyazsjlf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2yoxczrfb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2niukaihv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ynlttapw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pyeeepjx.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hocjyqjs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2bnylpepv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2sqgpawhm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fpvadyqs.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2nffrtbwg.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2dubohcoa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2bdjwxccx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xslrrhjr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uprptcme.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2nkjjfciz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ggiuebch.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2airawcyu.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2lmyebuih.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2wcbtsxgq.html


<!-- 参考信息 -->